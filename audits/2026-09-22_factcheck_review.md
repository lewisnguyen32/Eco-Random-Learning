# Review và kiểm chứng Eco Learning — 22/09/2026

## Kết quả và phạm vi

Đã rà soát toàn bộ 19 file ban đầu ngoài thư mục nội bộ Git: 4 bài học, 3 README nhóm, chỉ mục, hướng dẫn, ghi chú, bộ nhớ và audit cũ. Đã sửa lỗi kiến thức, đồng bộ các bản tóm tắt và bổ sung nguồn cụ thể. Tạo báo cáo này để phân biệt kết luận đã có bằng chứng với phạm vi chưa xác minh đầy đủ.

**Đánh giá sau sửa:** có thể tiếp tục dùng các bài làm tài liệu học cơ chế trong những giả định đã nêu. Không còn lỗi trọng yếu đã biết trong các phép tính, bút toán và quan hệ nội bộ được rà soát. Không coi đây là chứng nhận mọi phát biểu kinh tế đúng trong mọi bối cảnh hoặc mọi quy định đã được cập nhật toàn diện đến hôm nay.

Đây là đợt sửa/audit toàn kho theo yêu cầu rõ ràng của người dùng, nên được sửa bài cũ và dòng chỉ mục cũ; không phải phiên biên soạn một bài mới áp dụng giới hạn 5 loại file. Ngày học và ID cũ được giữ nguyên.

## 1. Phát hiện quan trọng và cách xử lý

P1 là lỗi có thể làm lệch cách hiểu hoặc tính toán; P2 là thiếu điều kiện, nguồn, phạm vi hoặc tính nhất quán. Tất cả các mục dưới đây đã được xử lý trong nội dung đang dùng.

