---
id: CORP-003
title: "Đòn bẩy tài chính: vì sao lợi nhuận trên vốn tăng kèm rủi ro mất vốn?"
category: corporate-and-markets
tags: [financial-leverage, debt, return-on-equity, cash-flow, refinancing-risk]
prerequisites: [CORP-002, MONEY-002]
difficulty: Intermediate
date: 2026-10-18
last_verified: 2026-10-18
---

# Đòn bẩy tài chính: vì sao lợi nhuận trên vốn tăng kèm rủi ro mất vốn?

## 1. Chủ đề hôm nay

**Đòn bẩy tài chính (financial leverage)**: dùng nợ để tài trợ tài sản và làm thay đổi kết quả dành cho vốn chủ sở hữu.

Bài này nối hai nền tảng: [CORP-002 — lợi nhuận và dòng tiền](cash-flow-statement-and-operating-cash-flow.md) và [MONEY-002 — lãi suất và kênh truyền dẫn](../monetary-and-banking/policy-rates-and-monetary-transmission.md). Phạm vi là doanh nghiệp phi tài chính; các con số trong bài đều **giả định**, dùng để tách riêng cơ chế. Ngày `last_verified` ghi lần đối chiếu các tài liệu tham khảo, không phải ngày khảo sát lãi vay thị trường.

## 2. Vấn đề cốt lõi

Hai doanh nghiệp có cùng tài sản và cùng lợi nhuận từ kinh doanh. Doanh nghiệp vay nợ phải trả thêm lãi, nên lợi nhuận còn lại ít hơn. Thế mà tỷ suất lợi nhuận trên vốn chủ của nó vẫn có thể cao hơn.

Điểm mấu chốt nằm ở **cả phần lợi nhuận còn lại lẫn lượng vốn chủ đã bỏ ra**. Một khoản lợi nhuận nhỏ hơn chia cho một nền vốn nhỏ hơn nữa có thể cho tỷ suất cao hơn. Nhưng khi kinh doanh xấu đi, phần lỗ cũng dồn vào nền vốn nhỏ ấy, trong khi nghĩa vụ trả nợ vẫn đến hạn.

## 3. Giải thích cơ chế

### 3.1. Ai cung cấp vốn, ai nhận phần còn lại?

