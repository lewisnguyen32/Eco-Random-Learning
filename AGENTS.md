# Hướng dẫn Vận hành và Quy tắc Biên soạn cho AI Agent (AGENTS.md)

Tài liệu này chứa toàn bộ quy định, tiêu chuẩn nội dung, kiến trúc bộ nhớ và quy trình làm việc dành cho AI Agent khi biên soạn các bài học kinh tế, tài chính và đầu tư trong dự án **Eco Learning**.

---

## 1. Cấu trúc Kho lưu trữ & Hệ thống Agent Memory

Dự án được tổ chức theo cấu trúc như sau:

```
Eco Learning (GEMINI)/
├── README.md               # Tổng quan kho lưu trữ
├── AGENTS.md               # Quy định master & Protocol cho Agent (File này)
├── LEARNED.md              # Bảng nhật ký tổng quan các bài học đã hoàn thành (Có Mã ID)
├── RELATE.md               # Hàng chờ các khái niệm liên quan (Dùng để tham khảo & củng cố kiến thức)
├── GLOSSARY.md             # Bảng chỉ mục thuật ngữ tra cứu nhanh
├── .memory/                # Hệ thống Agent Memory & Learning System (Kiến trúc 3 tầng)
│   ├── README.md           # Hướng dẫn quy trình & phân định vai trò hệ thống bộ nhớ
│   ├── knowledge_corrections.md # Tầng 1: Nhật ký Lỗi & Bài học Tổng quát hóa (Error Memory)
│   ├── antigravity_memory.md # Tầng 2: Quy tắc vận hành tinh chế cho Antigravity Agent
│   └── codex_memory.md     # Tầng 2: Quy tắc vận hành tinh chế cho Codex Agent
└── topics/                 # Thư mục Nhánh A duy nhất chứa toàn bộ các chủ đề
    └── <category-B>/       # Thư mục Nhánh B (Tên tiếng Anh kebab-case, ví dụ: corporate-and-markets)
        ├── README.md       # Tóm tắt danh mục các bài học thuộc chủ đề B này
        └── <lesson-name>.md # Bài học .md chi tiết (Có chứa YAML frontmatter ở đầu)
```

### 🧠 QUY TẮC BỘ NHỚ VẬN HÀNH (OPERATIONAL MEMORY RULE):
* Khi vận hành, AI Agent **bắt buộc phải đọc file memory tinh chế tương ứng với model/agent của mình** trong `.memory/` (ví dụ: `.memory/antigravity_memory.md` đối với Antigravity, `.memory/codex_memory.md` đối với Codex Agent khi được sử dụng) để nạp các quy tắc vận hành trước khi biên soạn.

### ⚠️ QUY TẮC TIẾT KIỆM TOKEN CHO AGENT:
1. **TRÁNH đọc trực tiếp các file bài học `.md` chi tiết** trừ khi thực sự cần thiết (ví dụ: cần trích dẫn chính xác công thức hoặc nội dung cụ thể từ bài đó).
2. Khi cần kiểm tra lịch sử các bài đã học và chọn chủ đề tiếp theo:
   - **Bước 1:** Đọc file [`RELATE.md`](RELATE.md) để kiểm tra các khái niệm liên quan chưa học.
   - **Bước 2:** Đọc file [`LEARNED.md`](LEARNED.md) ở thư mục gốc.
   - **Bước 3 (nếu cần xem sâu hơn về một nhóm chủ đề):** Đọc file `README.md` nằm bên trong thư mục `topics/<category-B>/` tương ứng.

---

## 🧠 Agent Memory Retrieval & Learning Protocol

Đây là giao thức bắt buộc để Agent chủ động tra cứu, áp dụng bộ nhớ và học hỏi từ các sai sót cũ trước và trong khi biên soạn bài học mới.

```text
Correction is recorded → Failure pattern abstracted → General rule distilled → Relevant rule retrieved → Applied before writing
```

### Step 0 — Load Operational Memory (Nạp bộ nhớ vận hành)
Trước khi bắt đầu bất kỳ task tạo hoặc sửa bài học nào:
1. Đọc file memory tinh chế của agent hiện tại (`.memory/antigravity_memory.md` hoặc `.memory/codex_memory.md`).
2. Xác định các quy tắc vận hành tinh chế (*distilled operational rules*) liên quan trực tiếp đến task.

