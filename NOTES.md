# Ghi chú: kiểm chứng thông tin và quản trị hàng chờ

Cập nhật sau rà soát ngày 22/09/2026. Đây là phân tích và đề xuất, không tự thay đổi quy trình trong AGENTS.md.

## 1. Tên nguồn đúng chưa chứng minh nội dung trích dẫn đúng

Một tài liệu có thật có thể bị dẫn sai tác giả, năm, chương hoặc nội dung. Việc tự ghi “đã xác minh” không thay thế việc đối chiếu đoạn nguồn liên quan.

Đợt rà soát này đã thay các nguồn chỉ trỏ trang chủ hoặc không xác minh được bằng tài liệu cụ thể. Ví dụ, tên “Money and Missed Conceptions” từng gắn với Fed St. Louis chưa tìm được tài liệu tương ứng; việc không tìm thấy không đủ để khẳng định chắc chắn tài liệu không tồn tại.

**Phân tầng kiểm tra:**

| Loại nhận định | Cách kiểm tra phù hợp |
| :--- | :--- |
| Đại số và ví dụ giả định | Nêu giả định, kiểm tra đơn vị và tính lại độc lập. |
| Cơ chế thể chế, hạch toán | Đối chiếu tài liệu chính thức; tách chủ thể, loại giao dịch và điều kiện vận hành. |
| Dữ liệu lịch sử, luật, thông tin hiện hành | Nguồn trực tiếp, kỳ dữ liệu, ngày công bố/hiệu lực; kiểm tra văn bản thay thế. |
| Diễn giải thực nghiệm | Đối chiếu nghiên cứu gốc và phạm vi mẫu; không gọi tương quan là nhân quả. |

Không cần bắt mọi công thức ổn định phải có truy vấn web riêng. Nhưng dẫn một nguồn để chứng minh nhận định phải kiểm tra nguồn thực sự hỗ trợ nhận định đó. Nếu chỉ đọc được kết quả tìm kiếm của nguồn chính thức do lỗi truy cập, cần ghi giới hạn bằng chứng.

## 2. Kích thước glossary: đo trước khi quyết định chia nhỏ

Bản cũ ước lượng số dòng và số token như thể có quan hệ cố định. Điều đó không hợp lý: số token còn phụ thuộc độ dài định nghĩa, tiếng Việt, URL và tokenizer.

[Theoretical Model] Nếu mỗi bài thêm trung bình a thuật ngữ **mới, không trùng**, sau n bài có khoảng $G_n=G_0+an$ thuật ngữ. Đây là mô hình tăng trưởng theo giả định, không phải dự báo đo được.

Việc chia glossary theo nhóm có thể hữu ích khi chi phí tìm/đọc tăng rõ rệt. Chưa có cơ sở để coi một ngưỡng như 150 dòng là tối ưu; nên đo dung lượng, tần suất tra cứu và tỷ lệ thuật ngữ trùng trước khi đổi cấu trúc.

## 3. RELATE là quan hệ giữa bài và khái niệm, không phải số chủ đề duy nhất

Một khái niệm có thể được gợi mở từ nhiều bài. Một bài học mới cũng có thể giải quyết nhiều dòng chờ, kể cả khi không mang nhãn “bài củng cố”. Vì vậy không thể suy ra tốc độ hoàn thành chỉ từ lịch “mỗi 3–4 bài mới có một bài củng cố”.

[Accounting Identity của mô hình hàng chờ] Đặt Q là số **khái niệm duy nhất chưa xử lý**:

$$Q_{n+1}=\max(0,Q_n+A_n-C_n-R_n)$$

A là số khái niệm mới thực sự được thêm, C là số được học, R là số được rút khỏi hàng chờ hoạt động. Các biến phải được định nghĩa không đếm trùng. Nếu việc hoàn thành một bài đóng ba dòng cùng khái niệm, C theo khái niệm chỉ tăng một.

[Theoretical Model] Nếu giả định A = 3, C trung bình = 0,25 và R = 0 thì tăng ròng là 2,75 khái niệm/bài, tức 11 sau bốn bài. Kết luận này **chỉ đúng trong giả định đó**. Không chứng minh hàng chờ thực tế chắc chắn tăng vô hạn, vì chủ đề có thể trùng, được học chung hoặc không tiếp tục được thêm mãi.

## 4. Các lựa chọn quản trị chưa triển khai

- Theo dõi số khái niệm duy nhất, không chỉ đếm dòng quan hệ.
- Hạn chế thêm mục trùng và đánh dấu phạm vi đã học rõ ràng.
- Có thể giới hạn hàng chờ hoạt động hoặc chuyển mục ít ưu tiên vào kho lưu, nếu người dùng muốn.
- Giảm số mục thêm mỗi bài chỉ làm giảm tốc độ tăng; không bảo đảm hàng chờ ổn định nếu tốc độ thêm vẫn lớn hơn tốc độ xử lý.

Giữ cấu trúc Markdown hiện tại trong đợt sửa kiến thức này. Không tự tạo cơ chế lưu trữ hoặc lịch ôn tập tự động từ các đề xuất trên.
