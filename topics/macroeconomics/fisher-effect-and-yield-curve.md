---
id: MACRO-002
title: "Hiệu ứng Fisher và đường cong lợi suất: vì sao lãi suất dài hạn có thể thấp hơn ngắn hạn?"
category: macroeconomics
tags: [lai-suat-thuc, lam-phat-ky-vong, duong-cong-loi-suat, trai-phieu]
prerequisites: [MACRO-001, MONEY-002]
difficulty: Intermediate
date: 2026-09-24
last_verified: 2026-09-24
---

# Hiệu ứng Fisher và đường cong lợi suất: vì sao lãi suất dài hạn có thể thấp hơn ngắn hạn?

### 1. Chủ đề hôm nay

**Hiệu ứng Fisher (Fisher effect)** nối lãi suất danh nghĩa với lãi suất thực và lạm phát kỳ vọng, khi các yếu tố khác được giữ cố định. **Đường cong lợi suất (yield curve)** đặt lợi suất của những trái phiếu có kỳ hạn khác nhau lên cùng một đồ thị. Đọc hai khái niệm cùng nhau giúp ta hiểu vì sao lãi suất ngắn hạn tăng mà lợi suất dài hạn có thể không tăng theo.

> 🔄 **Ôn tập Ngắt quãng (Delayed Active Recall):** Trước khi đọc tiếp, hãy thử nhớ lại: trong [MACRO-001](inflation-cpi-and-macro-transmission.md), vì sao lãi suất tiền gửi ấn định trước chưa cho biết sức mua tăng bao nhiêu sau kỳ gửi? Và trong [MONEY-002](../monetary-and-banking/policy-rates-and-monetary-transmission.md), lãi suất điều hành đi tới các lãi suất thị trường qua những kênh nào?

### 2. Vấn đề cốt lõi

Nếu lãi suất ngắn hạn là 6%/năm, tại sao một trái phiếu dài hạn lại có thể giao dịch với lợi suất dưới 6%/năm? Con số 6% cũng có thật sự là mức tăng sức mua của người gửi tiền? Hai câu hỏi liên hệ qua **kỳ vọng về tương lai**, nhưng phải tách rõ lạm phát đã xảy ra, lạm phát dự kiến và giá trái phiếu đang được giao dịch.

### 3. Giải thích cơ chế

#### 3.1. Lãi suất danh nghĩa, lãi suất thực và hiệu ứng Fisher

**[Definition]** Lãi suất danh nghĩa (nominal interest rate) cho biết số đơn vị tiền nhận thêm theo hợp đồng; lãi suất thực (real interest rate) đo thay đổi sức mua theo một thước đo giá đã chọn. **Lạm phát kỳ vọng (expected inflation)** là dự kiến *trước* khi kỳ đầu tư kết thúc, khác với lạm phát thực tế được đo *sau* kỳ đó.

**[Accounting Identity]** Với một khoản đầu tư một kỳ có lợi suất danh nghĩa thực nhận là \(i\), và lạm phát thực tế trong *cùng kỳ* là \(\pi\), lợi suất thực sau kỳ là:

\[
1+r_{\text{thực, sau kỳ}}=\frac{1+i}{1+\pi},
\qquad
r_{\text{thực, sau kỳ}}=\frac{1+i}{1+\pi}-1.
\]

Đây là phép đổi từ tiền danh nghĩa sang sức mua theo chỉ số giá đã chọn; \(i-\pi\) chỉ là xấp xỉ khi các tỷ lệ đủ nhỏ. Hãy dùng cùng khoảng thời gian cho \(i\) và \(\pi\), và phân biệt CPI chung với rổ chi tiêu riêng của một hộ. Trong trường hợp có thuế hoặc phí, \(i\) phải là lợi suất danh nghĩa **sau** các khoản đó nếu muốn tính sức mua ròng.