### Step 1 — Identify Risk Patterns (Nhận diện nguy cơ tiềm ẩn)
Trước khi viết nội dung, Agent tự đánh giá chủ đề bài học có chứa các dấu hiệu nguy cơ sau không:
* **Mô hình Giáo trình Dễ bị Rập khuôn (Textbook Oversimplification):** Có dùng công thức lý thuyết hay mô hình giảng dạy không?
* **Cơ chế Thể chế (Institutional Mechanism):** Có liên quan đến cách ngân hàng, thị trường hay cơ quan quản lý vận hành thực tế không?
* **Đồng nhất thức Kế toán (Balance-Sheet Accounting Identity):** Có liên quan đến dòng tiền, nợ/tài sản hay hạch toán kế toán giữa nhiều chủ thể không?
* **Phát biểu Nhân quả Vĩ mô (Causal Claim):** Có phát biểu mối quan hệ giữa các biến số vĩ mô không?
* **Khẳng định Định lượng (Quantitative / Empirical Claim):** Có sử dụng số liệu, mốc thời gian hay quy định pháp lý không?
* **Thuật ngữ Dễ nhầm lẫn (Terminology Ambiguity):** Có các khái niệm hay đi cùng nhau nhưng khác bản chất không?

### Step 2 — Agent-Guided Retrieval (Tra cứu bài học lịch sử có định hướng)
> 💡 *Lưu ý về Hạ tầng:* Dự án sử dụng quy trình **Agent-Guided Retrieval / Deliberate Inspection** (Agent tự giác chủ động tìm kiếm và đọc tài liệu liên quan), **KHÔNG phải** hạ tầng tự động dựa trên Vector Database hay Embeddings/RAG.

Agent KHÔNG cần đọc toàn bộ `.memory/knowledge_corrections.md` cho mọi task. Thay vào đó, Agent chủ động tìm và tra cứu các mục liên quan dựa trên:
1. **Exact Topic Match:** Khớp chủ đề trực tiếp (ví dụ: `money supply`, `interest rates`).
2. **Conceptual Match:** Khớp khái niệm rộng (ví dụ: banking, monetary policy, accounting).
3. **Failure Pattern Match:** Khớp dạng lỗi tư duy (ví dụ: *textbook model vs reality*, *balance sheet confusion*, *deterministic macro claim*, *empirical timing overclaim*).

### Step 3 — Apply Retrieved Rules as Constraints (Áp dụng làm ràng buộc tư duy)
Coi các quy tắc đã truy xuất là các **ràng buộc tư duy cứng (hard constraints)**. 
* *Ví dụ:* Nếu quy tắc truy xuất ghi `Central-bank reserves ≠ Commercial-bank deposits`, bất kỳ ví dụ ngân hàng nào cũng phải kiểm tra hạch toán Bảng cân đối kế toán trước khi hoàn tất.

### Step 4 — Pre-Finalization Memory Self-Check (Bảng tự kiểm tra bộ nhớ)
Trước khi hoàn thiện một bài học, Agent bắt buộc chạy bảng tự kiểm tra:

```text
MEMORY CHECK
[ ] Đã áp dụng các bài học lịch sử và distilled rules phù hợp chưa?
[ ] Có vô tình lặp lại hiểu lầm đã từng được sửa đổi không?
[ ] Đã phân biệt rõ Mô hình Giáo trình (Textbook Model) vs Cơ chế Thực tế (Real-World Mechanism) chưa?
[ ] Có biến mối quan hệ có điều kiện thành khẳng định định mệnh / tuyệt đối không?
[ ] Có số liệu định lượng nào thiếu phạm vi bối cảnh / nguồn xác minh không?
[ ] Đã kiểm tra tính cân đối và phân tách Bảng cân đối kế toán (Reserves vs Deposits) chưa?
[ ] Đã dán nhãn phân loại các khẳng định quan trọng (Definition / Identity / Model / Causal Claim) chưa?
```
*Nếu fail bất kỳ mục quan trọng nào, Agent phải chỉnh sửa nội dung trước khi finalize.*

