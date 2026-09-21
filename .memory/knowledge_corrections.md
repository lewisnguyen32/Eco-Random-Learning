# Nhật ký Sửa đổi Kiến thức & Học tập Dài hạn của Agent (Knowledge Corrections & Long-Term Error Memory)

Tài liệu lưu lịch sử lỗi và quy tắc phòng ngừa. Đợt đối chiếu 22/09/2026 đã đính chính cả một số “Corrected Understanding” và nguồn trong các entry cũ. Phần “Lỗi sai” là nội dung lịch sử để nhận diện, không được dùng làm kiến thức. Nguồn chưa xác minh không có thẩm quyền chứng minh chỉ vì được lưu ở memory.

---

## 📚 Chỉ mục Bài học Tổng quát hóa (Generalized Lesson Index)

| Mã Lesson | Tên Bài học Tổng quát hóa (Generalizable Lesson Title) | Phạm vi Áp dụng (Scope) |
| :--- | :--- | :--- |
| **`G-001`** | Textbook Model $\neq$ Real-World Institutional Reality | Mọi mô hình kinh tế / tài chính / ngân hàng / thị trường |
| **`G-002`** | Balance-Sheet Accounting Isolation | Nghiệp vụ ngân hàng, OMOs, báo cáo tài chính doanh nghiệp |
| **`G-003`** | Non-Deterministic Macroeconomic Relationships | Kinh tế vĩ mô, lạm phát, chính sách tiền tệ/tài khóa |
| **`G-004`** | Distinguish Closely Related Macro Concepts | Suy thoái, khủng hoảng, thanh khoản, thị trường tài sản |
| **`G-005`** | Quantitative & Empirical Claims Scope Verification | Số liệu thời sự, quy định pháp luật, mốc thời gian |
| **`G-006`** | Statement Classification Protocol | Trình bày công thức, lý thuyết, quan hệ nhân quả |
| **`G-007`** | Measurement Basis & Units | Tỷ số, quy đổi ngày sang tiền, NWC/OCF, chỉ số giá, lợi suất kỳ vọng |

---

## 🔍 Chi tiết Nhật ký Sửa đổi & Trích xuất Bài học (Correction Entries)

### 📌 Entry 001: Cơ chế Tạo tiền Ngân hàng Thương mại vs Mô hình Số nhân tiền
* **Mã bài học liên quan:** `MONEY-001` (`topics/monetary-and-banking/money-supply-and-bank-money-creation.md`)
* **Lỗi sai / Hiểu lầm cũ:** 
  - Mô tả cơ chế ngân hàng tạo tiền theo dạng literal `người dân gửi tiền → giữ dự trữ r → cho vay phần còn lại → gửi lại → cho vay tiếp`.
  - Coi công thức số nhân tiền $m = 1/r$ là cơ chế nhân quả trực tiếp ngân hàng dùng để tạo tiền trong thực tế.
* **Kiến thức chuẩn xác:**
  - Trong hệ thống ngân hàng hiện đại: **Khoản vay tạo ra tiền gửi** (`Loans Create Deposits`). Ngân hàng tạo ra tiền gửi mới $M1/M2$ khi cấp tín dụng bằng cách ghi nhận đồng thời khoản vay (Asset) và tiền gửi thanh toán (Liability).
  - Công thức $m = 1/r$ chỉ là **mô hình lý thuyết đơn giản hóa (pedagogical simplification)** thể hiện giới hạn dự trữ lý thuyết tối đa, không phải cơ chế nhân quả thực tế.
* **Nguyên nhân sai lầm tư duy (Why Reasoning Failed):**
  - AI bị rơi vào bẫy rập khuôn giáo trình nhập môn (*Textbook Over-Simplification Trap*), nhầm lẫn giữa một mô hình toán học đơn giản hóa dùng để giảng dạy với thực tế vận hành thể chế (*institutional reality*).
* **Bài học Tổng quát hóa (Generalizable Lesson - `G-001`):**
  > **Do not treat a pedagogical/textbook model as a literal description of real-world institutional mechanics.**
  > 
  > Khi sử dụng bất kỳ mô hình lý thuyết nào (ví dụ: Money Multiplier $1/r$, IS-LM, Cạnh tranh hoàn hảo, Modigliani-Miller, Mô hình Cung-Cầu đơn giản):
  > 1. Xác định rõ các giả định của mô hình (*assumptions*).
  > 2. Mức độ trừu tượng (*abstraction level*).
  > 3. Mô hình chứng minh điều gì (*what it demonstrates*) và chủ động bỏ qua điều gì (*what it intentionally omits*).
  > 4. Không bao giờ âm thầm chuyển từ mô hình sang mô tả thực tế vận hành nếu không dán nhãn phân biệt rõ ràng.
