---
id: INVEST-001
title: "Rủi ro lãi suất của trái phiếu: Vì sao giá giảm khi lợi suất tăng?"
category: investing
tags: [bonds, interest-rate-risk, duration, present-value, yield-to-maturity]
prerequisites: [MACRO-002, MONEY-002]
difficulty: Intermediate
date: 2026-10-03
last_verified: 2026-10-03
---

## 1. Chủ đề hôm nay

**Rủi ro lãi suất của trái phiếu (Bond Interest-Rate Risk)** và **độ nhạy giá theo lợi suất (Duration)**: vì sao một trái phiếu vẫn trả lãi đúng cam kết nhưng giá bán của nó lại giảm?

> 🔄 **Ôn tập Ngắt quãng (Delayed Active Recall):** Trong bài [MACRO-002 — Hiệu ứng Fisher và đường cong lợi suất](../macroeconomics/fisher-effect-and-yield-curve.md) ngày 24/09, bạn đã gặp sự khác nhau giữa coupon và lợi suất đến đáo hạn. Hãy thử nhớ lại: khi giá mua thay đổi nhưng dòng tiền hứa trả giữ nguyên, đại lượng nào sẽ thay đổi?

Bài này kiểm chứng cơ chế và công thức, không mô tả mức lợi suất hiện hành. Toàn bộ số tiền và lãi suất trong ví dụ đều là **giả định**; nguồn nước ngoài được dùng cho nguyên lý tài chính, không để suy ra quy định pháp luật Việt Nam.

## 2. Vấn đề cốt lõi

Bạn mua một trái phiếu mệnh giá 100 triệu đồng, trả 5 triệu đồng mỗi năm. Sau đó, lợi suất mà thị trường yêu cầu đối với khoản đầu tư tương đương tăng lên. Người phát hành vẫn trả đúng 5 triệu đồng: vì sao người mua mới không muốn trả bạn đủ 100 triệu đồng?

Giá mua hôm nay phải phù hợp với những dòng tiền mà người mua sẽ nhận **và lựa chọn thay thế họ đang có**. Cùng một dòng tiền hứa trả, giá mua thấp hơn cho người mua mới lợi suất cao hơn. Coupon cố định vì hợp đồng đã xác định nó; giá giao dịch thay đổi vì điều kiện định giá thay đổi.

**[Definition]** Trong bài, **rủi ro lãi suất** là rủi ro giá trị thị trường của trái phiếu thay đổi khi lợi suất chiết khấu thay đổi. Nó khác **rủi ro tín dụng (Credit Risk)**: người phát hành có thể không trả đủ hoặc đúng hạn. SEC trình bày hai rủi ro này riêng biệt trong [*What Are Corporate Bonds?*, 04/06/2013](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/what-are).

## 3. Giải thích cơ chế

### 3.1. TEXTBOOK MODEL — Mô hình giáo trình

**[Theoretical Model]** Ta bắt đầu với trái phiếu có các giả định rõ ràng:

- Coupon cố định, trả cuối mỗi năm; toàn bộ gốc trả ở cuối năm đáo hạn.
- Không vỡ nợ, không trả chậm, không có quyền mua lại trước hạn hoặc quyền chuyển đổi.
- Định giá ngay sau một ngày trả coupon, nên không có lãi dồn tích cần cộng vào giá.
- Mọi dòng tiền dùng cùng một lợi suất năm \(y\), theo quy ước ghép lãi hằng năm; bỏ qua phí, thuế và chênh lệch giá mua–bán.
- Khi so sánh hai mức lợi suất, giữ nguyên ngày định giá, đồng tiền và lịch dòng tiền. Đây là cú thay đổi lợi suất tại cùng thời điểm, không phải lợi nhuận qua một năm.

Mô hình chứng minh ảnh hưởng của **riêng mức chiết khấu** lên giá khi dòng tiền không đổi. Nó chưa giải thích tất cả nguyên nhân khiến giá thị trường biến động.

