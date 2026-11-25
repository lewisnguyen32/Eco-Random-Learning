# Tài chính doanh nghiệp (Corporate finance)

Cách doanh nghiệp đầu tư, tài trợ và phân phối tiền. Xem [Kế toán và báo cáo tài chính](accounting.md) để lần từ số liệu báo cáo tới các biến đầu vào.

[Bản đồ](../KNOWLEDGE_MAP.md) · [Các quan hệ](relationships.md) · Nguồn đối chiếu [FIN](sources.md#source-fin) · [CFA](sources.md#source-cfa) · [ACCA](sources.md#source-acca)

## Giá trị theo thời gian và đầu tư vốn

| ID | Khái niệm (VI / EN) | Phạm vi | Phân loại | Trạng thái và bằng chứng |
| --- | --- | --- | --- | --- |
| <a name="km-cf-time-value"></a>`KM-CF-time-value` | **Giá trị thời gian của tiền** (Time value of money) | Quy đổi tiền ở các thời điểm về cùng mốc theo kỳ và tỷ lệ chiết khấu tương thích. | CORE | PARTIALLY_LEARNED · [INDIV-001](../topics/personal-finance/installment-loans-flat-rates-and-effective-cost.md), [MONEY-002](../topics/monetary-and-banking/policy-rates-and-monetary-transmission.md) — Áp dụng chiết khấu và ghép lãi, chưa hệ thống hóa quy đổi cho nhiều cấu trúc dòng tiền. |
| <a name="km-cf-npv"></a>`KM-CF-npv` | **Giá trị hiện tại ròng** (Net present value) | Tổng giá trị hiện tại của dòng tiền tăng thêm, kể cả khoản đầu tư ban đầu. | CORE | LEARNED · [MONEY-002](../topics/monetary-and-banking/policy-rates-and-monetary-transmission.md) — Định nghĩa và mô hình cho thấy mức chiết khấu ảnh hưởng giá trị đầu tư ra sao. |
| <a name="km-cf-irr"></a>`KM-CF-irr` | **Tỷ suất hoàn vốn nội bộ** (Internal rate of return) | Mức chiết khấu làm NPV bằng không, có thể có nhiều nghiệm hoặc không phù hợp để xếp hạng. | IMPORTANT | PARTIALLY_LEARNED · [INDIV-001](../topics/personal-finance/installment-loans-flat-rates-and-effective-cost.md) — Giải IRR của dòng tiền vay thông thường, chưa xét nhiều nghiệm hoặc giới hạn xếp hạng dự án. |
| <a name="km-cf-capital-budgeting"></a>`KM-CF-capital-budgeting` | **Thẩm định đầu tư vốn** (Capital budgeting) | Chọn dự án qua dòng tiền tăng thêm, chi phí cơ hội, rủi ro và ràng buộc vốn. | CORE | PARTIALLY_LEARNED · [MONEY-002](../topics/monetary-and-banking/policy-rates-and-monetary-transmission.md) — Có công thức NPV nhiều kỳ và kênh chiết khấu, chưa phân tích dòng tiền tăng thêm và giới hạn ngân sách. |
| <a name="km-cf-cost-of-capital"></a>`KM-CF-cost-of-capital` | **Chi phí vốn** (Cost of capital) | Mức sinh lời cơ hội phù hợp rủi ro của bên cấp vốn. | CORE | PARTIALLY_LEARNED · [MONEY-002](../topics/monetary-and-banking/policy-rates-and-monetary-transmission.md) — Đổi tỷ lệ chiết khấu trong kênh đầu tư, chưa phân tích suất sinh lời theo từng nguồn vốn. |
| <a name="km-cf-wacc"></a>`KM-CF-wacc` | **Chi phí vốn bình quân gia quyền** (Weighted average cost of capital) | Gộp chi phí các nguồn tài trợ theo trọng số và giả định thích hợp. | IMPORTANT | NOT_LEARNED |
| <a name="km-cf-corporate-valuation"></a>`KM-CF-corporate-valuation` | **Định giá doanh nghiệp** (Corporate valuation) | Ước tính giá trị hoạt động hoặc vốn chủ bằng dòng tiền, tài sản hoặc đối chiếu thị trường phù hợp. | CORE | PARTIALLY_LEARNED · [MONEY-002](../topics/monetary-and-banking/policy-rates-and-monetary-transmission.md) — Có mô hình cổ tức tăng trưởng đều, chưa bao quát định giá hoạt động và tài sản. |
| <a name="km-cf-fcf"></a>`KM-CF-fcf` | **Dòng tiền tự do** (Free cash flow) | Dòng tiền còn lại sau đầu tư cần thiết, tính theo phạm vi doanh nghiệp hoặc vốn chủ. | IMPORTANT | NOT_LEARNED |

## Vốn lưu động và tài trợ ngắn hạn

| ID | Khái niệm (VI / EN) | Phạm vi | Phân loại | Trạng thái và bằng chứng |
| --- | --- | --- | --- | --- |
| <a name="km-cf-working-capital"></a>`KM-CF-working-capital` | **Vốn lưu động** (Working capital) | Xác định phần nguồn lực ngắn hạn theo phạm vi tổng quát hoặc phạm vi hoạt động. | CORE | LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md), [CORP-002](../topics/corporate-and-markets/cash-flow-statement-and-operating-cash-flow.md) — Phạm vi vốn lưu động và vốn lưu động hoạt động, tác động đến tiền. |
| <a name="km-cf-operating-cycle"></a>`KM-CF-operating-cycle` | **Chu kỳ hoạt động** (Operating cycle) | Thời gian từ lúc đưa hàng vào tồn kho đến khi thu tiền khách, xấp xỉ DIO cộng DSO. | IMPORTANT | LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md) — Lần theo hai chặng tồn kho và phải thu trước khi điều chỉnh thời gian trả nhà cung cấp. |
| <a name="km-cf-cash-conversion-cycle"></a>`KM-CF-cash-conversion-cycle` | **Chu kỳ chuyển đổi tiền mặt** (Cash conversion cycle) | Ước lượng khoảng chênh thời gian giữa trả nhà cung cấp và thu tiền, tính DIO cộng DSO trừ DPO. | IMPORTANT | LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md) — Công thức, CCC âm, thời gian so với số tiền và lịch thiếu hụt. |
| <a name="km-cf-dio"></a>`KM-CF-dio` | **Số ngày tồn kho bình quân** (Days inventory outstanding) | Quy đổi tồn kho bình quân sang số ngày theo giá vốn và kỳ tương ứng. | IMPORTANT | LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md) — Tồn kho bình quân, giá vốn và đổi đơn vị sang ngày. |
| <a name="km-cf-dso"></a>`KM-CF-dso` | **Số ngày thu tiền bình quân** (Days sales outstanding) | Quy đổi phải thu bình quân theo doanh số tín dụng hoặc đại lượng thay thế có ghi rõ. | IMPORTANT | LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md) — Dùng phải thu với doanh số tín dụng, nêu giới hạn của mẫu số thay thế. |
| <a name="km-cf-dpo"></a>`KM-CF-dpo` | **Số ngày trả nhà cung cấp bình quân** (Days payable outstanding) | Quy đổi phải trả bình quân theo mua chịu hoặc đại lượng thay thế có ghi rõ. | IMPORTANT | LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md) — Dùng phải trả với mua chịu, nêu giới hạn khi thay bằng giá vốn. |
| <a name="km-cf-working-capital-financing"></a>`KM-CF-working-capital-financing` | **Tài trợ vốn lưu động** (Working capital financing) | Khớp nhu cầu ngắn hạn và thường xuyên với vốn nội bộ, tín dụng và nguồn khác theo kỳ hạn. | IMPORTANT | PARTIALLY_LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md) — Tính thời điểm và mức thiếu tiền, chưa so cách tài trợ nhu cầu thường xuyên và mùa vụ. |
| <a name="km-cf-trade-credit"></a>`KM-CF-trade-credit` | **Tín dụng thương mại** (Trade credit) | Nhà cung cấp cho khách thanh toán sau, với kỳ hạn và chi phí ngầm trong điều khoản. | IMPORTANT | PARTIALLY_LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md) — Có động cơ kéo dài hạn trả và rủi ro nhà cung cấp, chưa tính chi phí ngầm từ chiết khấu. |
| <a name="km-cf-factoring"></a>`KM-CF-factoring` | **Bao thanh toán** (Factoring) | Bên tài trợ ứng vốn hoặc mua khoản phải thu, theo cơ chế truy đòi và dịch vụ đã thỏa thuận. | IMPORTANT | NOT_LEARNED |
| <a name="km-cf-supply-chain-finance"></a>`KM-CF-supply-chain-finance` | **Tài trợ chuỗi cung ứng** (Supply chain finance) | Dùng dữ liệu và quan hệ mua bán để cung cấp thanh khoản qua các mắt xích. | SPECIALIZED | NOT_LEARNED |

