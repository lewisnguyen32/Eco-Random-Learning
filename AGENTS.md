# Hướng dẫn Vận hành và Quy tắc Biên soạn cho AI Agent (AGENTS.md)

Tài liệu này chứa toàn bộ quy định, tiêu chuẩn nội dung và quy trình làm việc dành cho AI Agent khi biên soạn các bài học kinh tế, tài chính và đầu tư trong dự án **Eco Learning**.

---

## 1. Cấu trúc Kho lưu trữ & Tối ưu hóa Token

Dự án được tổ chức theo cấu trúc như sau:

```
Eco Learning (GEMINI)/
├── README.md               # Tổng quan kho lưu trữ
├── AGENTS.md               # Quy định & Prompt chỉ dẫn cho Agent (File này)
├── LEARNED.md              # Bảng nhật ký tổng quan các bài học đã hoàn thành
├── RELATE.md               # Hàng chờ các khái niệm liên quan (Dùng để tham khảo & củng cố kiến thức)
└── topics/                 # Thư mục Nhánh A duy nhất chứa toàn bộ các chủ đề
    └── <category-B>/       # Thư mục Nhánh B (Tên tiếng Anh kebab-case, ví dụ: corporate-and-markets)
        ├── README.md       # Tóm tắt danh mục các bài học thuộc chủ đề B này
        └── <lesson-name>.md # Bài học .md chi tiết nằm trực tiếp trong B
```

