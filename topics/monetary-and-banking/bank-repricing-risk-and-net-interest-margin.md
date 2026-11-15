---
id: MONEY-004
title: "Vì sao biên lãi ròng của ngân hàng có thể thu hẹp khi lãi suất tăng?"
category: monetary-and-banking
tags: [interest-rates, banking, repricing-risk, net-interest-margin]
prerequisites: [MONEY-003]
difficulty: Intermediate
date: 2026-11-15
last_verified: 2026-11-15
---

# Vì sao biên lãi ròng của ngân hàng có thể thu hẹp khi lãi suất tăng?

## 1. Chủ đề hôm nay

**Rủi ro tái định giá lãi suất (repricing risk)** và tác động lên **biên lãi ròng (net interest margin, NIM)** của ngân hàng. Kiến thức nền về tài sản, tiền gửi và nguồn vốn nằm trong [MONEY-003](bank-liquidity-and-funding-risk.md).

## 2. Vấn đề cốt lõi

Một ngân hàng vừa nâng lãi suất cho vay mới nhưng lại báo biên lãi ròng thấp hơn quý trước. Hai thông tin có thể cùng đúng. Mức lãi mới chỉ áp dụng cho một phần danh mục trong kỳ. Nếu phần lãi ngân hàng phải trả tăng nhiều hơn phần lãi ngân hàng thu thêm, thu nhập lãi thuần giảm. Biên lãi ròng còn phụ thuộc vào quy mô tài sản sinh lãi bình quân.

## 3. Giải thích cơ chế

### Ngân hàng đo biên lãi như thế nào?

