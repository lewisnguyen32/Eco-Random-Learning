# Note Cá Nhân: Phân Tích Bản Chất Toán Học của Kiểm Chứng Thông Tin & Quản Trị Backlog (RELATE / GLOSSARY)

Hai vấn đề này thực chất có bản chất toán học khác nhau — đáng tách riêng để xử lý đúng cách.

## 1. Kiểm chứng thông tin — vấn đề là "tự khai không phải bằng chứng"

Protocol hiện tại yêu cầu Agent *tự dán nhãn* độ tin cậy (`[CẦN XÁC MINH LẠI]`) và *tự tuyên bố* không bịa nguồn. Nhưng không có bước nào bắt buộc **thực sự chạy web search để đối chiếu** trước khi ghi vào bài — nó chỉ nói "nếu có công cụ tra cứu, ưu tiên xác minh", tức là tùy chọn chứ không bắt buộc.

Vấn đề cụ thể: 4 nguồn trong bài MONEY-001 (McLeay et al. 2014, Fed St. Louis 2021, Mishkin 2021, Friedman & Schwartz 1963) đều là tài liệu kinh điển có thật — nhưng tôi không có cách nào biết agent đã đọc chúng hay chỉ "nhớ mang máng" nội dung rồi diễn giải lại (đây chính là cách hallucination học thuật hay xảy ra: tên nguồn đúng, nội dung trích dẫn sai).

**Đề xuất phân tầng xác minh theo chi phí/lợi ích, không xác minh mọi thứ:**

| Loại nội dung | Rủi ro | Cách xử lý |
|---|---|---|
| Khái niệm/công thức ổn định (VD: CCC = DIO+DSO-DPO) | Thấp — dễ tự kiểm bằng trực giác toán học | Không cần xác minh thêm |
| Trích dẫn học thuật kinh điển (Mishkin, Friedman...) | Trung bình — tên đúng nhưng nội dung có thể bị diễn giải sai | Bạn tự search 1 câu nhanh mỗi ~5 bài để spot-check, không cần mỗi bài |
| Số liệu thời sự/quy định VN (lãi suất, thuế, tỷ giá) | Cao — dễ sai, dễ lỗi thời | **Bắt buộc** agent chạy web search thật và dán link nguồn gốc ngay trong bài, không chỉ tên báo cáo |

Việc đáng làm nhất: sửa `AGENTS.md` để phần "Nguồn tham khảo và độ tin cậy" đổi từ "ưu tiên xác minh nếu có công cụ" thành **bắt buộc chạy search cho mọi Current Fact/Empirical Relationship**, có log lại query đã dùng. Điều này biến "tôi tin agent không bịa" thành "tôi có thể truy vết được agent đã tra gì".

## 2. RELATE.md và GLOSSARY.md — hai file này có tốc độ phình khác hẳn nhau

**GLOSSARY.md: tăng tuyến tính, vô hại trong trung hạn.** Mỗi bài thêm ~5-6 thuật ngữ, không có cơ chế xóa. Làm phép tính nhanh: hiện 23 dòng ≈ 300 token để agent đọc. Nếu duy trì nhịp độ vài bài/tuần trong 1 năm (~150 bài) → khoảng 800-900 dòng ≈ 15.000-18.000 token phải nạp *mỗi lần* trước khi viết bài mới. Không phá hệ thống nhưng bắt đầu tốn kém thật sự sau ~1 năm kiên trì. Nên định sẵn ngưỡng chia nhỏ ngay từ bây giờ (VD: khi vượt 150 dòng → tách `GLOSSARY.md` thành index gốc trỏ tới `topics/<category>/GLOSSARY.md` con), thay vì để đến lúc file quá to mới cuống cuồng refactor.

**RELATE.md: đây mới là vấn đề thật — nó là một hàng đợi phình *nhanh hơn* tốc độ xử lý, không phải chỉ "file to".** Nhìn vào cấu trúc: mỗi bài học tạo ra 2-4 dòng RELATE mới (mục "Liên kết kiến thức"), nhưng protocol chỉ chọn 1 bài củng cố sau mỗi 3-4 bài mới (breadth-first ưu tiên). Tức là:

- Tốc độ nạp vào hàng đợi: ~3 mục/bài × mọi bài
- Tốc độ rút ra khỏi hàng đợi: ~1 mục / (3-4 bài)

→ Hàng đợi tăng ròng khoảng 10-11 mục sau mỗi 4 bài, **và không có cơ chế nào rút bớt**. Đây không phải lỗi thiết kế nhỏ — nó là backlog hội tụ về vô hạn về mặt toán học, giống hệt bug kinh điển trong task queue management. Sau vài trăm bài, `RELATE.md` sẽ có hàng nghìn dòng "⏳ Chưa học" mà phần lớn không bao giờ được chọn tới, nhiều mục sẽ lỗi thời hoặc không còn liên quan khi cuối cùng agent quay lại.

**Đề xuất cụ thể** (không cần làm ngay, nhưng nên viết luật vào AGENTS.md trước khi backlog vượt tầm kiểm soát):
- Thêm cơ chế "aging": mục nào nằm trong `RELATE.md` quá N bài (VD: 30 bài) mà chưa được chọn → tự động chuyển sang `RELATE_archive.md`, không hiển thị trong hàng đợi hoạt động nữa.
- Hoặc giới hạn cứng: mỗi bài chỉ được phép thêm tối đa 2 mục mới vào RELATE (thay vì 2-4), giảm tốc độ nạp thay vì tăng tốc độ rút — dễ implement hơn vì không cần logic archive.

Cả hai vấn đề đều chưa cấp bách ở quy mô hiện tại (2 bài học), nhưng đáng viết luật xử lý ngay bây giờ trong AGENTS.md, vì sửa một quy tắc trong file protocol dễ hơn nhiều so với việc dọn dẹp một file 1000 dòng đã rối sau này.