## Cấu trúc vốn và phân phối tiền

| ID | Khái niệm (VI / EN) | Phạm vi | Phân loại | Trạng thái và bằng chứng |
| --- | --- | --- | --- | --- |
| <a name="km-cf-debt-equity"></a>`KM-CF-debt-equity` | **Tài trợ bằng nợ và vốn chủ** (Debt and equity financing) | So sánh nghĩa vụ ưu tiên theo hợp đồng với quyền hưởng phần còn lại của chủ sở hữu. | CORE | LEARNED · [CORP-003](../topics/corporate-and-markets/financial-leverage-and-equity-risk.md) — Nguồn tài trợ, khác biệt cam kết, quyền hưởng phần còn lại và bút toán. |
| <a name="km-cf-capital-structure"></a>`KM-CF-capital-structure` | **Cấu trúc vốn** (Capital structure) | Phối hợp nợ và vốn chủ theo rủi ro, thuế, quyền kiểm soát và khả năng tài trợ. | IMPORTANT | PARTIALLY_LEARNED · [CORP-003](../topics/corporate-and-markets/financial-leverage-and-equity-risk.md) — Có phối hợp nợ và vốn chủ, chưa phân tích lựa chọn theo thuế, kiểm soát và chi phí kiệt quệ. |
| <a name="km-cf-financial-leverage"></a>`KM-CF-financial-leverage` | **Đòn bẩy tài chính** (Financial leverage) | Nghĩa vụ nợ khuếch đại biến động kết quả và rủi ro của phần vốn chủ trong điều kiện tương ứng. | CORE | LEARNED · [CORP-003](../topics/corporate-and-markets/financial-leverage-and-equity-risk.md) — Đo đòn bẩy và giải thích khi ROE hoặc rủi ro vốn thay đổi. |
| <a name="km-cf-interest-coverage"></a>`KM-CF-interest-coverage` | **Hệ số bảo đảm lãi vay** (Interest coverage ratio) | So nguồn thu nhập đo được với chi phí lãi, có giới hạn về trả gốc và thời điểm tiền về. | IMPORTANT | LEARNED · [CORP-003](../topics/corporate-and-markets/financial-leverage-and-equity-risk.md) — Tính hệ số và kiểm tra lịch gốc, lãi trả khác nhau. |
| <a name="km-cf-covenants"></a>`KM-CF-covenants` | **Điều khoản ràng buộc khoản vay** (Debt covenants) | Yêu cầu theo hợp đồng tạo ngưỡng giám sát, hạn chế hoặc quyền can thiệp cho chủ nợ. | IMPORTANT | PARTIALLY_LEARNED · [CORP-003](../topics/corporate-and-markets/financial-leverage-and-equity-risk.md) — Giới thiệu ngưỡng bảo vệ chủ nợ, chưa phân tích các dạng ràng buộc và hệ quả khi vi phạm. |
| <a name="km-cf-dividends"></a>`KM-CF-dividends` | **Chính sách cổ tức** (Dividend policy) | Quyết định phân phối tiền định kỳ theo nhu cầu tái đầu tư, kỳ vọng và ràng buộc. | IMPORTANT | NOT_LEARNED |
| <a name="km-cf-buybacks"></a>`KM-CF-buybacks` | **Mua lại cổ phần** (Share repurchases) | Dùng tiền công ty mua cổ phần lưu hành, với tác động tùy giá mua và cách tài trợ. | IMPORTANT | NOT_LEARNED |