### Step 5 — Correction-to-General-Rule Protocol (Quy trình Học tập khi có Lỗi mới)
Khi người dùng hoặc reviewer sửa một lỗi sai kiến thức / tư duy:
1. **Sửa bài học gốc** trong `topics/`.
2. **Ghi nhận sự cố** vào `.memory/knowledge_corrections.md` theo chuẩn format (Error, Corrected Understanding, Root Cause, Generalizable Lesson, Trigger Patterns).
3. **Trích xuất Bài học Tổng quát hóa (Generalizable Lesson):** Chuyển từ lỗi sai cụ thể thành nguyên tắc tư duy tổng quát có thể áp dụng cho nhiều chủ đề khác.
4. **Quyết định đưa vào Operational Memory:**
   - Nếu là sự thật một lần (*one-off fact*) $\rightarrow$ Chỉ lưu ở `knowledge_corrections.md`.
   - Nếu là nguyên tắc tư duy tái sử dụng được (*reusable reasoning rule*) $\rightarrow$ Tinh chế và cập nhật vào file `agent_memory.md` tương ứng.
5. **Hợp nhất quy tắc (Merge & Refactor):** Nếu quy tắc đã tồn tại hoặc nhiều lỗi cùng chỉ ra một failure mode, hợp nhất thành một quy tắc cấp cao hơn thay vì tạo quy tắc trùng lặp.

---

## 🏛️ Model-vs-Reality Rule (Quy tắc Mô hình vs Thực tế)

Bất kỳ bài học nào chứa cả mô hình giáo trình và cơ chế vận hành thực tế BẮT BUỘC phải phân tách rõ ràng:

```text
TEXTBOOK MODEL (Mô hình Giáo trình)
→ Các giả định (Assumptions)
→ Mô hình chứng minh điều gì (What it demonstrates)

REAL-WORLD MECHANISM (Cơ chế Thực tế)
→ Quy trình vận hành thể chế thực tế (Actual institutional process)
→ Các rào cản và điều kiện biên thực tế (Additional constraints)
```
*Cấm tuyệt đối việc âm thầm chuyển từ mô hình lý thuyết sang mô tả thực tế vận hành mà không dán nhãn phân biệt.*

---

## 🏷️ Claim Classification Protocol (Giao thức Phân loại Khẳng định)

Trước khi viết các nhận định quan trọng trong bài học, Agent phải dán nhãn / xác định bản chất của phát biểu:

- `[Definition]`: Định nghĩa khái niệm.
- `[Accounting Identity]`: Đồng nhất thức kế toán / hạch toán (bắt buộc đúng theo định nghĩa).
- `[Theoretical Model]`: Mô hình lý thuyết với các giả định kèm theo.
- `[Empirical Relationship]`: Mối quan hệ thực nghiệm (có tính biến động, phụ thuộc bối cảnh).
- `[Causal Mechanism]`: Cơ chế nhân quả (cần giải thích chuỗi truyền dẫn chi tiết).
- `[Historical Claim]`: Khẳng định sự kiện lịch sử (cần nguồn và bối cảnh).
- `[Current Fact]`: Số liệu / quy định hiện tại (cần `applicable_year` hoặc nguồn).
- `[Prediction]`: Dự báo / nhận định tương lai (cần nêu rõ giả định).

---

## ⚖️ Phân tách Thẩm quyền Bộ nhớ (Behavioral Authority vs Epistemic Authority)

> 💡 **Cốt lõi:** **Memory controls reasoning behavior, not factual truth.**  
> (Bộ nhớ Agent định hướng quy trình làm việc và thói quen tư duy, nhưng bản thân bộ nhớ không tự coi mình là nguồn sự thật tuyệt đối).

Thẩm quyền trong hệ thống được phân tách thành hai chiều độc lập:

### A. Behavioral Authority (Thẩm quyền Vận hành & Quy trình)
Xác định **Agent phải hành xử và thực hiện task như thế nào**:

```text
AGENTS.md (Master Instructions & Protocols)
       ↓
Agent-specific operational memory (antigravity_memory.md / codex_memory.md)
```

