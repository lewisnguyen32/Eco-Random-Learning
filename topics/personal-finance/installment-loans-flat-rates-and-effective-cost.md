---
id: INDIV-001
title: "Chi phí vay trả góp: vì sao cùng “12%/năm” có thể khác xa nhau?"
category: personal-finance
tags: [installment-loans, amortization, flat-rate, effective-cost, cash-flow]
prerequisites: [MONEY-002, MACRO-002]
difficulty: Intermediate
date: 2026-10-11
last_verified: 2026-10-11
---

## 1. Chủ đề hôm nay

**Chi phí vay trả góp (Installment-loan borrowing cost): lãi trên dư nợ giảm dần, lãi phẳng và cách so sánh bằng dòng tiền.**

Bài này mở rộng nền lãi suất ở [MONEY-002](../monetary-and-banking/policy-rates-and-monetary-transmission.md) và cách phân biệt các loại suất ở [MACRO-002](../macroeconomics/fisher-effect-and-yield-curve.md) sang một quyết định đời sống: đọc đúng giá của một khoản vay.

**Phạm vi:** Các con số đều là ví dụ giả định, không phải báo giá hoặc mức lãi suất thị trường Việt Nam. Nguồn được đối chiếu ngày 11/10/2026 để kiểm tra cơ chế và thuật ngữ; bài không trình bày quy định pháp luật về cho vay tại Việt Nam.

## 2. Vấn đề cốt lõi

Hai khoản vay cùng ghi “12%/năm” có thể tạo ra nghĩa vụ trả rất khác nhau. Muốn hiểu chênh lệch, cần biết **tỷ lệ đó nhân với số tiền nào, vào thời điểm nào**.

Người vay thường nhìn khoản trả mỗi tháng để biết mình có chịu được hay không. Nhưng khoản trả nhỏ cũng có thể đến từ kỳ hạn dài hơn, khiến tổng tiền lãi tăng. Vì vậy, ba câu hỏi cần được trả lời riêng: **mỗi kỳ phải trả bao nhiêu, cả hợp đồng tốn bao nhiêu tiền, và chi phí tính theo thời gian sử dụng vốn là bao nhiêu?**

## 3. Giải thích cơ chế

### 3.1. Xác định đúng số gốc và cách trả

**[Definition] Dư nợ gốc (Outstanding principal)** là phần gốc vay còn chưa hoàn trả tại thời điểm xét. Nó khác số tiền ban đầu được ghi trên hợp đồng và khác số tiền người vay thực nhận sau khi trừ phí.

