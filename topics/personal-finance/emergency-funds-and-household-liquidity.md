---
id: INDIV-002
title: "Quỹ dự phòng và thanh khoản cá nhân"
category: personal-finance
tags: [emergency-fund, household-liquidity, cash-flow-budget, income-volatility]
prerequisites: [BEHAV-002]
difficulty: Intermediate
date: 2026-11-24
last_verified: 2026-11-24
---

# Quỹ dự phòng và thanh khoản cá nhân

## 1. Chủ đề hôm nay

Quỹ dự phòng (*emergency fund*) và thanh khoản cá nhân (*household liquidity*).

> 🔄 **Ôn tập Ngắt quãng (Delayed Active Recall)**
>
> Trong [BEHAV-002](../behavioral-finance/mental-accounting-and-financial-decisions.md), vì sao một phương án phải dùng đến quỹ dự phòng khi trả nợ cuối năm dù lúc đầu khoản quỹ được để riêng? Hãy thử nhớ lại một ý trước khi đọc tiếp.

## 2. Vấn đề cốt lõi

Bạn có tiền gửi đáo hạn ngày 20, trong khi xe cần sửa để đi làm ngày 10. Cả tháng có thể thu nhiều hơn chi. Vào ngày 10, điều quyết định bạn trả được tiền sửa xe là số tiền có thể dùng khi hóa đơn đến hạn. Vậy cần có bao nhiêu tiền sẵn từ đầu kỳ, và phần nào trong số đó dành cho biến cố?

## 3. Giải thích cơ chế

**[Definition]** Thanh khoản cá nhân là khả năng huy động đủ phương tiện thanh toán đúng lúc có khoản phải trả. Khi xét thanh khoản của một tài sản, cần hỏi mất bao lâu để có tiền dùng được và thực nhận bao nhiêu sau phí, chênh lệch giá hoặc tổn thất khi bán gấp.

**[Accounting Identity]** Tài sản ròng (*net worth*) bằng giá trị tài sản trừ các khoản nợ tại cùng thời điểm. Hai hộ có cùng tài sản ròng có thể có số tiền dùng được rất khác nhau vào ngày mai.