### 3.2. Từ dòng tiền tương lai về giá hôm nay

Gọi \(F\) là **mệnh giá (Face Value)**, \(c\) là **lãi suất coupon (Coupon Rate)** và \(C=cF\) là số tiền coupon một năm. Mệnh giá là số gốc hứa hoàn trả theo giả định bài này; nó không nhất thiết bằng giá giao dịch.

Với \(n\) năm còn lại, dòng tiền \(CF_t=C\) khi \(t<n\), còn \(CF_n=C+F\). Giá là:

\[
P(y)=\sum_{t=1}^{n}\frac{CF_t}{(1+y)^t}.
\]

**Ý nghĩa kinh tế:** nhận tiền muộn hơn phải đánh đổi cơ hội sử dụng tiền trong thời gian chờ. Khi \(y\) cao hơn, một đồng nhận trong tương lai có giá trị hiện tại thấp hơn. Vì \(CF_t>0\), \(t>0\) và \(y>-1\), tăng \(y\) làm từng số hạng giảm, nên tổng giá giảm. Đây là kết quả toán học của mô hình, không phải bằng chứng rằng mọi lần NHTW tăng lãi suất đều khiến mọi trái phiếu giảm giá ngay.

**[Definition]** **Lợi suất đến đáo hạn (Yield to Maturity — YTM)** là suất chiết khấu làm giá trị hiện tại của các dòng tiền hứa trả bằng giá mua, tức suất hoàn vốn nội bộ của lịch dòng tiền đó. Có thể suy \(y\) từ giá quan sát được; một YTM duy nhất không có nghĩa đường cong lãi suất giao ngay của thị trường thực tế phải phẳng. Công thức định giá và cách tính duration được đối chiếu với [MIT, Andrew W. Lo, *Fixed-Income Securities*, 2008, slide 25–26 và 36](https://ocw.mit.edu/courses/15-401-finance-theory-i-fall-2008/df418b972d36cd53ae5c375b8af61e53_MIT15_401F08_lec04.pdf).

Ba đại lượng cần tách rõ:

| Đại lượng | Trong mô hình trả coupon năm | Nó đo gì? |
| :--- | :--- | :--- |
| Lãi suất coupon | \(c=C/F\) | Số coupon hứa trả so với mệnh giá |
| Lợi suất hiện hành (Current Yield) | \(C/P\) | Coupon một năm so với giá hiện tại; chưa tính chênh lệch giữa giá mua và gốc hoàn trả |
| YTM | Nghiệm của phương trình định giá | Kết hợp giá mua, coupon, gốc và thời điểm nhận tiền |

Do đó, trái phiếu coupon 5% có thể có YTM 6% khi được mua dưới mệnh giá. Người mua nhận cùng coupon nhưng bỏ ra ít tiền hơn và, nếu được trả đủ, còn nhận phần chênh giữa mệnh giá và giá mua.

### 3.3. Duration đo độ nhạy như thế nào?

**[Definition]** **Duration Macaulay (Macaulay Duration)** là bình quân thời gian nhận dòng tiền, với trọng số bằng tỷ trọng **giá trị hiện tại** của từng dòng tiền trong giá trái phiếu:

\[
w_t=\frac{CF_t/(1+y)^t}{P},\qquad
D_{Mac}=\sum_{t=1}^{n}t\,w_t,\qquad \sum_{t=1}^{n}w_t=1.
\]

Trọng số không phải tỷ trọng số tiền chưa chiết khấu. Khi phần lớn giá trị nằm ở dòng tiền rất xa, nhiều giá trị phải chịu tác động chiết khấu qua nhiều năm. Coupon trả sớm kéo thời gian bình quân này về gần hơn. Vì vậy, khi có coupon dương trả trước ngày đáo hạn trong mô hình, duration Macaulay nhỏ hơn kỳ hạn đáo hạn; với trái phiếu không coupon, nó bằng kỳ hạn vì chỉ có một dòng tiền cuối kỳ.

**[Definition / Theoretical Model]** Với quy ước trả và ghép lãi hằng năm đang dùng, **duration điều chỉnh (Modified Duration)** là:

\[
D_{mod}=\frac{D_{Mac}}{1+y}
=-\frac{1}{P}\frac{dP}{dy},
\qquad
\frac{\Delta P}{P}\approx-D_{mod}\,\Delta y.
\]

Đẳng thức với đạo hàm mô tả độ nhạy tại mức \(y\) đang xét; công thức dùng \(\Delta y\) hữu hạn là **xấp xỉ tuyến tính**, giữ nguyên dòng tiền. Duration được báo cáo theo đơn vị năm trong quy ước này; khi tính, lợi suất phải nhập dạng thập phân. Tăng từ 5% lên 6% là **1 điểm phần trăm**, tức \(\Delta y=0{,}01\), không phải 1 và cũng không phải mức tăng tương đối 20%.

**Giới hạn:** độ nhạy thay đổi theo mức lợi suất. **Độ lồi (Convexity)** đo độ cong của quan hệ giá–lợi suất và giúp giải thích sai số khi dùng một đường thẳng để xấp xỉ. Duration đơn lẻ cũng chưa mô tả đầy đủ thay đổi ở từng đoạn của đường cong. Với trái phiếu có quyền mua lại hoặc dòng tiền phụ thuộc lãi suất, không áp dụng nguyên công thức giữ dòng tiền cố định. [MIT, slide 39–41](https://ocw.mit.edu/courses/15-401-finance-theory-i-fall-2008/df418b972d36cd53ae5c375b8af61e53_MIT15_401F08_lec04.pdf) trình bày giới hạn và xấp xỉ bậc hai.

### 3.4. REAL-WORLD MECHANISM — Cơ chế thực tế

**[Causal Mechanism]** Người phát hành muốn huy động vốn với chi phí phù hợp; người mua muốn được bù đắp cho thời gian chờ và rủi ro. Trên thị trường thứ cấp, người đang nắm giữ có thể cần tiền, còn nhà môi giới hoặc nhà tạo lập thị trường đưa ra giá để kết nối giao dịch và bù chi phí giao dịch, rủi ro tồn kho.

Nếu lợi suất của khoản đầu tư thay thế đủ tương đồng tăng, người mua cân nhắc lại mức giá họ chấp nhận cho coupon cố định cũ. Giữ các yếu tố khác không đổi, giá thấp hơn đưa YTM của trái phiếu cũ lên mức cạnh tranh. Không cần có trái phiếu mới phát hành mới tồn tại cơ chế này: giá các khoản đầu tư sẵn có và yêu cầu lợi suất của nhà đầu tư cũng có thể thay đổi.

**[Theoretical Model / Causal Mechanism]** Thực tế có thể định giá từng dòng tiền bằng mức chiết khấu theo kỳ hạn tương ứng, thay vì coi một mức \(y\) chung là nguyên nhân duy nhất. Với trái phiếu doanh nghiệp, còn có **chênh lệch lợi suất tín dụng (Credit Spread)**: chênh lợi suất so với công cụ chuẩn được chọn với đồng tiền và kỳ hạn đủ tương đồng. Chênh lệch này có thể phản ánh tổn thất tín dụng dự kiến, phần bù rủi ro và ảnh hưởng thanh khoản; không phải riêng xác suất vỡ nợ. Các thành phần định giá này được thảo luận trong [MIT, slide 11 và 46](https://ocw.mit.edu/courses/15-401-finance-theory-i-fall-2008/df418b972d36cd53ae5c375b8af61e53_MIT15_401F08_lec04.pdf).

Hai quan hệ có mức độ chắc chắn khác nhau:

- **Giữ nguyên lịch dòng tiền và ngày định giá:** YTM cao hơn đi cùng giá thấp hơn theo phương trình định giá.
- **NHTW tăng lãi suất điều hành:** giá một trái phiếu cụ thể còn phụ thuộc tin đã được dự kiến hay chưa, kỳ vọng lãi suất tương lai, phần bù kỳ hạn, tín dụng và thanh khoản. Không suy thẳng từ quyết định chính sách sang một mức giảm giá cố định.

## 4. Ví dụ trực quan: 100 triệu đồng còn bán được bao nhiêu?

**[Theoretical Model — số liệu giả định]** Bạn mua ở giá 100 triệu đồng, ngay sau ngày trả coupon. Còn đúng ba năm; mỗi cuối năm nhận 5 triệu đồng, cuối năm thứ ba nhận thêm 100 triệu đồng gốc. Lợi suất năm lúc mua là 5%.

| Thời điểm nhận | Dòng tiền (triệu đồng) | Giá trị hiện tại ở 5% | Giá trị hiện tại ở 6% |
| :--- | ---: | ---: | ---: |
| Cuối năm 1 | 5 | 4,761905 | 4,716981 |
| Cuối năm 2 | 5 | 4,535147 | 4,449982 |
| Cuối năm 3 | 105 | 90,702948 | 88,160025 |
| **Tổng giá** | | **100,000000** | **97,326988** |

Giả sử YTM tăng tức thời lên 6%, còn các giả định khác không đổi:

\[
P(6\%)=\frac{5}{1{,}06}+\frac{5}{1{,}06^2}
+\frac{105}{1{,}06^3}\approx97{,}326988\text{ triệu đồng}.
\]

Giá giảm khoảng **2,673012 triệu đồng**, tương đương **2,673012%** so với giá cũ. Đây là thay đổi giá tại cùng thời điểm, chưa có coupon mới nhận, nên không cộng coupon để gọi nó là tổng lợi nhuận nắm giữ một năm.

Tại mức lợi suất ban đầu 5%, tính từ các giá trị hiện tại **chưa làm tròn**:

\[
D_{Mac}\approx2{,}859410\text{ năm},\qquad
D_{mod}\approx2{,}723248\text{ năm}.
\]

Duration ước tính mức thay đổi giá là \( -2{,}723248\times0{,}01=-2{,}723248\%\), cho giá khoảng **97,276752 triệu đồng**. Giá định giá đầy đủ cao hơn xấp xỉ khoảng **0,050236 triệu đồng**, tức 50.236 đồng. Sai số cho thấy duration mô tả một độ dốc tại điểm ban đầu; đường giá thực tế của trái phiếu này có độ lồi dương.

**Cùng cú tăng lợi suất, dòng tiền xa hơn chịu tác động lớn hơn trong ví dụ sau.** Hai trái phiếu không coupon, cùng mệnh giá giả định 100 triệu đồng và cùng YTM ban đầu 5%, được so sánh tại cùng ngày:

| Còn đến đáo hạn | Giá ở 5% (triệu đồng) | Giá ở 6% (triệu đồng) | Thay đổi giá |
| :--- | ---: | ---: | ---: |
| 1 năm | 95,238095 | 94,339623 | −0,943396% |
| 10 năm | 61,391325 | 55,839478 | −9,043375% |

Các giá được tính bằng \(100/(1+y)^n\). Với trái phiếu không coupon này, toàn bộ khoản hoàn trả ở xa hơn phải chiết khấu qua nhiều kỳ hơn. Không khái quát bảng thành “mọi trái phiếu kỳ hạn dài đều có duration cao hơn mọi trái phiếu kỳ hạn ngắn”: coupon, lợi suất, quyền chọn và cấu trúc dòng tiền cũng quan trọng.

## 5. Tình huống thực tế: giữ đến đáo hạn thì có hết rủi ro không?

### 5.1. Hai người cầm cùng một trái phiếu, nhu cầu tiền khác nhau

**[Causal Mechanism — tình huống giả định]** Người A cần tiền ngay sau cú tăng lợi suất trong ví dụ. Nếu bán được đúng giá mô hình, A thu khoảng 97,327 triệu đồng, thấp hơn vốn mua 100 triệu đồng. Giá thực thu còn chịu phí và giá chào của bên mua.

Người B có thể chờ đủ ba năm. Nếu hợp đồng không bị thay đổi và người phát hành trả đủ, đúng hạn, B vẫn nhận các coupon 5 triệu đồng và 100 triệu đồng gốc. Cú tăng lợi suất tự nó không sửa lịch trả tiền. Tuy nhiên, giá trị bán hiện tại đã giảm, sức mua của dòng tiền còn chịu lạm phát, và B đang nắm khoản đầu tư có điều kiện khác với những lựa chọn mới trên thị trường. Rủi ro tín dụng vẫn tồn tại. SEC nêu rõ điều kiện không vỡ nợ khi giải thích việc giữ trái phiếu đến đáo hạn trong [*What Are Corporate Bonds?*](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/what-are).

Giảm giá chưa hiện thực hóa vẫn có ý nghĩa: nếu nhu cầu tiền thay đổi, B phải đối mặt với giá bán hôm đó. Nhưng giảm giá cũng không tự dẫn đến kết luận “phải bán”: quyết định từ hôm nay cần so các lựa chọn bằng giá hiện tại, rủi ro, dòng tiền và chi phí giao dịch. Bán trái phiếu cũ rồi mua khoản tương đương có YTM cao hơn không tự tạo lợi ích miễn phí; giá bán thấp hơn đã phản ánh thay đổi điều kiện này.

### 5.2. Nhận đủ coupon vẫn chưa xác định tốc độ tăng tài sản cuối kỳ

**[Definition]** **Rủi ro tái đầu tư (Reinvestment Risk)** là sự bất định về lợi suất có thể kiếm được khi đem coupon hoặc khoản gốc đã nhận đầu tư tiếp. Lãi suất tăng làm giá hiện tại giảm nhưng có thể cải thiện cơ hội tái đầu tư; lãi suất giảm tạo chiều tác động ngược lại. Kết quả phụ thuộc thời gian nắm giữ và đường đi lãi suất, chứ không chỉ một con số duration.

**Phân biệt hai phép đo:** tính YTM như suất hoàn vốn nội bộ không cần giả định coupon được tái đầu tư. Để diễn giải YTM thành tốc độ tăng trưởng kép hằng năm của **tổng tài sản tích lũy đến đáo hạn**, coupon phải được tái đầu tư ở mức YTM, bên cạnh điều kiện trả đủ và đúng hạn. Các điều kiện của lợi suất kép thực nhận được trình bày trong [CFA Institute, *Interest Rate Risk and Return*, giáo trình Level I 2026, phần Overview](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/interest-rate-risk-and-return).

Trong ví dụ mua 100 triệu đồng có YTM 5%:

- **Giả định coupon giữ bằng tiền mặt không sinh lãi:** tổng tiền cuối năm thứ ba là \(5+5+105=115\) triệu đồng. Tốc độ tăng trưởng kép của tài sản gộp là \( (115/100)^{1/3}-1\approx4{,}768955\%/năm\).
- **Giả định tái đầu tư coupon ở 5%:** tổng tiền cuối năm thứ ba là \(5(1{,}05)^2+5(1{,}05)+105=115{,}7625\) triệu đồng; tốc độ tăng trưởng kép là 5%/năm.

Cả hai lịch coupon/gốc của chính trái phiếu vẫn có suất hoàn vốn nội bộ 5% so với giá mua 100 triệu đồng. Hai con số tăng trưởng tài sản khác nhau vì cách sử dụng coupon sau khi nhận khác nhau. Chúng đều là kết quả danh nghĩa trước phí, thuế và điều chỉnh sức mua.

### 5.3. Chứng chỉ quỹ trái phiếu cần được hiểu theo cấu trúc quỹ

Bạn sở hữu một phần danh mục khi mua chứng chỉ quỹ, thay vì trực tiếp có quyền nhận một mệnh giá cụ thể từ một trái phiếu. Nhiều quỹ liên tục thay thế trái phiếu đáo hạn và không có một ngày cố định hoàn trả “mệnh giá chứng chỉ quỹ”; cần đọc mục tiêu và điều khoản của từng quỹ. Đây là điểm phân biệt được giải thích trong [Vanguard, *What is a Bond and How do they Work?*, phần so sánh trái phiếu với quỹ](https://investor.vanguard.com/investor-resources-education/understanding-investment-types/what-is-a-bond).

Giá trị chứng chỉ quỹ có thể giảm theo giá danh mục ngay cả khi quỹ chỉ giữ trái phiếu có rủi ro tín dụng thấp. SEC xác nhận rủi ro này trong [*Bond Funds and Income Funds*](https://www.investor.gov/introduction-investing/investing-basics/glossary/bond-funds-and-income-funds). Vì vậy, không lấy lời hứa trả gốc của một trái phiếu riêng lẻ làm bảo đảm cho số tiền thu về từ chứng chỉ quỹ.

## 6. Những hiểu lầm dễ gặp

| Hiểu lầm | Cách hiểu chính xác trong phạm vi bài |
| :--- | :--- |
| “Coupon cố định thì giá trị đầu tư cố định.” | Coupon cố định là điều khoản dòng tiền; giá thị trường vẫn thay đổi. |
| “Giá giảm nghĩa là doanh nghiệp đã vỡ nợ.” | Mức chiết khấu tăng có thể làm giá giảm dù dòng tiền vẫn được trả đủ; suy giảm tín dụng là một cơ chế khác. |
| “Duration 3 năm nghĩa là trái phiếu đáo hạn sau 3 năm.” | Duration Macaulay là thời gian bình quân có trọng số; modified duration đo độ nhạy. Cả hai khác kỳ hạn đáo hạn. |
| “Lãi suất tăng 1 điểm phần trăm, giá luôn giảm đúng bằng duration phần trăm.” | Công thức là xấp xỉ cho thay đổi lợi suất đã xác định, với dòng tiền cố định; không áp trực tiếp mức đổi lãi suất điều hành. |
| “Chỉ cần giữ lâu là nhận đúng vốn mua.” | Khoản gốc hứa hoàn trả là mệnh giá, có thể khác giá mua; còn phải xét khả năng chi trả và điều khoản hợp đồng. |

## 7. Kiến thức này có ích gì với tôi?

Khi đọc tin “lợi suất trái phiếu tăng”, trước hết hãy nhận diện **lợi suất nào, kỳ hạn nào, đồng tiền nào và loại trái phiếu nào**. Sau đó mới xét ảnh hưởng đến giá và lý do lợi suất thay đổi. Giá giảm theo YTM là quan hệ định giá; nguyên nhân khiến YTM thay đổi là câu hỏi kinh tế riêng.

Khi đánh giá một khoản đầu tư được giới thiệu bằng mức coupon hấp dẫn, hãy nối **giá thực trả → lịch dòng tiền → YTM → khả năng nhận đủ → thời điểm bạn cần tiền**. Mức coupon không mô tả đầy đủ lợi suất, và YTM không phải cam kết về tổng tài sản tương lai.

Kiến thức này cũng giúp hiểu một ngân hàng hoặc nhà đầu tư có thể nắm tài sản vẫn trả coupon nhưng gặp khó nếu phải bán nhanh. Giá tài sản giảm và thiếu tiền chi trả là hai vấn đề có thể tương tác; không dùng biến động giá để tự kết luận về vốn hoặc mất khả năng thanh toán của một tổ chức. Đây là kết nối với [MONEY-003 — Thanh khoản ngân hàng](../monetary-and-banking/bank-liquidity-and-funding-risk.md).

## 8. Nguồn tham khảo

Các nguồn sau hỗ trợ nguyên lý và định nghĩa nêu trong bài. Ví dụ và phép tính là mô hình tự xây dựng, đã kiểm tra độc lập; không phải số liệu thị trường trong các tài liệu.

1. **Andrew W. Lo, MIT OpenCourseWare**, [*15.401 Finance Theory I — Lectures 4–6: Fixed-Income Securities*](https://ocw.mit.edu/courses/15-401-finance-theory-i-fall-2008/df418b972d36cd53ae5c375b8af61e53_MIT15_401F08_lec04.pdf), khóa Fall 2008, tài liệu ghi bản quyền 2007–2008. Dùng slide 11, 25–26, 36, 39–41 và 46 cho định giá, duration và các thành phần rủi ro; không dùng dữ liệu lịch sử trong slide làm tình hình hiện tại.
2. **SEC, Office of Investor Education and Advocacy**, [*What Are Corporate Bonds?*](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/what-are), 04/06/2013. Dùng phần fixed coupon, price–yield, giữ đến đáo hạn và các rủi ro; không vận dụng các mô tả pháp lý Mỹ cho Việt Nam.
3. **CFA Institute**, [*Interest Rate Risk and Return*](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/interest-rate-risk-and-return), **2026 Curriculum, Level I, Fixed Income**. Dùng phần Overview công khai cho quan hệ giữa dòng tiền, tái đầu tư và lợi suất kép; không nhận là đã đọc toàn bộ giáo trình có yêu cầu đăng nhập.
4. **Vanguard**, [*What is a Bond and How do they Work?*](https://investor.vanguard.com/investor-resources-education/understanding-investment-types/what-is-a-bond), trang không hiển thị ngày công bố, truy cập 03/10/2026. Chỉ dùng đoạn mô tả cấu trúc quỹ trái phiếu thông thường và kỳ hạn, không dùng nội dung quảng bá sản phẩm.
5. **SEC, Investor.gov**, [*Bond Funds and Income Funds*](https://www.investor.gov/introduction-investing/investing-basics/glossary/bond-funds-and-income-funds), trang không hiển thị ngày công bố, truy cập 03/10/2026. Dùng phần rủi ro lãi suất của quỹ trái phiếu.

## 9. Liên kết kiến thức

- **Tái đầu tư coupon và lợi suất trong kỳ nắm giữ:** kết hợp khoản thu, giá bán và cách sử dụng tiền đã nhận để đo kết quả đầu tư.
- **Chênh lệch lợi suất tín dụng:** tách thay đổi của mức lợi suất chuẩn với phần bù của một người phát hành cụ thể.
- **Convexity và thay đổi đường cong không song song:** mở rộng duration khi cú thay đổi lớn hoặc từng kỳ hạn dịch chuyển khác nhau.

## 10. Điều đáng nhớ nhất

1. Coupon cố định không giữ giá cố định. Với dòng tiền và ngày định giá không đổi, lợi suất chiết khấu tăng làm giá hiện tại giảm.
2. Duration nối thời điểm nhận dòng tiền với độ nhạy giá, nhưng dự báo từ nó chỉ là xấp xỉ có điều kiện.
3. Giữ đến đáo hạn có thể tránh phải bán ở giá thấp, nếu bạn có thể chờ và người phát hành trả đủ. Nó không xóa rủi ro tín dụng, sức mua hay tái đầu tư; phải phân biệt YTM của dòng tiền với tăng trưởng tài sản cuối kỳ.

## 11. Góc Phản xạ & Active Recall (Dành cho bạn)

Hãy thử giải thích cho một người bạn bằng 2–3 câu: vì sao trái phiếu vẫn trả đúng 5 triệu đồng mỗi năm nhưng người mua mới chỉ chấp nhận trả khoảng 97,327 triệu đồng sau khi YTM tăng từ 5% lên 6%?

**Thang tự đánh giá (1–5):** Bạn thấy mức độ hiểu/nhớ cơ chế hôm nay ở mức nào — 1 = cần đọc lại sớm, 3 = nắm vững, 5 = rất tự tin? Nếu bạn chọn 1–2, lần chọn bài tiếp theo có thể ưu tiên củng cố cơ chế này khi nhận được phản hồi của bạn.
