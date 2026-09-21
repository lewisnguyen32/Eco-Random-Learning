---
id: MONEY-001
title: "Cung tiền M1, M2 và Cơ chế Tạo tiền của Ngân hàng Thương mại"
category: monetary-and-banking
tags: [money-supply, liquidity, fractional-reserve, central-bank, core-anchor]
prerequisites: []
difficulty: Fundamental
date: 2026-08-12
last_verified: 2026-09-22
---

# Cung tiền và cơ chế tạo tiền của ngân hàng thương mại

## 1. Chủ đề hôm nay

**Cung tiền (Money supply)**, **tiền gửi ngân hàng (Commercial-bank deposits)** và cơ chế **khoản vay tạo tiền gửi (Loans create deposits)**.

## 2. Vấn đề cốt lõi

Khi ngân hàng giải ngân, tiền trên tài khoản người vay xuất hiện thế nào? Vì sao ngân hàng vẫn cần huy động tiền gửi nếu có thể tạo tiền gửi mới? Và vì sao NHTW “bơm thanh khoản” chưa chắc làm tiền gửi của công chúng tăng?

Bài phân biệt việc tạo một nghĩa vụ thanh toán với việc có đủ tài sản, vốn và phương tiện thanh toán để thực hiện nghĩa vụ đó. Không gán một tỷ lệ “80–90%” chung cho mọi quốc gia hoặc mọi thước đo cung tiền.

## 3. Giải thích cơ chế

### 3.1. Ba khái niệm tiền cần tách biệt

[Definition]

| Hình thái | Chủ thể nắm giữ và bản chất |
| :--- | :--- |
| Tiền mặt công chúng nắm giữ ($C$) | Tiền giấy/tiền xu ngoài các tổ chức nhận tiền gửi; cơ quan phát hành cụ thể tùy quốc gia. |
| Tiền gửi khách hàng ($D$) | Tài sản của khách hàng và nợ phải trả của ngân hàng; khả năng rút/chuyển phụ thuộc loại tài khoản và điều kiện hợp đồng. |
| Số dư dự trữ tại NHTW ($R_{CB}$) | Tài sản của ngân hàng đủ điều kiện mở tài khoản và nợ của NHTW; được dùng để quyết toán giữa các ngân hàng. |

**Tiền mặt trong két ngân hàng (vault cash) không phải số dư tài khoản tại NHTW.** Một số quy ước thống kê hoặc chế độ dự trữ có gộp chúng vào khái niệm dự trữ rộng hơn; cần nói rõ khi sử dụng.

[Accounting Identity] Để tránh bỏ sót hoặc đếm hai lần tiền mặt, bài dùng:

$$B = C + C_{\text{két}} + R_{CB}$$