| Mã | Mức | Trước sửa | Sau sửa / nơi sửa |
| :--- | :--- | :--- | :--- |
| F01 | P1 | COGS/ngày × CCC được coi là nhu cầu vốn/vay chính xác. | Tách vốn hoạt động khỏi lịch tài trợ; ví dụ có W = 37,5 tỷ, còn phép quy theo giá vốn ra 30 tỷ. CORP-001 mục 3.3 và 4. |
| F02 | P1 | OCF dùng ΔNWC nhưng NWC bao gồm tiền và nợ vay; DSO/DPO thiếu giả định mẫu số. | Dùng W hoạt động trong mô hình OCF rút gọn; DSO theo bán chịu, DPO theo mua chịu; dùng COGS thay mua chịu là xấp xỉ. CORP-001 mục 3.2–3.4. |
| F03 | P1 | Tiền mặt trong két bị gộp vào reserve balances; công thức tiền cơ sở có thể bỏ sót tiền két. | Phân biệt C công chúng, C két và R tại NHTW; công thức phù hợp quy ước. MONEY-001 mục 3.1; GLOSSARY. |
| F04 | P1 | QE được mô tả chỉ tăng tiền gửi khi ngân hàng cho vay thêm. | Bổ sung mua tài sản từ chủ thể phi ngân hàng có thể tăng tiền gửi ngay, với phạm vi thống kê rõ. MONEY-001 mục 4; MACRO-001 mục 3.5. |
| F05 | P1 | P trong MV = PY bị liên hệ như CPI dù Y là GDP thực; Fisher ex-ante được gọi là đồng nhất thức tổng quát. | P tương thích GDP danh nghĩa/thực; tách đồng nhất thức khỏi nhân quả và kỳ vọng của phép chia khỏi phép chia với kỳ vọng. MACRO-001 mục 3.4, 3.6. |
| F06 | P1 | Repo làm giảm trái phiếu ngân hàng và không tạo nợ, giống bán đứt. | Với repo tài trợ, ngân hàng tăng dự trữ và nợ repo, tiếp tục ghi chứng khoán theo điều kiện dừng ghi nhận. MONEY-002 mục 3.4. |
| F07 | P1 | ECB và NHNN được gán chung hành lang đối xứng; tăng lãi suất luôn đi kèm giảm dự trữ. | Tách mô hình khỏi khung từng NHTW; ghi đúng mốc ECB 2024 và Fed/IORB; không mặc định co dự trữ. MONEY-002 mục 3.2–3.5; memory Entry 005. |
| F08 | P1 | Dữ liệu cả năm 2023 dùng để giải thích quyết định giữa năm; sơ đồ đảo thứ tự 2022–2023. | Dùng mốc quyết định có ngày ban hành/hiệu lực và chỉ diễn giải bằng thông tin có thể biết khi đó. MONEY-002 mục 5. |
| F09 | P2 | Số nhân tiền còn bị dùng như cơ chế nhân quả trong README/LEARNED; tỷ lệ “80–90%” thiếu quốc gia/mẫu số. | Loại tỷ lệ không đủ phạm vi; trình bày số nhân là tỷ số hoặc mô hình có giả định; đồng bộ chỉ mục. |
| F10 | P2 | Tăng lãi suất được mô tả như tất yếu làm giảm cổ phiếu, tăng nội tệ hoặc chặn lạm phát; “6–24 tháng” là khoảng chung. | Nêu điều kiện, phản ứng bù trừ và độ trễ bất định; bỏ gợi ý phân bổ tài sản/đòn bẩy chỉ dựa vào chiều lãi suất. MONEY-002. |
| F11 | P2 | NIM được dùng như khoản cộng vào lãi vay; DTI có thể nhầm với tỷ lệ dư nợ/thu nhập. | Định nghĩa NIM cấp ngân hàng; mô tả rõ tỷ lệ nghĩa vụ trả nợ hàng tháng trong ví dụ. MONEY-002 mục 4, 6, 8; GLOSSARY. |
| F12 | P2 | Cơ quan thống kê cũ và rổ CPI 2020–2025 được dùng như hiện trạng 2026; TT07/2014 dùng như quy định hiện hành. | Cập nhật tên cơ quan; đặt rổ cũ đúng kỳ; đối chiếu TT48/2024 thay thế TT07; không đưa số hiện hành chưa đủ căn cứ. |
| F13 | P2 | Link bài học sai tương đối, ID tương lai lỗi thời; thiếu Active Recall ở CORP-001/MONEY-002. | Sửa đường dẫn và trạng thái; đủ mục bắt buộc cho 4 bài; giữ ID/ngày học. |
| F14 | P2 | Nguồn chỉ trỏ trang chủ, tên nguồn chưa xác minh, audit tự chấm độ chính xác rất cao. | Thay bằng tài liệu cụ thể; ghi rõ nguồn chưa xác minh; thêm đính chính lên audit cũ, giữ phần gốc làm lịch sử. |
| F15 | P2 | NOTES suy backlog chắc chắn vô hạn và số token từ số dòng; “9 mục” không khớp những phần bắt buộc khác. | Nêu mô hình hàng chờ có điều kiện, không đếm trùng khái niệm; bỏ ước lượng token vô căn cứ; làm rõ hai câu trong AGENTS. |

Các ví dụ được gắn nhãn giả định. Đã bỏ các suy diễn “CCC = 0 là không cần tài trợ”, “OCF âm là gian lận”, “hết tiền đồng nghĩa phá sản pháp lý”, cũng như phân biệt trả nợ ngân hàng, trả nợ phi ngân hàng và xóa nợ xấu.

## 2. Bằng chứng nguồn chính

Các nguồn dưới đây được dùng cho khẳng định cụ thể, không chỉ liệt kê tên tổ chức. “Đọc nội dung” nghĩa công cụ web trả về phần nội dung hỗ trợ kết luận; không có nghĩa đã đọc mọi trang của cả cẩm nang.

