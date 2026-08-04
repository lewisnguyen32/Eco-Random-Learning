# Eco Learning - Kho lưu trữ & Lộ trình Tích lũy Kiến thức Kinh tế

Chào mừng bạn đến với **Eco Learning** — hệ thống tích lũy kiến thức kinh tế, tài chính, ngân hàng và đầu tư dài hạn.

## 🎯 Mục tiêu
* **Hiểu bản chất cơ chế:** Giải thích chuỗi nguyên nhân - kết quả của các hiện tượng kinh tế thay vì chỉ đưa ra định nghĩa.
* **Đọc hiểu tin tức:** Nâng cao khả năng phân tích bản tin tài chính, báo cáo lưu chuyển tiền tệ và chính sách vĩ mô.
* **Ứng dụng thực tế:** Quản trị tài chính cá nhân, nhận diện rủi ro đầu tư và đánh giá sức khỏe doanh nghiệp.
* **Tích lũy lâu dài:** Xây dựng vốn khái niệm mở rộng liên tục, không giới hạn trong thời gian hay khung giáo trình cố định.

---

## 📂 Cấu trúc Kho lưu trữ

Hệ thống được tổ chức phân cấp linh hoạt:

```
Eco Learning (GEMINI)/
├── README.md               # File tổng quan dự án (File này)
├── AGENTS.md               # Prompt chỉ dẫn & Quy định vận hành dành cho AI Agent
├── LEARNED.md              # Bảng nhật ký học tập (Lịch sử các bài học đã hoàn thành)
├── RELATE.md               # Hàng chờ các khái niệm liên quan (Dùng để củng cố kiến thức theo định kỳ)
└── topics/                 # Thư mục Nhánh A duy nhất chứa toàn bộ các chủ đề
    └── <category-B>/       # Thư mục chủ đề B (tiếng Anh không dấu, ví dụ: corporate-and-markets)
        ├── README.md       # Danh mục & tóm tắt các bài học trong chủ đề B này
        └── <lesson-name>.md # Bài học .md chi tiết
```

---

## 🔍 Chiến lược Học tập & Cách Tra cứu

Dự án áp dụng chiến lược **Bao phủ chiều rộng trước (Breadth-First)** kết hợp với **Củng cố định kỳ chiều sâu (Spaced Reinforcement)**:

1. **Bao phủ chiều rộng:** Ưu tiên luân phiên các bài học nền tảng thuộc nhiều nhóm chủ đề chính khác nhau để tạo bức tranh toàn cảnh về nền kinh tế.
2. **Củng cố chiều sâu:** File [`RELATE.md`](file:///d:/Projects/Clone/Eco%20Learning%20(GEMINI)/RELATE.md) lưu trữ các khái niệm mở ra từ mục *Liên kết kiến thức* của các bài trước. Sau một số bài mở rộng chiều rộng, Agent sẽ thỉnh thoảng quay lại chọn 1 khái niệm trong `RELATE.md` để củng cố và đào sâu kiến thức.
3. **Lịch sử bài đã học:** Mở file [`LEARNED.md`](file:///d:/Projects/Clone/Eco%20Learning%20(GEMINI)/LEARNED.md) để xem danh sách toàn bộ các bài học đã hoàn thành.
4. **Tóm tắt theo chủ đề:** Mở file `README.md` trong thư mục `topics/<category-B>/` để xem tóm tắt các bài học thuộc chủ đề đó.