Nếu đặt $R=C_{\text{két}}+R_{CB}$ thì $B=C+R$. Đây là quy ước cho mô hình. Trong thống kê H.6 của Fed, tiền cơ sở gồm currency in circulation (bao gồm tiền trong két tổ chức nhận tiền gửi) cộng reserve balances. [Fed, H.6 ngày 23/11/2021, chú thích bảng tiền cơ sở](https://www.federalreserve.gov/releases/h6/20211123/).

### 3.2. M1 và M2 phải đi kèm khung thống kê

[Theoretical Model] Để học cơ chế, có thể đặt tiền giao dịch đơn giản là $M=C+D$ với D là tiền gửi thanh toán. Nhưng không được coi $M=C+D$ là định nghĩa đầy đủ của M1 mọi nơi.

[Historical Claim] Trong H.6 của Mỹ, từ tháng 5/2020 M1 bao gồm cả tiền gửi tiết kiệm trong nhóm “other liquid deposits”; M2 còn bổ sung một số tiền gửi có kỳ hạn nhỏ và quỹ thị trường tiền tệ bán lẻ. Vì vậy không nên suy ra thay đổi hoạt động kinh tế chỉ từ một bước nhảy chuỗi M1 khi định nghĩa thay đổi. [Fed, H.6, chú thích M1/M2](https://www.federalreserve.gov/releases/h6/20211123/).

Đọc dữ liệu Việt Nam hoặc một nước khác phải tra phạm vi tài sản, chủ thể giữ tiền và đơn vị tiền tệ trong phương pháp luận của chính cơ quan công bố.

### 3.3. REAL-WORLD MECHANISM – khoản vay tạo tiền gửi

[Causal Mechanism] Giả sử ngân hàng A cấp một khoản vay mới 100 triệu và ghi có vào tài khoản thanh toán của khách hàng X. X thuộc khu vực được tính trong cung tiền và khoản tiền gửi này đủ điều kiện tính vào chỉ tiêu đang xét:

| Chủ thể | Thay đổi tài sản | Thay đổi nợ phải trả | Thay đổi vốn chủ/tài sản ròng |
| :--- | :--- | :--- | :--- |
| Ngân hàng A | Khoản cho vay +100 | Tiền gửi X +100 | 0 |
| Khách hàng X | Tiền gửi +100 | Nợ vay +100 | 0 |

Không có khoản tiền gửi nào của người khác bị trừ tại thời điểm này. **Tiền gửi tăng nhưng tài sản ròng của X không tự tăng**, vì X đồng thời mắc nợ. Đây là cơ chế hạch toán khoản vay mới, không phải một cách tạo của cải miễn phí. [Bank of England, Money creation in the modern economy, 2014](https://www.bankofengland.co.uk/quarterly-bulletin/2014/q1/money-creation-in-the-modern-economy).

Các khoản vay có cách giải ngân khác có thể tạo bút toán ở ngân hàng của người bán hoặc dùng ngay để trả khoản vay cũ. Phải xét giao dịch ròng và chủ thể nhận tiền, không mặc định mọi con số “giải ngân” đều bằng tăng cung tiền ròng.

### 3.4. Chuyển khoản và huy động vẫn quan trọng

[Accounting Identity] X dùng 100 triệu trả người bán Y tại ngân hàng B; giả sử thanh toán riêng lẻ, không bù trừ:

| Chủ thể | Tài sản | Nợ phải trả |
| :--- | :--- | :--- |
| Ngân hàng A | Dự trữ tại NHTW −100 | Tiền gửi X −100 |
| Ngân hàng B | Dự trữ tại NHTW +100 | Tiền gửi Y +100 |

Tổng tiền gửi và tổng dự trữ hệ thống không đổi qua bước chuyển khoản; chúng đổi nơi nắm giữ. A vẫn giữ tài sản khoản vay 100 triệu đã tạo ở bước trước.

A cần có hoặc thu xếp số dư thanh toán: nhận tiền gửi/chuyển tiền đến, vay liên ngân hàng, bán tài sản hay vay NHTW nếu đủ điều kiện. **Huy động ảnh hưởng chi phí và độ ổn định nguồn vốn**, nên “loans create deposits” không có nghĩa ngân hàng khỏi cần quản trị nguồn vốn.

### 3.5. Vì sao không tạo tiền vô hạn?

[Causal Mechanism] Trước khi cho vay, ngân hàng phải đánh giá:

- **Rủi ro và khả năng sinh lời:** người vay có trả được không, lãi thu có bù được chi phí và tổn thất dự kiến không?
- **Vốn chủ và yêu cầu an toàn vốn:** tăng tài sản rủi ro hoặc ghi nhận lỗ có thể làm suy giảm tỷ lệ an toàn vốn. Tiền gửi mới là nợ, không phải vốn chủ.
- **Thanh khoản và nguồn vốn:** khoản tiền gửi có thể chuyển đi ngay, còn khoản vay khó thu hồi tức thì.
- **Nhu cầu tín dụng và quy định áp dụng:** khách đủ điều kiện có muốn vay không; ngân hàng có bị giới hạn bởi quy định cụ thể không?

NHTW có thể cung ứng dự trữ nhằm thực thi chính sách nhưng không cam kết cứu mọi ngân hàng, nhận mọi tài sản bảo đảm hoặc đáp ứng mọi yêu cầu vô điều kiện. Kế hoạch nguồn vốn phải được tính trước; không phải ngân hàng cứ cho vay xong rồi chắc chắn kiếm được dự trữ. [Bank of England, 2014, phần giới hạn tạo tiền](https://www.bankofengland.co.uk/quarterly-bulletin/2014/q1/money-creation-in-the-modern-economy).

### 3.6. Trả nợ, rút tiền và mất vốn là ba việc khác nhau

[Accounting Identity] Nếu X dùng tiền gửi để trả **gốc khoản vay đang nằm trên bảng cân đối ngân hàng**, tài sản khoản vay và nợ tiền gửi đều giảm. Nếu trả qua ngân hàng khác, thêm bước chuyển dự trữ nhưng tổng tiền gửi hệ thống vẫn giảm, giả định không có giao dịch bù trừ khác.

- Trả nợ cho một **chủ nợ phi ngân hàng** thường chuyển tiền gửi từ người trả sang chủ nợ, không tự xóa tiền gửi toàn hệ thống.
- **Rút tiền mặt** chuyển tiền gửi thành tiền mặt; trong mô hình $M=C+D$, M không đổi chỉ do việc đổi hình thái này.
- **Xóa sổ nợ xấu** làm giảm giá trị khoản vay và được phản ánh qua dự phòng/vốn chủ; không tự xóa khoản tiền gửi mà người vay đã chuyển cho người bán.

[Bank of England, How is money created?, cập nhật 01/10/2019](https://www.bankofengland.co.uk/explainers/how-is-money-created) giải thích cơ chế tiền gửi hình thành và bị xóa khi trả nợ; các trường hợp trên là kiểm tra hạch toán của từng giao dịch.

### 3.7. TEXTBOOK MODEL – hiểu đúng số nhân tiền

[Accounting Identity trong mô hình] Đặt $M=C+D$, $B=C+R$, $c=C/D$, $r=RR/D$ và $e=ER/D$, với $R=RR+ER$ theo quy ước dự trữ của mô hình:

$$\frac{M}{B}=\frac{C+D}{C+R}=\frac{1+c}{c+r+e}$$

Nếu c, r, e là các tỷ số đo được, đây là phép biến đổi đại số. Nó **không tự nói biến nào gây ra biến nào**.

[Theoretical Model] Để dùng $m=1/r$ làm giới hạn mở rộng tiền gửi, cần thêm giả định: B cố định, công chúng không giữ tiền mặt, ngân hàng không giữ dự trữ dôi dư, có đủ người vay và các ràng buộc khác không chặn mở rộng tín dụng. Khi đó, $D \le B/r$, đạt dấu bằng nếu toàn bộ dự trữ là bắt buộc.

Ví dụ mô hình: B = 1.000, r = 10% thì mức D tối đa theo điều kiện này là 10.000. Đây là **mức tiền gửi**, không đương nhiên là “tăng thêm 10.000”: thay đổi phải trừ mức ban đầu. Nếu r = 0 thì mô hình này không cho giới hạn hữu hạn; không có nghĩa ngân hàng thực tế cho vay vô hạn.

## 4. Ví dụ trực quan: NHTW mua tài sản

Toàn bộ số liệu giả định, đơn vị triệu đồng; giao dịch **mua đứt**, chưa xét phí hay lãi/lỗ.

### Trường hợp A: mua từ ngân hàng

| Chủ thể | Tài sản | Nợ phải trả |
| :--- | :--- | :--- |
| NHTW | Trái phiếu +100 | Dự trữ ngân hàng A +100 |
| Ngân hàng A | Trái phiếu −100; dự trữ +100 | Không đổi |

Dự trữ tăng, **chưa có tiền gửi khách hàng mới**.

### Trường hợp B: mua từ một doanh nghiệp phi ngân hàng

| Chủ thể | Tài sản | Nợ phải trả |
| :--- | :--- | :--- |
| NHTW | Trái phiếu +100 | Dự trữ ngân hàng A +100 |
| Ngân hàng A | Dự trữ +100 | Tiền gửi doanh nghiệp +100 |
| Doanh nghiệp | Trái phiếu −100; tiền gửi +100 | Không đổi |

Giả sử doanh nghiệp và tài khoản thuộc phạm vi cung tiền đang xét, tiền gửi được tính vào cung tiền tăng 100 **mà không cần ngân hàng cấp khoản vay mới**. Đó là lý do không thể giải thích mọi tăng trưởng tiền gửi chỉ bằng cho vay. [Bank of England, QE: functioning and effectiveness, 2022](https://www.bankofengland.co.uk/quarterly-bulletin/2022/2022-q1/qe-at-the-bank-of-england-a-perspective-on-its-functioning-and-effectiveness).

Hai trường hợp không làm người bán giàu thêm đúng 100: họ đổi trái phiếu lấy tài sản thanh khoản. Giá tài sản và hành vi chi tiêu về sau là kênh khác, không phải hệ quả kế toán tự động.

## 5. Tình huống thực tế

### Tín dụng yếu dù thanh khoản ngân hàng dồi dào

[Causal Mechanism] Dự trữ tăng có thể giúp ngân hàng thanh toán dễ hơn. Nhưng nếu người vay ít đơn hàng hoặc ngân hàng thiếu vốn/rủi ro nợ xấu cao, tín dụng vẫn có thể yếu.

[Definition] **Credit crunch** là sự thu hẹp mạnh nguồn cung tín dụng. **Liquidity trap** là tình huống mô hình trong đó tiền và tài sản ngắn hạn an toàn gần thay thế nhau khi lãi suất ở vùng thấp/sát giới hạn hiệu dụng, khiến nới lỏng tiền tệ thông thường kém hiệu lực. Nhu cầu vay yếu riêng lẻ không đủ để chẩn đoán bẫy thanh khoản; hai hiện tượng không đồng nghĩa và không nhất thiết kéo theo nhau.

Không đồng nhất giới hạn hiệu dụng với ngưỡng 0% cứng, hoặc kết luận mọi công cụ tiền tệ đều vô hiệu ở vùng lãi suất thấp. [Stanley Fischer – Fed, Low Interest Rates, 05/10/2016](https://www.federalreserve.gov/newsevents/speech/fischer20161005a.htm).

### Một minh họa lịch sử có phạm vi rõ ràng

[Historical Claim] Theo bài *The Great Depression* của Federal Reserve History, cung tiền Mỹ giảm gần 30% **từ mùa thu 1930 đến mùa đông 1933**. Không đổi khoảng này thành “1929–1933” hoặc tự gắn nhãn M2 nếu không đối chiếu chuỗi tương ứng. [Federal Reserve History, 22/11/2013](https://www.federalreservehistory.org/essays/great-depression).

Bài học cơ chế là rút tiền, khủng hoảng ngân hàng và suy giảm chi tiêu có thể khuếch đại nhau. Con số trên không tự chứng minh một nguyên nhân duy nhất cho toàn bộ Đại Khủng hoảng.

## 6. Kiến thức này có ích gì với tôi?

Khi đọc tin “bơm tiền”, hãy hỏi: giao dịch gì, với ai, tài khoản nào tăng? Mua đứt từ ngân hàng, repo với ngân hàng và mua từ công chúng không có cùng bút toán.

Tiền gửi là quyền đòi ngân hàng, không phải phong bì tiền mặt được cất riêng cho từng người. Do đó cần phân biệt **thiếu thanh khoản** với **thiếu vốn/tài sản không đủ bù nợ**; tạo tiền gửi không tự giải quyết được cả hai.

Khi đọc tin M2 tăng, không suy ngay ra CPI sẽ tăng một tỷ lệ cố định sau một số tháng cố định. Cần xét chi tiêu, sản lượng, cầu nắm giữ tiền và các cú sốc khác; xem [MACRO-001](../macroeconomics/inflation-cpi-and-macro-transmission.md).

## 7. Thuật ngữ

- **Tiền gửi ngân hàng (Bank deposit):** tài sản của khách hàng, nợ của ngân hàng.
- **Số dư dự trữ (Reserve balances):** số dư tài khoản của tổ chức đủ điều kiện tại NHTW; khác tiền mặt trong két.
- **Tiền cơ sở (Monetary base):** tiền mặt do công chúng/ngân hàng nắm giữ cộng số dư dự trữ theo quy ước đã nêu.
- **Số nhân tiền (Money multiplier):** tỷ số cung tiền/tiền cơ sở; chỉ là giới hạn nhân quả trong mô hình khi thêm giả định.
- **Thanh khoản (Liquidity):** khả năng đáp ứng thanh toán; không đồng nhất với vốn chủ.
- **Siết chặt tín dụng (Credit crunch):** suy giảm nguồn cung tín dụng, phân biệt với giảm nhu cầu vay.

## 8. Nguồn tham khảo

1. **McLeay, Radia & Thomas – Bank of England (14/03/2014)**, [Money creation in the modern economy](https://www.bankofengland.co.uk/quarterly-bulletin/2014/q1/money-creation-in-the-modern-economy).
2. **Federal Reserve Board (23/11/2021)**, [Money Stock Measures – H.6](https://www.federalreserve.gov/releases/h6/20211123/), dùng cho định nghĩa và thay đổi phân loại, không dùng làm số liệu hiện tại.
3. **Bank of England (01/10/2019)**, [How is money created?](https://www.bankofengland.co.uk/explainers/how-is-money-created).
4. **Bank of England (2022 Q1)**, [QE at the Bank of England: a perspective on its functioning and effectiveness](https://www.bankofengland.co.uk/quarterly-bulletin/2022/2022-q1/qe-at-the-bank-of-england-a-perspective-on-its-functioning-and-effectiveness).
5. **Gary Richardson – Federal Reserve History (22/11/2013)**, [The Great Depression](https://www.federalreservehistory.org/essays/great-depression).

## 9. Liên kết kiến thức

- [MACRO-001](../macroeconomics/inflation-cpi-and-macro-transmission.md) – Lạm phát và CPI (✅ Đã học).
- [MONEY-002](policy-rates-and-monetary-transmission.md) – Lãi suất và truyền dẫn tiền tệ, bao gồm ví dụ repo/OMO (✅ Đã học).
- [CORP-001](../corporate-and-markets/cash-conversion-cycle.md) – Chu kỳ tiền mặt và thanh khoản doanh nghiệp (✅ Đã học).

## Điều đáng nhớ nhất

1. Cho vay có thể tạo tiền gửi nhưng đồng thời tạo nợ; ngân hàng vẫn bị giới hạn bởi vốn, rủi ro, nguồn vốn và nhu cầu vay.
2. Tiền gửi khách hàng, số dư dự trữ và tiền mặt trong két phải được theo dõi riêng.
3. Tác động lên cung tiền phụ thuộc **đối tác và bút toán giao dịch**, không chỉ tên gọi “bơm tiền”.

## Góc Phản xạ & Active Recall (Dành cho bạn)

Hãy giải thích vì sao cùng là NHTW mua trái phiếu 100 triệu, mua từ ngân hàng và mua từ doanh nghiệp có thể tác động khác nhau lên tiền gửi khách hàng.

**Thang tự đánh giá (1–5):** 1 = cần đọc lại sớm; 3 = nắm vững; 5 = tự lập được bảng cân đối cho hai giao dịch.
