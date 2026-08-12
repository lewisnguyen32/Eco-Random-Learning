# Codex Operational Memory (Distilled Agent Rules)

Tài liệu này chứa các quy tắc vận hành tinh chế (*Distilled Operational Rules*) dành riêng cho AI Agent **Codex**. Các quy tắc này được trích xuất từ nhật ký sửa lỗi dài hạn (`.memory/knowledge_corrections.md`) và phải được áp dụng làm ràng buộc tư duy trước khi tạo hoặc sửa bài học.

---

## 🧠 Distilled Operational Rules

### 1. Rule G-001 — Model vs Reality Isolation
* **Rule:** Do not treat a pedagogical/textbook model as a literal description of real-world institutional mechanics.
* **Application:** Whenever presenting a simplified formula or textbook diagram (e.g., money multiplier $1/r$, IS-LM, perfect competition), explicitly label:
  - `TEXTBOOK MODEL`: State assumptions, abstraction level, and what it demonstrates.
  - `REAL-WORLD MECHANISM`: Explain actual institutional processes and real-world constraints.

### 2. Rule G-002 — Balance-Sheet Accounting Isolation
* **Rule:** Maintain strict accounting identities and isolate balance sheets across different entities.
* **Application:** Always distinguish central-bank reserves from commercial-bank deposits ($\text{Reserves} \neq \text{Deposits}$). Verify balance-sheet entries for each entity separately.

### 3. Rule G-003 — Non-Deterministic Macro Relationships
* **Rule:** Do not turn conditional macroeconomic relationships into universal or deterministic causal laws.
* **Application:** Avoid claiming fixed timeframes for policy transmission. Frame macro relationships conditionally using exchange equations ($M \cdot V = P \cdot Y$).

### 4. Rule G-004 — Concept Distinction & Causality Prevention
* **Rule:** Distinguish closely related macro concepts and avoid assuming direct causality merely because they co-occur.
* **Application:** Differentiate Credit Crunch from Liquidity Trap. Do not present one as automatically causing the other.

### 5. Rule G-005 — Scope & Quantitative Verification
* **Rule:** Definitions and regulations vary by statistical framework and country; do not present localized data as universal facts.
* **Application:** Specify the governing central bank, country, or statistical framework (e.g., Fed vs SBV vs ECB). Always include `applicable_year` or `last_verified` for legal/tax topics.

---

## 🔄 Quick Self-Check Protocol Before Finalization
Before finalizing any lesson, Codex MUST verify:
- [ ] Explicitly distinguished textbook model from real-world mechanism?
- [ ] Checked balance-sheet identities across entities?
- [ ] Avoided turning conditional relationships into deterministic laws?
- [ ] Classified major statements (Definition / Identity / Model / Causal Claim)?
- [ ] Specified country / framework scope for quantitative and legal claims?