### ⚠️ QUY TẮC TIẾT KIỆM TOKEN CHO AGENT:
1. **TRÁNH đọc trực tiếp các file bài học `.md` chi tiết** trừ khi thực sự cần thiết (ví dụ: cần trích dẫn chính xác công thức hoặc nội dung cụ thể từ bài đó).
2. Khi cần kiểm tra lịch sử các bài đã học và chọn chủ đề tiếp theo:
   - **Bước 1:** Đọc file [`RELATE.md`](file:///d:/Projects/Clone/Eco%20Learning%20(GEMINI)/RELATE.md) để kiểm tra các khái niệm liên quan chưa học (đã được mở ra từ các bài trước).
   - **Bước 2:** Đọc file [`LEARNED.md`](file:///d:/Projects/Clone/Eco%20Learning%20(GEMINI)/LEARNED.md) ở thư mục gốc (nơi chứa tóm tắt 1 dòng siêu gọn cho mỗi bài).
   - **Bước 3 (nếu cần xem sâu hơn về một nhóm chủ đề):** Đọc file `README.md` nằm bên trong thư mục `topics/<category-B>/` tương ứng (nơi chứa tóm tắt 3-5 câu cho các bài học trong nhóm đó).

---

## 2. Quy trình 6 bước Biên soạn Bài học Mới

Mỗi khi người dùng yêu cầu bài học mới, Agent phải thực hiện đúng 6 bước sau:

1. **Lựa chọn chủ đề (Cân bằng giữa Chiều rộng và Chiều sâu):** 
   - Đọc [`LEARNED.md`](file:///d:/Projects/Clone/Eco%20Learning%20(GEMINI)/LEARNED.md) và [`RELATE.md`](file:///d:/Projects/Clone/Eco%20Learning%20(GEMINI)/RELATE.md).
   - **ƯU TIÊN HÀNG ĐẦU (Chiều rộng):** Ưu tiên bao phủ các khái niệm nền tảng thuộc các nhóm chủ đề chính chưa học hoặc lâu chưa quay lại (vi mô, vĩ mô, ngân hàng, lạm phát/lãi suất, tài chính cá nhân, đầu tư, doanh nghiệp, lịch sử kinh tế...) để xây dựng bức tranh toàn cảnh rộng.
   - **THỈNH THOẢNG CỦNG CỐ (Chiều sâu - Reinforcement):** Không chọn chủ đề liên tục theo dạng DFS (đi quá sâu vào một nhánh ngay lập tức). Sau một khoảng thời gian mở rộng kiến thức rộng, thỉnh thoảng mới quay lại chọn 1 khái niệm trong `RELATE.md` để đi sâu hơn và củng cố (reinforce) bài học trước đó.
2. **Soạn bài học:** Biên soạn nội dung chuẩn xác, sâu sắc theo đúng tiêu chuẩn nội dung và prompt quy định tại Mục 3 bên dưới.
3. **Lưu file bài học:**
   - Xác định tên thư mục Nhánh B dạng tiếng Anh không dấu `kebab-case` (ví dụ: `corporate-and-markets`, `monetary-and-banking`, `macroeconomics`).
   - Nếu thư mục B chưa tồn tại trong `topics/`, tạo thư mục mới.
   - Lưu bài học vào `topics/<category-B>/<lesson-name-in-english>.md`.
4. **Cập nhật README của Thư mục B:**
   - Tạo mới hoặc cập nhật file `topics/<category-B>/README.md` để thêm tiêu đề bài học mới, ngày tạo, đường dẫn và đoạn tóm tắt cơ chế (3-5 câu).
5. **Cập nhật nhật ký LEARNED.md:**
   - Thêm một dòng mới vào bảng trong [`LEARNED.md`](file:///d:/Projects/Clone/Eco%20Learning%20(GEMINI)/LEARNED.md) với thông tin: Ngày, Category (Folder B), Tên bài học, Đường dẫn file và Ý chính cốt lõi.
6. **Cập nhật Hàng chờ RELATE.md:**
   - Nếu bài học vừa viết nằm trong danh sách `RELATE.md`, đánh dấu trạng thái thành `✅ Đã học` và điền đường dẫn bài mới.
   - Trích xuất 2 đến 4 khái niệm từ mục **"### Liên kết kiến thức"** của bài học mới và thêm vào bảng trong `RELATE.md` với trạng thái `⏳ Chưa học` để tích lũy cho việc củng cố chiều sâu trong tương lai.

---

## 3. Prompt Yêu cầu Biên soạn Bài học Kinh tế (Prompt Gốc)

Hãy gửi cho tôi một bài học về kinh tế, tài chính hoặc cách nền kinh tế vận hành.

## Mục tiêu

Nội dung cần giúp tôi:

* Hiểu bản chất của các hiện tượng kinh tế và tài chính.
* Đọc và hiểu tin tức kinh tế tốt hơn.
* Áp dụng kiến thức vào quản lý tài chính cá nhân.
* Mở rộng dần vốn khái niệm về kinh tế, tài chính, ngân hàng, doanh nghiệp và đầu tư.
* Xây dựng kiến thức lâu dài, không giới hạn trong một khóa học có thời hạn.

Tôi đã có kiến thức cơ bản về tiền tệ, lãi suất, cung cầu và tài chính cá nhân. Vì vậy, không cần luôn bắt đầu từ mức nhập môn tuyệt đối, nhưng cũng không được mặc định rằng tôi đã học chính quy về kinh tế.

## Cách lựa chọn chủ đề

Mỗi ngày chọn một chủ đề chính thuộc một trong các nhóm sau:

* Kinh tế vi mô.
* Kinh tế vĩ mô.
* Tiền tệ và ngân hàng.
* Lạm phát, lãi suất và tỷ giá.
* Tài chính cá nhân.
* Chứng khoán và đầu tư.
* Doanh nghiệp và thị trường.
* Kinh tế Việt Nam.
* Kinh tế thế giới.
* Lịch sử kinh tế.
* Kinh tế hành vi.
* Các cuộc khủng hoảng kinh tế và tài chính.
* Những cơ chế kinh tế đứng sau các sự kiện đời sống thường ngày.

Hạn chế các bài tập trung chủ yếu vào chính sách công.

Việc chọn chủ đề cần có yếu tố ngẫu nhiên để tạo sự đa dạng, nhưng không được hoàn toàn rời rạc. Hãy duy trì một lộ trình ngầm:

* Thỉnh thoảng nối bài mới với kiến thức đã trình bày trước đó.
* Tránh lặp lại cùng một nội dung trong thời gian ngắn.
* Dần mở rộng từ khái niệm nền tảng sang các cơ chế phức tạp hơn.
* Có thể quay lại một chủ đề cũ ở mức sâu hơn hoặc dưới một góc nhìn khác.
* Luân phiên hợp lý giữa vi mô, vĩ mô, tài chính cá nhân, ngân hàng, đầu tư, doanh nghiệp và lịch sử kinh tế.

## Yêu cầu về chiều sâu

Ưu tiên giải thích bản chất thay vì chỉ giới thiệu định nghĩa.

Không được oversimplify đến mức làm sai lệch cơ chế thực tế. Khi một vấn đề có nhiều lớp, hãy trình bày từng lớp theo thứ tự từ dễ hiểu đến sâu hơn.

Mỗi bài nên trả lời rõ các câu hỏi:

1. Khái niệm hoặc hiện tượng này là gì?
2. Nó xuất hiện do đâu?
3. Cơ chế hoạt động của nó như thế nào?
4. Những chủ thể nào tham gia và động cơ của họ là gì?
5. Yếu tố nào khiến kết quả thay đổi?
6. Nó liên hệ với những khái niệm kinh tế nào khác?
7. Những hiểu lầm phổ biến về vấn đề này là gì?
8. Trong thực tế, cơ chế có điểm nào phức tạp hơn mô hình lý thuyết?

Không chỉ nói rằng hai yếu tố “có liên quan”. Hãy giải thích chuỗi nguyên nhân và kết quả ở giữa.

Ví dụ, thay vì chỉ nói “lãi suất tăng làm giá cổ phiếu giảm”, hãy giải thích các kênh truyền dẫn như chi phí vốn, chiết khấu dòng tiền, hành vi nhà đầu tư, sức khỏe doanh nghiệp và sự dịch chuyển giữa các loại tài sản.

## Cách trình bày

Mỗi bài có thể dài hoặc ngắn tùy theo độ phức tạp của chủ đề. Không cần ép mọi bài vào cùng một độ dài.

Bố cục ưu tiên:

### 1. Chủ đề hôm nay

Nêu tên chủ đề bằng tiếng Việt và thuật ngữ tiếng Anh tương ứng.

### 2. Vấn đề cốt lõi

Giới thiệu ngắn gọn câu hỏi trung tâm mà bài học sẽ giải thích.

### 3. Giải thích cơ chế

Trình bày chi tiết, có hệ thống và theo chuỗi logic.

Sử dụng công thức, bảng, số liệu giả định hoặc đồ thị đơn giản khi chúng thực sự giúp làm rõ bản chất. Tôi thoải mái với nội dung định lượng, vì vậy không cần né tránh công thức.

Mỗi công thức cần giải thích ý nghĩa kinh tế, không chỉ trình bày phép tính.

### 4. Ví dụ trực quan

Dùng một ví dụ cụ thể có số liệu hoặc tình huống rõ ràng để minh họa.

Ưu tiên các ví dụ liên quan đến:

* Gửi tiết kiệm.
* Lãi suất ngân hàng.
* Thẻ tín dụng và thẻ ghi nợ.
* Quản lý dòng tiền cá nhân.
* Lạm phát.
* Tỷ giá.
* Chứng khoán.
* Hoạt động của doanh nghiệp.
* Giá cả hàng hóa.
* Quyết định của người tiêu dùng.
* Các hiện tượng kinh tế tại Việt Nam hoặc quốc tế.

### 5. Tình huống thực tế

Đưa ra một tình huống như:

* Điều gì xảy ra nếu lãi suất tăng?
* Vì sao ngân hàng tăng lãi suất huy động?
* Vì sao một doanh nghiệp có lợi nhuận nhưng vẫn thiếu tiền mặt?
* Vì sao giá hàng hóa giảm nhưng người tiêu dùng chưa chắc mua nhiều hơn?
* Vì sao đồng nội tệ mất giá ảnh hưởng khác nhau đến từng nhóm người?
* Vì sao một chính sách tốt trong lý thuyết có thể tạo kết quả khác trong thực tế?

Sau đó phân tích tình huống thay vì đặt câu hỏi để tôi tự trả lời.

## Ứng dụng trong đời sống

Mỗi bài phải có mục:

### Kiến thức này có ích gì với tôi?

Phần này cần giải thích cách kiến thức có thể giúp tôi:

* Hiểu một bản tin kinh tế.
* Đánh giá một quyết định tài chính cá nhân.
* Hiểu hành vi của ngân hàng, doanh nghiệp, nhà đầu tư hoặc người tiêu dùng.
* Nhận ra rủi ro khi gửi tiết kiệm, vay tiền, đầu tư hoặc chi tiêu.
* Tránh những kết luận kinh tế trực giác nhưng sai.
* Nhìn một hiện tượng tại Việt Nam trong bối cảnh kinh tế quốc tế.

Không được cố biến mọi bài học thành lời khuyên đầu tư. Nếu kiến thức không trực tiếp dẫn đến một hành động tài chính, hãy giải thích nó giúp cải thiện cách tư duy như thế nào.

## Thuật ngữ

Khi xuất hiện một thuật ngữ quan trọng, ghi:

* Tên tiếng Việt.
* Tên tiếng Anh trong ngoặc.
* Định nghĩa theo đúng ngữ cảnh.
* Phân biệt với những khái niệm dễ nhầm lẫn, nếu có.

Ví dụ:

* Thanh khoản (liquidity).
* Cung tiền (money supply).
* Chi phí cơ hội (opportunity cost).
* Lợi suất danh nghĩa (nominal return).
* Lợi suất thực (real return).
* Đường cong lợi suất (yield curve).

Không cần dịch máy móc tất cả từ ngữ. Chỉ giữ thuật ngữ tiếng Anh khi nó có ích cho việc đọc tài liệu hoặc tin tức sau này.

## Tin tức và tính cập nhật

Khi chủ đề liên quan đến số liệu, quy định, lãi suất, thị trường hoặc một sự kiện đang diễn ra, hãy kiểm tra thông tin hiện tại trước khi viết.

Phân biệt rõ:

* Kiến thức lý thuyết ổn định.
* Số liệu hoặc sự kiện thực tế có thể thay đổi theo thời gian.
* Nhận định hoặc cách diễn giải còn gây tranh luận.

Nếu dùng một sự kiện thời sự làm ví dụ, không để bài học biến thành một bản tin ngắn hạn. Hãy dùng sự kiện để giải thích một cơ chế kinh tế có giá trị lâu dài.

## Nguồn tham khảo và độ tin cậy

Mọi thông tin mang tính thực tế, số liệu, sự kiện, quy định, chính sách, lãi suất, diễn biến thị trường hoặc kết luận dựa trên nghiên cứu phải được lấy từ các nguồn uy tín, có độ tin cậy cao và phù hợp với chủ đề.

Ưu tiên nguồn theo thứ tự sau:

1. **Nguồn chính thức và nguồn sơ cấp**

   * Ngân hàng Nhà nước Việt Nam.
   * Tổng cục Thống kê Việt Nam.
   * Bộ Tài chính, Bộ Công Thương và các cơ quan nhà nước có thẩm quyền.
   * Văn bản pháp luật, thông tư, nghị định và báo cáo chính thức.
   * Ngân hàng trung ương các nước.
   * IMF, World Bank, BIS, OECD, WTO và các tổ chức quốc tế có uy tín.
   * Báo cáo tài chính, báo cáo thường niên, hồ sơ công bố thông tin và tài liệu chính thức của doanh nghiệp.
   * Bài nghiên cứu gốc, dữ liệu gốc hoặc tài liệu do chính tổ chức liên quan công bố.

2. **Nguồn học thuật**

   * Giáo trình đại học có uy tín.
   * Bài báo khoa học đã được phản biện.
   * Tạp chí kinh tế, tài chính hoặc ngân hàng có chất lượng.
   * Nghiên cứu từ các trường đại học và viện nghiên cứu đáng tin cậy.

3. **Nguồn báo chí và phân tích chuyên môn**

   * Chỉ sử dụng các hãng tin, báo kinh tế và tổ chức phân tích có uy tín.
   * Ưu tiên bài viết dẫn lại rõ nguồn dữ liệu, tài liệu chính thức hoặc ý kiến chuyên gia có thể kiểm chứng.
   * Không dựa chủ yếu vào tiêu đề báo, bài viết quảng cáo, nội dung tài trợ hoặc nhận định không có bằng chứng.

Không sử dụng làm nguồn chính:

* Blog cá nhân không có chuyên môn rõ ràng.
* Bài đăng mạng xã hội.
* Diễn đàn.
* Nội dung SEO tổng hợp.
* Video hoặc bài viết không dẫn nguồn.
* Website sao chép nội dung từ nguồn khác.
* Nguồn có xung đột lợi ích nhưng không công khai.
* Số liệu không xác định được thời điểm hoặc phương pháp thu thập.

Khi sử dụng nguồn, cần tuân thủ các nguyên tắc sau:

* Ưu tiên nguồn sơ cấp thay vì chỉ dựa vào bài báo tóm tắt nguồn sơ cấp.
* Đối chiếu nhiều nguồn khi thông tin có thể gây tranh cãi hoặc ảnh hưởng lớn đến cách hiểu.
* Kiểm tra ngày công bố và khoảng thời gian mà số liệu phản ánh.
* Không dùng số liệu cũ như thể đó là tình hình hiện tại.
* Phân biệt rõ số liệu thực tế, dự báo, ước tính và quan điểm cá nhân.
* Không suy rộng kết luận của một nghiên cứu vượt quá phạm vi dữ liệu của nghiên cứu đó.
* Khi các nguồn đáng tin cậy đưa ra kết luận khác nhau, trình bày nguyên nhân khác biệt thay vì tự chọn một kết luận duy nhất.

Cuối mỗi bài, thêm mục:

### Nguồn tham khảo

Liệt kê từ 2 đến 5 nguồn quan trọng nhất đã dùng trong bài.

Với mỗi nguồn, ghi rõ:

* Tên cơ quan, tổ chức hoặc tác giả.
* Tên báo cáo, nghiên cứu, dữ liệu hoặc bài viết.
* Ngày hoặc năm công bố.
* Đường dẫn trực tiếp đến nguồn, khi có thể.

Không liệt kê nguồn chỉ để làm bài viết có vẻ đáng tin cậy. Mỗi nguồn được dẫn phải thực sự hỗ trợ cho nội dung trong bài.

Các nhận định hoặc số liệu quan trọng cần được dẫn nguồn ngay tại đoạn liên quan, không chỉ gom toàn bộ nguồn xuống cuối bài.

Nếu bài học chỉ giải thích một lý thuyết kinh tế ổn định và không sử dụng số liệu thời sự, vẫn nên tham khảo ít nhất một giáo trình, tài liệu học thuật hoặc nguồn chính thức đáng tin cậy.

Nếu không tìm được nguồn đủ đáng tin cậy cho một thông tin, phải nói rõ rằng thông tin đó chưa được xác minh và không được trình bày nó như một sự thật chắc chắn.

## Yêu cầu về tính chính xác

* Không khẳng định một mối quan hệ kinh tế luôn đúng nếu nó chỉ đúng trong một số điều kiện.
* Nêu rõ giả định của mô hình.
* Phân biệt tương quan và quan hệ nhân quả.
* Khi có nhiều trường phái hoặc cách giải thích, trình bày quan điểm chính một cách cân bằng.
* Không đưa lời khuyên tài chính cá nhân hóa khi chưa có đủ dữ liệu.
* Không dùng các câu sáo rỗng như “hãy đa dạng hóa đầu tư” nếu không giải thích cơ chế và điều kiện áp dụng.
* Không trình bày định nghĩa qua loa rồi chuyển ngay sang chủ đề khác.

## Kết thúc bài

Cuối mỗi bài, thêm hai phần ngắn:

### Liên kết kiến thức

Nêu từ 2 đến 4 khái niệm có liên quan mà bài học hôm nay giúp mở đường để hiểu.

### Điều đáng nhớ nhất

Tóm tắt một đến ba ý cốt lõi, tập trung vào cơ chế thay vì chỉ nhắc lại định nghĩa.

Không đặt câu hỏi kiểm tra, không giao bài tập và không yêu cầu tôi trả lời. Mục tiêu của nội dung hằng ngày là để tôi đọc, hiểu và tích lũy kiến thức lâu dài.

---

## 4. Giao thức Chống Bịa Thông tin & Chống Sửa Tung

### A. Giao thức Chống Bịa Thông tin (Anti-Fabrication Protocol)

Trước khi ghi bất kỳ nội dung nào vào bài học, Agent PHẢI tuân thủ:

#### 1. Phân loại thông tin theo độ rủi ro
- **Định tính / cơ chế** (công thức, logic nhân-quả, định nghĩa) → độ tin cậy cao, có thể viết từ kiến thức nền mà không cần xác minh thêm.
- **Định lượng / thời sự** (số liệu CPI, lãi suất, tỷ giá, GDP theo năm cụ thể, tên báo cáo...) → độ rủi ro cao, **PHẢI** gắn nhãn nguồn + thời điểm rõ ràng.

#### 2. Không bịa số liệu để "cho tròn ví dụ"
- Cần ví dụ minh họa → dùng số liệu **giả định, gắn nhãn rõ** ("giả sử doanh nghiệp X có doanh thu...") thay vì trình bày như số liệu thực tế không nguồn.
- Dùng số liệu thực tế → phải nêu năm/quý + nguồn cụ thể (NHNN, GSO, IMF, World Bank, BCTC công ty...).
- Không chắc chắn về độ chính xác của một số liệu → đánh dấu ngay trong file bằng `[CẦN XÁC MINH LẠI]` thay vì bỏ qua hoặc đoán đại.

#### 3. Không tự tạo nguồn tham khảo giả
- Mục "Nguồn tham khảo" chỉ liệt kê tổ chức/loại báo cáo mà Agent có cơ sở hợp lý để tin là tồn tại, **không** bịa tên báo cáo cụ thể, số liệu, hay đường link không xác thực được.
- Nếu có công cụ tra cứu (web search), ưu tiên xác minh trước khi ghi số liệu định lượng quan trọng vào bài.

#### 4. Không chắc chắn — nói rõ, không đoán
- Ưu tiên diễn đạt kiểu "cơ chế này thường được minh họa qua ví dụ như..." thay vì khẳng định một sự kiện/số liệu cụ thể mà Agent không chắc.

---

### B. Giao thức Chống Sửa Tung (Scope Control Protocol)

#### 1. Giới hạn phạm vi file mỗi phiên
Mỗi phiên biên soạn chỉ được tạo/sửa đúng 4 loại file:
- 1 file bài học mới: `topics/<category>/<lesson>.md`
- 1 file README nhóm: `topics/<category>/README.md`
- `LEARNED.md`
- `RELATE.md`

Không tự ý sửa file ngoài danh sách này trong cùng phiên, kể cả khi "tiện thể" phát hiện lỗi ở nơi khác.

#### 2. Chỉ ghi thêm (append-only) vào log
- `LEARNED.md` và `RELATE.md`: chỉ **thêm dòng mới**, không sửa/xóa dòng cũ — trừ khi người dùng yêu cầu rõ ràng (ví dụ: "sửa lại dòng về bài CCC").
- Cấm Agent tự ý "dọn dẹp" hay viết lại các dòng cũ để "gọn hơn" nếu không được yêu cầu.

#### 3. Phát hiện lỗi ở bài cũ → không tự sửa, chỉ ghi nhận
Nếu trong lúc soạn bài mới phát hiện bài cũ có sai sót, Agent **không** tự sửa file cũ. Thay vào đó, ghi một dòng vào `ISSUES.md` (tạo mới nếu chưa có), theo định dạng:

```
[Ngày] - [Tên bài] - [Mô tả lỗi nghi ngờ] - [Cần người dùng xác nhận]
```

#### 4. Xác nhận trước khi hoàn tất (diff summary)
Trước khi kết thúc phiên, Agent liệt kê tóm tắt:
- File nào được tạo mới
- File nào được sửa, và sửa đúng những dòng nào (không phải mô tả chung chung "đã cập nhật")

---

### C. Prompt mẫu — dùng đầu mỗi phiên biên soạn bài học

```
Bạn là AI Agent quản trị kho tri thức Eco Learning. Trước khi biên soạn bài học mới, hãy:

1. Đọc LEARNED.md và RELATE.md để chọn chủ đề (ưu tiên breadth-first,
   xen kẽ 1 bài củng cố sau mỗi 3-4 bài mới).
2. Biên soạn bài học theo đúng 9 mục chuẩn trong AGENTS.md.
3. Tuân thủ NGHIÊM NGẶT Giao thức Chống Bịa Thông tin (Mục A) —
   không bịa số liệu, không bịa nguồn, đánh dấu rõ [CẦN XÁC MINH LẠI]
   nếu không chắc chắn.
4. Tuân thủ NGHIÊM NGẶT Giao thức Chống Sửa Tung (Mục B) —
   chỉ sửa đúng 4 file được phép, chỉ append vào LEARNED.md/RELATE.md,
   không tự sửa bài cũ, ghi lỗi nghi ngờ vào ISSUES.md.
5. Trước khi kết thúc, in ra bảng tóm tắt:
   - File đã tạo mới: ...
   - File đã sửa và dòng cụ thể: ...
   - Các điểm [CẦN XÁC MINH LẠI] (nếu có): ...
```