## Kiểm soát, thay đổi sở hữu và khó khăn

| ID | Khái niệm (VI / EN) | Phạm vi | Phân loại | Trạng thái và bằng chứng |
| --- | --- | --- | --- | --- |
| <a name="km-cf-governance"></a>`KM-CF-governance` | **Quản trị công ty** (Corporate governance) | Quyền, trách nhiệm và cơ chế giám sát giữa cổ đông, hội đồng và ban điều hành. | IMPORTANT | NOT_LEARNED |
| <a name="km-cf-distress"></a>`KM-CF-distress` | **Kiệt quệ tài chính doanh nghiệp** (Corporate financial distress) | Áp lực trả nghĩa vụ có thể làm giảm giá trị hoạt động trước khi có thủ tục pháp lý. | IMPORTANT | PARTIALLY_LEARNED · [CORP-003](../topics/corporate-and-markets/financial-leverage-and-equity-risk.md) — Có áp lực tái tài trợ và thiếu tiền theo hạn, chưa bao quát chi phí kiệt quệ và xử lý. |
| <a name="km-cf-restructuring"></a>`KM-CF-restructuring` | **Tái cấu trúc doanh nghiệp và nợ** (Corporate and debt restructuring) | Điều chỉnh tài trợ hoặc hoạt động để phân bổ tổn thất và khôi phục khả năng tồn tại. | IMPORTANT | NOT_LEARNED |
| <a name="km-cf-ma"></a>`KM-CF-ma` | **Sáp nhập và mua lại** (Mergers and acquisitions) | Thay đổi quyền kiểm soát với động cơ hiệp lực, định giá thương vụ và rủi ro tích hợp. | IMPORTANT | NOT_LEARNED |