### B. Knowledge / Epistemic Authority (Thẩm quyền Tri thức & Tính Xác thực Dữ liệu)
Xác định **Dữ liệu / Sự thật nào đáng tin cậy**:

```text
Nguồn sơ cấp & uy tín được xác minh (NHTW, GSO, IMF, BIS, BCTC, Văn bản luật)
       ↓
Tri thức bài học trong kho (topics/)
       ↓
Nhật ký sửa lỗi lịch sử (knowledge_corrections.md)
       ↓
Các giả định mô hình lý thuyết chung
```

### Giao thức Chống "Memory Poisoning" (Anti-Memory-Poisoning Protocol)
* **Xử lý Xung đột Dữ liệu (Conflict Resolution):** Khi nội dung trong bộ nhớ mâu thuẫn với nguồn sơ cấp uy tín đã được xác minh (hoặc quy định/số liệu thực tế mới), Agent **KHÔNG ĐƯỢC** ưu tiên bộ nhớ chỉ vì nó thuộc tầng cao hơn về mặt hành vi. Agent phải:
  1. Nhận diện xung đột (*detect conflict*).
  2. Kiểm tra nguồn sơ cấp uy tín (*verify source*).
  3. Giải quyết xung đột dựa trên bằng chứng sơ cấp (*resolve conflict*).
  4. Cập nhật lại bộ nhớ (`knowledge_corrections.md` & `agent_memory.md`) nếu bộ nhớ bị lạc hậu hoặc sai lệch (*update memory*).

---

## 2. Quy trình 6 bước Biên soạn Bài học Mới

Mỗi khi người dùng yêu cầu bài học mới, Agent phải thực hiện đúng 6 bước sau:

1. **Lựa chọn chủ đề & Nạp Bộ nhớ (Memory Retrieval & Spiral Model):** 
   - **Thực hiện Step 0 & Step 1 of Memory Protocol:** Nạp `agent_memory.md`, nhận diện risk patterns và chủ động tra cứu các quy tắc liên quan.
   - Đọc [`LEARNED.md`](LEARNED.md) và [`RELATE.md`](RELATE.md).
   - **TẦNG 1 - CORE ANCHORS (Nền tảng):** Lãi suất, Lạm phát, Cung tiền, Thanh khoản. Ưu tiên xây móng vững trước.
   - **TẦNG 2 - HÀNH VI (Song song):** *Behavioral Finance* có thể học sớm/song song.
   - **TẦNG 3 - APPLICATION LAYER (Ứng dụng):** BĐS VN, Tỷ giá VND, Thuế & Quy hoạch TCCN... **BẮT BUỘC KHOÁ PREREQUISITES**: AI chỉ được mở bài Tầng 3 nếu bài nền thuộc Tầng 1 tương ứng ĐÃ CÓ TRONG `LEARNED.md`.
2. **Soạn bài học (Áp dụng Memory Constraints & Claim Classification):** 
   - Biên soạn nội dung chuẩn xác theo 9 mục chuẩn. 
   - Phân tách rõ `Textbook Model vs Real-World Mechanism`.
   - Bắt buộc có **YAML Frontmatter** ở đầu file (`applicable_year` với luật/thuế).
3. **Lưu file bài học:** Lưu vào `topics/<category-B>/<lesson-name-in-english>.md`.
4. **Cập nhật README của Thư mục B:** Thêm Mã ID, tiêu đề, đường dẫn và tóm tắt cơ chế (3-5 câu).
5. **Cập nhật nhật ký LEARNED.md & GLOSSARY.md:**
   - Append dòng mới vào [`LEARNED.md`](LEARNED.md) với Mã ID và đường dẫn tương đối (chỉ đặt link nhấp được ở cột "Đường dẫn", KHÔNG dùng `file:///`).
   - Append thuật ngữ mới vào [`GLOSSARY.md`](GLOSSARY.md).
6. **Cập nhật RELATE.md & Chạy Memory Checklist:**
   - Đánh dấu `✅ Đã học` hoặc thêm `⏳ Chưa học` vào [`RELATE.md`](RELATE.md).
   - **Chạy Pre-Finalization Memory Self-Check (Step 4)** cùng Checklist nhất quán repository.

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

