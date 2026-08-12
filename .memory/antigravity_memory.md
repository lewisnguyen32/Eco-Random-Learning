# Antigravity Operational Memory (Distilled Agent Rules)

Tài liệu này chứa các quy tắc vận hành tinh chế (*Distilled Operational Rules*) dành riêng cho AI Agent **Antigravity**. Các quy tắc này được trích xuất từ nhật ký sửa lỗi dài hạn (`.memory/knowledge_corrections.md`) và phải được áp dụng làm ràng buộc tư duy trước khi tạo hoặc sửa bài học.

---

## 🧠 Distilled Operational Rules

### 1. Rule G-001 — Model vs Reality Isolation
* **Rule:** Do not treat a pedagogical/textbook model as a literal description of real-world institutional mechanics.
* **Application:** Whenever presenting a simplified formula or textbook diagram (e.g., money multiplier $1/r$, IS-LM, perfect competition), explicitly label:
  - `TEXTBOOK MODEL`: State assumptions, abstraction level, and what it demonstrates.
  - `REAL-WORLD MECHANISM`: Explain actual institutional processes and real-world constraints.
  - Do not silently bridge from model to reality.

### 2. Rule G-002 — Balance-Sheet Accounting Isolation
* **Rule:** Maintain strict accounting identities and isolate balance sheets across different entities.
* **Application:** When a central bank purchases securities directly from a commercial bank, the immediate balance-sheet change is in securities and reserves; do not infer a new customer deposit from that transaction. Distinguish this from purchases from non-bank sellers, where the seller's bank deposit can increase. Always verify:
  $$\text{Central-bank reserves} \neq \text{Commercial-bank deposits}$$

### 3. Rule G-003 — Non-Deterministic Macro Relationships
* **Rule:** Do not turn conditional macroeconomic relationships into universal or deterministic causal laws.
* **Application:** Avoid claiming fixed timeframes (e.g., "inflation always follows M2 growth in 12-18 months"). Frame macro relationships conditionally using exchange equations ($M \cdot V = P \cdot Y$), considering money velocity $V$, output capacity, and public money demand.

### 4. Rule G-004 — Concept Distinction & Causality Prevention
* **Rule:** Distinguish closely related macro concepts and avoid assuming direct causality merely because they co-occur.
* **Application:** Differentiate Credit Crunch (commercial bank credit supply contraction) from Liquidity Trap (near-zero interest rate with extreme liquidity preference). Do not present one as automatically causing the other.

### 5. Rule G-005 — Scope & Quantitative Verification
* **Rule:** Definitions, numbers, and legal regulations vary by statistical framework and country; do not present localized or simplified data as universal facts.
* **Application:** Specify the governing central bank, country, or statistical framework (e.g., Fed vs SBV vs ECB) when discussing M1/M2 definitions, interest rate tools, or legal tax rules. Always include `applicable_year` or `last_verified` for legal/tax topics.

---

## 🔄 Quick Self-Check Protocol Before Finalization
Before finalizing any lesson, Antigravity MUST verify:
- [ ] Explicitly distinguished textbook model from real-world mechanism?
- [ ] Checked balance-sheet identities across entities (Reserves vs Deposits)?
- [ ] Avoided turning conditional relationships into deterministic laws or fixed timeframes?
- [ ] Classified major statements (Definition / Identity / Model / Causal Claim)?
- [ ] Specified country / framework scope for quantitative and legal claims?
