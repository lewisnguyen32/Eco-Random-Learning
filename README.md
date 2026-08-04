# Eco Learning - Kho lưu trữ & Lộ trình Tích lũy Kiến thức Kinh tế

Chào mừng bạn đến với **Eco Learning** — hệ thống tích lũy kiến thức kinh tế, tài chính, ngân hàng và đầu tư dài hạn cá nhân hóa.

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
├── AGENTS.md               # Quy định & Prompt chỉ dẫn master cho AI Agent
├── LEARNED.md              # Nhật ký học tập (Lịch sử & Mã ID bài học)
├── RELATE.md               # Hàng chờ các khái niệm liên quan (Dùng để củng cố định kỳ)
├── GLOSSARY.md             # Chỉ mục thuật ngữ tra cứu nhanh A-Z
├── .memory/                # Bộ nhớ làm việc tạm thời cho Multi-Agent (Antigravity, Codex...)
│   ├── README.md           # Hướng dẫn sử dụng bộ nhớ tạm
│   ├── antigravity_memory.md # Bộ nhớ tạm cho Antigravity (Gemini)
│   └── codex_memory.md     # Bộ nhớ tạm cho Codex
└── topics/                 # Thư mục Nhánh A duy nhất chứa toàn bộ các chủ đề
    └── <category-B>/       # Thư mục chủ đề B (ví dụ: corporate-and-markets)
        ├── README.md       # Danh mục & tóm tắt các bài học trong chủ đề B này
        └── <lesson-name>.md # Bài học .md chi tiết (chứa YAML Frontmatter chuẩn)
```

---

## 🔍 Chiến lược Học tập & Hệ thống Tích lũy

Dự án áp dụng mô hình học tập **Phân tầng Xoắn ốc (Spiral Learning Model)** kết hợp **Ghi nhớ Chủ động (Active Recall)**:

1. **Phân tầng Xoắn ốc & Khóa Prerequisite:**
   - **Tầng 1 - Core Anchors (Nền tảng):** Lãi suất, Lạm phát, Cung tiền & Thanh khoản. Bắt buộc xây móng vững trước.
   - **Tầng 2 - Behavioral Layer (Hành vi):** *Behavioral Finance* (Tâm lý học hành vi) được học sớm/song song để giải thích phản ứng tâm lý con người với kinh tế.
   - **Tầng 3 - Application Layer (Ứng dụng):** BĐS Việt Nam, Tỷ giá VND, Thuế & Quy hoạch TCCN... **Khóa điều kiện tiên quyết**: Chỉ mở bài Tầng 3 khi bài móng Tầng 1 tương ứng đã hoàn thành trong [`LEARNED.md`](LEARNED.md).
2. **Ghi nhớ Chủ động (Active Recall):**
   - **Mở đầu bài (Delayed Active Recall):** Ôn tập ngắt quãng lại 1 ý cốt lõi của bài học cũ từ 1-2 tuần trước.
   - **Cuối bài (Góc Phản xạ & Thang 1-5):** Đưa ra 1 câu hỏi gợi mở phản xạ tự nhiên (tự tóm tắt / liên hệ thực tế) kèm thang tự đánh giá độ tự tin (1-5) để ưu tiên lịch củng cố.
3. **Tra cứu & Metadata chuẩn:**
   - [Mã ID bài học & Nhật ký](LEARNED.md): Ghi nhận toàn bộ tiến trình theo ID (`CORP-001`, `MACRO-001`...).
   - [Chỉ mục Thuật ngữ GLOSSARY.md](GLOSSARY.md): Tra cứu nhanh thuật ngữ A-Z và đường dẫn bài học gốc.
   - **Versioning cho Thuế & Pháp luật:** Các bài học về luật/thuế có trường `applicable_year` và `last_verified` để kiểm soát dữ liệu khi luật thay đổi.
