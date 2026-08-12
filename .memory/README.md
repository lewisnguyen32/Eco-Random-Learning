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
├── antigravity_memory.md   # Tầng 2: Quy tắc Vận hành Tinh chế cho Antigravity Agent
└── codex_memory.md        # Tầng 2: Quy tắc Vận hành Tinh chế cho Codex Agent (khi Codex được sử dụng)
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

### 2. `antigravity_memory.md` & `codex_memory.md` (Distilled Operational Memory)
* **Bản chất:** Chứa các quy tắc vận hành tinh chế (*distilled operational rules*) dành riêng cho từng Agent (Antigravity hoặc Codex khi được dùng).
* **Đặc điểm:**
  - Không sao chép nguyên văn toàn bộ nhật ký lỗi chi tiết.
  - Ngắn gọn, súc tích, tối ưu token.
  - Trình bày dạng các chỉ dẫn có điều kiện ngữ cảnh (*context-dependent rules*), tránh phát biểu tuyệt đối thiếu căn cứ.

### 3. `AGENTS.md` (Protocol Master & Authority Framework)
* **Agent-Guided Retrieval:** Chứa quy trình tra cứu có định hướng (deliberate agent-guided retrieval, KHÔNG phải tự động bằng vector DB / RAG code).
* **Phân tách Thẩm quyền (Authority Separation):** Phân định rõ *Behavioral Authority* (bộ nhớ chỉ đạo quy trình làm việc) vs *Epistemic Authority* (nguồn sơ cấp/uy tín chỉ đạo sự thật dữ liệu).

---

## ⚖️ Phân tách Thẩm quyền: Behavioral vs Epistemic Authority

> **"Memory controls reasoning behavior, not factual truth."**

1. **Behavioral Authority (Quy trình Vận hành):**
   `AGENTS.md` $\rightarrow$ `agent_memory.md` định hướng Agent phải thực hiện task như thế nào (phải kiểm tra balance sheet, phải dán nhãn model vs reality, phải self-check).
2. **Epistemic Authority (Nguồn Sự thật Dữ liệu):**
   Nguồn sơ cấp uy tín (NHNN, GSO, Fed, IMF, BIS, BCTC) $\rightarrow$ Nội dung bài học (`topics/`) $\rightarrow$ Nhật ký lỗi (`knowledge_corrections.md`).

Khi bộ nhớ mâu thuẫn với bằng chứng sơ cấp uy tín, Agent **không** ưu tiên bộ nhớ chỉ vì vị trí tầng. Agent phải nhận diện xung đột $\rightarrow$ kiểm tra nguồn $\rightarrow$ giải quyết xung đột $\rightarrow$ cập nhật lại bộ nhớ.