**[Definition]** **Thu nhập lãi thuần (net interest income, NII)** là thu nhập lãi trừ chi phí lãi trong kỳ. **Biên lãi ròng (NIM)** cho biết ngân hàng tạo ra bao nhiêu thu nhập lãi thuần trên mỗi đồng tài sản sinh lãi bình quân. Tài sản sinh lãi có thể gồm khoản cho vay và chứng khoán sinh lãi. Chi phí lãi có thể đến từ tiền gửi và các khoản vay khác của ngân hàng. Nếu dùng NIM quý đã quy đổi theo năm, tử số là thu nhập lãi thuần quý đã quy đổi theo năm, còn mẫu số là tài sản sinh lãi bình quân của kỳ đo. [FDIC, *The Historic Relationship Between Bank Net Interest Margins and Short-Term Interest Rates*, tr. 31 và chú thích 6](https://archive.fdic.gov/view/fdic/15523/fdic_15523_DS1.pdf#page=35).

$$
\mathrm{NIM}=\frac{\mathrm{NII}}{\text{Tài sản sinh lãi bình quân}}
$$

**[Accounting Identity]** Tách tử số cho thấy NIM bằng lợi suất tài sản sinh lãi trừ tỷ suất chi phí tài trợ khi cả hai tỷ suất cùng dùng tài sản sinh lãi bình quân làm mẫu số và cùng cơ sở quy đổi theo năm. Nếu lấy chi phí lãi tiền gửi chia cho số dư tiền gửi bình quân, kết quả là lãi suất tiền gửi bình quân mà ngân hàng thực trả. Tỷ lệ đó dùng mẫu số của riêng tiền gửi.

### Mô hình giáo trình (Textbook Model)

**[Definition]** Một khoản được **tái định giá (repricing)** khi lãi suất áp dụng được xác lập lại. Khoản vay thả nổi có thể đổi lãi vào ngày điều chỉnh dù còn lâu mới đáo hạn. Với tiền gửi lãi cố định, lãi suất mới có thể áp dụng khi người gửi tái tục sau đáo hạn. **Rủi ro tái định giá** phát sinh khi thời điểm đổi lãi hoặc số dư được đổi lãi lệch nhau giữa tài sản và nguồn vốn, khiến lãi thu và lãi trả phản ứng khác nhau. [Ủy ban Basel, SRP98, mục 98.15 và 98.44](https://www.bis.org/committees/bcbs/basel-framework/standard/srp/98/inforce/2019-12-15/published/2019-12-15).

**[Theoretical Model]** So sánh một kịch bản có cú sốc lãi suất với kịch bản cơ sở trong cùng kỳ một năm, với cùng số dư tính lãi. Nhóm khoản vay và nhóm nguồn vốn nhạy lãi suất đổi lãi ngay đầu kỳ rồi áp dụng mức mới suốt năm. Nhóm lãi suất cố định dùng mức đã cam kết cho cả năm. Mô hình lược bỏ trả trước, vỡ nợ, tái đầu tư phần lãi và công cụ phòng hộ.

$$
\Delta\mathrm{NII}=A_R\,\Delta r_A - L_R\,\Delta r_L
$$

$A_R$ là số dư tài sản sinh lãi được tái định giá, $L_R$ là số dư nợ chịu lãi được tái định giá. $\Delta r_A$ và $\Delta r_L$ là mức thay đổi lãi suất năm của hai nhóm, viết dưới dạng thập phân. Tích thứ nhất đo khoản lãi thu thêm trong năm, còn tích thứ hai đo khoản lãi trả thêm. Với tài sản sinh lãi bình quân cố định, NIM đi cùng chiều với NII.

Nếu lãi suất áp dụng cho hai nhóm cùng tăng $\Delta r$, công thức rút gọn thành $(A_R-L_R)\Delta r$. **Chênh lệch tái định giá (repricing gap)** là $A_R-L_R$ trong kỳ xét. Chênh lệch âm làm NII giảm trong kịch bản tăng lãi suất đồng mức. Khi hai mức lãi biến động khác nhau, cần dùng mức thay đổi riêng của mỗi nhóm. [Ủy ban Basel, SRP98, mục 98.44](https://www.bis.org/committees/bcbs/basel-framework/standard/srp/98/inforce/2019-12-15/published/2019-12-15).

### Cơ chế thực tế (Real-World Mechanism)

- **[Causal Mechanism] Khoản vay đổi lãi theo hợp đồng.** Khi lãi suất tham chiếu tăng, ngân hàng có thể thu thêm trên các khoản vay thả nổi khi đến ngày điều chỉnh, tùy công thức, trần hoặc sàn trong hợp đồng. Khoản vay cố định tiếp tục áp dụng mức đã thỏa thuận trong thời hạn cố định. Tỷ trọng khoản vay đổi lãi và số tháng còn lại trong kỳ quyết định phần thu thêm xuất hiện nhanh đến đâu. [Ủy ban Basel, SRP98, mục 98.15 và 98.44](https://www.bis.org/committees/bcbs/basel-framework/standard/srp/98/inforce/2019-12-15/published/2019-12-15).
- **[Causal Mechanism] Chi phí huy động phản ứng theo cạnh tranh và lựa chọn của người gửi.** Khi có nơi trả lãi cao hơn, người gửi có thể chuyển sang kỳ hạn dài hơn, sang ngân hàng khác hoặc sang sản phẩm thay thế. Ngân hàng cần giữ nguồn vốn có thể nâng lãi cho tiền gửi mới hoặc tái tục. Chi phí bình quân cũng có thể tăng ngay cả khi lãi từng sản phẩm giữ nguyên, nếu tỷ trọng tiền gửi lãi cao tăng. [Kang-Landsberg, Luck và Plosser, *Deposit Betas: Up, Up, and Away?*](https://libertystreeteconomics.newyorkfed.org/2023/04/deposit-betas-up-up-and-away/).
- **[Definition] Hệ số truyền dẫn vào lãi suất tiền gửi (deposit beta)** đo mức thay đổi của một lãi suất tiền gửi chia cho mức thay đổi khác 0 của lãi suất tham chiếu trong cùng khoảng thời gian. Ví dụ, lãi tham chiếu tăng 2 điểm phần trăm, còn lãi của một sản phẩm tiền gửi tăng 1 điểm phần trăm, thì hệ số của sản phẩm trong kỳ đó là 0,5. Khi dùng lãi suất tiền gửi bình quân toàn ngân hàng, kết quả còn phản ánh sự dịch chuyển giữa các loại tiền gửi. [Kang-Landsberg, Luck và Plosser, *Deposit Betas: Up, Up, and Away?*](https://libertystreeteconomics.newyorkfed.org/2023/04/deposit-betas-up-up-and-away/).

**[Causal Mechanism]** Cùng một cú tăng lãi suất có thể làm lợi suất chiết khấu của trái phiếu lãi cố định tăng, kéo giá trị hiện tại của các khoản thanh toán theo hợp đồng xuống. Tiền lãi theo hợp đồng vẫn theo lịch cũ nếu bên phát hành trả đầy đủ. Vì vậy ngân hàng có thể ghi nhận NII tăng trong năm và đồng thời thấy giá trị thị trường của một phần tài sản giảm. Để xem tác động đến giá trị kinh tế của vốn chủ sở hữu, ngân hàng còn phải xét giá trị hiện tại của các nghĩa vụ và các vị thế phòng hộ. [Ủy ban Basel, SRP98, mục 98.2 và 98.25–98.29](https://www.bis.org/committees/bcbs/basel-framework/standard/srp/98/inforce/2019-12-15/published/2019-12-15).

## 4. Ví dụ trực quan

**[Theoretical Model] Số liệu giả định.** Bảng cân đối đầu kỳ của ngân hàng có tổng tài sản 1.050 tỷ đồng, bằng 900 tỷ nợ tiền gửi cộng 150 tỷ vốn chủ sở hữu. Bảng dùng tiền mặt tại quỹ làm tài sản thanh toán không sinh lãi. Nếu xét số dư dự trữ tại ngân hàng trung ương, khoản đó cũng nằm bên tài sản. Theo giả định số dư tính lãi cố định, mẫu số NIM là 1.000 tỷ tài sản sinh lãi bình quân.

| Khoản mục đầu kỳ | Phân loại | Số dư (tỷ đồng) | Lãi suất năm ban đầu |
| :--- | :--- | ---: | ---: |
| Khoản vay cố định lãi đến hết năm | Tài sản sinh lãi | 700 | 7% |
| Khoản vay thả nổi điều chỉnh đầu kỳ | Tài sản sinh lãi | 300 | 7% |
| Tiền mặt tại quỹ | Tài sản | 50 | 0% |
| Tiền gửi cố định lãi đến hết năm | Nợ chịu lãi | 400 | 4% |
| Tiền gửi đáo hạn đầu kỳ, giả định tái tục toàn bộ | Nợ chịu lãi | 500 | 4% |
| Vốn chủ sở hữu | Vốn chủ sở hữu | 150 | — |

Giả sử lãi suất tham chiếu tăng 2 điểm phần trăm đầu kỳ. Lãi trên 300 tỷ khoản vay thả nổi tăng từ 7% lên 9% trong cả hai kịch bản. Chỉ mức lãi của 500 tỷ tiền gửi tái tục khác nhau giữa hai kịch bản.

| Kết quả cả năm | Không có cú sốc | Kịch bản A | Kịch bản B |
| :--- | ---: | ---: | ---: |
| Lãi suất năm của tiền gửi tái tục | 4% | 5% | 6% |
| Thu nhập lãi (tỷ đồng) | 70 | 76 | 76 |
| Chi phí lãi (tỷ đồng) | 36 | 41 | 46 |
| NII (tỷ đồng) | 34 | 35 | 30 |
| NIM | 3,40% | 3,50% | 3,00% |

Ngân hàng thu thêm $300\times2\%=6$ tỷ đồng. Ở A, ngân hàng trả thêm $500\times1\%=5$ tỷ, nên NII tăng 1 tỷ. Ở B, ngân hàng trả thêm $500\times2\%=10$ tỷ, nên NII giảm 4 tỷ dù thu nhập lãi vẫn tăng. Điểm cân bằng trong ví dụ là lãi suất trên nhóm tái tục tăng **1,2 điểm phần trăm**, vì $6/500=1{,}2\%$ khiến lãi thu thêm vừa đủ bù lãi trả thêm.

Thời điểm cũng có thể đổi kết quả. Nếu 500 tỷ tiền gửi ở B chỉ tái tục vào giữa năm và khoản vay thả nổi vẫn đổi lãi ngay đầu năm, chi phí lãi năm đó tăng $500\times2\%\times0{,}5=5$ tỷ. Trong biến thể đó, NII tăng 1 tỷ.

## 5. Tình huống thực tế

**[Historical Claim]** Trong quý II/2024, NIM tổng hợp của các tổ chức tại Mỹ được FDIC bảo hiểm giảm 1 điểm cơ bản, tương đương 0,01 điểm phần trăm, so với quý I và còn **3,16%**. Theo FDIC, mức tăng của tỷ suất chi phí tài trợ nhỉnh hơn mức tăng của lợi suất tài sản sinh lãi. Cùng kỳ, tổng thu nhập lãi thuần tăng 0,1% so với quý I, còn NIM tăng ở tất cả nhóm quy mô ngoài nhóm ngân hàng lớn nhất. [FDIC, *Quarterly Banking Profile*, quý II/2024, tr. 2](https://www.fdic.gov/quarterly-banking-profile/quarterly-banking-profile-second-quarter-2024#page=2).

Số liệu minh họa hai việc có thể xảy ra cùng lúc. Toàn nhóm có thêm thu nhập lãi thuần tính bằng tiền trong khi biên lãi tính trên mỗi đồng tài sản sinh lãi thu hẹp. Kết quả tổng hợp cũng có thể đi ngược kết quả của các nhóm ngân hàng nhỏ hơn. Để biết vì sao NIM của một ngân hàng cụ thể thay đổi, cần xem cơ cấu tài sản và nguồn vốn, ngày đổi lãi và số dư bình quân của chính ngân hàng đó.

## 6. Kiến thức này có ích gì với tôi?

- **Khi đọc tin ngân hàng tăng lãi huy động**, hãy xem mức mới áp dụng cho sản phẩm nào và cho bao nhiêu tiền gửi đến kỳ tái tục. Khi đọc kết quả kinh doanh, đối chiếu thu nhập lãi, chi phí lãi và tài sản sinh lãi bình quân trên cùng cơ sở kỳ đo. Ba dòng này giúp giải thích một phần thay đổi lợi nhuận. Phí, chi phí hoạt động và dự phòng tín dụng cũng có thể làm lợi nhuận ròng đi theo hướng khác với NIM. [FDIC, *Quarterly Banking Profile*, quý II/2024, tr. 1–2](https://www.fdic.gov/quarterly-banking-profile/quarterly-banking-profile-second-quarter-2024).
- **Khi đọc điều khoản vay hoặc gửi tiết kiệm**, với khoản vay thả nổi hãy xem ngày điều chỉnh, lãi tham chiếu và biên độ cộng thêm. Với tiền gửi có điều khoản tự động tái tục, hãy xem khi nào kỳ mới bắt đầu và mức lãi nào được dùng cho kỳ đó. Hai hợp đồng có thể truyền cùng một biến động lãi suất vào dòng tiền của bạn ở hai thời điểm khác nhau.

## 7. Nguồn tham khảo

1. Angela Hinton và Chester Polson, FDIC Quarterly, 2021. [*The Historic Relationship Between Bank Net Interest Margins and Short-Term Interest Rates*](https://archive.fdic.gov/view/fdic/15523/fdic_15523_DS1.pdf#page=35).
2. Basel Committee on Banking Supervision, 2019. [*Application guidance on interest rate risk in the banking book* (SRP98)](https://www.bis.org/committees/bcbs/basel-framework/standard/srp/98/inforce/2019-12-15/published/2019-12-15).
3. Alena Kang-Landsberg, Stephan Luck và Matthew Plosser, Liberty Street Economics, Federal Reserve Bank of New York, 11/04/2023. [*Deposit Betas: Up, Up, and Away?*](https://libertystreeteconomics.newyorkfed.org/2023/04/deposit-betas-up-up-and-away/).
4. Federal Deposit Insurance Corporation, 2024. [*Quarterly Banking Profile, Second Quarter 2024*](https://www.fdic.gov/quarterly-banking-profile/quarterly-banking-profile-second-quarter-2024).

## 8. Liên kết kiến thức

- **Truyền dẫn lãi suất điều hành** giải thích vì sao các lãi suất tham chiếu của khoản vay và nguồn vốn có thể dịch chuyển khác nhau. [MONEY-002](policy-rates-and-monetary-transmission.md).
- **Duration trái phiếu** giúp ước tính độ nhạy của giá trị tài sản với lợi suất trong khi theo dõi thu nhập lãi theo kỳ. [INVEST-001](../investing/bond-prices-duration-and-interest-rate-risk.md).
- **Cạnh tranh huy động và deposit beta** mở đường để phân tích riêng tác động của lãi niêm yết và dịch chuyển cơ cấu tiền gửi.
- **Phòng hộ bằng hoán đổi lãi suất (interest rate swaps)** là bước tiếp theo để hiểu ngân hàng có thể thay đổi độ nhạy của dòng lãi bằng một hợp đồng trao đổi các khoản thanh toán lãi.

## 9. Điều đáng nhớ nhất

- Dấu của thay đổi thu nhập lãi thuần phụ thuộc bên nào có phần lãi thay đổi lớn hơn. Mỗi phần chịu tác động của số dư, mức lãi thay đổi và thời gian áp dụng.
- NIM đo thu nhập lãi thuần trên mỗi đồng tài sản sinh lãi bình quân. Khi quy mô tài sản sinh lãi đổi, thu nhập lãi thuần và NIM có thể đi khác chiều.

## 10. Góc Phản xạ & Active Recall (Dành cho bạn)

Bạn sẽ giải thích thế nào trong 2–3 câu việc ngân hàng ở kịch bản B thu thêm 6 tỷ tiền lãi nhưng biên lãi ròng giảm?

**Thang tự đánh giá (1–5)** Bạn thấy mình hiểu cơ chế hôm nay đến đâu? Mức 1 là cần đọc lại sớm, mức 3 là nắm vững và mức 5 là rất tự tin. Chọn mức 1–2 sẽ giúp ưu tiên củng cố chủ đề sớm hơn.