* **Dấu hiệu Kích hoạt (Trigger Patterns):**
  - Khi trình bày một mô hình giáo trình hoặc công thức số nhân / điểm cân bằng.
  - Khi giải thích cơ chế vận hành của một thể chế tài chính / ngân hàng / thị trường.
  - Khi kết nối công thức toán học lý thuyết với thực tế kinh doanh.
* **Nguồn đối chiếu đã xác minh:** [Bank of England (2014), Money creation in the modern economy](https://www.bankofengland.co.uk/quarterly-bulletin/2014/q1/money-creation-in-the-modern-economy). Không dùng dẫn chiếu “Fed St. Louis (2021)” thiếu định danh làm bằng chứng.

---

### 📌 Entry 002: Phân biệt Dự trữ tại NHTW ($R$) và Tiền gửi Khách hàng ($D$)
* **Mã bài học liên quan:** `MONEY-001` (`topics/monetary-and-banking/money-supply-and-bank-money-creation.md`)
* **Lỗi sai / Hiểu lầm cũ:**
  - Trong ví dụ NHTW mua $1.000 trái phiếu chính phủ từ Ngân hàng A, ví dụ cũ nhầm lẫn rằng giao dịch này tạo ra ngay $1.000 tiền gửi khách hàng.
* **Kiến thức chuẩn xác:**
  - $\text{Central-bank reserves} \neq \text{Commercial-bank deposits}$.
  - Giao dịch NHTW mua trái phiếu trực tiếp từ Ngân hàng A chỉ làm thay đổi tài sản của Ngân hàng A (giảm Trái phiếu, tăng Dự trữ tại NHTW), **không tạo ra bất kỳ khoản tiền gửi khách hàng ($D$) nào**. Trong giao dịch mua tài sản này, mua từ chủ thể phi ngân hàng có thể làm tiền gửi và dự trữ tăng cùng lúc; còn phải kiểm tra khu vực chủ thể và tài khoản có thuộc phạm vi cung tiền hay không. Đây không phải tuyên bố mua tài sản là cách duy nhất tạo tiền gửi.
* **Nguyên nhân sai lầm tư duy (Why Reasoning Failed):**
  - AI không thực hiện phân tách Bảng cân đối kế toán (*Balance-Sheet Isolation*) giữa các chủ thể riêng biệt (NHTW, NHTM, Khách hàng), dẫn đến việc đánh đồng hai loại tài sản/nợ thuộc hai tầng lưu thông hoàn toàn khác nhau.
* **Bài học Tổng quát hóa (Generalizable Lesson - `G-002`):**
  > **Enforce Balance-Sheet Accounting Isolation & Identities.**
  > 
  > Trước khi đưa ra bất kỳ khẳng định nào về dòng tiền hay tác động của một giao dịch tài chính:
  > 1. Xác định rõ Bảng cân đối kế toán của từng chủ thể tham gia (NHTW, Ngân hàng thương mại, Doanh nghiệp, Cá nhân).
  > 2. Đảm bảo tính cân đối đồng nhất thức: $\text{Assets} = \text{Liabilities} + \text{Equity}$ cho từng chủ thể.
  > 3. Phân biệt rõ các loại tài sản/nợ nằm ở các tầng lưu thông khác nhau (ví dụ: interbank/central-bank reserves vs public economy deposits).
* **Dấu hiệu Kích hoạt (Trigger Patterns):**
  - Khi phân tích các nghiệp vụ thị trường mở (OMOs), nới lỏng định lượng (QE), bơm/hút thanh khoản của NHTW.
  - Khi phân tích báo cáo tài chính ngân hàng, doanh nghiệp, giao dịch tín dụng hay dòng tiền.
* **Nguồn đối chiếu:** [Bank of England (2022), QE at the Bank of England](https://www.bankofengland.co.uk/quarterly-bulletin/2022/2022-q1/qe-at-the-bank-of-england-a-perspective-on-its-functioning-and-effectiveness). Tên nguồn cũ “Fed St. Louis (2021), Money and Missed Conceptions” chưa tìm được tài liệu tương ứng qua tìm kiếm ngày 22/09/2026; đã ngừng dùng, không kết luận tài liệu chắc chắn không tồn tại.

---

### 📌 Entry 003: Phân biệt Credit Crunch (Siết chặt Tín dụng) vs Liquidity Trap (Bẫy Thanh khoản)
* **Mã bài học liên quan:** `MONEY-001` (`topics/monetary-and-banking/money-supply-and-bank-money-creation.md`)
* **Lỗi sai / Hiểu lầm cũ:**
  - Viết ngụ ý `Credit Crunch dẫn đến Liquidity Trap` như hai khái niệm đồng nghĩa hoặc có quan hệ nhân quả kéo theo trực tiếp.
* **Kiến thức chuẩn xác:**
  - **Credit Crunch (Siết chặt tín dụng):** Trạng thái thắt chặt nguồn cung tín dụng từ phía các ngân hàng thương mại do lo sợ rủi ro nợ xấu hoặc suy giảm vốn an toàn.
  - **Liquidity Trap (Bẫy thanh khoản):** Trong mô hình, tiền và tài sản ngắn hạn an toàn gần thay thế nhau ở vùng lãi suất thấp/sát giới hạn hiệu dụng, khiến chính sách thông thường kém hiệu lực. Không đồng nhất với bi quan, mọi dạng tín dụng yếu, ngưỡng 0% cứng hoặc sự vô hiệu của tất cả công cụ tiền tệ.
  - Đây là hai khái niệm phân biệt có thể tương tác trong suy thoái; không có quan hệ kéo theo tất yếu. “Phân biệt” không có nghĩa độc lập thống kê hoặc không thể liên quan nhân quả trong một mô hình cụ thể.
* **Nguyên nhân sai lầm tư duy (Why Reasoning Failed):**
  - AI bị lỗi ngụy biện vội vã gom nhóm (*Correlation-to-Causality Fallacy*), biến hai hiện tượng có xu hướng xuất hiện đồng thời thành quan hệ nguyên nhân - kết quả.
* **Bài học Tổng quát hóa (Generalizable Lesson - `G-004`):**
  > **Distinguish Closely Related Macro Concepts & Avoid False Causality.**
  > 
  > 1. Không bao giờ ngụ ý quan hệ nhân quả đơn giản giữa hai khái niệm vĩ mô chỉ vì chúng thường xuất hiện trong cùng một bối cảnh (như suy thoái hay khủng hoảng).
  > 2. Phân tích rõ bản chất của từng khái niệm từ góc độ hành vi của các chủ thể khác nhau (ví dụ: hành vi của ngân hàng thương mại vs hành vi của người tiêu dùng/doanh nghiệp).
* **Dấu hiệu Kích hoạt (Trigger Patterns):**
  - Khi so sánh hoặc kết nối các hiện tượng khủng hoảng, suy thoái, lạm phát, thiểu phát, bẫy thanh khoản, bong bóng tài sản.
* **Nguồn đối chiếu đã đọc:** [Stanley Fischer – Fed (05/10/2016), Low Interest Rates](https://www.federalreserve.gov/newsevents/speech/fischer20161005a.htm). Dẫn chiếu Mishkin trước đây không kèm trang/chương đã kiểm tra nên không được dùng làm bằng chứng riêng cho entry.

---

### 📌 Entry 004: Loại bỏ Mốc thời gian Cố định Deterministic cho M2 và Lạm phát
* **Mã bài học liên quan:** `MONEY-001` (`topics/monetary-and-banking/money-supply-and-bank-money-creation.md`)
* **Lỗi sai / Hiểu lầm cũ:**
  - Đưa ra khẳng định "M2 tăng $\rightarrow$ lạm phát xuất hiện sau 12–18 tháng" như một quy luật cố định.
* **Kiến thức chuẩn xác:**
  - Mối quan hệ giữa tiền tệ và lạm phát phụ thuộc vào tốc độ lưu thông $V$, sản lượng $GDP$, nhu cầu nắm giữ tiền và năng lực sản xuất dư thừa ($M \cdot V = P \cdot Y$). Độ trễ truyền dẫn biến động linh hoạt tùy bối cảnh vĩ mô, không tồn tại mốc thời gian cố định cho mọi trường hợp.
* **Nguyên nhân sai lầm tư duy (Why Reasoning Failed):**
  - AI phạm lỗi phán quyết tuyệt đối (*Deterministic Macro Claim Bias*), tự gán mốc thời gian cố định cho một mối quan hệ kinh tế có tính điều kiện cao.
* **Bài học Tổng quát hóa (Generalizable Lesson - `G-003` & `G-005`):**
  > **Avoid Deterministic Macro Claims & Verify Quantitative Scope.**
  > 
  > 1. Không biến các mối quan hệ kinh tế có tính điều kiện thành quy luật định mệnh hoặc tuyệt đối trong ngắn hạn.
  > 2. Không đưa ra các mốc thời gian cố định hay con số định lượng mà không có phạm vi bối cảnh (*scope*) và bằng chứng xác minh cụ thể.
  > 3. Phân biệt rõ phát biểu đồng nhất thức, phát biểu mô hình lý thuyết và phát biểu thực nghiệm (*empirical claim*).
* **Dấu hiệu Kích hoạt (Trigger Patterns):**
  - Khi phân tích lạm phát, lãi suất, tỷ giá, tác động chính sách tiền tệ/tài khóa.
* **Nguồn đối chiếu:** [ECB, Transmission mechanism](https://www.ecb.europa.eu/mopo/intro/transmission/html/index.en.html). Dẫn chiếu cũ “ECB & Fed ... Studies” không định danh một nghiên cứu cụ thể.

---

### 📌 Entry 005: Xác minh Số hiệu Văn bản Pháp lý & Phân biệt Khung Vận hành NHTW (Corridor vs Floor)
* **Mã bài học liên quan:** `MONEY-002` (`topics/monetary-and-banking/policy-rates-and-monetary-transmission.md`)
* **Lỗi sai / Hiểu lầm cũ:**
  - Trích dẫn sai số hiệu văn bản điều hành ngày 24/10/2022 của NHNN thành `1810/QĐ-NHNN` (số hiệu không tồn tại trong đợt điều chỉnh này).
  - Mô tả mô hình hành lang lãi suất (Corridor System) nhưng thiếu phân định với khung sàn dự trữ dồi dào (Ample-Reserves Floor System) của Fed sau 2008.
* **Kiến thức chuẩn xác:**
  - Ngày 24/10/2022, NHNN ban hành bộ 3 quyết định: `1809/QĐ-NHNN` (lãi suất điều hành), `1812/QĐ-NHNN` (trần lãi suất tiền gửi), và `1813/QĐ-NHNN` (trần lãi suất cho vay ngắn hạn 5 lĩnh vực ưu tiên).
  - **Đính chính ngày 22/09/2026:** Nhận định cũ gán ECB và NHNN cùng vận hành hành lang đối xứng là không được giữ lại. Thông báo ECB 13/03/2024 lấy DFR làm mức định hướng; từng công cụ NHNN phải tra riêng, không suy từ sơ đồ giáo trình. Fed có khung dự trữ dồi dào; tên IORB chỉ áp dụng từ 29/07/2021, không gán ngược về 2008.
* **Nguyên nhân sai lầm tư duy (Why Reasoning Failed):**
  - AI bị lỗi giả định số hiệu văn bản liên tiếp (*Sequential Number Hallucination*) khi trích dẫn các quyết định ban hành cùng ngày mà không tra cứu cơ sở dữ liệu pháp luật sơ cấp.
* **Bài học Tổng quát hóa (Generalizable Lesson - `G-005`):**
  - Mọi số hiệu văn bản quy phạm pháp luật / quyết định hành chính điều hành bắt buộc phải được tra cứu đối chiếu trực tiếp từ CSDL văn bản pháp luật trước khi hoàn tất.
* **Dấu hiệu Kích hoạt (Trigger Patterns):**
  - Khi trích dẫn thông tư, nghị định, quyết định điều hành lãi suất hoặc quy định pháp luật.
* **Nguồn đối chiếu:** [Thông báo gốc NHNN đợt 24/10/2022](https://www.sbv.gov.vn/documents/d/sbv_portal/524653); [ECB, Operational framework, 13/03/2024](https://www.ecb.europa.eu/press/pr/date/2024/html/ecb.pr240313~807e240020.en.html); [Fed, Implementation Note, 28/07/2021](https://www.federalreserve.gov/newsevents/pressreleases/monetary20210728a1.htm).

---

## Đợt rà soát toàn kho ngày 22/09/2026

### Entry 006: CCC, vốn lưu động và số tiền cần tài trợ
- **Bài liên quan:** CORP-001; LEARNED, GLOSSARY và README nhóm.
- **Error:** COGS/ngày × CCC được gọi là nhu cầu vốn chính xác; OCF dùng ΔNWC trong khi NWC đã định nghĩa gồm cả tiền và nợ vay.
- **Corrected Understanding:** Tính riêng tồn kho, phải thu và phải trả theo mẫu số phù hợp. Ví dụ cũ có W = 37,5 tỷ, không phải 30 tỷ; nhu cầu vay phải có lịch tiền mặt và nguồn tài trợ. Dùng W hoạt động, cùng giả định, khi minh họa OCF rút gọn.
- **Root Cause:** Cộng các số ngày tính trên cơ sở doanh thu và giá vốn khác nhau rồi nhân chung một mẫu số; nhầm phạm vi đại lượng.
- **Generalizable Lesson:** G-007: kiểm tra đơn vị, cơ sở định giá, stock/flow và số dư bình quân/đầu-cuối kỳ trước khi quy đổi.
- **Trigger Patterns:** CCC, DSO/DPO, vốn lưu động, OCF, tỷ số ngày sang tiền.
- **Verification Source:** [ACCA – Working capital management](https://www.accaglobal.com/gb/en/student/exam-support-resources/fundamentals-exams-study-resources/f9/technical-articles/wcm.html); [ACCA – Cash flow statements](https://www.accaglobal.com/uk/en/student/exam-support-resources/fundamentals-exams-study-resources/f3/technical-articles/cashflow-statements.html).

### Entry 007: Repo không phải mua đứt
- **Bài liên quan:** MONEY-002.
- **Error:** Ngân hàng mất trái phiếu, tăng dự trữ và không tăng nợ khi nhận tiền repo.
- **Corrected Understanding:** Với repo mang bản chất tài trợ và bên vay giữ rủi ro/lợi ích, ngân hàng tăng dự trữ và nợ repo, tiếp tục ghi nhận chứng khoán. Bán đứt có bút toán khác; NHTW ghi khoản cấp vốn repo.
- **Root Cause:** Dùng câu chuyện chuyển giao pháp lý chứng khoán thay phân tích điều kiện dừng ghi nhận và nghĩa vụ mua lại.
- **Generalizable Lesson:** Mở rộng G-002: phân loại giao dịch và bản chất tài trợ trước khi lập bảng cân đối.
- **Trigger Patterns:** Repo, reverse repo, cầm cố, mua/bán đứt, tài sản bảo đảm.
- **Verification Source:** [Fed Financial Accounting Manual, Chapter 4, 40.15–40.20; cập nhật 22/01/2026](https://www.federalreserve.gov/aboutthefed/chapter-4-system-open-market-account.htm).

### Entry 008: Tiền cơ sở, QE và phạm vi cung tiền
- **Bài liên quan:** MONEY-001, MACRO-001 và GLOSSARY.
- **Error:** Gộp tiền két vào reserve balances; bỏ sót tiền két trong MB; ngụ ý QE chỉ tăng tiền gửi nếu ngân hàng cho vay.
- **Corrected Understanding:** Tách C công chúng, C trong két, R tại NHTW. QE mua từ chủ thể phi ngân hàng có thể tăng tiền gửi ngay; ảnh hưởng lên chỉ tiêu cung tiền tùy phạm vi thống kê.
- **Root Cause:** Trộn thuật ngữ giữa giáo trình và H.6; suy diễn cơ chế cho vay là cơ chế duy nhất.
- **Generalizable Lesson:** G-002 + G-005: luôn xác định đối tác, tài khoản và khu vực được thống kê, tránh đếm trùng/bỏ sót.
- **Trigger Patterns:** M1/M2/MB, vault cash, reserve balances, QE, “bơm tiền”.
- **Verification Source:** [Fed H.6 ngày 23/11/2021](https://www.federalreserve.gov/releases/h6/20211123/); [BoE QE 2022](https://www.bankofengland.co.uk/quarterly-bulletin/2022/2022-q1/qe-at-the-bank-of-england-a-perspective-on-its-functioning-and-effectiveness).

### Entry 009: Đồng nhất thức, kỳ vọng và chỉ số giá
- **Bài liên quan:** MACRO-001.
- **Error:** Dùng CPI như P trong MV = PY khi Y là GDP thực; gọi Fisher ex-ante là đồng nhất thức chính xác với lạm phát kỳ vọng.
- **Corrected Understanding:** P phải tương thích GDP danh nghĩa/thực. Đồng nhất thức không xác định chiều nhân quả. Lợi suất ex-post là phép chia chính xác; kỳ vọng của phép chia không bằng phép chia với kỳ vọng nói chung.
- **Root Cause:** Bỏ qua phạm vi chỉ số và tính phi tuyến của toán tử kỳ vọng.
- **Generalizable Lesson:** G-006 + G-007: tách định nghĩa, đồng nhất thức, mô hình và ước lượng; kiểm tra mẫu số cùng kỳ và điều kiện kỳ vọng.
- **Trigger Patterns:** MV = PY, CPI/GDP deflator, Fisher, ex-ante/ex-post, phần trăm/điểm phần trăm.
- **Verification Source:** [FRED Blog – The velocity of money, 2015](https://fredblog.stlouisfed.org/2015/01/the-velocity-of-money/); [IMF CPI Manual, 2020](https://www.imf.org/en/data/statistics/cpi-manual). Công thức lợi suất và kỳ vọng được kiểm tra bằng đại số, không gán cho nguồn phát biểu điều chưa đối chiếu.

### Entry 010: Dữ liệu tương lai, luật cũ và cơ quan đã đổi tên
- **Bài liên quan:** MACRO-001, MONEY-002.
- **Error:** Dùng tên cơ quan thống kê cũ làm hiện trạng 2026; gắn rổ 2020–2025 vào hiện tại; dùng CPI cả năm 2023 lý giải quyết định giữa năm; trích TT07/2014 như căn cứ hiện hành.
- **Corrected Understanding:** Cục Thống kê thuộc Bộ Tài chính từ thay đổi năm 2025. Số mặt hàng/quyền số phải có kỳ áp dụng. TT48/2024 thay TT07/2014 từ 20/11/2024. Quyết định phải được diễn giải bằng thông tin có thể biết tại thời điểm đó.
- **Root Cause:** Sao chép thông tin quen thuộc và nhầm ngày truy cập với thời kỳ áp dụng; hindsight bias.
- **Generalizable Lesson:** Mở rộng G-005: kiểm tra ngày ban hành, hiệu lực, kỳ quan sát, ngày công bố và thời điểm quyết định riêng biệt.
- **Trigger Patterns:** Current Fact, tên cơ quan, CPI basket, luật thay thế, “đầu năm”, “cuối năm”.
- **Verification Source:** [Cục Thống kê – lịch sử tổ chức](https://www.nso.gov.vn/gioi-thieu/lich-su-phat-trien/); [phương pháp CPI 2025](https://www.nso.gov.vn/default/2025/11/chi-so-gia-tieu-dung-va-phuong-phap-do-luong-tai-viet-nam/); [CSDL VBPL TT48/2024](https://vbpl.vn/TW/Pages/vbpq-toanvan.aspx?ItemID=170156). TT48 được đối chiếu qua nội dung chỉ mục tìm kiếm nguồn chính thức; công cụ mở toàn văn gặp lỗi trong phiên, xem giới hạn ở báo cáo audit.

### Entry 011: Tóm tắt, nguồn và bộ nhớ vẫn có thể lưu lỗi
- **Bài liên quan:** toàn bộ chỉ mục, hai operational memories và audit cũ.
- **Error:** Bài MONEY-001 đã sửa nhưng README/LEARNED vẫn diễn giải ngân hàng cho vay tiền gửi còn lại; memory Entry 005 lại khẳng định hành lang đối xứng sai; audit cũ tuyên bố độ chính xác quá mức.
- **Corrected Understanding:** Sửa kiến thức cần đồng bộ bản tóm tắt và glossary; nguồn có tên thật chưa chứng minh đoạn diễn giải đúng. Báo cáo lịch sử không thay thế kiểm chứng hiện tại.
- **Root Cause:** Xem memory và tóm tắt như phần thủ tục, bỏ qua tác động của chúng lên lần biên soạn sau.
- **Generalizable Lesson:** G-001/G-005/G-006: nguồn sơ cấp có thẩm quyền tri thức; rà soát mọi nơi lặp lại khẳng định đã sửa và nêu giới hạn chứng cứ.
- **Trigger Patterns:** “đã kiểm chứng”, điểm audit, tên nguồn không có link, tóm tắt còn khác bài gốc.
- **Verification Source:** đối chiếu trực tiếp các file và nguồn đã dẫn tại Entries 005–010; báo cáo ngày 22/09/2026 lưu riêng trong audits/.
