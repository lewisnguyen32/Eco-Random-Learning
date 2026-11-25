# Quan hệ giữa các khái niệm

[Bản đồ](../KNOWLEDGE_MAP.md) · [Quy tắc duy trì](../KNOWLEDGE_MAP.md#duy-trì-bản-đồ)

Đọc từng dòng theo hướng **A → loại quan hệ → B**. `RELATED_TO` và `CONTRASTS_WITH` đọc được theo cả hai hướng và chỉ ghi một lần. `PREREQUISITE_OF` mô tả điều cần hiểu để suy ra một cơ chế cụ thể. Trường `prerequisites` của từng bài vẫn nằm trong siêu dữ liệu bài học. Chỉ cạnh `PREREQUISITE_OF` được kiểm tra chu trình.

| Quan hệ | Cách đọc |
| --- | --- |
| `PREREQUISITE_OF` | A là kiến thức cần để hiểu cơ chế của B. |
| `RELATED_TO` | A và B có liên hệ hữu ích, ví dụ cùng được dùng trong một quyết định. |
| `COMPONENT_OF` | A là một cấu phần hoặc một số hạng của B. |
| `APPLICATION_OF` | A vận dụng B trong một công cụ, phương pháp hoặc trường hợp cụ thể. |
| `CONTRASTS_WITH` | Phân biệt A và B vì hai khái niệm dễ bị đánh đồng. |
| `MEASURES` | A đo B hoặc một phần xác định của B trong phạm vi ghi trên cạnh. |
| `INFLUENCES` | A có thể tác động đến B theo kênh và điều kiện ghi trên cạnh. |
| `CONTEXTUALIZES` | A cung cấp bối cảnh thể chế, dữ liệu hoặc giả định để diễn giải B. |

<a name="relations-indicators"></a>

## Đo lường, giá và sản lượng

| A | Quan hệ | B | Vì sao liên quan |
| --- | --- | --- | --- |
| [Khan hiếm](foundations.md#km-fnd-scarcity) | `RELATED_TO` | [Đánh đổi](foundations.md#km-fnd-trade-offs) | Giới hạn đầu vào tạo đánh đổi giữa các mục đích sử dụng. |
| [Chi phí cơ hội](foundations.md#km-fnd-opportunity-cost) | `PREREQUISITE_OF` | [Lợi thế so sánh](international-economics.md#km-int-comparative-advantage) | So lợi thế dựa trên chi phí cơ hội tương đối. |
| [Lựa chọn duy lý](foundations.md#km-fnd-rational-choice) | `CONTRASTS_WITH` | [Lý tính hữu hạn](behavioral-economics.md#km-beh-bounded-rationality) | Chuẩn lựa chọn nhất quán và hành vi dưới giới hạn nhận thức trả lời các câu hỏi khác nhau. |
| [Đại lượng tồn và luồng](foundations.md#km-fnd-stocks-flows) | `PREREQUISITE_OF` | [Tài khoản và bảng cân đối theo khu vực](macroeconomics.md#km-mac-sector-accounts) | Tiết kiệm là luồng, còn số dư tài sản và nợ là tồn lượng. |
| [Giá trị danh nghĩa và giá trị thực](foundations.md#km-fnd-nominal-real) | `PREREQUISITE_OF` | [Quy đổi theo mức giá](analytical-tools.md#km-ana-nominal-real-conversion) | Xác định đại lượng sức mua cần giữ trước khi chọn chỉ số giá. |
| [Quy đổi theo mức giá](analytical-tools.md#km-ana-nominal-real-conversion) | `RELATED_TO` | [GDP thực](macroeconomics.md#km-mac-real-gdp) | Tài khoản quốc gia dùng phương pháp khối lượng phù hợp với phạm vi GDP. |
| [Chỉ số và năm gốc](analytical-tools.md#km-ana-index-numbers) | `PREREQUISITE_OF` | [Chỉ số giá tiêu dùng](macroeconomics.md#km-mac-cpi) | Trọng số, kỳ gốc và phạm vi rổ quyết định cách đọc chỉ số. |
| [Chỉ số giá tiêu dùng](macroeconomics.md#km-mac-cpi) | `MEASURES` | [Lạm phát](macroeconomics.md#km-mac-inflation) | Tốc độ đổi của CPI đo lạm phát giá tiêu dùng trên kỳ đã chọn. |
| [Chỉ số giá tiêu dùng](macroeconomics.md#km-mac-cpi) | `CONTRASTS_WITH` | [Chỉ số giảm phát GDP](macroeconomics.md#km-mac-gdp-deflator) | Một chỉ số theo tiêu dùng, còn chỉ số kia theo sản lượng trong nước. |
| [Giá tương đối](foundations.md#km-fnd-relative-price) | `CONTRASTS_WITH` | [Lạm phát](macroeconomics.md#km-mac-inflation) | Một giá tăng tương đối có thể xảy ra dù mức giá chung ổn định. |
| [GDP thực](macroeconomics.md#km-mac-real-gdp) | `MEASURES` | [Tăng trưởng kinh tế dài hạn](macroeconomics.md#km-mac-growth) | Dùng biến động GDP thực qua kỳ hoặc GDP thực đầu người theo câu hỏi. |
| [Cú sốc cung](macroeconomics.md#km-mac-supply-shock) | `INFLUENCES` | [Lạm phát chi phí đẩy](macroeconomics.md#km-mac-cost-push) | Chi phí đầu vào có thể đi vào giá bán nếu doanh nghiệp chuyển được một phần chi phí. |
| [Lạm phát chi phí đẩy](macroeconomics.md#km-mac-cost-push) | `RELATED_TO` | [Đình lạm](macroeconomics.md#km-mac-stagflation) | Cùng cú sốc có thể đẩy giá lên và làm sản lượng suy yếu. |
| [Kỳ vọng lạm phát](macroeconomics.md#km-mac-inflation-expectations) | `INFLUENCES` | [Lạm phát](macroeconomics.md#km-mac-inflation) | Nếu kỳ vọng được phản ánh trong định giá, hợp đồng và quyết định chi tiêu. |
| [Neo kỳ vọng lạm phát](macroeconomics.md#km-mac-expectations-anchoring) | `CONTEXTUALIZES` | [Điều hành theo mục tiêu lạm phát](money-banking.md#km-mon-inflation-targeting) | Độ nhạy của kỳ vọng dài hạn giúp đánh giá cách đọc cam kết ổn định giá. |
| [Lạm phát hòa vốn](macroeconomics.md#km-mac-breakeven-inflation) | `RELATED_TO` | [Kỳ vọng lạm phát](macroeconomics.md#km-mac-inflation-expectations) | Chênh lệch lợi suất cũng có thể biến động theo phần bù và thanh khoản. |
| [Chính sách tài khóa](public-economics.md#km-pub-fiscal-policy) | `RELATED_TO` | [Ổn định kinh tế vĩ mô](macroeconomics.md#km-mac-stabilization) | Thu và chi có thể làm tổng cầu đổi, với mức tác động và độ trễ tùy công cụ. |
| [Thâm hụt tài khóa](public-economics.md#km-pub-fiscal-deficit) | `CONTRASTS_WITH` | [Nợ công](public-economics.md#km-pub-public-debt) | Thâm hụt là luồng theo kỳ, nợ là số dư tại một thời điểm. |
| [Năng suất](macroeconomics.md#km-mac-productivity) | `INFLUENCES` | [Tăng trưởng kinh tế dài hạn](macroeconomics.md#km-mac-growth) | Năng suất cao hơn có thể nâng sản lượng khả thi với các đầu vào cho trước. |

<a name="relations-firms"></a>

## Vi mô, thể chế và doanh nghiệp

| A | Quan hệ | B | Vì sao liên quan |
| --- | --- | --- | --- |
| [Cầu](microeconomics.md#km-mic-demand) | `PREREQUISITE_OF` | [Độ co giãn của cầu theo giá](microeconomics.md#km-mic-price-elasticity-demand) | Độ co giãn theo đường cầu đòi hỏi phân biệt cầu với lượng bán quan sát. |
| [Độ co giãn của cầu theo giá](microeconomics.md#km-mic-price-elasticity-demand) | `RELATED_TO` | [Chiến lược định giá](business-economics.md#km-bus-pricing-strategy) | Phản ứng lượng trước giá giúp dự tính doanh thu, cần xét riêng chi phí và đối thủ. |
| [Độ co giãn của cung theo giá](microeconomics.md#km-mic-price-elasticity-supply) | `RELATED_TO` | [Gánh nặng thuế](public-economics.md#km-pub-tax-incidence) | Phía ít phản ứng hơn thường gánh phần lớn hơn trong mô hình cạnh tranh chuẩn. |
| [Thất bại thị trường](microeconomics.md#km-mic-market-failure) | `RELATED_TO` | [Công cụ can thiệp công](public-economics.md#km-pub-public-intervention) | Đánh giá cả thất bại thị trường lẫn chi phí và giới hạn thực thi. |
| [Bất cân xứng thông tin](microeconomics.md#km-mic-asymmetric-information) | `PREREQUISITE_OF` | [Lựa chọn bất lợi](microeconomics.md#km-mic-adverse-selection) | Cần biết ai nắm thông tin ẩn trước khi giải thích việc thay đổi thành phần tham gia. |
| [Lựa chọn bất lợi](microeconomics.md#km-mic-adverse-selection) | `CONTRASTS_WITH` | [Rủi ro đạo đức](microeconomics.md#km-mic-moral-hazard) | Tách thay đổi loại người tham gia khỏi thay đổi hành động dưới cách chia sẻ hậu quả. |
| [Phát tín hiệu](microeconomics.md#km-mic-signaling) | `CONTRASTS_WITH` | [Sàng lọc](microeconomics.md#km-mic-screening) | Bên có thông tin chủ động phát tín hiệu, bên thiếu thông tin chủ động sàng lọc. |
| [Vấn đề người ủy quyền và đại diện](microeconomics.md#km-mic-principal-agent) | `RELATED_TO` | [Quản trị công ty](corporate-finance.md#km-cf-governance) | Quyền quyết định, giám sát và lợi ích có thể phân bổ khác nhau giữa cổ đông và quản lý. |
| [Ngoại tác](microeconomics.md#km-mic-externality) | `PREREQUISITE_OF` | [Định giá phát thải](specialized-economics.md#km-sp-carbon-pricing) | Hiểu khoảng chênh chi phí tư nhân và xã hội trước khi xét công cụ định giá phát thải. |
| [Chi phí giao dịch](specialized-economics.md#km-sp-transaction-costs) | `RELATED_TO` | [Tự làm hay thuê ngoài](business-economics.md#km-bus-make-or-buy) | Chi phí thương lượng, kiểm tra và thực thi ảnh hưởng lựa chọn ranh giới doanh nghiệp. |
| [Thiết kế thị trường](specialized-economics.md#km-sp-market-design) | `RELATED_TO` | [Lý thuyết trò chơi](microeconomics.md#km-mic-game-theory) | Phản ứng chiến lược giúp đánh giá quy tắc đấu giá hoặc ghép cặp. |
| [Hiệu ứng mạng lưới](specialized-economics.md#km-sp-network-effects) | `RELATED_TO` | [Nền tảng đa phía](specialized-economics.md#km-sp-multi-sided-platforms) | Tăng người dùng một phía có thể làm nền tảng hấp dẫn hơn với phía kia. |
| [Vốn nhân lực](specialized-economics.md#km-sp-human-capital) | `RELATED_TO` | [Kinh tế giáo dục](specialized-economics.md#km-sp-education-economics) | Lợi ích thu nhập từ giáo dục có thể gồm kỹ năng và tín hiệu. |
| [Nhân khẩu học kinh tế](specialized-economics.md#km-sp-demographics) | `CONTEXTUALIZES` | [Lập kế hoạch hưu trí](personal-finance.md#km-pf-retirement-planning) | Tuổi thọ và cơ cấu dân số ảnh hưởng thời hạn cần thu nhập và bối cảnh hệ thống hưu trí. |
| [Bất bình đẳng và dịch chuyển xã hội](specialized-economics.md#km-sp-inequality) | `RELATED_TO` | [Tái phân phối thu nhập](public-economics.md#km-pub-redistribution) | Tác động phân phối phải được đo theo quần thể và giai đoạn thích hợp. |
| [Chi phí thích hợp cho quyết định](accounting.md#km-acc-relevant-cost) | `RELATED_TO` | [Chi phí cơ hội](foundations.md#km-fnd-opportunity-cost) | Giá trị phương án bị từ bỏ là một dữ liệu đầu vào bên cạnh các dòng tiền tương lai thay đổi theo lựa chọn. |
| [Số dư đảm phí](business-economics.md#km-bus-contribution-margin) | `PREREQUISITE_OF` | [Phân tích chi phí–sản lượng–lợi nhuận](business-economics.md#km-bus-cvp-break-even) | Phần đóng góp trên mỗi đơn vị bù chi phí cố định trong mô hình tuyến tính cơ bản. |
| [Đòn bẩy hoạt động](business-economics.md#km-bus-operating-leverage) | `CONTRASTS_WITH` | [Đòn bẩy tài chính](corporate-finance.md#km-cf-financial-leverage) | Một cơ chế qua chi phí vận hành cố định, cơ chế kia qua nghĩa vụ tài trợ. |

<a name="relations-reporting"></a>

## Báo cáo, vốn lưu động và đầu tư doanh nghiệp

| A | Quan hệ | B | Vì sao liên quan |
| --- | --- | --- | --- |
| [Phương trình kế toán](accounting.md#km-acc-accounting-equation) | `PREREQUISITE_OF` | [Bảng cân đối kế toán](accounting.md#km-acc-balance-sheet) | Giải thích vì sao tài sản và nguồn tài trợ cân bằng trong cùng đơn vị. |
| [Cơ sở dồn tích](accounting.md#km-acc-accrual) | `CONTRASTS_WITH` | [Cơ sở tiền mặt](accounting.md#km-acc-cash-basis) | Thời điểm hoạt động và tiêu chí ghi nhận có thể khác thời điểm thanh toán. |
| [Cơ sở dồn tích](accounting.md#km-acc-accrual) | `PREREQUISITE_OF` | [Đối chiếu dòng tiền hoạt động theo phương pháp gián tiếp](accounting.md#km-acc-ocf-reconciliation) | Cần hiểu lợi nhuận dồn tích để điều chỉnh khoản không bằng tiền và độ lệch thu chi. |
| [Dòng tiền từ hoạt động kinh doanh](accounting.md#km-acc-operating-cash-flow) | `COMPONENT_OF` | [Báo cáo lưu chuyển tiền tệ](accounting.md#km-acc-cash-flow-statement) | Dòng kinh doanh là một nhóm trình bày trên báo cáo. |
| [Đối chiếu dòng tiền hoạt động theo phương pháp gián tiếp](accounting.md#km-acc-ocf-reconciliation) | `RELATED_TO` | [Dòng tiền từ hoạt động kinh doanh](accounting.md#km-acc-operating-cash-flow) | Phương pháp gián tiếp là một cách xác định và trình bày dòng tiền kinh doanh. |
| [Dòng tiền từ hoạt động kinh doanh](accounting.md#km-acc-operating-cash-flow) | `RELATED_TO` | [Chất lượng lợi nhuận](accounting.md#km-acc-earnings-quality) | Đối chiếu qua nhiều kỳ có thể gợi ý vấn đề cần kiểm tra thêm. |
| [Phải thu và phải trả thương mại](accounting.md#km-acc-receivables-payables) | `RELATED_TO` | [Vốn lưu động](corporate-finance.md#km-cf-working-capital) | Thay đổi các khoản thương mại có thể làm thay đổi vốn lưu động hoạt động. |
| [Số ngày tồn kho bình quân](corporate-finance.md#km-cf-dio) | `COMPONENT_OF` | [Chu kỳ hoạt động](corporate-finance.md#km-cf-operating-cycle) | Đại diện phần thời gian tồn kho. |
| [Số ngày thu tiền bình quân](corporate-finance.md#km-cf-dso) | `COMPONENT_OF` | [Chu kỳ hoạt động](corporate-finance.md#km-cf-operating-cycle) | Đại diện phần chờ thu tiền khách hàng. |
| [Chu kỳ hoạt động](corporate-finance.md#km-cf-operating-cycle) | `COMPONENT_OF` | [Chu kỳ chuyển đổi tiền mặt](corporate-finance.md#km-cf-cash-conversion-cycle) | Lấy thời gian tồn kho và thu tiền rồi điều chỉnh thời gian trả nhà cung cấp. |
| [Số ngày trả nhà cung cấp bình quân](corporate-finance.md#km-cf-dpo) | `COMPONENT_OF` | [Chu kỳ chuyển đổi tiền mặt](corporate-finance.md#km-cf-cash-conversion-cycle) | Thời gian được nhà cung cấp cho trả chậm là số hạng trừ. |
| [Chu kỳ chuyển đổi tiền mặt](corporate-finance.md#km-cf-cash-conversion-cycle) | `RELATED_TO` | [Tài trợ vốn lưu động](corporate-finance.md#km-cf-working-capital-financing) | Thời gian có thể chỉ ra chỗ cần xem, còn số tiền cần lập lịch dòng tiền. |
| [Tín dụng thương mại](corporate-finance.md#km-cf-trade-credit) | `APPLICATION_OF` | [Tài trợ vốn lưu động](corporate-finance.md#km-cf-working-capital-financing) | Nhà cung cấp tài trợ một phần hoạt động khi cho trả sau. |
| [Bao thanh toán](corporate-finance.md#km-cf-factoring) | `APPLICATION_OF` | [Tài trợ vốn lưu động](corporate-finance.md#km-cf-working-capital-financing) | Có thể ứng tiền trên phải thu, với truy đòi tùy hợp đồng. |
| [Giá trị thời gian của tiền](corporate-finance.md#km-cf-time-value) | `PREREQUISITE_OF` | [Giá trị hiện tại ròng](corporate-finance.md#km-cf-npv) | Quy đổi dòng tiền về cùng ngày để cộng và so với vốn đầu tư. |
| [Giá trị hiện tại ròng](corporate-finance.md#km-cf-npv) | `APPLICATION_OF` | [Thẩm định đầu tư vốn](corporate-finance.md#km-cf-capital-budgeting) | Một tiêu chí đánh giá giá trị tăng thêm theo giả định dòng tiền và chi phí vốn. |
| [Chi phí vốn bình quân gia quyền](corporate-finance.md#km-cf-wacc) | `APPLICATION_OF` | [Chi phí vốn](corporate-finance.md#km-cf-cost-of-capital) | Phối hợp suất sinh lời đòi hỏi theo cấu trúc tài trợ có liên quan. |
| [Đòn bẩy tài chính](corporate-finance.md#km-cf-financial-leverage) | `INFLUENCES` | [Rủi ro tái tài trợ](risk-crises.md#km-rsk-refinancing-risk) | Nợ đến hạn nhiều hơn có thể làm rủi ro tăng nếu nguồn thay thế khó tiếp cận. |

<a name="relations-markets"></a>

## Tiền tệ, trái phiếu và danh mục

| A | Quan hệ | B | Vì sao liên quan |
| --- | --- | --- | --- |
| [Bảng cân đối kế toán](accounting.md#km-acc-balance-sheet) | `PREREQUISITE_OF` | [Bảng cân đối ngân hàng](money-banking.md#km-mon-bank-balance-sheet) | Áp dụng phân loại tài sản và nghĩa vụ theo góc nhìn ngân hàng. |
| [Dự trữ ngân hàng và tiền gửi](money-banking.md#km-mon-reserves-deposits) | `PREREQUISITE_OF` | [Tạo và hủy tiền gửi ngân hàng](money-banking.md#km-mon-bank-money-creation) | Phân biệt tiền gửi được tạo với tài sản quyết toán sau chuyển khoản. |
| [Tiền cơ sở](money-banking.md#km-mon-monetary-base) | `CONTRASTS_WITH` | [Các khối tiền tệ](money-banking.md#km-mon-monetary-aggregates) | Tiền cơ sở và tiền rộng có phạm vi chủ thể và công cụ không trùng nhau. |
| [Tốc độ lưu thông tiền](money-banking.md#km-mon-money-velocity) | `COMPONENT_OF` | [Lý thuyết số lượng tiền](money-banking.md#km-mon-quantity-theory) | Cách giả định tốc độ lưu thông phản ứng là một phần của lập luận lý thuyết. |
| [Lãi suất điều hành](money-banking.md#km-mon-policy-rates) | `RELATED_TO` | [Truyền dẫn chính sách tiền tệ](money-banking.md#km-mon-monetary-transmission) | Lãi điều hành tác động qua lãi thị trường, tín dụng, tài sản, tỷ giá và kỳ vọng tùy bối cảnh. |
| [Khung điều hành lãi suất](money-banking.md#km-mon-operating-frameworks) | `CONTEXTUALIZES` | [Lãi suất điều hành](money-banking.md#km-mon-policy-rates) | Vị trí của một lãi công bố tùy hệ thống dự trữ, công cụ và mục tiêu vận hành. |
| [Giao dịch mua lại](financial-markets.md#km-mkt-repo) | `RELATED_TO` | [Nghiệp vụ thị trường mở](money-banking.md#km-mon-open-market-operations) | Ngân hàng trung ương có thể dùng repo trong OMO, thị trường tư nhân cũng giao dịch repo. |
| [Chênh lệch tái định giá lãi suất](money-banking.md#km-mon-repricing-gap) | `INFLUENCES` | [Biên lãi ròng](money-banking.md#km-mon-net-interest-margin) | Tùy thời điểm, hệ số truyền lãi và quy mô tài sản sinh lãi. |
| [Thanh khoản tài trợ của ngân hàng](money-banking.md#km-mon-bank-funding-liquidity) | `CONTRASTS_WITH` | [Thanh khoản thị trường](financial-markets.md#km-mkt-market-liquidity) | Huy động tiền đúng hạn và bán tài sản ít tác động giá là hai vấn đề liên quan. |
| [Tỷ lệ bao phủ thanh khoản](money-banking.md#km-mon-lcr) | `MEASURES` | [Bộ đệm thanh khoản ngân hàng](money-banking.md#km-mon-liquidity-buffers) | Chuẩn hóa phần đệm tài sản tương ứng với kịch bản dòng tiền ra ngắn hạn. |
| [Khả năng thanh toán theo giá trị của ngân hàng](money-banking.md#km-mon-bank-solvency) | `CONTRASTS_WITH` | [Thanh khoản tài trợ của ngân hàng](money-banking.md#km-mon-bank-funding-liquidity) | Tài sản có thể đủ bù nghĩa vụ theo định giá nhưng chưa chuyển thành tiền đúng lúc. |
| [Bù trừ giao dịch](financial-markets.md#km-mkt-clearing) | `RELATED_TO` | [Quyết toán và lưu ký chứng khoán](financial-markets.md#km-mkt-settlement-custody) | Bù trừ xác định nghĩa vụ, quyết toán thực hiện chuyển giao. |
| [Chênh lệch giá mua và bán](financial-markets.md#km-mkt-bid-ask) | `MEASURES` | [Thanh khoản thị trường](financial-markets.md#km-mkt-market-liquidity) | Phản ánh một phần chi phí giao dịch, cần xem thêm độ sâu và tác động lên giá. |
| [Giá trị thời gian của tiền](corporate-finance.md#km-cf-time-value) | `PREREQUISITE_OF` | [Giá trái phiếu và lợi suất đến đáo hạn](investment.md#km-inv-bond-pricing-ytm) | Giá trái phiếu được tính từ dòng tiền chiết khấu. |
| [Giá trái phiếu và lợi suất đến đáo hạn](investment.md#km-inv-bond-pricing-ytm) | `PREREQUISITE_OF` | [Duration trái phiếu](investment.md#km-inv-duration) | Độ nhạy giá cần có quan hệ giá và lợi suất được xác định. |
| [Duration trái phiếu](investment.md#km-inv-duration) | `MEASURES` | [Rủi ro lãi suất](risk-crises.md#km-rsk-interest-rate-risk) | Duration điều chỉnh đo xấp xỉ độ nhạy giá trước mức đổi lợi suất nhỏ theo giả định bài toán. |
| [Phần bù kỳ hạn](financial-markets.md#km-mkt-term-premium) | `RELATED_TO` | [Cấu trúc kỳ hạn và đường cong lợi suất](financial-markets.md#km-mkt-term-structure) | Phần bù có thể làm độ dốc khác với dự kiến về lãi suất ngắn hạn. |
| [Tương quan](analytical-tools.md#km-ana-correlation) | `PREREQUISITE_OF` | [Rủi ro danh mục](investment.md#km-inv-portfolio-risk) | Biết mức cùng biến động để tính phương sai danh mục theo trọng số. |
| [Rủi ro hệ thống thị trường và rủi ro riêng](investment.md#km-inv-systematic-idiosyncratic) | `CONTRASTS_WITH` | [Rủi ro hệ thống tài chính](risk-crises.md#km-rsk-systemic-risk) | Rủi ro chung trong lợi suất khác với nguy cơ gián đoạn chức năng tài chính toàn hệ thống. |
| [Rủi ro danh mục](investment.md#km-inv-portfolio-risk) | `RELATED_TO` | [Đa dạng hóa](investment.md#km-inv-diversification) | Đa dạng hóa phụ thuộc rủi ro và mức cùng biến động, không chỉ số lượng khoản đầu tư. |
| [Bán tháo tài sản](risk-crises.md#km-rsk-fire-sales) | `INFLUENCES` | [Lây lan tài chính](risk-crises.md#km-rsk-contagion) | Bán gấp có thể ép giá tài sản chung và làm xấu bảng cân đối của bên khác. |
| [Bảo hiểm tiền gửi](risk-crises.md#km-rsk-deposit-insurance) | `INFLUENCES` | [Rút tiền hàng loạt](risk-crises.md#km-rsk-bank-runs) | Bảo vệ đáng tin cậy có thể giảm động cơ rút trước với tiền gửi đủ điều kiện. |
| [Người cho vay cuối cùng](risk-crises.md#km-rsk-lender-last-resort) | `RELATED_TO` | [Thanh khoản tài trợ của ngân hàng](money-banking.md#km-mon-bank-funding-liquidity) | Hỗ trợ có điều kiện có thể bù thiếu hụt thanh khoản ngắn hạn. |

<a name="relations-households"></a>

## Hành vi, hộ gia đình và bối cảnh Việt Nam

| A | Quan hệ | B | Vì sao liên quan |
| --- | --- | --- | --- |
| [Phụ thuộc điểm tham chiếu](behavioral-economics.md#km-beh-reference-dependence) | `COMPONENT_OF` | [Lý thuyết triển vọng](behavioral-economics.md#km-beh-prospect-theory) | Đánh giá kết quả theo mức thay đổi quanh điểm tham chiếu. |
| [Ngại thua lỗ](behavioral-economics.md#km-beh-loss-aversion) | `RELATED_TO` | [Hiệu ứng bán lãi sớm, giữ lỗ lâu](behavioral-economics.md#km-beh-disposition-effect) | Một cơ chế được đề xuất, bên cạnh các giải thích khác và điều kiện thị trường. |
| [Kế toán tinh thần](behavioral-economics.md#km-beh-mental-accounting) | `RELATED_TO` | [Ngân sách cá nhân](personal-finance.md#km-pf-personal-budget) | Đặt ngăn ngân sách có thể hỗ trợ cam kết và cũng tạo phân bổ cứng nhắc. |
| [Dòng tiền hộ gia đình](personal-finance.md#km-pf-household-cash-flow) | `PREREQUISITE_OF` | [Quỹ dự phòng](personal-finance.md#km-pf-emergency-fund) | Lịch thu chi cho biết thiếu tiền ở thời điểm nào và trong kịch bản nào. |
| [Thanh khoản hộ gia đình](personal-finance.md#km-pf-household-liquidity) | `CONTRASTS_WITH` | [Tài sản ròng hộ gia đình](personal-finance.md#km-pf-household-net-worth) | Đủ tài sản ròng có thể vẫn thiếu tiền sẵn dùng đúng hạn. |
| [Giá trị thời gian của tiền](corporate-finance.md#km-cf-time-value) | `PREREQUISITE_OF` | [Chi phí vay hiệu dụng](personal-finance.md#km-pf-effective-borrowing-cost) | Các lịch vay chỉ so sánh được khi đặt dòng tiền vào đúng mốc thời gian. |
| [Tài khoản vãng lai](international-economics.md#km-int-current-account) | `COMPONENT_OF` | [Cán cân thanh toán quốc tế](international-economics.md#km-int-balance-of-payments) | Vãng lai là một tài khoản bên cạnh tài khoản vốn và tài khoản tài chính. |
| [Dòng vốn xuyên biên giới](international-economics.md#km-int-capital-flows) | `RELATED_TO` | [Vị thế đầu tư quốc tế](international-economics.md#km-int-international-investment-position) | Giao dịch giải thích một phần biến động vị thế cùng định giá lại và các thay đổi khác. |
| [Tỷ giá danh nghĩa song phương](international-economics.md#km-int-exchange-rate) | `PREREQUISITE_OF` | [Truyền dẫn tỷ giá vào giá](international-economics.md#km-int-pass-through) | Cần quy ước yết giá trước khi tính giá nhập khẩu bằng nội tệ. |
| [Đồng tiền ghi giá và thanh toán trong thương mại](international-economics.md#km-int-currency-invoicing) | `CONTEXTUALIZES` | [Truyền dẫn tỷ giá vào giá](international-economics.md#km-int-pass-through) | Đồng tiền ghi giá ảnh hưởng nơi biến động tỷ giá xuất hiện trước. |
| [Truyền dẫn tỷ giá VND vào giá tiêu dùng](vietnam.md#km-vn-vnd-price-pass-through) | `APPLICATION_OF` | [Truyền dẫn tỷ giá vào giá](international-economics.md#km-int-pass-through) | Áp dụng cơ chế chung vào cấu trúc nhập khẩu, định giá và CPI Việt Nam. |
| [Khung điều hành của Ngân hàng Nhà nước](vietnam.md#km-vn-sbv-framework) | `CONTEXTUALIZES` | [Khung điều hành lãi suất](money-banking.md#km-mon-operating-frameworks) | Đọc công cụ và thẩm quyền trong phạm vi điều hành trong nước. |
| [Tổ chức thị trường chứng khoán Việt Nam](vietnam.md#km-vn-domestic-securities) | `CONTEXTUALIZES` | [Quyết toán và lưu ký chứng khoán](financial-markets.md#km-mkt-settlement-custody) | Nối khái niệm chung với hạ tầng đăng ký, lưu ký và quyết toán trong nước. |
| [Chế độ kế toán doanh nghiệp Việt Nam](vietnam.md#km-vn-local-accounting) | `CONTEXTUALIZES` | [Liên kết các báo cáo tài chính](accounting.md#km-acc-statement-integration) | Phạm vi báo cáo và quy tắc theo kỳ áp dụng cần được tra theo chế độ trong nước. |
| [FDI tại Việt Nam](vietnam.md#km-vn-local-fdi) | `CONTEXTUALIZES` | [Đầu tư trực tiếp nước ngoài](international-economics.md#km-int-fdi) | Tách số liệu đăng ký và thực hiện ở Việt Nam trước khi đối chiếu thống kê đối ngoại. |
| [Tín dụng và chu kỳ bất động sản Việt Nam](vietnam.md#km-vn-local-real-estate-credit) | `CONTEXTUALIZES` | [Rủi ro tái tài trợ](risk-crises.md#km-rsk-refinancing-risk) | Đọc nghĩa vụ đáo hạn, tín dụng và tài sản bảo đảm trong bối cảnh dự án nhà đất. |
| [Hệ thống chỉ tiêu thống kê Việt Nam](vietnam.md#km-vn-nso-indicators) | `CONTEXTUALIZES` | [Chỉ số giá tiêu dùng](macroeconomics.md#km-mac-cpi) | Tìm quyền số, kỳ gốc và phạm vi đối tượng trong phương pháp công bố. |
| [Đối chứng phản thực](analytical-tools.md#km-ana-counterfactual) | `PREREQUISITE_OF` | [Tương quan và suy luận nhân quả](analytical-tools.md#km-ana-causation) | Tác động đòi hỏi so kết quả quan sát với điều kiện khác có thể xảy ra. |
| [Tương quan và suy luận nhân quả](analytical-tools.md#km-ana-causation) | `CONTRASTS_WITH` | [Tương quan](analytical-tools.md#km-ana-correlation) | Tương quan mô tả cách hai biến biến động cùng hoặc ngược chiều. Tác động cần thiết kế nhận diện và giả định. |
| [Biến gây nhiễu](analytical-tools.md#km-ana-confounding) | `RELATED_TO` | [Trực giác hồi quy](analytical-tools.md#km-ana-regression) | Thêm biến có thể hỗ trợ so sánh có điều kiện, với giới hạn về biến bỏ sót và cách đo. |