| Nguồn / thời điểm | Nội dung đối chiếu | Mức truy cập trong phiên |
| :--- | :--- | :--- |
| [ACCA – Working capital management](https://www.accaglobal.com/gb/en/student/exam-support-resources/fundamentals-exams-study-resources/f9/technical-articles/wcm.html), không ghi năm | CCC và các giả định khi dùng cost of sales thay credit purchases | Đọc nội dung liên quan |
| [ACCA – Cash flow statements](https://www.accaglobal.com/uk/en/student/exam-support-resources/fundamentals-exams-study-resources/f3/technical-articles/cashflow-statements.html), không ghi năm | Điều chỉnh dòng tiền theo tồn kho, phải thu, phải trả | Đọc nội dung liên quan |
| [IFRS Foundation – IAS 7](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/) | Nguyên tắc phân loại và điều chỉnh dòng tiền | Đọc trang tổng quan; không dùng để khẳng định chế độ kế toán Việt Nam hiện hành |
| [BoE – Money creation in the modern economy, 14/03/2014](https://www.bankofengland.co.uk/quarterly-bulletin/2014/q1/money-creation-in-the-modern-economy) | Khoản vay tạo tiền gửi; mô hình số nhân không phải quy trình ngân hàng thực tế | Đọc nội dung; kết quả tìm kiếm cũng trả trích đoạn PDF gốc |
| [BoE – How is money created?, 01/10/2019](https://www.bankofengland.co.uk/explainers/how-is-money-created) | Tạo và xóa tiền gửi khi cấp vay/trả gốc | Nội dung nguồn chính thức qua tìm kiếm |
| [BoE – QE, 2022 Q1](https://www.bankofengland.co.uk/quarterly-bulletin/2022/2022-q1/qe-at-the-bank-of-england-a-perspective-on-its-functioning-and-effectiveness) | Mua tài sản từ phi ngân hàng làm tăng tiền gửi và dự trữ | Nội dung đoạn cơ chế qua tìm kiếm nguồn chính thức |
| [Fed – H.6, 23/11/2021](https://www.federalreserve.gov/releases/h6/20211123/) | Phạm vi M1/M2, tiền mặt và reserve balances | Đọc chú thích thống kê; dữ liệu lịch sử không được gắn nhãn hiện tại |
| [Federal Reserve History – Great Depression, 22/11/2013](https://www.federalreservehistory.org/essays/great-depression) | Gần 30% giảm cung tiền từ mùa thu 1930 đến mùa đông 1933 | Đọc đúng đoạn và khoảng thời gian |
| [IMF – CPI Manual, 2020](https://www.imf.org/en/data/statistics/cpi-manual) và [chương 1](https://www.elibrary.imf.org/display/book/9781484354841/ch01.xml) | CPI, công thức chỉ số và phân biệt mục tiêu đo lường | Trang tài liệu và nội dung chương qua tìm kiếm; không đọc toàn bộ sách |
| [FRED Blog – The velocity of money, 2015](https://fredblog.stlouisfed.org/2015/01/the-velocity-of-money/) | V = GDP danh nghĩa / M | Đọc nội dung |
| [BLS – CPI June 2022, công bố 13/07/2022](https://www.bls.gov/news.release/archives/cpi_07132022.htm) | CPI-U +9,1% so cùng kỳ, chưa điều chỉnh mùa vụ | Đọc thông cáo |
| [Powell – Review and Outlook, 23/08/2024](https://www.federalreserve.gov/newsevents/speech/powell20240823a.htm) | Diễn giải cung, cầu và kỳ vọng trong đợt lạm phát đại dịch | Đọc bài phát biểu, gắn rõ là diễn giải |
| [Fed – Ample-reserves regime, 01/07/2020](https://www.federalreserve.gov/econres/notes/feds-notes/implementing-monetary-policy-in-an-ample-reserves-regime-the-basics-note-1-of-3-20200701.html) | Công cụ lãi suất quản lý và chế độ dự trữ dồi dào | Đọc nội dung và kiểm tra tác giả |
| [Fed – IORB, Implementation Note 28/07/2021](https://www.federalreserve.gov/newsevents/pressreleases/monetary20210728a1.htm) | Đổi IORR/IOER thành IORB từ 29/07/2021 | Nội dung nguồn chính thức qua tìm kiếm |
| [ECB – Operational framework, 13/03/2024](https://www.ecb.europa.eu/press/pr/date/2024/html/ecb.pr240313~807e240020.en.html) | DFR và chênh lệch MRO–DFR từ tháng 9/2024 | Đọc thông báo, không coi là xác nhận toàn bộ tham số 2026 |
| [Fed – Accounting Manual, Chapter 4, cập nhật 22/01/2026](https://www.federalreserve.gov/aboutthefed/chapter-4-system-open-market-account.htm) | Repo/reverse repo là giao dịch tài trợ/vay có bảo đảm | Đọc mục 40.15–40.20 |
| [ECB – Transmission mechanism](https://www.ecb.europa.eu/mopo/intro/transmission/html/index.en.html) và [Lane, 11/10/2022](https://www.ecb.europa.eu/press/key/date/2022/html/ecb.sp221011~5062b44330.ga.html) | Các kênh, hợp đồng và độ trễ biến thiên | Đọc nội dung liên quan |
| [Fed – Banking System Conditions, 05/2023](https://www.federalreserve.gov/publications/2023-may-supervision-and-regulation-report-banking-system-conditions.htm) | NIM = thu nhập lãi thuần / tài sản sinh lãi bình quân, quy đổi năm | Đọc chú thích Figure 3 |
| [NHNN – Thông báo đợt 24/10/2022](https://www.sbv.gov.vn/documents/d/sbv_portal/524653) | Quyết định 1809, 1812, 1813; hiệu lực 25/10/2022 | Đọc PDF gốc 2 trang qua trích xuất văn bản |
| [Cổng Chính phủ – Thông báo NHNN 16/06/2023](https://xaydungchinhsach.chinhphu.vn/nhnn-tiep-tuc-dieu-chinh-lai-suat-dieu-hanh-119230616150218505.htm) | Quyết định 1123–1125, hiệu lực 19/06/2023 | Đọc nội dung công bố |
| [Luật 46/2010/QH12, Điều 11](https://chinhphu.vn/default.aspx?docid=96040&pageid=27160) | Nhiều hình thức tái cấp vốn | Đọc nội dung điều luật |
| [Cục Thống kê – Lịch sử phát triển](https://www.nso.gov.vn/gioi-thieu/lich-su-phat-trien/) | Tổ chức thuộc Bộ Tài chính từ năm 2025 | Đọc các mốc 2025; không dựa vào đoạn “hiện nay” cũ còn nằm ở phần lịch sử trước đó |
| [Cục Thống kê – Phương pháp CPI, 2025](https://www.nso.gov.vn/default/2025/11/chi-so-gia-tieu-dung-va-phuong-phap-do-luong-tai-viet-nam/) | 752 mặt hàng thuộc giai đoạn 2020–2025; chuyển năm gốc | Đọc nội dung; không suy rộng số mặt hàng sang 2026 |

Nguồn FOMC 16/03/2022 và 26/07/2023, cùng nguồn về bẫy thanh khoản của Fischer, được dẫn ngay trong bài tương ứng.

## 3. Giới hạn bằng chứng và nội dung đã loại khỏi khẳng định hiện tại

1. **TT48/2024 và chú thích CPI tháng 02/2026:** công cụ mở toàn văn gặp lỗi. Đã đối chiếu được thông tin qua chỉ mục tìm kiếm của [CSDL VBPL chính thức](https://vbpl.vn/TW/Pages/vbpq-toanvan.aspx?ItemID=170156) và [PDF chính thức của Cục Thống kê](https://www.nso.gov.vn/wp-content/uploads/2026/03/Tong-quan-CPI-thang-02-nam-2026-1.pdf). Hai đoạn bài học ghi rõ giới hạn này. Không nhận đã kiểm tra toàn bộ tình trạng pháp lý, các sửa đổi tiếp theo hay toàn bộ báo cáo CPI.
2. **Thông số hiện hành chưa đủ căn cứ:** không giữ bảng quyền số, tổng số mặt hàng CPI hoặc mục tiêu CPI 2026 như sự thật hiện tại. Không đưa bảng mức lãi suất hiện hành năm 2026.
3. **Nguồn cũ thiếu căn cứ:** bỏ tên *Money and Missed Conceptions* chưa xác minh, các dẫn chiếu HBR/chương sách không có đoạn hỗ trợ và các link trang chủ thay cho tài liệu. Không kết luận những tài liệu đó chắc chắn giả.
4. **Chi tiết không cần thiết cho cơ chế:** bỏ DXY 114,78, lãi huy động 9–10%, mệnh đề “nhanh nhất hơn 4 thập kỷ” và các khuyến nghị phân bổ tài sản cứng khi không có đủ phạm vi/bằng chứng ngay tại đoạn.
5. **Review bằng chính agent:** đây là vòng tự kiểm tra lại sau sửa bằng nguồn và phép tính độc lập, không phải đánh giá của một chuyên gia thứ hai. Không có subagent hoặc peer review bên ngoài.

## 4. Kiểm tra sau sửa

### Số học và hạch toán

| Kiểm tra | Kết quả |
| :--- | :--- |
| DIO, DSO, DPO → CCC | 91,25 + 91,25 − 60,833333… = 121,666666… ngày |
| W hoạt động trong ví dụ | 22,5 + 30 − 15 = 37,5 tỷ |
| COGS/ngày × CCC | 30 tỷ; không bằng W, chênh lệch đã được giải thích |
| CPI giả định | 117,682926… |
| Lợi suất thực với i = 7% | −9,077720…%, làm tròn −9,08% |
| Sức mua 10,7 triệu cuối kỳ | 9,092227… triệu theo giá đầu kỳ |
| MV/PY với các giả định trong bài | Tăng P khoảng 1,456311%, không gọi là dự báo CPI |
| Nghĩa vụ vay trước/sau | 22,5 và 26,666666… triệu; tỷ lệ trên thu nhập 37,5% và 44,444444…% |
| Bảng cân đối khoản vay/chuyển tiền/mua đứt/repo | Đã kiểm tra tài sản = nợ + vốn chủ; tách các chủ thể và nghĩa vụ hoàn trả |

Số học được tính lại bằng Python Decimal trên runtime có sẵn. Bảng cân đối được đọc đối chiếu theo từng bút toán; phép kiểm tra số học không tự xác nhận tính đúng của giả định kinh tế.

### Nhất quán repository

- 4 ID bài học duy nhất, khớp LEARNED; ngày học gốc được giữ.
- Prerequisites tồn tại; category khớp thư mục.
- 4 bài đủ các phần bắt buộc, kể cả Active Recall và nhãn mô hình/thực tế.
- 39 thuật ngữ đã đồng bộ định nghĩa và bài liên quan.
- RELATE có 13 dòng quan hệ: 4 đã học, 9 chưa học; không diễn giải thành 13 khái niệm duy nhất.
- Kiểm tra liên kết tương đối trên toàn bộ Markdown và kiểm tra khoảng trắng bằng git diff --check.
- Các câu sai còn xuất hiện trong phần lịch sử lỗi/audit đều được đánh dấu là nội dung cũ, không phải kết luận hiện tại.

### Memory self-check

- [x] Áp dụng G-001 đến G-007 và ghi các lỗi mới vào Entries 006–011.
- [x] Phân biệt mô hình giáo trình, cơ chế thực tế và điều kiện biên.
- [x] Kiểm tra số dư dự trữ, tiền gửi, tiền mặt và từng bảng cân đối.
- [x] Bỏ quan hệ nhân quả định mệnh và độ trễ định lượng thiếu phạm vi.
- [x] Phân loại khẳng định; ví dụ giả định có nhãn.
- [x] Định lượng có kỳ đo/nguồn hoặc giả định; giới hạn truy cập nguồn được nêu.
- [x] Đồng bộ bài học, chỉ mục và cả hai operational memories.

## 5. File thay đổi

**Tạo mới:** báo cáo này.

**Sửa nội dung kiến thức:** 4 bài học; 3 README nhóm; LEARNED, GLOSSARY và một số dòng RELATE.

**Sửa hệ thống phòng ngừa tái lỗi:** knowledge_corrections và hai operational memories; NOTES; thêm đính chính đầu audit 12/08/2026. AGENTS chỉ làm rõ hai câu về “9 mục”, không thay mô hình học hay cơ chế cấp phép.

README gốc, .memory/README và .gitignore đã được đọc, không cần đổi nội dung. Không tạo bài mới, không đổi ID, không thay cấu trúc thư mục và không tạo commit.


### Dòng thay đổi trong bản sau sửa

Số dòng lấy từ git diff --unified=0 so với HEAD trước phiên. Các vùng là dòng mới/thay thế; phần nội dung cũ bị xóa xem trực tiếp trong diff. Báo cáo mới này được tạo toàn bộ.

<details>
<summary>Mở bảng dòng thay đổi của 16 file đã có</summary>

| File | Dòng mới hoặc thay thế |
| :--- | :--- |
| [.memory/antigravity_memory.md](../.memory/antigravity_memory.md) | 1, 3, 5, 7, 9, 11, 13–16, 18, 20, 22, 24, 26, 28–69 |
| [.memory/codex_memory.md](../.memory/codex_memory.md) | 1, 3, 5, 7, 9, 11, 13–16, 18, 20, 22, 24, 26, 28–69 |
| [.memory/knowledge_corrections.md](../.memory/knowledge_corrections.md) | 3, 14, 17, 45, 55, 68, 78–79, 89, 109, 120, 127, 129–185 |
| [AGENTS.md](../AGENTS.md) | 183, 550 |
| [GLOSSARY.md](../GLOSSARY.md) | 1, 3, 5, 7–45 |
| [LEARNED.md](../LEARNED.md) | 3, 7–10 |
| [NOTES.md](../NOTES.md) | 1, 3, 5, 7, 9, 11, 13–18, 20, 22, 24, 26, 28, 30, 32, 34–49 |
| [RELATE.md](../RELATE.md) | 3, 16–17, 22 |
| [audits/2026-08-12_audit_report.md](../audits/2026-08-12_audit_report.md) | 3–4 |
| [topics/corporate-and-markets/README.md](../topics/corporate-and-markets/README.md) | 1, 3, 5, 7, 9–11 |
| [topics/corporate-and-markets/cash-conversion-cycle.md](../topics/corporate-and-markets/cash-conversion-cycle.md) | 9, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44–46, 48, 50, 52–53, 55, 57, 59, 61, 63, 65, 67, 69, 71, 73–76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 96, 98, 100, 102, 104–111, 113, 115, 117, 119, 121, 123, 125, 127–131, 133, 135, 137–140, 142, 144–151, 153, 155–157, 159, 161, 163–166, 168, 170–172, 174, 176, 178 |
| [topics/macroeconomics/README.md](../topics/macroeconomics/README.md) | 1, 3, 5, 7, 9–12 |
| [topics/macroeconomics/inflation-cpi-and-macro-transmission.md](../topics/macroeconomics/inflation-cpi-and-macro-transmission.md) | 10, 13, 17, 21, 23, 27, 29, 31, 33, 35, 37, 39, 41, 43, 45, 47–49, 51, 53, 55, 57, 59–63, 65, 67, 69, 71, 73, 75, 77, 79, 81, 83, 85, 87, 89, 91, 93, 95–97, 99, 101, 103–105, 107, 109, 111, 113, 115, 117, 119, 121, 123, 125, 127, 129–134, 136, 138, 140, 142, 144, 146, 148, 150, 152, 154, 156–159, 161, 163–168, 170, 172, 174, 176, 178, 180, 182, 184–188, 190, 192–195, 197, 199–201, 203, 205, 207 |
| [topics/monetary-and-banking/README.md](../topics/monetary-and-banking/README.md) | 3, 5, 7, 9–11, 13, 15–18 |
| [topics/monetary-and-banking/money-supply-and-bank-money-creation.md](../topics/monetary-and-banking/money-supply-and-bank-money-creation.md) | 9, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30–34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56–59, 61, 63, 65, 67, 69–72, 74, 76, 78, 80, 82–85, 87, 89, 91, 93–95, 97, 99, 101, 103, 105, 107, 109, 111, 113, 115, 117–120, 122, 124, 126–130, 132, 134, 136, 138, 140, 142, 144, 146, 148, 150, 152, 154, 156, 158, 160, 162–167, 169, 171–175, 177, 179–181, 183, 185–187, 189, 191, 193 |
| [topics/monetary-and-banking/policy-rates-and-monetary-transmission.md](../topics/monetary-and-banking/policy-rates-and-monetary-transmission.md) | 10, 13, 17, 19, 23, 25, 27, 29, 31, 33, 35–53, 55, 57, 59–71, 73–74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94–122, 126, 128, 130–133, 135, 137–138, 140, 142, 144, 146, 148–153, 155, 157, 159, 161, 163–167, 169, 171, 173, 175, 177, 179, 181–189, 191, 193, 195–199, 201–214, 216, 218 |

</details>
