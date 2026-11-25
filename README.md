# Eco Learning

[![Bắt đầu đọc](https://img.shields.io/badge/🧭_Bắt_đầu_đọc-0f766e?style=for-the-badge)](READING-ORDER.md)

Kho tự học kinh tế, tài chính, ngân hàng và đầu tư bằng tiếng Việt.

[Nhật ký bài học](LEARNED.md) · [Khái niệm liên quan](RELATE.md) · [Thuật ngữ](GLOSSARY.md) · [Ghi chú cá nhân](NOTES.md) · [Quy định biên soạn](AGENTS.md) · [Bản đồ kiến thức](KNOWLEDGE_MAP.md)

## Bạn sẽ học gì?

- Hiểu vì sao một hiện tượng kinh tế xảy ra bằng cách lần theo từng bước từ nguyên nhân đến hệ quả.
- Đọc và phân tích bản tin tài chính, báo cáo lưu chuyển tiền tệ và tin về chính sách vĩ mô.
- Vận dụng kiến thức để quản lý tài chính cá nhân, nhận diện rủi ro đầu tư và đánh giá sức khỏe doanh nghiệp.
- Mở rộng vốn khái niệm lâu dài theo nhịp và mối quan tâm của mình.

## Cách học

Lộ trình theo mô hình xoắn ốc (*Spiral Learning Model*). Những khái niệm đã học sẽ trở lại khi cần giải thích một tình huống mới.

1. **Nền tảng.** Các bài nền xoay quanh lãi suất, lạm phát, cung tiền và thanh khoản.
2. **Hành vi.** Có thể đọc tài chính hành vi (*Behavioral Finance*) song song với các bài nền để hiểu cách con người ra quyết định kinh tế.
3. **Ứng dụng.** Các chủ đề gồm bất động sản Việt Nam, tỷ giá VND, thuế và lập kế hoạch tài chính cá nhân. Mỗi bài ứng dụng chỉ mở sau khi bài nền tương ứng đã hoàn thành và có trong [nhật ký](LEARNED.md).

Bài củng cố mở đầu bằng việc thử nhớ lại một ý từ bài đã đọc cách đó 1–2 tuần (*Delayed Active Recall*). Cuối mỗi bài có một câu hỏi để tự tóm tắt hoặc liên hệ thực tế (*Active Recall*). Thang tự đánh giá độ tự tin từ 1 đến 5 giúp ưu tiên bài cần ôn lại.

## Tra cứu trong kho

Nhật ký dùng mã như `CORP-001` hay `MACRO-001` để theo dõi các bài đã học. Bảng thuật ngữ có định nghĩa ngắn và đường dẫn về bài gốc. Với chủ đề thuế và pháp luật, `applicable_year` ghi năm áp dụng, còn `last_verified` ghi ngày xác minh gần nhất.

```text
Eco Learning/
├── README.md                   # Tổng quan dự án
├── READING-ORDER.md            # Lộ trình cho người đọc lần đầu
├── KNOWLEDGE_MAP.md            # Bản đồ lĩnh vực và độ bao phủ
├── LEARNED.md                  # Nhật ký, mã bài và thứ tự theo điều kiện tiên quyết
├── RELATE.md                   # Hàng chờ các khái niệm để củng cố định kỳ
├── GLOSSARY.md                 # Chỉ mục thuật ngữ A–Z
├── NOTES.md                    # Ghi chú kiểm chứng và các việc cần làm
├── AGENTS.md                   # Quy định biên soạn
├── knowledge-map/              # Danh mục concept, quan hệ và nguồn đối chiếu
├── .memory/                    # Bộ nhớ phục vụ biên soạn
│   ├── README.md               # Quy trình và vai trò của ba tầng bộ nhớ
│   ├── knowledge_corrections.md # Nhật ký đính chính và bài học tổng quát
│   ├── antigravity_memory.md   # Quy tắc vận hành của Antigravity
│   └── codex_memory.md         # Quy tắc vận hành của Codex
└── topics/                     # Toàn bộ nhóm chủ đề
    └── <category>/             # Tên nhóm bằng tiếng Anh, ví dụ corporate-and-markets
        ├── README.md           # Danh mục và tóm tắt các bài trong nhóm
        └── <lesson-name>.md    # Bài học với YAML frontmatter
```

## Cách biên soạn

Quy trình năm bước bắt đầu bằng việc ghi lỗi vào `.memory/`, rút ra bài học chung và cập nhật quy tắc biên soạn. Hai bước sau là tra lại quy tắc liên quan trước khi viết và tự kiểm tra trước khi hoàn tất.

Phần mô hình giáo trình nêu giả định và kết quả. Phần cơ chế thực tế giải thích cách các bên tham gia vận hành và những điều kiện có thể làm kết quả thay đổi.

## Phạm vi sử dụng

Toàn bộ nội dung trong kho lưu trữ này được tổng hợp và biên soạn bởi AI phục vụ mục đích nghiên cứu và tích lũy kiến thức cá nhân, không phải là giáo trình chính thống hay khuyến nghị tài chính chính thức.