**[Theoretical Model]** Trước kỳ, vì chưa biết \(\pi\), người ta thường dùng phép tính nhanh \(r_{\text{dự kiến}}\approx i-E_t(\pi)\). Đây là xấp xỉ dựa trên lạm phát dự kiến và giả định các rủi ro khác không đổi. Nếu giả sử lạm phát tương lai *được biết chắc*, có thể thay \(\pi\) trong công thức chính xác ở trên bằng tỷ lệ đã biết. Khi lạm phát còn bất định, nhìn chung \(E_t[(1+i)/(1+\pi)-1]\ne(1+i)/(1+E_t\pi)-1\); do đó không gọi biểu thức dùng \(E_t\pi\) là đồng nhất thức chính xác cho lợi suất thực kỳ vọng.

**Hiệu ứng Fisher** là nhận định có điều kiện: nếu lãi suất thực kỳ vọng và các phần bù rủi ro không đổi, lạm phát kỳ vọng cao hơn thường đi cùng lãi suất danh nghĩa cao hơn, xấp xỉ cùng số **điểm phần trăm**. Trong định giá trái phiếu thực tế, lợi suất danh nghĩa còn phản ánh lãi suất thực kỳ vọng, phần bù rủi ro lạm phát và phần bù cho rủi ro nắm giữ dài hạn; đây là cách phân rã của một mô hình nghiên cứu, không phải phép đọc trực tiếp từng thành phần từ một mức lợi suất quan sát được. [Fed Board, *Tips from TIPS*, 2019](https://www.federalreserve.gov/econres/notes/feds-notes/tips-from-tips-update-and-discussions-20190521.html).

#### 3.2. Đường cong lợi suất đo điều gì?

**[Definition]** Đường cong lợi suất là đồ thị lợi suất theo kỳ hạn **tại cùng một thời điểm**. Để giải thích độ dốc, cần so sánh những công cụ đủ tương đồng về đồng tiền, chủ thể phát hành, rủi ro tín dụng, cách tính lợi suất và đặc điểm thuế hoặc thanh khoản. Một đường cong trái phiếu chính phủ Mỹ không phải đường cong lãi suất tiền gửi ngân hàng Việt Nam. **Chênh lệch kỳ hạn (term spread)** là lợi suất kỳ hạn dài trừ lợi suất kỳ hạn ngắn được chọn, chẳng hạn lợi suất trái phiếu Mỹ 10 năm trừ lợi suất tín phiếu Mỹ 3 tháng. [Bauer và Hamilton, Fed San Francisco, 2016](https://www.frbsf.org/research-and-insights/publications/economic-letter/2016/06/do-macroeconomic-variables-help-forecast-interest-rates/); [Bauer và Mertens, Fed San Francisco, 2018](https://www.frbsf.org/research-and-insights/publications/economic-letter/2018/08/information-in-yield-curve-about-future-recessions/).

**[Causal Mechanism]** Lợi suất trái phiếu trên thị trường đến từ **giá giao dịch**, không đơn thuần là lãi coupon ghi trên trái phiếu. Với trái phiếu không trả coupon và trả \(F\) sau \(n\) năm, theo quy ước ghép lãi năm, \(P=F/(1+y_n)^n\). Cùng dòng tiền \(F\), người mua trả giá \(P\) cao hơn thì lợi suất đến đáo hạn \(y_n\) thấp hơn. Trái phiếu có coupon dùng phép chiết khấu *từng* dòng tiền; lợi suất đến đáo hạn và lãi coupon vì thế là hai khái niệm khác nhau. [Bộ Tài chính Mỹ, *Understanding Pricing and Interest Rates*](https://www.treasurydirect.gov/marketable-securities/understanding-pricing/).

#### 3.3. Mô hình giáo trình và cơ chế thực tế

**TEXTBOOK MODEL — Mô hình giáo trình [Theoretical Model].** Giả sử hai trái phiếu không coupon có cùng đồng tiền, cùng chủ thể phát hành, không có rủi ro vỡ nợ hay ma sát giao dịch; lãi suất một năm bắt đầu sau một năm được biết chắc; không có phần bù kỳ hạn hay cơ hội kinh doanh chênh lệch giá. Khi đó, đầu tư hai năm trực tiếp và đầu tư hai lần một năm phải cho cùng khoản tiền cuối kỳ:

\[
(1+y_2)^2=(1+y_{1,0})(1+y_{1,1}).
\]

\(y_{1,0}\) là lợi suất một năm hiện tại, \(y_{1,1}\) là lãi suất một năm *ở năm sau* trong giả định biết chắc, còn \(y_2\) là lợi suất hai năm hiện tại. Công thức chứng minh rằng **đường đi tương lai của lãi suất ngắn hạn** có thể khiến lợi suất dài hạn thấp hơn lãi suất ngắn hạn hôm nay. Khi tương lai bất định, cách nói “lợi suất dài hạn xấp xỉ bình quân lãi suất ngắn hạn kỳ vọng” chỉ là mô hình giả thuyết kỳ vọng, không phải đồng nhất thức hay quy tắc định giá chính xác.

**REAL-WORLD MECHANISM — Cơ chế thực tế [Causal Mechanism].** Ngân hàng trung ương tác động mạnh nhất lên lãi suất rất ngắn hạn qua công cụ và truyền thông chính sách; nhà đầu tư định giá trái phiếu dài hạn theo đường đi lãi suất ngắn hạn họ dự kiến, khả năng lạm phát, rủi ro thay đổi giá và nhu cầu nắm giữ tài sản. Khi họ mua trái phiếu dài hạn, giá có thể tăng và lợi suất giảm. **Phần bù kỳ hạn (term premium)** trong một mô hình cấu trúc kỳ hạn là phần chênh giữa lợi suất dài hạn và bình quân lãi suất ngắn hạn kỳ vọng tương ứng; nó thay đổi theo rủi ro, nhu cầu tài sản và giả định mô hình, thậm chí không nhất thiết dương ở mọi thời điểm. Vì kỳ vọng và phần bù không quan sát riêng được, cùng một lợi suất dài hạn có thể có nhiều cách giải thích. [Bauer và Hamilton, Fed San Francisco, 2016](https://www.frbsf.org/research-and-insights/publications/economic-letter/2016/06/do-macroeconomic-variables-help-forecast-interest-rates/); [Fed Board, *Three-Factor Nominal Term Structure Model*](https://www.federalreserve.gov/data/three-factor-nominal-term-structure-model.htm).

Các chủ thể có động cơ khác nhau: ngân hàng trung ương muốn truyền chính sách tới điều kiện tài chính; người phát hành chọn kỳ hạn huy động vốn; nhà đầu tư cân nhắc khóa lợi suất dài hạn với rủi ro giá nếu cần bán sớm; ngân hàng và người gửi tiền lại cân nhắc lãi suất hợp đồng, thanh khoản và sức mua. Cung trái phiếu, khả năng giao dịch và mức chấp nhận rủi ro của người mua có thể thay đổi giá ngay cả khi dự báo lãi suất ngắn hạn chưa đổi. Vì vậy, đường cong trái phiếu chính phủ không tự ấn định lãi suất tiền gửi hay lãi vay của từng ngân hàng. Xem thêm [MONEY-002](../monetary-and-banking/policy-rates-and-monetary-transmission.md) về các kênh truyền dẫn từ chính sách tới lãi suất bán lẻ.

Mối nối với Fisher nằm ở đây: lãi suất danh nghĩa ngắn hạn dự kiến có thể đổi vì **lãi suất thực dự kiến**, **lạm phát kỳ vọng** hoặc cả hai. Lợi suất dài hạn còn có phần bù rủi ro. Vì vậy, không thể nhìn một đường cong danh nghĩa rồi kết luận toàn bộ thay đổi là do lạm phát kỳ vọng hoặc do một quyết định lãi suất điều hành. Trong thị trường trái phiếu Mỹ, ngay cả chênh lệch giữa lợi suất trái phiếu danh nghĩa và trái phiếu chống lạm phát TIPS cũng chứa phần bù rủi ro lạm phát và chênh lệch thanh khoản; nó không đo thuần túy kỳ vọng lạm phát. [Fed Board, *Tips from TIPS*, 2019](https://www.federalreserve.gov/econres/notes/feds-notes/tips-from-tips-update-and-discussions-20190521.html).

#### 3.4. Đường cong đảo ngược có nói trước suy thoái không?

**[Definition]** Nếu chênh lệch giữa *một cặp kỳ hạn được nêu rõ* âm, ta nói đoạn đó của đường cong bị đảo ngược; không cần mọi kỳ hạn đều thấp dần. **[Empirical Relationship]** Nghiên cứu của Fed San Francisco công bố năm 2018 thấy chênh lệch lợi suất 10 năm trừ 3 tháng có giá trị dự báo suy thoái trong dữ liệu lịch sử Mỹ được nghiên cứu. Đây là bằng chứng về **tương quan dự báo**, không phải lời bảo đảm rằng mỗi lần đảo ngược sẽ có suy thoái theo một lịch cố định, và cũng không tự suy rộng sang Việt Nam. Chính nghiên cứu này nêu rằng tương quan không xác định chiều nhân quả; thay đổi phần bù kỳ hạn và điều kiện thị trường có thể làm cách diễn giải phức tạp hơn. [Bauer và Mertens, Fed San Francisco, 2018](https://www.frbsf.org/research-and-insights/publications/economic-letter/2018/08/information-in-yield-curve-about-future-recessions/).

### 4. Ví dụ trực quan — tất cả số liệu dưới đây đều **giả định**

**Sức mua của khoản gửi tiền.** Bạn gửi 100 triệu đồng một năm, nhận lãi danh nghĩa 6% và không xét thuế, phí. Trước khi gửi, bạn dự kiến lạm phát của đúng một năm đó là 4%: nếu lạm phát thật sự bằng 4%, sức mua tăng \(1{,}06/1{,}04-1\approx1{,}92\%\). Nhưng nếu lạm phát thực tế là 7%, sức mua *sau kỳ* thay đổi \(1{,}06/1{,}07-1\approx-0{,}93\%\). Dự kiến 1,92% trong kịch bản lạm phát 4% không phải lợi suất thực đã chắc chắn nhận được, cũng không tự là kỳ vọng toán học của lợi suất thực khi lạm phát có nhiều kết quả khả dĩ.

**Một đoạn đường cong đảo ngược.** Giả sử hai trái phiếu không coupon cùng chủ thể phát hành, lợi suất một năm hôm nay là 6%, và lãi suất một năm *bắt đầu năm sau* được biết chắc là 3%. Theo đúng giả định mô hình ở trên, \(y_2=\sqrt{1{,}06\times1{,}03}-1\approx4{,}49\%\): lợi suất hai năm thấp hơn một năm. Nếu lãi suất năm sau bất định hoặc có phần bù kỳ hạn, không thể dùng riêng 6% và dự báo 3% để tính chính xác lợi suất hai năm đang giao dịch.

### 5. Tình huống thực tế: ngân hàng trung ương nâng lãi suất ngắn hạn

**[Causal Mechanism]** Giả sử lãi suất ngắn hạn trên thị trường tăng sau tín hiệu thắt chặt. Nếu nhà đầu tư đồng thời cho rằng sức cầu và lạm phát tương lai sẽ giảm, họ có thể dự kiến lãi suất ngắn hạn về sau thấp hơn; cầu trái phiếu dài hạn tăng, giá tăng và lợi suất dài hạn tăng ít hơn, giữ nguyên hoặc giảm. Đường cong có thể phẳng đi hoặc đảo ngược. Ngược lại, nếu họ dự kiến lạm phát dai dẳng, lãi suất thực cao hơn hoặc đòi phần bù kỳ hạn lớn hơn, lợi suất dài hạn vẫn có thể tăng. Đây là **hai chuỗi truyền dẫn có điều kiện**, không phải phản ứng cơ học của mọi thị trường. [Bauer và Hamilton, Fed San Francisco, 2016](https://www.frbsf.org/research-and-insights/publications/economic-letter/2016/06/do-macroeconomic-variables-help-forecast-interest-rates/); [Fed Board, *Tips from TIPS*, 2019](https://www.federalreserve.gov/econres/notes/feds-notes/tips-from-tips-update-and-discussions-20190521.html).

### Kiến thức này có ích gì với tôi?

- Khi đọc tin “đường cong lợi suất đảo ngược”, hãy hỏi **thị trường nào, cặp kỳ hạn nào, ngày nào và lợi suất của loại trái phiếu nào**. Sau đó xem khả năng thay đổi của kỳ vọng lãi suất ngắn hạn và phần bù kỳ hạn; đừng tự biến tín hiệu lịch sử Mỹ thành dự báo chắc chắn cho nơi khác.
- Khi so sánh gửi tiết kiệm với mức tăng giá, tính lợi suất thực từ **lãi thực nhận và lạm phát cùng kỳ**. Trước kỳ chỉ có thể lập kịch bản dựa trên lạm phát dự kiến và rủi ro sai lệch dự báo; CPI chung cũng có thể khác rổ chi tiêu của bạn.
- Khi nắm trái phiếu lãi cố định, phân biệt **coupon**, **lợi suất đến đáo hạn khi mua** và **giá có thể bán trước hạn**. Lãi suất thị trường tăng có thể làm giá trái phiếu đang nắm giữ giảm, dù coupon ghi trên trái phiếu không đổi. [Ủy ban Chứng khoán Mỹ, *Fixed Income Investments: When Interest Rates Go Up, Prices of Fixed-Rate Bonds Fall*, 2013](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins-86).

### Thuật ngữ và những nhầm lẫn thường gặp

| Thuật ngữ | Nghĩa trong bài | Dễ nhầm với |
| :--- | :--- | :--- |
| Lạm phát kỳ vọng (*expected inflation*) | Dự kiến trước kỳ về mức tăng giá trong kỳ tương ứng. | Lạm phát đã công bố sau kỳ. |
| Hiệu ứng Fisher (*Fisher effect*) | Mối liên hệ có điều kiện giữa lạm phát kỳ vọng và lãi suất danh nghĩa khi lãi suất thực cùng các phần bù giữ nguyên. | Công thức lợi suất thực **sau kỳ**, vốn là phép đổi sức mua từ số liệu đã xảy ra. |
| Đường cong lợi suất (*yield curve*) | Lợi suất của các kỳ hạn tại cùng một thời điểm, với các công cụ đủ tương đồng. | Đường thời gian của **một** lãi suất hay biểu lãi suất tiền gửi từ nhiều ngân hàng. |
| Lợi suất đến đáo hạn (*yield to maturity*) | Mức sinh lời quy đổi từ giá mua và các dòng tiền hứa trả, theo giả định giữ đến đáo hạn và nhận đủ dòng tiền. | Coupon cố định ghi trên trái phiếu hoặc lợi nhuận chắc chắn nếu bán trước hạn. |
| Phần bù kỳ hạn (*term premium*) | Trong mô hình cấu trúc kỳ hạn, phần chênh giữa lợi suất dài hạn và bình quân lãi suất ngắn hạn kỳ vọng tương ứng. | Một khoản phụ thu cố định, luôn dương hoặc quan sát trực tiếp được. |

### Liên kết kiến thức

- [MACRO-001 — Lạm phát và CPI](inflation-cpi-and-macro-transmission.md): dùng lạm phát cùng kỳ để tính sức mua sau kỳ; kỳ vọng lạm phát là đại lượng khác.
- [MONEY-002 — Lãi suất điều hành và truyền dẫn](../monetary-and-banking/policy-rates-and-monetary-transmission.md): công cụ ngắn hạn ảnh hưởng điều kiện thị trường qua kỳ vọng và nhiều kênh, không ấn định toàn bộ đường cong.
- **Độ nhạy giá trái phiếu với lãi suất (duration)** và **đo lạm phát kỳ vọng từ TIPS** là hai hướng học tiếp để đọc rủi ro của trái phiếu kỹ hơn.

### Điều đáng nhớ nhất

1. Lãi suất danh nghĩa nói về số tiền; sức mua sau kỳ phụ thuộc lạm phát thực tế. Fisher trước kỳ dùng kỳ vọng và điều kiện giữ các yếu tố khác ổn định.
2. Lợi suất dài hạn phản ánh giá trái phiếu, kỳ vọng đường đi lãi suất ngắn hạn và phần bù kỳ hạn. Vì vậy, lãi suất ngắn hạn cao hơn lãi suất dài hạn là điều có thể xảy ra.
3. Đường cong đảo ngược là tín hiệu cần điều tra, không phải đồng hồ đếm ngược chắc chắn đến suy thoái.

### Góc Phản xạ & Active Recall (Dành cho bạn)

Nếu đọc một tin nói “lãi suất ngắn hạn tăng nhưng lợi suất trái phiếu dài hạn giảm”, bạn sẽ thử giải thích **hai kênh** nào trước khi kết luận nền kinh tế sắp suy thoái?

**Thang tự đánh giá (1–5):** Bạn tự thấy mức độ hiểu/nhớ cơ chế hôm nay ở mức nào (1 = Cần đọc lại sớm / 3 = Nắm vững / 5 = Rất tự tin)? Nếu chọn 1–2, hãy ưu tiên quay lại củng cố sớm hơn.

### Nguồn tham khảo

1. Don Kim, Cait Walsh và Min Wei, Board of Governors of the Federal Reserve System, [*Tips from TIPS: Update and Discussions*](https://www.federalreserve.gov/econres/notes/feds-notes/tips-from-tips-update-and-discussions-20190521.html), 21/05/2019 — phân rã lợi suất danh nghĩa, lạm phát kỳ vọng và các phần bù rủi ro/thanh khoản.
2. Michael D. Bauer và James D. Hamilton, Federal Reserve Bank of San Francisco, [*Do Macro Variables Help Forecast Interest Rates?*](https://www.frbsf.org/research-and-insights/publications/economic-letter/2016/06/do-macroeconomic-variables-help-forecast-interest-rates/), 27/06/2016 — định nghĩa đường cong lợi suất, giả thuyết kỳ vọng và phần bù kỳ hạn.
3. Michael Bauer và Thomas Mertens, Federal Reserve Bank of San Francisco, [*Information in the Yield Curve about Future Recessions*](https://www.frbsf.org/research-and-insights/publications/economic-letter/2018/08/information-in-yield-curve-about-future-recessions/), 27/08/2018 — bằng chứng dự báo suy thoái trong dữ liệu Mỹ và giới hạn diễn giải nhân quả.
4. U.S. Department of the Treasury, Bureau of the Fiscal Service, [*Understanding Pricing and Interest Rates*](https://www.treasurydirect.gov/marketable-securities/understanding-pricing/), không ghi ngày công bố trên trang, truy cập 24/09/2026 — phân biệt giá, coupon và lợi suất đến đáo hạn của trái phiếu.
5. U.S. Securities and Exchange Commission, [*Investor Bulletin: Fixed Income Investments — When Interest Rates Go Up, Prices of Fixed-Rate Bonds Fall*](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins-86), 26/06/2013 — rủi ro giá của trái phiếu lãi cố định khi lãi suất thị trường thay đổi.