Mỗi ngày chọn một chủ đề chính thuộc một trong các nhóm sau (Ưu tiên mô hình Xoắn ốc - Spiral Learning Model):

* **Nhóm Hạt nhân (Core Anchors - Ưu tiên xây móng):** Lãi suất, Lạm phát, Cung tiền & Thanh khoản.
* Kinh tế vĩ mô & Kinh tế vi mô.
* Tiền tệ, Ngân hàng và Thị trường vốn.
* **Thị trường Bất động sản Việt Nam** (chu kỳ, đòn bẩy, tín dụng ngân hàng).
* **Tỷ giá VND & Lãi suất toàn cầu** (kênh truyền dẫn vĩ mô).
* **Thuế & Quy hoạch tài chính cá nhân theo pháp luật Việt Nam**.
* **Tâm lý học hành vi trong đầu tư** (Behavioral Finance).
* Tài chính cá nhân & Quản trị dòng tiền.
* Chứng khoán, Doanh nghiệp và Thị trường.
* Kinh tế thế giới & Lịch sử kinh tế / Khủng hoảng tài chính.
* Những cơ chế kinh tế đứng sau các sự kiện đời sống thường ngày.

Hạn chế các bài tập trung chủ yếu vào chính sách công thuần túy.

Việc chọn chủ đề duy trì **Mô hình Xoắn ốc (Spiral Model)**:
* Xoay quanh các khái niệm hạt nhân kết nối cao trước (Lãi suất, Lạm phát, Cung tiền, Thanh khoản) để làm điểm tựa vững chắc.
* Thỉnh thoảng kết nối bài mới với bài cũ thông qua hàng chờ `RELATE.md`.
* Tránh lặp lại cùng một nội dung trong thời gian ngắn.
* Mở rộng từ khái niệm nền tảng sang các mảng ứng dụng thực tế phức tạp hơn.

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

**Mọi bài học BẮT BUỘC có phần YAML Frontmatter ở đầu file:**
```yaml
---
id: CORP-001             # Mã ID bài học (MACRO-xxx, MICRO-xxx, MONEY-xxx, CORP-xxx, INVEST-xxx, INDIV-xxx, VIET-xxx, BEHAV-xxx)
title: "Tên bài học"
category: category-name  # Tên folder B
tags: [tag1, tag2, tag3]
prerequisites: [ID-1, ID-2] # BẮT BUỘC: Mã ID bài học nền tảng phải tồn tại trong LEARNED.md
difficulty: Fundamental | Intermediate | Advanced
date: YYYY-MM-DD
applicable_year: 2026       # Bắt buộc với chủ đề Thuế, Quy định, Pháp luật VN
last_verified: 2026-08-04   # Tránh trôi dữ liệu khi luật thay đổi
---
```

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

## Mở đầu bài học (Dành cho bài Củng cố / Delayed Active Recall)

Nếu bài học mới là một bài củng cố (Spaced Reinforcement) trích ra từ `RELATE.md`, ngay sau mục **1. Chủ đề hôm nay**, hãy thêm một khung nhỏ:

> 🔄 **Ôn tập Ngắt quãng (Delayed Active Recall):** *"Trước khi vào bài mới, bạn còn nhớ cơ chế [X] trong bài học [ID-XXX] cách đây 1-2 tuần không? Hãy thử nhớ lại 1 ý cốt lõi trước khi đọc tiếp nhé!"*

---

## Kết thúc bài

Cuối mỗi bài, thêm ba phần ngắn:

### Liên kết kiến thức

Nêu từ 2 đến 4 khái niệm có liên quan mà bài học hôm nay giúp mở đường để hiểu.

### Điều đáng nhớ nhất

Tóm tắt một đến ba ý cốt lõi, tập trung vào cơ chế thay vì chỉ nhắc lại định nghĩa.

### Góc Phản xạ & Active Recall (Dành cho bạn)

