# Công cụ đọc dữ liệu và lập luận (Analytical tools)

Công cụ đọc số, so bằng chứng và nhận diện điều kiện suy luận ở mức trực giác kinh tế.

[Bản đồ](../KNOWLEDGE_MAP.md) · [Các quan hệ](relationships.md) · Nguồn đối chiếu [CORE](sources.md#source-core) · [DOING](sources.md#source-doing) · [MITDATA](sources.md#source-mitdata) · [MITMET](sources.md#source-mitmet)

## Đọc chỉ tiêu

| ID | Khái niệm (VI / EN) | Phạm vi | Phân loại | Trạng thái và bằng chứng |
| --- | --- | --- | --- | --- |
| <a name="km-ana-growth-rates"></a>`KM-ANA-growth-rates` | **Tỷ lệ và tốc độ tăng trưởng** (Percentages and growth rates) | Chọn đúng mức gốc, kỳ so và phân biệt thay đổi phần trăm với điểm phần trăm. | CORE | LEARNED · [MICRO-001](../topics/microeconomics/price-elasticity-of-demand-and-revenue.md), [MONEY-004](../topics/monetary-and-banking/bank-repricing-risk-and-net-interest-margin.md), [VIET-001](../topics/vietnam-economy/exchange-rate-pass-through-to-consumer-prices.md) — Dùng đúng cơ sở đổi phần trăm, kỳ và điểm phần trăm. |
| <a name="km-ana-ratios"></a>`KM-ANA-ratios` | **Tỷ số và cơ sở so sánh** (Ratios and denominators) | Ghép tử với mẫu theo cùng phạm vi, kỳ và đơn vị trước khi so sánh. | CORE | LEARNED · [CORP-001](../topics/corporate-and-markets/cash-conversion-cycle.md), [MONEY-004](../topics/monetary-and-banking/bank-repricing-risk-and-net-interest-margin.md) — Kiểm tra tử mẫu, kỳ và quy đổi theo ngày hoặc năm. |
| <a name="km-ana-index-numbers"></a>`KM-ANA-index-numbers` | **Chỉ số và năm gốc** (Index numbers) | Dùng trọng số và kỳ gốc để gộp biến động, với kết quả có thể đổi theo cách lập chỉ số. | CORE | LEARNED · [MACRO-001](../topics/macroeconomics/inflation-cpi-and-macro-transmission.md) — Tính chỉ số giá có trọng số, hiểu năm gốc và phạm vi rổ. |
| <a name="km-ana-base-effects"></a>`KM-ANA-base-effects` | **Hiệu ứng nền so sánh** (Base effects) | Tốc độ so với kỳ gốc có thể đổi khi nền thay đổi, dù diễn biến ngắn hạn ít thay đổi. | IMPORTANT | PARTIALLY_LEARNED · [MACRO-001](../topics/macroeconomics/inflation-cpi-and-macro-transmission.md) — Có các kỳ so tháng và năm, chưa làm rõ cơ chế ảnh hưởng của nền bằng ví dụ riêng. |
| <a name="km-ana-nominal-real-conversion"></a>`KM-ANA-nominal-real-conversion` | **Quy đổi theo mức giá** (Deflation of nominal series) | Dùng chỉ số giá phù hợp để biến đổi chuỗi danh nghĩa thành thước đo khối lượng hoặc sức mua. | IMPORTANT | PARTIALLY_LEARNED · [MACRO-001](../topics/macroeconomics/inflation-cpi-and-macro-transmission.md), [MACRO-002](../topics/macroeconomics/fisher-effect-and-yield-curve.md) — Đổi tỷ suất danh nghĩa về sức mua thực, chưa áp dụng chỉ số giá để quy đổi cả chuỗi danh nghĩa. |
| <a name="km-ana-per-capita-distribution"></a>`KM-ANA-per-capita-distribution` | **Bình quân đầu người và phân phối** (Per capita measures and distributions) | Tách thay đổi tổng khỏi quy mô dân số và tách mức bình quân khỏi trải nghiệm từng nhóm. | IMPORTANT | NOT_LEARNED |

## Xác suất và bằng chứng

| ID | Khái niệm (VI / EN) | Phạm vi | Phân loại | Trạng thái và bằng chứng |
| --- | --- | --- | --- | --- |
| <a name="km-ana-probability"></a>`KM-ANA-probability` | **Xác suất cơ bản** (Basic probability) | Diễn giải khả năng xảy ra theo mô hình hoặc dữ liệu, có xét thông tin điều kiện. | CORE | NOT_LEARNED |
| <a name="km-ana-expected-value"></a>`KM-ANA-expected-value` | **Giá trị kỳ vọng** (Expected value) | Trung bình các kết quả khả dĩ có trọng số xác suất, có thể khác mọi kết quả riêng lẻ. | CORE | LEARNED · [MICRO-002](../topics/microeconomics/asymmetric-information-and-adverse-selection.md) — Tính mức sẵn lòng trả theo xác suất loại xe và cập nhật khi thành phần đổi. |
| <a name="km-ana-correlation"></a>`KM-ANA-correlation` | **Tương quan** (Correlation) | Đo mức độ và chiều liên hệ tuyến tính giữa hai biến trên mẫu và kỳ xác định. | CORE | LEARNED · [INVEST-002](../topics/investing/diversification-correlation-and-portfolio-risk.md) — Chiều và mức liên hệ tuyến tính, phạm vi mẫu và ví dụ tương quan bằng không vẫn có lúc cùng lỗ. |
| <a name="km-ana-sampling-selection"></a>`KM-ANA-sampling-selection` | **Lấy mẫu và thiên lệch chọn mẫu** (Sampling and selection bias) | Mẫu quan sát có thể khác tổng thể hoặc loại bỏ các trường hợp quan trọng một cách có hệ thống. | CORE | NOT_LEARNED |
| <a name="km-ana-uncertainty-forecast"></a>`KM-ANA-uncertainty-forecast` | **Bất định dự báo** (Forecast uncertainty) | Nêu giả định, khoảng hoặc kịch bản thay cho diễn giải dự báo điểm như kết quả chắc chắn. | IMPORTANT | PARTIALLY_LEARNED · [MACRO-004](../topics/macroeconomics/inflation-expectations-and-anchoring.md), [MACRO-002](../topics/macroeconomics/fisher-effect-and-yield-curve.md) — Có độ phân tán và tín hiệu có điều kiện, chưa khảo sát khoảng dự báo và đánh giá sai số. |
| <a name="km-ana-empirical-evidence"></a>`KM-ANA-empirical-evidence` | **Đọc bằng chứng thực nghiệm** (Evaluating empirical evidence) | Kiểm tra dữ liệu, thiết kế, kích thước hiệu ứng và phạm vi có thể áp dụng kết quả. | CORE | NOT_LEARNED |

## Lập luận nhân quả

| ID | Khái niệm (VI / EN) | Phạm vi | Phân loại | Trạng thái và bằng chứng |
| --- | --- | --- | --- | --- |
| <a name="km-ana-causation"></a>`KM-ANA-causation` | **Tương quan và suy luận nhân quả** (Correlation and causal inference) | Tách biến động đi cùng nhau khỏi tác động của can thiệp trong một thiết kế có giả định. | CORE | PARTIALLY_LEARNED · [VIET-001](../topics/vietnam-economy/exchange-rate-pass-through-to-consumer-prices.md), [MACRO-002](../topics/macroeconomics/fisher-effect-and-yield-curve.md) — Phân biệt quan sát đồng biến, dự báo và tác động, chưa trình bày thiết kế nhận diện. |
| <a name="km-ana-counterfactual"></a>`KM-ANA-counterfactual` | **Đối chứng phản thực** (Counterfactual reasoning) | Hỏi kết quả khả dĩ của cùng đối tượng nếu điều kiện hoặc can thiệp khác đi. | CORE | NOT_LEARNED |
| <a name="km-ana-confounding"></a>`KM-ANA-confounding` | **Biến gây nhiễu** (Confounding variables) | Một yếu tố ảnh hưởng cả điều kiện so sánh lẫn kết quả có thể làm sai lệch ước lượng. | IMPORTANT | PARTIALLY_LEARNED · [VIET-001](../topics/vietnam-economy/exchange-rate-pass-through-to-consumer-prices.md) — Có yếu tố chi phí ngoài tỷ giá khi đọc thực nghiệm, chưa bao quát cách kiểm soát nhiễu. |
| <a name="km-ana-regression"></a>`KM-ANA-regression` | **Trực giác hồi quy** (Regression intuition) | Ước lượng quan hệ có điều kiện giữa các biến, phụ thuộc dữ liệu, đặc tả và giả định. | IMPORTANT | NOT_LEARNED |
| <a name="km-ana-experiment"></a>`KM-ANA-experiment` | **Thí nghiệm ngẫu nhiên và tự nhiên** (Randomized and natural experiments) | Dùng cơ chế phân bổ hoặc thay đổi gần ngoại sinh để xây dựng đối chứng có điều kiện. | IMPORTANT | NOT_LEARNED |
| <a name="km-ana-sensitivity"></a>`KM-ANA-sensitivity` | **Kiểm tra độ nhạy** (Sensitivity analysis) | Thay đầu vào hoặc giả định để thấy kết luận nào ổn định và chỗ nào dễ đảo chiều. | IMPORTANT | LEARNED · [CORP-003](../topics/corporate-and-markets/financial-leverage-and-equity-risk.md), [MONEY-004](../topics/monetary-and-banking/bank-repricing-risk-and-net-interest-margin.md) — Giữ các giả định khác cố định, thay EBIT, lãi vay hoặc mức truyền lãi để tìm kết luận đổi chiều. |