**[Definition]** Quỹ dự phòng là khoản tiền để dành cho chi phí bất ngờ hoặc cho những khoản thiết yếu khi thu nhập bị gián đoạn. Tiền dành cho hóa đơn đã biết trước thuộc ngân sách thông thường. Cả hai đều góp vào số tiền có thể chi nếu chúng thực sự tiếp cận được vào thời điểm cần thiết. [CFPB, hướng dẫn về quỹ dự phòng](https://www.consumerfinance.gov/an-essential-guide-to-building-an-emergency-fund/).

### Mô hình giáo trình (Textbook Model)

**[Accounting Identity]** Trong phạm vi số tiền sẵn để chi của hộ, số dư sau mốc $t$ bằng số dư ban đầu $B_0$ cộng tiền vào khả dụng $I_s$ và trừ tiền ra $O_s$ lũy kế qua các mốc $s$.

$$
B_t = B_0 + \sum_{s=1}^{t}(I_s - O_s)
$$

Mỗi mốc là một thời điểm dòng tiền phát sinh. Nếu tiền vào và hóa đơn đến hạn cùng ngày, thứ tự trong ngày vẫn quan trọng. Khoản chuyển giữa hai tài khoản đều đã nằm trong số tiền sẵn để chi giữ nguyên số dư của cả nhóm. Khi một tài sản trước đó nằm ngoài nhóm được chuyển thành tiền dùng được, chỉ ghi khoản tiền ròng vào ngày có thể sử dụng.

**[Theoretical Model]** Để dự phóng, lấy $I_s$ theo lịch tiền có thể dùng và $O_s$ theo lịch các khoản phải trả đủ, đúng hạn trong một kịch bản. Giữ nguyên lịch tương lai khi so các mức $B_0$. Giả sử hộ không vay mới và các nguồn chuyển thành tiền đã được liệt kê đầy đủ. Với $T$ là mốc cuối kỳ, điều kiện để đáp ứng lịch là $B_t \geq 0$ tại mọi mốc từ $0$ đến $T$. Mức tiền khả dụng tối thiểu đầu kỳ là

$$
B_0^{\min} = \max\left\{0,\ \max_{1\leq t\leq T} \sum_{s=1}^{t}(O_s-I_s)\right\}.
$$

Hộ phải có đủ tiền để bù **mức chi vượt tiền vào lũy kế lớn nhất** trong kỳ. Số dư âm trong phép dự phóng cho biết mức thiếu ròng tại riêng mốc đang xét. Với số dư đầu kỳ hiện có, phần tiền cần bổ sung để trả đúng hạn đến một mốc bằng mức thiếu ròng lớn nhất qua tất cả các hạn thanh toán tính đến mốc đó.

CFPB minh họa ngân sách dòng tiền (*cash flow budget*) theo tuần bằng cách chuyển số dư cuối tuần sang tuần kế tiếp. Công thức trên áp dụng cùng logic ở từng mốc thanh toán. [CFPB, *Your Money, Your Goals*, mục 5](https://files.consumerfinance.gov/f/documents/cfpb_your-money-your-goals_financial-empowerment_toolkit.pdf#page=100).

### Cơ chế thực tế (Real-World Mechanism)

**[Causal Mechanism]** Hộ gia đình cần chi đúng hạn để duy trì sinh hoạt và công việc. Chủ nhà hoặc bên sửa xe cần nhận tiền theo thỏa thuận. Nếu một bên đồng ý dời hạn, thời điểm tiền ra thay đổi và khoảng thiếu hụt có thể giảm. Nếu hộ chuyển một tài sản thành tiền, thời điểm nhận tiền phụ thuộc vào điều kiện rút hoặc thời gian hoàn tất giao dịch. Giá trị dùng để lập lịch là số tiền ròng có thể chi vào ngày đó. [CFPB, quản lý dòng tiền và khả năng tiếp cận khoản dự phòng](https://www.consumerfinance.gov/an-essential-guide-to-building-an-emergency-fund/).

**[Causal Mechanism]** Vay có thể bù thiếu hụt nếu khoản tiền thực nhận đến kịp. Bên cho vay quyết định có cấp vốn và với điều kiện nào. Khi giải ngân bằng tiền, trước phí, tiền khả dụng và nợ gốc của hộ tăng cùng số tiền. Sau đó, lịch chi phải tính cả gốc, lãi và phí đến hạn. Hạn mức chưa sử dụng là một nguồn vay tiềm năng, còn quỹ dự phòng nằm trong tài sản của hộ. [CFPB, phần “When should I use it?”](https://www.consumerfinance.gov/an-essential-guide-to-building-an-emergency-fund/).

## 4. Ví dụ trực quan

**[Theoretical Model]** Tất cả số liệu sau đây đều giả định, đơn vị triệu đồng. Đầu kỳ, Lan có 10 triệu dùng ngay và 20 triệu tiền gửi. Trong kịch bản này, tiền gửi chỉ dùng được từ ngày 20 và ta bỏ qua lãi. Lan không vay mới, các khoản chi trong bảng đều đến hạn và các mục còn lại giữ nguyên khi so mức tiền đầu kỳ.

| Ngày | Giao dịch | Tiền vào khả dụng | Tiền phải chi | Chi trừ tiền vào lũy kế | Số dư nếu đầu kỳ có 14 triệu khả dụng |
| :--- | :--- | ---: | ---: | ---: | ---: |
| 5 | Trả tiền thuê nhà | 0 | 9 | 9 | 5 |
| 10 | Sửa xe đột xuất | 0 | 5 | **14** | **0** |
| 15 | Khách hàng trả thù lao | 7 | 0 | 7 | 7 |
| 18 | Đóng học phí đến hạn | 0 | 6 | 13 | 1 |
| 20 | Nhận tiền gửi đáo hạn | 20 | 0 | −7 | 21 |
| 30 | Nhận lương | 16 | 0 | −23 | 37 |

Sau khi trả tiền thuê, Lan còn 1 triệu trên thực tế. Đến ngày sửa xe, Lan **thiếu 4 triệu** để thanh toán đủ. Nếu có 14 triệu khả dụng từ đầu kỳ với cùng lịch sau đó, Lan vừa đủ trả mọi khoản. Thu nhập trong tháng là 23 triệu, chi là 20 triệu. Khoản đáo hạn chuyển 20 triệu Lan đã sở hữu từ tiền gửi sang số dư có thể chi.

Với 10 triệu đầu kỳ, mức thiếu ròng dự phóng vào ngày 18 là 3 triệu, tính theo lịch dự kiến. Để thanh toán đúng hạn đến hết ngày 18, Lan vẫn cần bổ sung 4 triệu từ đầu kỳ vì số tiền thiếu nhiều nhất rơi vào ngày 10.

Với lịch thông thường không có khoản sửa xe, Lan cần 9 triệu khả dụng đầu kỳ. Khoản sửa xe nâng mức tối thiểu của kịch bản lên 14 triệu, tức cần thêm 5 triệu so với lịch thông thường. Phần Lan còn thiếu là 4 triệu vì Lan đã có sẵn 10 triệu.

## 5. Tình huống thực tế · Khi chi phí bất ngờ trùng với tiền về muộn

**[Theoretical Model]** Xét lại lịch trên với một thay đổi. Khách hàng của Lan trả thù lao muộn hơn bảy ngày, vào ngày 22. Đến ngày 18, Lan phải chi lũy kế $9+5+6=20$ triệu và chưa có khoản tiền vào nào. Ngày 20 mới có tiền gửi đáo hạn. Số tiền cần sẵn từ đầu kỳ tăng từ **14 lên 20 triệu**. Cả hai lịch có cùng tổng tiền vào và tiền ra trong tháng. Khoản đến muộn làm Lan phải tự trang trải thêm một lần thanh toán trước khi tiền về.

**[Empirical Relationship]** Một nghiên cứu năm 2019 của JPMorgan Chase Institute dùng dữ liệu tài khoản Chase tại Mỹ từ tháng 10/2012 đến tháng 12/2018, lấy chủ tài khoản chính làm đơn vị phân tích. Trong các quan sát theo từng chủ tài khoản và từng tháng, nhóm tác giả xét trường hợp thu nhập giảm mạnh cùng lúc chi tiêu tăng mạnh theo tiêu chí nghiên cứu. Độ lớn trung vị của cú sốc quy đổi tương đương **6,2 tuần thu nhập thực nhận tham chiếu**. Thu nhập tham chiếu là trung vị thu nhập tháng trong 12 tháng trước đó của từng đơn vị. Quan sát được tổng hợp theo tháng, còn “tuần” là đơn vị quy đổi số tiền. Kết quả phụ thuộc vào mẫu khách hàng và cách chọn cú sốc. [JPMorgan Chase Institute, Bảng 2](https://www.jpmorganchase.com/content/dam/jpmc/jpmorgan-chase-and-co/institute/pdf/institute-volatility-cash-buffer-report.pdf#page=31).

**[Causal Mechanism]** Chi phí thiết yếu khó dời và thu nhập dễ trễ làm tiền dùng ngay có giá trị hơn, vì nó giúp hộ tránh phải bán gấp hoặc vay thêm nếu biến cố xảy ra. Phần đánh đổi có thể là tiền lãi bỏ qua khi giữ tiền dễ rút, hoặc lãi vay tiếp tục phải trả khi giữ lại số tiền có thể dùng để giảm nợ. Giá trị của quỹ tùy hậu quả của việc trễ hạn và các cách xoay tiền thực sự có trong từng kịch bản. [CFPB, phần về nơi giữ quỹ và khi nào sử dụng](https://www.consumerfinance.gov/an-essential-guide-to-building-an-emergency-fund/).

## 6. Kiến thức này có ích gì với tôi?

- **Đọc tin về sức khỏe tài chính hộ gia đình.** Khi gặp số liệu quỹ dự phòng theo “số tuần”, hãy xem mẫu gồm những ai, mẫu số là thu nhập thực nhận hay chi phí thiết yếu, và biến cố được đo theo kỳ nào.
- **Đánh giá một lựa chọn giữ tiền hoặc vay.** Đặt số tiền ròng có thể rút, thời điểm rút và các khoản phải trả lên cùng lịch. Khoản tiền đến sớm hơn một ngày có thể giúp tránh trễ hạn. Nếu khoản đó là tiền vay, tính cả lần trả sau. Xem cách đọc dòng tiền vay ở [INDIV-001](installment-loans-flat-rates-and-effective-cost.md).
- **Ước lượng phần dự phòng.** Tính mức tiền đầu kỳ cho lịch bình thường, rồi thử thêm một khoản chi khó dời hoặc lùi khoản thu dễ chậm. So các mức tối thiểu thu được để thấy khoản dự phòng đang bảo vệ trước tình huống nào và nó còn bao nhiêu sau khi đã chi.

## 7. Nguồn tham khảo

1. Consumer Financial Protection Bureau, *An essential guide to building an emergency fund*, cập nhật 29/10/2025. [Bài hướng dẫn](https://www.consumerfinance.gov/an-essential-guide-to-building-an-emergency-fund/).
2. Consumer Financial Protection Bureau, *Your Money, Your Goals: A financial empowerment toolkit*, tháng 6/2020, mục 5, trang 97–102. [Tài liệu chính thức](https://files.consumerfinance.gov/f/documents/cfpb_your-money-your-goals_financial-empowerment_toolkit.pdf#page=97).
3. JPMorgan Chase Institute, *Weathering Volatility 2.0: A Monthly Stress Test to Guide Savings*, 23/10/2019, Bảng 2 và phần phương pháp. [Báo cáo nghiên cứu](https://www.jpmorganchase.com/content/dam/jpmc/jpmorgan-chase-and-co/institute/pdf/institute-volatility-cash-buffer-report.pdf).

## 8. Liên kết kiến thức

- **Thanh khoản ngân hàng.** Cùng câu hỏi về khả năng thanh toán đúng hạn, với nghĩa vụ và công cụ thanh toán khác ở cấp ngân hàng. [MONEY-003](../monetary-and-banking/bank-liquidity-and-funding-risk.md).
- **Tiết kiệm phòng ngừa (*precautionary saving*).** Động cơ tiết kiệm hôm nay khi thu nhập hoặc chi phí tương lai bất định.
- **Bảo hiểm và phần chi phí tự trả (*insurance and out-of-pocket costs*).** Khoản phải tự trả và thời điểm nhận bồi hoàn quyết định hộ còn cần chuẩn bị bao nhiêu tiền khả dụng.

## 9. Điều đáng nhớ nhất

1. Mức tiền cần có đầu kỳ phụ thuộc vào khoảng thiếu hụt lũy kế lớn nhất trước các hạn thanh toán. Khoản thu đến sau hạn chỉ giúp từ khi có thể dùng.
2. Tính tiền cần cho lịch thường trước, rồi thử các biến cố có thể xảy ra cùng lúc để thấy phần đệm bổ sung mà mỗi kịch bản đòi hỏi.

## 10. Góc Phản xạ & Active Recall (Dành cho bạn)

Bạn sẽ giải thích bằng hai câu thế nào để một người bạn hiểu vì sao Lan cần thêm 6 triệu tiền sẵn dù tổng thu chi cả tháng giữ nguyên?

**Thang tự đánh giá (1–5)** · 1 = cần đọc lại sớm, 3 = nắm vững, 5 = rất tự tin. Nếu bạn chọn 1–2, bài này sẽ được ưu tiên khi có dịp ôn lại.