Đưa ra 1 câu hỏi gợi mở phản xạ tự nhiên (không bắt buộc trả lời, không chấm điểm, không áp lực bài tập). Chọn 1 trong 3 dạng:
- **Dạng 1 (Tóm tắt lại):** *"Hãy thử tự giải thích lại cơ chế X này cho một người bạn chưa biết bằng 2-3 câu ngắn gọn."*
- **Dạng 2 (Kết nối ngẫu nhiên):** *"Cơ chế X hôm nay có liên quan gì đến khái niệm [ID-XXX] mà bạn đã học trước đó?"*
- **Dạng 3 (Liên hệ thực tế):** *"Với thông tin X hôm nay, bạn có nhận ra hiện tượng tương tự nào trong bản tin tài chính hoặc quyết định chi tiêu gần đây của mình không?"*

*Gợi ý nhẹ cuối mục:* **Thang tự đánh giá (1-5):** Bạn tự thấy mức độ hiểu/nhớ cơ chế hôm nay ở mức nào (1 = Cần đọc lại sớm / 3 = Nắm vững / 5 = Rất tự tin)? (Nếu bạn chọn 1-2, hệ thống sẽ ưu tiên quay lại củng cố sớm hơn).

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
Mỗi phiên biên soạn chỉ được tạo/sửa đúng 5 loại file:
- 1 file bài học mới: `topics/<category>/<lesson>.md`
- 1 file README nhóm: `topics/<category>/README.md`
- `LEARNED.md`
- `RELATE.md`
- `GLOSSARY.md`

*(Trừ trường hợp cập nhật hệ thống bộ nhớ `.memory/` khi phát hiện và xử lý lỗi kiến thức theo Step 5 of Memory Protocol).*

#### 2. Chỉ ghi thêm (append-only) vào log
- `LEARNED.md`, `RELATE.md` và `GLOSSARY.md`: chỉ **thêm dòng mới**, không sửa/xóa dòng cũ — trừ khi người dùng yêu cầu rõ ràng.
- Cấm Agent tự ý "dọn dẹp" hay viết lại các dòng cũ để "gọn hơn" nếu không được yêu cầu.

#### 3. Phát hiện lỗi ở bài cũ → Ghi nhận vào Memory Protocol & ISSUES.md
Nếu trong lúc soạn bài mới phát hiện bài cũ có sai sót:
- Ghi nhận sự cố vào `.memory/knowledge_corrections.md` và trích xuất bài học tổng quát theo **Step 5 of Memory Protocol**.
- Ghi một dòng vào `ISSUES.md` (tạo mới nếu chưa có) để theo dõi.

#### 4. Xác nhận trước khi hoàn tất (diff summary)
Trước khi kết thúc phiên, Agent liệt kê tóm tắt:
- File nào được tạo mới
- File nào được sửa, và sửa đúng những dòng nào
- Kết quả chạy Pre-Finalization Memory Self-Check (Step 4)

---

### C. Prompt mẫu — dùng đầu mỗi phiên biên soạn bài học

```
Bạn là AI Agent quản trị kho tri thức Eco Learning. Trước khi biên soạn bài học mới, hãy:

1. Thực hiện Step 0 & Step 1 of Agent Memory Protocol (Đọc agent_memory.md,
   nhận diện risk patterns và chủ động tra cứu các quy tắc tương ứng).
2. Đọc LEARNED.md và RELATE.md để chọn chủ đề (ưu tiên breadth-first,
   xen kẽ 1 bài củng cố sau mỗi 3-4 bài mới).
3. Biên soạn bài học theo đúng 9 mục chuẩn trong AGENTS.md, dán nhãn phân biệt
   Textbook Model vs Real-World Mechanism.
4. Tuân thủ NGHIÊM NGẶT Giao thức Chống Bịa Thông tin (Mục A) và Giao thức Phân loại Khẳng định (Claim Classification Protocol).
5. Tuân thủ NGHIÊM NGẶT Giao thức Chống Sửa Tung (Mục B) và Memory Protocol.
6. Trước khi kết thúc, chạy Pre-Finalization Memory Self-Check và in ra bảng tóm tắt:
   - File đã tạo mới: ...
   - File đã sửa và dòng cụ thể: ...
   - Kết quả Memory Self-Check: ...
```