**[Definition] Lãi phẳng (Flat-rate interest)** trong bài là cách tính lãi trên **gốc ban đầu** suốt kỳ hạn, dù gốc đã được trả dần. Với cách tính trên **dư nợ giảm dần (Reducing-balance interest)**, lãi từng kỳ được tính trên gốc còn nợ. Đây là sự khác biệt về cơ sở tính lãi. [MoneySense, phần How interest rates are calculated](https://www.moneysense.gov.sg/costs-of-borrowing-flat-rate-monthly-rest-and-effective-interest-rate/).

Một sự khác biệt khác nằm ở lịch trả gốc:

| Cách trả nợ | Phần gốc trả mỗi kỳ | Tổng gốc và lãi mỗi kỳ, khi lãi suất cố định và tính trên dư nợ |
| :--- | :--- | :--- |
| Trả gốc đều (Equal-principal repayment) | Bằng nhau | Giảm dần vì lãi giảm |
| Trả góp với tổng khoản trả đều (Level-payment amortization) | Tăng dần | Bằng nhau |

**Khoản trả hằng tháng bằng nhau vẫn có thể tính lãi trên dư nợ giảm dần.** Đừng suy phương pháp tính lãi chỉ từ hình dạng khoản trả.

### 3.2. TEXTBOOK MODEL — Mô hình giáo trình: dư nợ giảm dần, tổng khoản trả đều

**[Theoretical Model] Giả định:** Nhận toàn bộ gốc $P$ tại tháng 0; có $n$ khoản trả bằng nhau $A$, khoản đầu vào cuối tháng 1; lãi suất tháng $j$ cố định; trả đúng hạn; không có phí, ân hạn, khoản trả lớn cuối kỳ hoặc lãi chưa trả nhập gốc. Các tháng được coi là các kỳ bằng nhau. Đây là mô hình khoản trả đều dựa trên giá trị hiện tại, như [OpenStax, §8.3 Loan Amortization](https://openstax.org/books/principles-finance/pages/8-3-loan-amortization).

Gọi $B_{t-1}$ là dư nợ gốc đầu tháng $t$, $I_t$ là lãi và $G_t$ là gốc trả trong tháng:

$$
I_t=jB_{t-1},\qquad G_t=A-I_t,\qquad B_t=B_{t-1}-G_t.
$$

**[Accounting Identity — trong phạm vi mô hình]** Khoản trả được phân thành gốc và lãi: $A=G_t+I_t$; gốc cuối kỳ bằng gốc đầu kỳ trừ gốc đã trả. Tiền lãi đã trả không được trừ thêm một lần nữa khỏi dư nợ gốc.

Để dư nợ cuối kỳ bằng 0, khoản trả đều phải là:

$$
A=\frac{Pj}{1-(1+j)^{-n}}\quad(j>0).
$$

Khi $j=0$, $A=P/n$. Công thức bảo đảm giá trị hiện tại của toàn bộ khoản trả bằng số gốc được cấp: tiền trả càng xa thì được chiết khấu càng nhiều. Đây là cùng logic chiết khấu đã dùng với trái phiếu, nhìn từ phía người đi vay.

**Mô hình chứng minh điều gì?** Khi gốc giảm, $I_t$ giảm; nếu $A$ giữ nguyên thì phần trả gốc $G_t$ tăng. “Trả đều” mô tả tổng khoản trả, không mô tả riêng gốc hay lãi. Tổng lãi là $nA-P$, không phải mặc định bằng lãi suất niêm yết nhân toàn bộ gốc và toàn bộ số năm.

### 3.3. TEXTBOOK MODEL — Mô hình giáo trình: lãi phẳng

**[Theoretical Model] Giả định:** Gốc ban đầu $P$; lãi phẳng năm $f$; kỳ hạn $n$ tháng; trả đều tổng gốc và lãi vào cuối mỗi tháng; không có phí và không trả trước hạn. Lãi được xác định theo phép tính đơn trên gốc ban đầu:

$$
I_{\text{tổng, flat}}=P f\frac{n}{12},\qquad
A_{\text{flat}}=\frac{P+I_{\text{tổng, flat}}}{n}.
$$

Người vay đã trả một phần gốc nhưng phép tính lãi vẫn giữ nguyên cơ sở $P$. Bởi vậy, **cùng tỷ lệ niêm yết, cùng gốc, cùng kỳ hạn và trả gốc dần**, cách tính này có thể đắt hơn tính lãi trên số gốc thực còn nợ. Không có quy tắc “lãi phẳng luôn đắt gấp đôi”: chênh lệch còn phụ thuộc tỷ lệ, kỳ hạn, lịch trả và phí.

Công thức này xác định dòng tiền của ví dụ. Nó không xác định cách mọi bên cho vay phân bổ lãi trong sổ sách, hoặc số tiền phải trả nếu tất toán sớm.

### 3.4. Quy các cách báo giá về cùng dòng tiền

**[Definition] Tiền giải ngân ròng (Net loan proceeds), ký hiệu $N$,** là số tiền người vay dùng được tại thời điểm nhận vốn sau khoản phí trả ngay trong ví dụ. Nếu gốc hợp đồng là 100 triệu và phí đầu kỳ bị khấu trừ 2 triệu, $N=98$ triệu; nghĩa vụ gốc vẫn là 100 triệu theo giả định hợp đồng.

**[Definition] Suất chi phí tháng theo dòng tiền (Borrowing-cost IRR), ký hiệu $i$,** là tỷ lệ làm giá trị hiện tại của các khoản phải trả bằng tiền giải ngân ròng:

$$
N=\sum_{t=1}^{n}\frac{C_t}{(1+i)^t}.
$$

$C_t$ là toàn bộ tiền phải trả tại cuối tháng $t$ đã đưa vào phép so sánh, gồm gốc, lãi và phí kỳ đó. Đây là định nghĩa toán học của chỉ tiêu dùng trong bài, không phải phép cộng trực tiếp các tỷ lệ phí vào lãi suất. Với một lần nhận vốn rồi các khoản trả dương ở những tháng sau như ví dụ, phương trình cho một nghiệm chi phí phù hợp.

Ý nghĩa kinh tế: hoàn trả 10 triệu tháng sau khác hoàn trả 10 triệu sau một năm, vì thời gian giữ vốn khác nhau. So sánh tổng lãi mà bỏ thời điểm trả sẽ bỏ mất khác biệt này. Khi không có phí và lịch trả đúng mô hình dư nợ giảm dần, $i=j$; khi có phí, hai tỷ lệ có thể khác nhau.

**[Definition] Suất chi phí hiệu dụng năm (Effective annual borrowing cost)** trong bài được quy đổi rõ ràng bằng:

$$
i_{\text{năm, hiệu dụng}}=(1+i)^{12}-1.
$$

Quy đổi này khác $12i$, là cách năm hóa danh nghĩa theo tỷ lệ tháng. Chẳng hạn, $i=1\%$ cho $12i=12\%$, nhưng suất hiệu dụng năm là khoảng $12{,}68\%$. Cách phân biệt hai quy ước được trình bày tại [OpenStax, §8.4 Stated versus Effective Rates](https://openstax.org/books/principles-finance/pages/8-4-stated-versus-effective-rates).

Đây là **quy ước quy đổi chi phí theo thời gian**, không phải khẳng định hợp đồng đang nhập lãi đã trả vào gốc để thu thêm lãi. Nó cũng không có nghĩa tổng tiền lãi của khoản vay trả góp 100 triệu trong một năm phải bằng 12,68 triệu: gốc được hoàn trả dần, không tồn tại nguyên vẹn suốt năm.

Hai điểm dễ nhầm cần giữ riêng:

- **Hiệu dụng (Effective) khác thực (Real):** “hiệu dụng” ở đây xử lý quy đổi kỳ và dòng tiền; “thực” xử lý sức mua sau lạm phát. Bài chưa điều chỉnh chi phí theo lạm phát.
- **APR/EIR phải được đọc cùng phương pháp công bố:** CFPB phân biệt APR có tính các khoản phí với lãi suất khoản vay trong ngữ cảnh vay mua ô tô tại Hoa Kỳ. Không vì thế mà đồng nhất một APR/EIR bất kỳ với công thức hiệu dụng năm của bài; phải kiểm tra phí được tính và cách năm hóa. [CFPB, What is the difference between a loan interest rate and the APR?](https://www.consumerfinance.gov/ask-cfpb/what-is-the-difference-between-a-loan-interest-rate-and-the-apr-en-733/).

### 3.5. REAL-WORLD MECHANISM — Cơ chế thực tế: từ báo giá tới hợp đồng

Trong một giao dịch vay, người vay muốn có vốn dùng ngay nhưng phải bảo đảm dòng tiền trả sau. Bên cho vay quan tâm tới khoản thu về và khả năng người vay thực hiện nghĩa vụ. Đơn vị bán hàng hoặc môi giới, nếu tham gia, có thể nhấn mạnh khoản trả mỗi tháng để người mua đánh giá việc mua hàng là vừa khả năng chi trả. Những động cơ này giúp giải thích vì sao cần đọc cả lịch trả, thay vì một tỷ lệ hoặc một con số quảng cáo riêng lẻ.

Để đưa một hợp đồng vào phép tính, cần lần theo chuỗi:

```text
Gốc hợp đồng và thời điểm giải ngân
    → tiền thực dùng được sau phí ban đầu
    → cơ sở tính lãi và các ngày đến hạn
    → toàn bộ khoản phải trả theo lịch
    → suất chi phí theo cùng quy ước và áp lực tiền mặt từng kỳ.
```

**[Causal Mechanism]** Nếu phí bị trừ khi giải ngân nhưng lịch trả không giảm, người vay được dùng ít vốn hơn cho cùng nghĩa vụ tương lai; suất chi phí dòng tiền tăng. Nếu phí được nhập vào gốc để tài trợ, gốc và lịch trả có thể cùng thay đổi: phải tính lại từ hợp đồng đó, không lấy tiền ròng của một phương án ghép với khoản trả của phương án khác.

Thực tế có thể dùng số ngày và cơ sở ngày khác mô hình tháng đều; lãi suất có thể đổi sau thời gian ưu đãi; có thể có phí, bảo hiểm kèm khoản vay, ân hạn hoặc khoản trả lớn cuối kỳ. Với khoản phí hoặc sản phẩm kèm theo, cần xác định nghĩa vụ nào bắt buộc cho phương án đang so sánh và thời điểm chi tiền. MoneySense cũng nêu phí xử lý và phí trả sớm trong phần [Other costs of loans](https://www.moneysense.gov.sg/costs-of-borrowing-flat-rate-monthly-rest-and-effective-interest-rate/); đó là ví dụ loại chi phí cần kiểm tra, không phải biểu phí Việt Nam.

Nếu lãi suất tương lai chưa biết, một suất chi phí tính từ lịch trả giả định chỉ là **[Theoretical Model] theo kịch bản**, không phải chi phí đã được bảo đảm. Hợp đồng, lịch trả và các giả định về lãi suất phải đi cùng kết quả.

## 4. Ví dụ trực quan: cùng “12%/năm”, ba dòng tiền

**Ví dụ hoàn toàn giả định.** Gốc hợp đồng 100 triệu đồng; kỳ hạn 12 tháng; nhận vốn tại tháng 0; trả vào cuối mỗi tháng; không trả trễ hoặc trả sớm. Với phương án A, “12%/năm” được **quy ước danh nghĩa thành $j=12\%/12=1\%$ mỗi tháng**, không phải lãi suất hiệu dụng năm 12%. Phương án B dùng lãi phẳng $f=12\%$ trên gốc ban đầu.

**A — Dư nợ giảm dần, tổng khoản trả đều:**

$$
A=\frac{100\times0{,}01}{1-(1{,}01)^{-12}}
\approx8{,}884879\ \text{triệu đồng/tháng}.
$$

Tổng trả khoảng 106,618546 triệu; tổng lãi khoảng **6,618546 triệu**.

| Tháng | Dư nợ đầu kỳ | Lãi | Gốc trả | Tổng khoản trả | Dư nợ cuối kỳ |
| :--- | ---: | ---: | ---: | ---: | ---: |
| 1 | 100,000 | 1,000 | 7,885 | 8,885 | 92,115 |
| 2 | 92,115 | 0,921 | 7,964 | 8,885 | 84,151 |
| … | … | … | … | … | … |
| 12 | 8,797 | 0,088 | 8,797 | 8,885 | 0,000 |

Đơn vị: triệu đồng. Bảng làm tròn ba chữ số sau dấu phẩy; các tổng được tính từ số chưa làm tròn. Gốc giảm về 0, tổng gốc hoàn trả là 100 triệu. Phần lãi giảm và phần gốc tăng dù khoản trả giữ nguyên.

**B — Lãi phẳng, chưa có phí:**

$$
I_{\text{tổng}}=100\times12\%\times1=12\ \text{triệu},\qquad
A_{\text{flat}}=\frac{100+12}{12}=9{,}333333\ \text{triệu/tháng}.
$$

Để tìm chi phí tháng, giải phương trình:

$$
100=\sum_{t=1}^{12}\frac{9{,}333333\ldots}{(1+i)^t}.
$$

Nghiệm khoảng $i=1{,}788099\%$ mỗi tháng, tương đương **23,70%/năm theo quy đổi hiệu dụng**. 12 triệu lãi chia 100 triệu bằng 12%, nhưng phép chia đó không ghi nhận rằng người vay đã phải trả gốc từng tháng.

**B thêm phí 2 triệu trả tại tháng 0:** Giả sử phí bị khấu trừ ngay, nên chỉ nhận ròng 98 triệu; gốc hợp đồng và 12 khoản trả 9,333333… triệu vẫn giữ nguyên. Thay vế trái phương trình thành 98, nghiệm tăng lên khoảng $2{,}116611\%$ mỗi tháng, tương đương **28,58%/năm theo quy đổi hiệu dụng**.

| Chỉ tiêu | A: dư nợ giảm dần | B: lãi phẳng | B: lãi phẳng + phí đầu kỳ |
| :--- | ---: | ---: | ---: |
| Gốc hợp đồng | 100 triệu | 100 triệu | 100 triệu |
| Tiền dùng được tại tháng 0 | 100 triệu | 100 triệu | 98 triệu |
| Khoản trả mỗi tháng | 8,885 triệu | 9,333 triệu | 9,333 triệu |
| Tổng trả từ tháng 1–12 | 106,619 triệu | 112 triệu | 112 triệu |
| Tổng tiền lãi | 6,619 triệu | 12 triệu | 12 triệu |
| Phí tại tháng 0 | 0 | 0 | 2 triệu |
| Tổng chi phí lãi và phí | 6,619 triệu | 12 triệu | 14 triệu |
| Suất chi phí tháng theo dòng tiền | 1,0000% | 1,7881% | 2,1166% |
| Suất chi phí hiệu dụng năm $(1+i)^{12}-1$ | 12,68% | 23,70% | 28,58% |

Đây là **kết quả tính toán từ giả định**, không phải bằng chứng thực nghiệm. Phương án có phí không tăng tiền lãi thành 14 triệu: lãi vẫn 12 triệu và phí là 2 triệu. Khi dùng tiền ròng 98 triệu trong phương trình, không trừ thêm phí ấy lần nữa.

Để so sánh các báo giá cho nhu cầu thực tế cần đủ 100 triệu dùng được, hãy yêu cầu các phương án cấp **cùng số tiền ròng** rồi tính lại lịch trả nếu cần tăng gốc. Bảng trên giữ cùng gốc hợp đồng để tách riêng tác động của phí.

## 5. Tình huống thực tế: kéo dài kỳ hạn để “nhẹ tiền mỗi tháng”

**Tình huống giả định:** Giữ phương án A với gốc 100 triệu, lãi cố định 1%/tháng, không phí; người vay có thể chọn trả trong 12 hoặc 24 tháng. Áp dụng cùng công thức:

| Chỉ tiêu | 12 tháng | 24 tháng |
| :--- | ---: | ---: |
| Khoản trả mỗi tháng | 8,885 triệu | 4,707 triệu |
| Tổng gốc và lãi | 106,619 triệu | 112,976 triệu |
| Tổng tiền lãi | 6,619 triệu | 12,976 triệu |
| Suất chi phí hiệu dụng năm | 12,68% | 12,68% |

**[Causal Mechanism — trong giả định trên]** Kéo dài thời gian trả giúp giảm khoản trả từng tháng, nhưng gốc được hoàn trả chậm hơn nên chịu lãi lâu hơn. Suất chi phí giữ nguyên còn tổng tiền lãi tăng. Vì vậy, khoản trả nhỏ hơn không tự chứng minh khoản vay rẻ hơn.

Ngược lại, tổng lãi thấp hơn cũng không tự chứng minh một lịch trả phù hợp: nếu phải trả 8,885 triệu đúng vào tháng thiếu thu nhập, sức ép tiền mặt có thể lớn. Rủi ro trả trễ và phí phát sinh là một câu hỏi khác với suất chi phí tính khi mọi khoản được trả đúng lịch.

Nếu dự định tất toán sớm, cần lấy **số tiền tất toán tại ngày dự định**, gồm gốc còn nợ, lãi phải trả, phí và phần lãi chưa đến hạn được hoàn hoặc miễn nếu hợp đồng quy định. Không mặc định mọi lãi còn lại trong mô hình flat đều được xóa. Lịch trả sau thay đổi phải được tính lại trước khi đánh giá khoản vay.

## 6. Kiến thức này có ích gì với tôi?

- **Đọc quảng cáo tín dụng:** Khi thấy “lãi chỉ X%” hoặc “chỉ Y đồng/tháng”, tìm cơ sở tính lãi, thời hạn và tiền ròng nhận được. Một tỷ lệ riêng lẻ chưa đủ mô tả giá vay.
- **So sánh báo giá:** Đưa các phương án về cùng nhu cầu tiền ròng, đồng tiền, ngày nhận và quy ước năm hóa. Xem song song suất chi phí, tổng lãi/phí và lịch trả; không xếp hạng chỉ bằng một con số.
- **Quản lý tiền mặt:** Đặt từng khoản trả vào các tháng có thu nhập và chi tiêu. Giá trị hiện tại có thể đúng về toán nhưng không cung cấp sẵn tiền tại ngày đến hạn.
- **Hiểu tin lãi suất:** Lãi suất điều hành thay đổi không cho biết ngay hợp đồng cá nhân giảm bao nhiêu chi phí. Cần xem điều khoản cố định/thả nổi, kỳ điều chỉnh và phí — kết nối với cơ chế truyền dẫn ở MONEY-002.

## 7. Những hiểu lầm phổ biến

| Hiểu lầm | Cách hiểu đúng trong ngữ cảnh bài |
| :--- | :--- |
| “12%/năm thì vay 100 triệu một năm luôn trả 12 triệu lãi.” | Còn tùy dư nợ, lịch trả và quy ước lãi suất; phương án A chỉ có khoảng 6,62 triệu lãi. |
| “Trả cùng một số tiền mỗi tháng là lãi trên gốc ban đầu.” | Trả đều tổng tiền và cơ sở tính lãi là hai đặc điểm riêng; A trả đều nhưng tính lãi trên dư nợ. |
| “Suất hiệu dụng năm 12,68% nghĩa là hợp đồng thu thêm lãi kép trên lãi đã trả.” | Đây là quy đổi tỷ lệ tháng; không tự mô tả điều khoản nhập lãi vào gốc. |
| “Phí chỉ 2% nên cộng 2 điểm phần trăm là xong.” | Phải đưa phí vào đúng thời điểm của dòng tiền, cùng tiền thực nhận và lịch trả. |
| “Suất chi phí thấp nhất luôn là phương án phù hợp nhất.” | Kỳ hạn, sức ép trả tiền, rủi ro lãi thay đổi và điều kiện tất toán cũng ảnh hưởng quyết định. |

## 8. Nguồn tham khảo

1. **MoneySense — Chính phủ Singapore**, *Costs of borrowing: Flat rate, monthly rest, and Effective Interest Rate*, cập nhật **22/04/2026**. [Nguồn trực tiếp](https://www.moneysense.gov.sg/costs-of-borrowing-flat-rate-monthly-rest-and-effective-interest-rate/). Dùng để đối chiếu cơ sở tính lãi và các loại phí; không lấy các con số EIR trên trang làm đồng nghĩa với quy đổi hiệu dụng năm của bài.
2. **Julie Dahlquist và Rainford Knight — OpenStax**, *Principles of Finance*, xuất bản **24/03/2022**, [§8.3 Loan Amortization](https://openstax.org/books/principles-finance/pages/8-3-loan-amortization). Dùng để đối chiếu mô hình giá trị hiện tại của khoản trả đều. Ví dụ và bảng số trong bài này được tự xây dựng và tính lại.
3. **Julie Dahlquist và Rainford Knight — OpenStax**, *Principles of Finance*, **2022**, [§8.4 Stated versus Effective Rates](https://openstax.org/books/principles-finance/pages/8-4-stated-versus-effective-rates). Dùng để đối chiếu quy đổi danh nghĩa và hiệu dụng năm.
4. **Consumer Financial Protection Bureau — Hoa Kỳ**, *What is the difference between a loan interest rate and the APR?*, rà soát **28/08/2026**. [Nguồn trực tiếp](https://www.consumerfinance.gov/ask-cfpb/what-is-the-difference-between-a-loan-interest-rate-and-the-apr-en-733/). Dùng cho phân biệt lãi suất và chỉ tiêu có tính phí trong ngữ cảnh nguồn; không suy sang định nghĩa pháp lý Việt Nam.

## 9. Liên kết kiến thức

- **Giá trị thời gian của tiền và giá trị hiện tại ròng (Time value of money & NPV):** Mở rộng từ một lịch trả nợ sang so sánh các quyết định thu/chi ở nhiều thời điểm.
- **Lãi suất thả nổi và rủi ro tái định giá (Floating rates & Repricing risk):** Vì sao chi phí và khoản trả có thể đổi sau thời gian ưu đãi; nối với [MONEY-002](../monetary-and-banking/policy-rates-and-monetary-transmission.md).
- **Tất toán sớm và tái cấp vốn khoản vay cá nhân (Prepayment & Loan refinancing):** So sánh dòng tiền còn lại với chi phí đóng khoản vay và mở khoản vay mới.
- **Lạm phát và lãi suất thực:** Suất chi phí danh nghĩa trong bài khác gánh nặng sức mua, đồng thời lạm phát không tự làm thu nhập người vay tăng; nối với [MACRO-002](../macroeconomics/fisher-effect-and-yield-curve.md).

## 10. Điều đáng nhớ nhất

1. **Tỷ lệ cần đi cùng cơ sở tính và lịch trả.** Cùng “12%/năm” có thể cho chi phí khác nhau vì gốc ban đầu khác gốc còn nợ.
2. **Tiền ròng nhận được và thời điểm hoàn trả quyết định suất chi phí dòng tiền.** Phí đầu kỳ có thể làm chi phí tăng dù khoản trả hằng tháng không đổi.
3. **Chi phí theo tỷ lệ, tổng số tiền và khả năng trả đúng hạn là ba góc nhìn bổ sung.** Kéo dài kỳ hạn có thể giảm khoản trả nhưng tăng tổng lãi.

## 11. Góc Phản xạ & Active Recall (Dành cho bạn)

Hãy thử giải thích cho một người bạn bằng 2–3 câu: **vì sao khoản vay lãi phẳng 12% trả gốc dần có thể đắt hơn khoản vay 12% tính trên dư nợ còn lại?**

**Thang tự đánh giá (1–5):** Bạn tự thấy mức độ hiểu/nhớ cơ chế hôm nay ở mức nào (1 = Cần đọc lại sớm / 3 = Nắm vững / 5 = Rất tự tin)? Nếu bạn chọn 1–2, hệ thống sẽ ưu tiên quay lại củng cố sớm hơn.
