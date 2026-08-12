# Agent Memory & Learning System (.memory/)

Thư mục này chứa **Hệ thống Bộ nhớ và Học tập dành cho AI Agent (Agent Memory & Learning System)** trong dự án **Eco Learning**.

Khác với các tài liệu lưu trữ tri thức bài học dành cho người đọc (`LEARNED.md`, `RELATE.md`, `GLOSSARY.md` và thư mục `topics/`), thư mục `.memory/` lưu trữ **bộ nhớ phía Agent (agent-side memory)** nhằm mục đích:
* Ghi nhận các sự cố sai lệch kiến thức/tư duy đã được phát hiện và sửa chữa.
* Trích xuất các **Bài học Tư duy Tổng quát hóa (Generalizable Lessons)**.
* Duy trì các **Quy tắc Vận hành Tinh chế (Distilled Operational Rules)** để ngăn ngừa lỗi cùng loại trong tương lai.

---

## 🏗️ Kiến trúc Bộ nhớ 3 Tầng (3-Layer Architecture)

```text
.memory/
├── README.md               # Hướng dẫn hệ thống & quy trình vận hành bộ nhớ (File này)
│
├── knowledge_corrections.md # Tầng 1: Nhật ký Lỗi & Bài học Tổng quát hóa (Long-Term Error Memory)
│
├── antigravity_memory.md   # Tầng 2: Bộ nhớ Vận hành Tinh chế cho Antigravity Agent (Operational Memory)
└── codex_memory.md        # Tầng 2: Bộ nhớ Vận hành Tinh chế cho Codex Agent (Operational Memory)
```

---

## 📌 Vai trò Chi tiết của Các Tầng Bộ nhớ

### 1. `knowledge_corrections.md` (Long-Term Error Memory / Learning Log)
* **Bản chất:** Lưu trữ toàn bộ lịch sử sai sót kiến thức đã được rà soát và sửa đổi.
* **Cấu trúc chuẩn cho mỗi Correction Entry:**
  - **Mã bài học & Tên sự cố**
  - **Lỗi sai / Hiểu lầm cũ (Error / Misconception)**
  - **Kiến thức chuẩn xác (Corrected Understanding)**
  - **Nguyên nhân sai lầm tư duy (Why Reasoning Failed)**
  - **Bài học Tổng quát hóa (Generalizable Lesson)** (ví dụ: `G-001`, `G-002`...)
  - **Dấu hiệu Kích hoạt (Trigger Patterns)**
  - **Nguồn đối chiếu (Verification Source)**
* **Quy tắc cốt lõi:** Một correction entry tốt không chỉ sửa một câu chữ cụ thể, mà phải trích xuất ra bài học tư duy có khả năng tổng quát hóa cho nhiều chủ đề khác nhau (kinh tế vĩ mô, kế toán, ngân hàng, thị trường...).

### 2. `antigravity_memory.md` & `codex_memory.md` (Distilled Operational Memory)
* **Bản chất:** Chứa các quy tắc vận hành tinh chế (*distilled operational rules*) được rút gọn từ các bài học tổng quát.
* **Đặc điểm:**
  - Không sao chép nguyên văn toàn bộ nhật ký lỗi chi tiết.
  - Ngắn gọn, súc tích, tối ưu token.
  - Viết dưới dạng các chỉ dẫn có điều kiện ngữ cảnh (*context-dependent rules*), tránh phát biểu tuyệt đối thiếu căn cứ.
  - Được Agent nạp ở **Step 0** mỗi khi bắt đầu một phiên làm việc.

### 3. `AGENTS.md` (Retrieval & Application Protocol)
* Chứa quy trình 5 bước bắt buộc (**Memory Retrieval & Learning Protocol**) để Agent truy xuất bộ nhớ, tự đánh giá nguy cơ, áp dụng quy tắc làm ràng buộc tư duy, và chạy bảng kiểm tra (*Memory Check*) trước khi hoàn tất bài học.

---

## 🔄 Vòng lặp Học tập của Agent (Correction-to-Rule Loop)

```text
Agent makes mistake / Reviewer corrects error
                    ↓
Correction is recorded in knowledge_corrections.md
                    ↓
Failure pattern is abstracted & General lesson extracted (G-xxx)
                    ↓
Distilled operational rule is updated in agent_memory.md
                    ↓
Relevant rules retrieved on future tasks via AGENTS.md Protocol
                    ↓
Agent applies rules as constraints before writing content
                    ↓
Future mistakes of the same class are prevented
```

---

## ⚠️ Phân định Ranh giới Quan trọng

1. **Memory $\neq$ Repository Knowledge:** `.memory/` lưu trữ quy tắc tư duy phía Agent, không thay thế hoặc duplicate nội dung bài học chính thức trong `topics/`.
2. **Memory $\neq$ Unquestionable Source of Truth:** Bộ nhớ đóng vai trò là **hệ thống hướng dẫn tư duy và phòng ngừa lỗi (reasoning prior / error prevention)**, không thay thế cho việc xác minh nguồn sơ cấp khi có dữ liệu thời sự hay quy định pháp lý mới.