**[Definition]** **Cấu trúc vốn (capital structure)** là cách kết hợp nợ và vốn chủ để tài trợ doanh nghiệp. Người cho vay nhận quyền đòi gốc và lãi theo hợp đồng; cổ đông nhận phần kết quả còn lại sau các nghĩa vụ liên quan. Dùng nợ tạo đòn bẩy tài chính. Xem [OpenStax, §17.1](https://openstax.org/books/principles-finance/pages/17-1-the-concept-of-capital-structure).

Động cơ của các bên khác nhau:

| Chủ thể | Điều họ tìm kiếm | Điều họ phải chú ý |
| :--- | :--- | :--- |
| Chủ doanh nghiệp/cổ đông | Tài trợ hoạt động với ít vốn tự góp hơn, giữ quyền sở hữu, nhận phần lợi nhuận còn lại | Lãi vay có thể ăn hết lợi nhuận; vốn chủ chịu lỗ trước chủ nợ trong ví dụ đơn giản |
| Chủ nợ | Thu đủ gốc và lãi đúng lịch | Dòng tiền trả nợ, tài sản bảo đảm và khả năng thu hồi khi có sự cố |
| Ban điều hành | Có vốn triển khai hoạt động và duy trì doanh nghiệp | Cân bằng cơ hội kinh doanh với sức ép trả nợ và các cam kết hợp đồng |

**[Causal Mechanism]** Với lãi vay cố định trong kỳ, EBIT biến động nhưng chi phí lãi không giảm tương ứng → phần lợi nhuận dành cho cổ đông biến động mạnh so với vốn họ góp. Cơ chế phần dư này được giải thích trong [OpenStax, §17.4](https://openstax.org/books/principles-finance/pages/17-4-capital-structure-choices).

### 3.2. Giữ đúng bảng cân đối trước khi tính tỷ suất

**[Accounting Identity]** Trên cùng một cơ sở kế toán:

$$
A=L+E
$$

Trong đó, $A$ là tổng tài sản, $L$ là toàn bộ nợ phải trả, $E$ là vốn chủ. Nếu tách $L=D+O$, với $D$ là nợ vay và $O$ là các nghĩa vụ khác, thì phải viết $A=D+O+E$. Chẳng hạn, phải trả người bán không tự biến mất chỉ vì ta chỉ đang quan tâm đến nợ ngân hàng.

Chỉ khi **giả định $O=0$** mới rút gọn thành $A=D+E$. Bài dùng giả định đó trong mô hình bên dưới. Tài sản và vốn chủ ở đây đo theo sổ sách, không trộn với vốn hóa thị trường. Đồng nhất thức và sự phân biệt cơ sở định giá được trình bày trong [OpenStax, §17.1](https://openstax.org/books/principles-finance/pages/17-1-the-concept-of-capital-structure).

Hai cách tài trợ **tại thời điểm bắt đầu** cho cùng 1.000 triệu đồng tài sản:

| Phương án giả định | Tài sản $A_0$ | Nợ vay $D$ | Vốn chủ $E_0$ | Kiểm tra |
| :--- | ---: | ---: | ---: | :--- |
| U: hoàn toàn bằng vốn chủ | 1.000 | 0 | 1.000 | 1.000 = 0 + 1.000 |
| L: có vay nợ | 1.000 | 600 | 400 | 1.000 = 600 + 400 |

**[Definition]** **Tỷ lệ nợ vay trên vốn chủ (debt-to-equity ratio — D/E)** trong bài là nợ vay chia vốn chủ trên cùng cơ sở đo. Với L tại đầu kỳ, tỷ lệ bằng $600/400=1{,}5$ lần. Khi đọc tài liệu khác, phải kiểm tra “debt” có bao gồm toàn bộ nợ phải trả hay không.

Đây là hai phương án tài trợ riêng cho cùng hoạt động. Khi doanh nghiệp L nhận tiền vay, tiền nhận được là tài sản và nghĩa vụ hoàn trả là nợ; tiền vay không phải doanh thu. Để kiểm tra riêng một giao dịch cho vay 600 triệu từ **chủ nợ phi ngân hàng bằng tiền sẵn có**, biến động trước khi dùng tiền là:

| Chủ thể | Biến động tài sản | Biến động nợ phải trả | Biến động vốn chủ |
| :--- | :--- | :--- | :--- |
| Doanh nghiệp vay | Tiền +600 | Nợ vay +600 | 0 |
| Chủ nợ phi ngân hàng | Tiền −600; khoản cho vay +600, tổng tài sản không đổi | 0 | 0 |

Mỗi bên đều cân đối. Bảng này chỉ minh họa khoản vay từ phi ngân hàng, không mô tả bút toán tạo tiền gửi khi ngân hàng cấp tín dụng.

### 3.3. TEXTBOOK MODEL — Mô hình giáo trình

**[Theoretical Model] Các giả định:**

- Xét một năm; hai phương án có cùng tài sản đầu kỳ và cùng kết quả kinh doanh trước lãi vay trong mỗi kịch bản.
- Chỉ có nợ vay và vốn cổ đông thường; bỏ thuế, phí vay và mọi khoản thu nhập/chi phí ngoài các mục được nêu.
- Nợ vay $D$ không đổi suốt năm; lãi suất $i$ cố định, toàn bộ lãi được ghi nhận và trả cuối năm. Gốc đáo hạn sau kỳ đang xét.
- Không góp thêm vốn hay chia cổ tức trong năm; $E_0>0$. Các tỷ suất mô hình đều dùng **cơ sở đầu kỳ**, không giả định tài sản cuối kỳ bằng tài sản đầu kỳ.

**[Definition]** **Lợi nhuận trước lãi vay và thuế (earnings before interest and taxes — EBIT)** trong mô hình là lợi nhuận hoạt động sau các chi phí kinh doanh, gồm khấu hao, nhưng trước chi phí lãi vay và thuế. EBIT là chỉ tiêu lợi nhuận, chưa cho biết đã thu được bao nhiêu tiền.

Đặt $I=iD$ là chi phí lãi năm và $NI$ là lợi nhuận còn lại cho cổ đông. Từ các giả định:

$$
NI=EBIT-iD
$$

Đặt $r_A=EBIT/A_0$, tức tỷ suất hoạt động trước lãi và thuế trên **tài sản đầu kỳ**. Đây là ký hiệu của bài, không mặc định bằng mọi chỉ tiêu ROA trong báo cáo phân tích.

**[Definition]** **Tỷ suất lợi nhuận trên vốn chủ sở hữu (return on equity — ROE)** so sánh lợi nhuận thuộc cổ đông với nền vốn chủ tương ứng. Ở đây ký hiệu riêng $ROE_0=NI/E_0$ để nhấn mạnh mẫu số đầu kỳ. Khi phân tích báo cáo, ROE thường dùng vốn chủ bình quân, như công thức trong [OpenStax, §6.6](https://openstax.org/books/principles-finance/pages/6-6-profitability-ratios-and-the-dupont-method); phải đọc quy ước trước khi so sánh.

Thay $A_0=D+E_0$, ta tự suy ra:

$$
ROE_0
=\frac{r_A(D+E_0)-iD}{E_0}
=r_A+(r_A-i)\frac{D}{E_0}
$$

**Ý nghĩa kinh tế:** với các giả định trên, đòn bẩy làm tỷ suất của cổ đông cao hơn phương án không vay khi $r_A>i$, thấp hơn khi $r_A<i$, và bằng nhau khi $r_A=i$. Chênh lệch đó được nhân với tỷ lệ nợ vay/vốn chủ.

Đây là phép phân rã tỷ suất kế toán trong mô hình; không phải công thức lợi suất cổ phiếu hay bằng chứng rằng tăng nợ tự tạo thêm giá trị doanh nghiệp.

### 3.4. REAL-WORLD MECHANISM — Cơ chế thực tế

**[Causal Mechanism]** Trong thực tế, doanh nghiệp phải thương lượng khoản vay, chịu thẩm định, thỏa thuận lịch trả nợ và đáp ứng điều kiện hợp đồng. Tiền vay được dùng cho tài sản hoặc hoạt động; sau đó doanh nghiệp phải tạo hoặc huy động tiền để trả từng nghĩa vụ đúng lịch. Lợi nhuận kế toán chỉ giải thích một phần khả năng ấy.

Các điều kiện bị giữ cố định trong mô hình có thể thay đổi:

- **Chi phí vay:** lãi thả nổi chỉ đổi theo cơ chế điều chỉnh trong hợp đồng; lãi cố định không tự đổi ngay khi lãi suất thị trường tăng. Khi vay thêm hoặc tái tài trợ, điều kiện mới có thể bất lợi hơn.
- **Kết quả hoạt động:** nếu nợ tài trợ mở rộng quy mô, EBIT có thể đổi; không được giữ nguyên EBIT rồi coi đó là toàn bộ kết quả của dự án mở rộng.
- **Nguồn vốn và điều kiện vay:** chủ nợ có thể yêu cầu bảo đảm, giới hạn vay thêm hoặc các cam kết tài chính. **Điều khoản ràng buộc khoản vay (loan covenant)** là cam kết như vậy; hậu quả vi phạm phải theo hợp đồng cụ thể.
- **Lịch đáo hạn:** **rủi ro tái tài trợ (refinancing risk)** xuất hiện khi cần nguồn vốn mới thay khoản đến hạn nhưng không huy động được, hoặc chỉ huy động với điều kiện xấu hơn. Đây khác công cụ tái cấp vốn của NHTW.

**[Causal Mechanism]** Kinh doanh yếu → ít tiền phục vụ nợ → khó đáp ứng lịch trả → có thể phải thu hẹp hoạt động, thương lượng lại hoặc bán tài sản. Nếu bán gấp dưới giá trị ghi sổ, khoản lỗ còn làm mỏng vốn chủ; nợ không tự giảm tương ứng. Chi phí khó khăn tài chính là một lý do thực tế hạn chế lợi ích của việc vay thêm. Xem [OpenStax, §17.5](https://openstax.org/books/principles-finance/pages/17-5-optimal-capital-structure).

## 4. Ví dụ trực quan: tỷ suất cao hơn đi cùng độ nhạy lớn hơn

**[Theoretical Model — số liệu giả định]** Dùng hai phương án ở mục 3.2 và lãi vay **10%/năm**. Phương án L chịu $600\times10\%=60$ triệu tiền lãi; U không có lãi vay. Đơn vị lợi nhuận trong bảng là triệu đồng/năm.

| Kịch bản EBIT | NI của U | $ROE_0$ của U | NI của L sau lãi | $ROE_0$ của L |
| ---: | ---: | ---: | ---: | ---: |
| 150 | 150 | 15% | 90 | 22,5% |
| 80 | 80 | 8% | 20 | 5% |
| 30 | 30 | 3% | −30 | −7,5% |
| −50 | −50 | −5% | −110 | −27,5% |

Ở kịch bản EBIT 150, phương án L để lại **90 triệu trên 400 triệu vốn chủ**, nên tỷ suất 22,5% cao hơn 15% của U. Nhưng lợi nhuận tuyệt đối sau lãi vẫn thấp hơn: 90 so với 150 triệu. Hai con số trả lời hai câu hỏi khác nhau.

Khi EBIT chỉ còn 30, hoạt động vẫn có lợi nhuận trước lãi, nhưng không đủ bù 60 triệu chi phí lãi: L lỗ 30 triệu. Khi EBIT âm 50, cổ đông còn chịu thêm sức ép lãi vay và lỗ 110 triệu.

Một cách nhìn trực tiếp hơn: EBIT thay đổi 10 triệu thì NI của mỗi phương án cũng thay đổi 10 triệu. Với U, $10/1.000$ làm tỷ suất đổi **1 điểm phần trăm**; với L, $10/400$ làm tỷ suất đổi **2,5 điểm phần trăm**. Đòn bẩy ở đây khuếch đại **độ nhạy** 2,5 lần, không có nghĩa mọi mức ROE của L bằng 2,5 lần U.

Hai ngưỡng cần tách:

- EBIT **60 triệu**: L vừa đủ bù chi phí lãi, NI bằng 0 trong mô hình.
- EBIT **100 triệu**: $r_A=10\%=i$, hai phương án cùng $ROE_0=10\%$. Đây là ngưỡng so sánh tỷ suất, không phải điểm lợi nhuận của L bằng 0.

### Khi một khoản lỗ làm vốn chủ mỏng đi

**[Accounting Identity — tình huống giả định riêng]** Bắt đầu lại từ bảng cân đối L: $A=1.000,D=600,E=400$. Giả sử một tổn thất tài sản **100 triệu được ghi nhận trực tiếp làm giảm tài sản và vốn chủ**, không có thuế, bảo hiểm hoặc thay đổi nợ:

$$
A=900=600+300
$$

Tài sản giảm 10%, nhưng vốn chủ giảm $100/400=25\%$; nợ vay/vốn chủ tăng từ $600/400=1{,}5$ lên $600/300=2$ lần. Vốn chủ hấp thụ tổn thất trên nền nhỏ hơn, nên tỷ lệ mất vốn lớn hơn.

Ví dụ này nói về tổn thất **đã được ghi nhận trên cùng cơ sở kế toán**. Giá thị trường giảm không mặc định khiến mọi tài sản ghi sổ giảm ngay, và giảm giá trị tài sản không tự đồng nghĩa đã chi tiền mặt. Đây cũng không phải phép tính mức giảm của giá cổ phiếu.

## 5. Tình huống thực tế: lãi suất tăng và khách hàng trả tiền chậm

### 5.1. Lãi vay đổi trong khi hoạt động chưa kịp phục hồi

**[Theoretical Model — kịch bản giả định]** Giữ EBIT 80 triệu và D 600 triệu. So sánh hai năm/kịch bản mà **lãi suất tương ứng được áp dụng trọn năm**:

| Lãi suất | Chi phí lãi | NI | $ROE_0$, với $E_0=400$ |
| ---: | ---: | ---: | ---: |
| 10% | 60 | 20 | 5% |
| 14% | 84 | −4 | −1% |

Chi phí tăng 24 triệu làm lợi nhuận 20 triệu chuyển thành lỗ 4 triệu dù EBIT không đổi. Kịch bản 14% phù hợp khi khoản vay đã được điều chỉnh hoặc ký lại với mức ấy cho cả kỳ; không áp thẳng cho khoản lãi cố định chưa đến ngày điều chỉnh.

**[Causal Mechanism]** Nếu cùng lúc khách hàng mua ít hơn, EBIT còn có thể giảm. Nếu khách vẫn mua nhưng trả tiền chậm, lợi nhuận có thể chưa giảm tương ứng mà tiền sẵn trả nợ đã ít đi. Tác động thực tế phụ thuộc cả kinh doanh, hợp đồng lãi suất và lịch thu tiền, không thể suy từ một mức lãi suất điều hành ra toàn bộ kết quả doanh nghiệp.

### 5.2. Có lợi nhuận và hệ số bảo đảm lãi lớn hơn 1 vẫn thiếu tiền

**[Definition]** **Hệ số bảo đảm lãi vay (interest coverage ratio — ICR)** trong bài dùng $ICR=EBIT/I$, với $I>0$ và các đại lượng cùng kỳ. Nó cho biết lợi nhuận trước lãi gấp bao nhiêu lần chi phí lãi; đây là chỉ tiêu lợi nhuận, chưa kiểm tra đủ lịch tiền trả cả gốc và lãi. Công thức EBIT/lãi được trình bày trong [OpenStax, §6.4](https://openstax.org/books/principles-finance/pages/6-4-solvency-ratios).

**[Theoretical Model — tình huống giả định riêng]** Lấy EBIT 80 và lãi 60 triệu như trên, nhưng **đổi lịch gốc: 100 triệu đến hạn ngay cuối năm**, sau khi tính lãi cả năm. Thêm các giả định dòng tiền:

- Đầu năm có 20 triệu tiền sử dụng được.
- Khấu hao 20 triệu là khoản phi tiền duy nhất cần cộng lại.
- Phải thu và tồn kho tăng tổng cộng 70 triệu; không có phải trả hoạt động hay khoản điều chỉnh khác. Đây là phần tăng vốn lưu động hoạt động, loại trừ tiền và nợ vay.
- Không thuế, không mua tài sản cố định mới, không cổ tức, không bán tài sản, không góp vốn hay vay mới. Tính tổng nguồn và nghĩa vụ tại cuối năm; lịch trong năm có thể tạo thêm sức ép sớm hơn.

Tiền tạo ra từ hoạt động **trước trả lãi**:

$$
C_{\text{trước lãi}}=EBIT+\text{khấu hao}-\Delta\text{vốn lưu động hoạt động}
=80+20-70=30\text{ triệu}
$$

Khấu hao làm giảm EBIT nhưng không chi tiền trong kỳ nên cộng lại. Phải thu và tồn kho tăng giữ thêm tiền trong hoạt động nên trừ đi. Ta gọi rõ đây là tiền trước lãi để tránh lẫn với cách phân loại lãi trong báo cáo lưu chuyển tiền tệ.

| Đối chiếu thanh toán cuối năm | Triệu đồng |
| :--- | ---: |
| Tiền đầu năm + tiền từ hoạt động trước lãi | 20 + 30 = 50 |
| Lãi + gốc đến hạn | 60 + 100 = 160 |
| **Nguồn thanh toán còn thiếu** | **160 − 50 = 110** |

Trong khi đó, NI vẫn là $80-60=20$ triệu và ICR là $80/60\approx1{,}33$ lần. Doanh nghiệp có lợi nhuận, nhưng theo các nguồn đã giả định, **thiếu 110 triệu để hoàn thành toàn bộ nghĩa vụ cuối năm**. Đây là khoảng thiếu cần xử lý, không phải số dư tiền mặt thực tế được phép âm khi chưa có nguồn tài trợ.

**[Accounting Identity]** Trả gốc bằng tiền làm giảm tiền và giảm nợ cùng một lượng; bản thân phần gốc trả không phải chi phí làm giảm NI. Vì vậy báo cáo lợi nhuận không thể thay lịch trả nợ. Nếu tính tiền sau lãi từ NI, kết quả là $20+20-70=-30$ triệu; khi đó chỉ cộng tiền đầu kỳ và trừ gốc, **không trừ lãi 60 triệu thêm lần nữa**.

Ví dụ minh họa thiếu thanh khoản; nó chưa đủ để kết luận vốn chủ âm hoặc đã rơi vào một thủ tục phá sản pháp lý.

**[Historical Claim]** Một trường hợp thực tế khác về sự khác biệt này được [RBA phân tích năm 2023](https://www.rba.gov.au/publications/bulletin/2023/jun/leverage-liquidity-and-non-bank-financial-institutions.html): trong căng thẳng năng lượng châu Âu năm 2022, nghĩa vụ bổ sung ký quỹ tạo nhu cầu tiền tức thời, kể cả với nhà sản xuất còn được đánh giá có khả năng thanh toán tổng thể. Cơ chế ở nguồn là ký quỹ trên hợp đồng phái sinh, không phải lịch trả khoản vay thông thường trong ví dụ của bài.

## 6. Những hiểu lầm thường gặp

| Hiểu lầm | Cách phân tích đúng hơn |
| :--- | :--- |
| “ROE cao hơn chứng tỏ kinh doanh tốt hơn.” | Tách thay đổi EBIT khỏi thay đổi cấu trúc tài trợ và mẫu số vốn chủ; ROE mô hình khác lợi suất cổ phiếu. |
| “Chỉ cần tỷ suất hoạt động cao hơn lãi vay là an toàn.” | Đó là điều kiện so sánh tỷ suất trong mô hình; còn phải kiểm tra kịch bản xấu, dòng tiền và gốc đến hạn. |
| “ICR lớn hơn 1 nghĩa là trả được nợ.” | EBIT không phải tiền, và mẫu số ICR không gồm gốc. Không có một ngưỡng an toàn chung suy ra từ ví dụ. |
| “Debt/equity lúc nào cũng là cùng một tỷ số.” | Đọc xem tử số là nợ vay hay toàn bộ nợ phải trả, dùng sổ sách hay thị trường, tại thời điểm nào. Ví dụ §6.4 OpenStax dùng tổng nợ phải trả; $D/E$ trong mô hình bài này chỉ dùng nợ vay. |
| “Vốn chủ càng nhỏ thì ROE càng đáng khen.” | Khi E gần 0, tỷ suất rất nhạy; khi E bằng 0 không tính được, khi E âm thì dấu tỷ số có thể gây hiểu lầm. Lỗ chia vốn âm cho số dương không biến thành hiệu quả tốt. |

## 7. Kiến thức này có ích gì với tôi?

Khi đọc bản tin “lợi nhuận cổ đông giảm dù doanh thu vẫn tăng”, hãy lần theo chuỗi: doanh thu tạo được bao nhiêu EBIT → chi phí lãi lấy đi bao nhiêu → còn lại bao nhiêu cho vốn chủ. Doanh thu tăng chưa trả lời được hai bước sau.

Khi xem một doanh nghiệp, đặt tỷ suất cạnh **quy mô nợ, cơ sở vốn chủ, lịch điều chỉnh lãi và lịch trả gốc**. Cùng một D/E có thể đi với khả năng thu tiền rất khác nhau. Đọc báo cáo lợi nhuận cùng báo cáo lưu chuyển tiền tệ và thuyết minh nợ giúp nhận ra khác biệt ấy.

Với một kế hoạch kinh doanh cá nhân có vay vốn, có thể lập hai bảng riêng: kết quả lãi/lỗ và lịch tiền thu–trả theo từng thời điểm. Sau đó thử một kịch bản doanh thu yếu hoặc thu tiền chậm. Cách kiểm tra này giúp nhìn thấy nghĩa vụ cố định phía sau tỷ suất hấp dẫn; nó không tự đưa ra mức vay phù hợp cho từng người.

## 8. Nguồn tham khảo

Các tài liệu sau được mở và đối chiếu ngày **18/10/2026**. Công thức tỷ suất và các ví dụ số trong bài được tự suy ra theo giả định đã nêu.

1. **Julie Dahlquist & Rainford Knight, OpenStax — *Principles of Finance* (24/03/2022), [§17.1: The Concept of Capital Structure](https://openstax.org/books/principles-finance/pages/17-1-the-concept-of-capital-structure) và [§17.4: Capital Structure Choices](https://openstax.org/books/principles-finance/pages/17-4-capital-structure-choices).** Dùng cho cấu trúc tài trợ, bảng cân đối và phần dư của cổ đông; không đồng nhất lợi suất yêu cầu trong MM với ROE kế toán của ví dụ.
2. **Julie Dahlquist & Rainford Knight, OpenStax — *Principles of Finance* (2022), [§6.4: Solvency Ratios](https://openstax.org/books/principles-finance/pages/6-4-solvency-ratios) và [§6.6: Profitability Ratios and the DuPont Method](https://openstax.org/books/principles-finance/pages/6-6-profitability-ratios-and-the-dupont-method).** Dùng cho EBIT/lãi, đối chiếu phạm vi nợ và mẫu số vốn chủ bình quân của ROE.
3. **Julie Dahlquist & Rainford Knight, OpenStax — *Principles of Finance* (2022), [§17.5: Optimal Capital Structure](https://openstax.org/books/principles-finance/pages/17-5-optimal-capital-structure).** Dùng cho sức ép nghĩa vụ nợ và chi phí khó khăn tài chính; bài không áp dụng thuế suất hay quy định thuế của ví dụ giáo trình vào Việt Nam.
4. **Rhea Choudhary, Suchita Mathur & Peter Wallis, Reserve Bank of Australia — [*Leverage, Liquidity and Non-bank Financial Institutions: Key Lessons from Recent Market Events*](https://www.rba.gov.au/publications/bulletin/2023/jun/leverage-liquidity-and-non-bank-financial-institutions.html) (15/06/2023).** Dùng cho tình huống nghĩa vụ ký quỹ làm phát sinh nhu cầu thanh khoản dù giá trị hoạt động dài hạn có thể còn đủ.

## 9. Liên kết kiến thức

- **Đòn bẩy hoạt động (operating leverage):** chi phí hoạt động cố định làm EBIT nhạy với doanh thu; nợ vay có thể tạo thêm một lớp khuếch đại sau EBIT.
- **Chi phí vốn bình quân gia quyền (weighted average cost of capital — WACC):** để xét tài trợ và giá trị doanh nghiệp, cần xét chi phí và rủi ro của cả chủ nợ lẫn cổ đông, thay vì chỉ tối đa hóa ROE.
- **Điều khoản vay và tái cơ cấu nợ (covenants & debt restructuring):** khi dòng tiền yếu, thiết kế hợp đồng và việc thương lượng lại ảnh hưởng cách phân bổ tổn thất và khả năng tiếp tục hoạt động.

## 10. Điều đáng nhớ nhất

1. Nợ để lại nghĩa vụ lãi trên một nền vốn chủ nhỏ hơn, nên làm kết quả dành cho cổ đông nhạy hơn với kinh doanh. Tỷ suất cao hơn trong kịch bản tốt đi cùng sức ép lớn hơn khi kịch bản xấu xảy ra.
2. Lợi nhuận, vốn chủ và tiền sẵn trả nợ là ba góc nhìn khác nhau. Gốc đến hạn có thể gây thiếu tiền dù không phải chi phí làm giảm lợi nhuận.
3. Công thức chỉ có ý nghĩa khi giữ đúng giả định, kỳ đo và mẫu số; phải đưa lịch lãi, lịch gốc và tốc độ thu tiền trở lại khi phân tích thực tế.

## 11. Góc Phản xạ & Active Recall (Dành cho bạn)

*Hãy thử giải thích cho một người bạn bằng 2–3 câu: vì sao cùng 1.000 triệu tài sản, doanh nghiệp có nợ có thể đạt ROE cao hơn, nhưng đến ngày trả nợ vẫn thiếu tiền dù báo lãi?*

**Thang tự đánh giá (1–5):** Bạn tự thấy mức độ hiểu/nhớ cơ chế hôm nay ở mức nào (1 = Cần đọc lại sớm / 3 = Nắm vững / 5 = Rất tự tin)? Nếu bạn chọn 1–2, hệ thống sẽ ưu tiên quay lại củng cố sớm hơn.
