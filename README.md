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
├── LEARNED.md              # Bảng nhật ký học tập (Lịch sử & Mã ID bài học)
├── RELATE.md               # Hàng chờ các khái niệm liên quan (Dùng để củng cố kiến thức theo định kỳ)
├── GLOSSARY.md             # Chỉ mục thuật ngữ tra cứu nhanh
└── topics/                 # Thư mục Nhánh A duy nhất chứa toàn bộ các chủ đề
    └── <category-B>/       # Thư mục chủ đề B (tiếng Anh không dấu, ví dụ: corporate-and-markets)
        ├── README.md       # Danh mục & tóm tắt các bài học trong chủ đề B này
        └── <lesson-name>.md # Bài học .md chi tiết (chứa YAML Frontmatter chuẩn)
```

---

## 🔍 Chiến lược Học tập & Hệ thống Tích lũy

Dự án áp dụng mô hình học tập **Xoắn ốc (Spiral Learning Model)** kết hợp **Ghi nhớ Chủ động (Active Recall)**:

1. **Tập trung Khái niệm Hạt nhân (Core Anchors):** Ưu tiên đào sâu các khái niệm nền có độ kết nối cao nhất (Lãi suất, Lạm phát, Cung tiền, Thanh khoản) để làm móng trước khi xoay rộng sang các chủ đề ứng dụng.
2. **Mở rộng theo mô hình Xoắn ốc:** Xoay quanh móng hạt nhân sang các mảng thực tế tại Việt Nam (Bất động sản, Tỷ giá VND, Thuế & Quy hoạch TCCN, Tâm lý đầu tư, Ngân hàng, Doanh nghiệp...).
3. **Củng cố định kỳ (Spaced Reinforcement):** Thỉnh thoảng lấy khái niệm từ [RELATE.md](RELATE.md) để kết nối lại các bài học đã qua.
4. **Ghi nhớ Chủ động (Active Recall):** Cuối mỗi bài học có mục *Góc Phản xạ* gợi mở 1 câu hỏi tự tóm tắt/liên hệ thực tế nhẹ nhàng (không áp lực bài tập).
5. **Tra cứu & Metadata chuẩn:**
   - [Mã ID bài học & Nhật ký](LEARNED.md): Ghi nhận toàn bộ tiến trình theo ID (`CORP-001`, `MACRO-001`...).
   - [Chỉ mục Thuật ngữ GLOSSARY.md](GLOSSARY.md): Tra cứu nhanh thuật ngữ A-Z và đường dẫn bài học gốc.
