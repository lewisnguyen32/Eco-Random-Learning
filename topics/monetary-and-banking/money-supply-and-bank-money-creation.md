---
id: MONEY-001
title: "Cung tiền M1, M2 và Cơ chế Tạo tiền của Ngân hàng Thương mại"
category: monetary-and-banking
tags: [money-supply, liquidity, fractional-reserve, central-bank, core-anchor]
prerequisites: []
difficulty: Fundamental
date: 2026-08-12
---

### 1. Chủ đề hôm nay

**Cung tiền M1, M2 và Cơ chế Tạo tiền của Ngân hàng Thương mại** (*Money Supply M1/M2 and Commercial Bank Money Creation*).

---

### 2. Vấn đề cốt lõi

Khi báo chí đưa tin *"Ngân hàng Trung ương bơm tiền vào nền kinh tế"* hoặc *"Cung tiền M2 tăng mạnh 10%"*, nhiều người hình dung Ngân hàng Trung ương đang vận hành các máy in tiền giấy liên tục ngày đêm.

Tuy nhiên, trong nền kinh tế hiện đại, **hơn 80% - 90% lượng tiền lưu hành không được tạo ra từ máy in của Ngân hàng Trung ương**, mà được tạo ra bởi các ngân hàng thương mại thông qua hoạt động cấp tín dụng (cho vay). 

Bài học này giải thích:
* Tiền trong nền kinh tế thực chất được đo lường như thế nào qua các chỉ số $M0, M1, M2$?
* Làm thế nào một khoản tiền gửi ban đầu lại có thể nhân lên gấp nhiều lần thông qua hệ thống ngân hàng?
* Giới hạn nào ngăn cản các ngân hàng tạo ra vô hạn tiền?

---

### 3. Giải thích cơ chế

#### a. Phân loại Cung tiền: Từ Tiền cơ sở đến Tiền rộng

Tiền không chỉ là những tờ tiền giấy trong ví của bạn. Trong kinh tế học vĩ mô, tiền được phân loại theo độ thanh khoản (khả năng chuyển đổi thành tiền mặt tức thì mà không mất giá trị):

1. **Tiền cơ sở (Base Money - $MB$ hoặc $B$):**
   * Do Ngân hàng Trung ương (NHTW) phát hành duy nhất.
   * Bao gồm: Tiền mặt lưu thông ngoài hệ thống ngân hàng ($C$) + Tiền dự trữ của các ngân hàng thương mại gửi tại NHTW ($R$).
   * Formula: $MB = C + R$.

2. **Cung tiền hẹp ($M1$ - Transaction Money):**
   * Đo lường lượng tiền sẵn sàng dùng ngay để thanh toán hàng ngày.
   * Bao gồm: Tiền mặt lưu thông ($C$) + Tiền gửi thanh toán không kỳ hạn tại các ngân hàng thương mại ($D$).
   * Formula: $M1 = C + D$.

3. **Cung tiền rộng ($M2$ - Broad Money):**
   * Đo lường toàn bộ phương tiện thanh toán và các tài sản có tính thanh khoản cao gần như tiền.
   * Bao gồm: $M1$ + Tiền gửi tiết kiệm có kỳ hạn của cá nhân, tiền gửi có kỳ hạn của doanh nghiệp và các chứng chỉ tiền gửi ngắn hạn.
   * Formula: $M2 = M1 + \text{Tiền gửi có kỳ hạn}$.

#### b. Cơ chế Tạo tiền của Hệ thống Ngân hàng Dự trữ Một phần (Fractional-Reserve Banking)

Khi bạn gửi 100 triệu đồng vào Ngân hàng A, ngân hàng không cất 100 triệu đó vào két sắt chờ bạn đến rút. Theo quy định, ngân hàng chỉ cần giữ lại một tỷ lệ nhất định gọi là **Tỷ lệ dự trữ bắt buộc** ($r$), phần còn lại được đem cho vay.

Chính hành động cho vay này đã **tạo ra tiền mới** trong nền kinh tế:

1. Người vay nhận tiền giải ngân dưới dạng chuyển khoản hoặc tiền mặt.
2. Họ dùng số tiền đó để thanh toán cho người bán hàng / đối tác.
3. Người nhận tiền lại đem gửi số tiền này vào Ngân hàng B.
4. Ngân hàng B tiếp tục trích giữ dự trữ $r$ và cho vay phần dư còn lại.

Vòng lặp này tiếp diễn qua Ngân hàng C, D, E... làm cho tổng lượng tiền gửi ($D$) trong toàn hệ thống tăng vọt so với số tiền cơ sở ($MB$) ban đầu.

#### c. Công thức Số nhân Tiền (Money Multiplier)

Trong mô hình lý thuyết đơn giản nhất (giả định người dân không giữ tiền mặt, ngân hàng không giữ dự trữ dôi dư):

$$\text{Số nhân tiền lý thuyết } (m) = \frac{1}{r}$$

Trong đó:
* $m$: Số nhân tiền (*Money Multiplier*).
* $r$: Tỷ lệ dự trữ bắt buộc (*Required Reserve Ratio*).

Tổng cung tiền tối đa ($M$) tạo ra từ lượng tiền gửi ban đầu ($D_0$) là:

$$\Delta M = D_0 \times \frac{1}{r}$$

**Trong thực tế phức tạp hơn:**
Số nhân tiền thực tế ($m_{\text{thực tế}}$) luôn nhỏ hơn $\frac{1}{r}$ vì có hai yếu tố rò rỉ (leakage):
1. **Tỷ lệ giữ tiền mặt của người dân ($c = C/D$):** Người dân rút một phần tiền mặt ra khỏi hệ thống để chi tiêu tự do.
2. **Tỷ lệ dự trữ dôi dư của ngân hàng ($e = ER/D$):** Ngân hàng giữ lại thêm một khoản dự trữ phòng hộ rủi ro thanh khoản ngoài mức bắt buộc.

Công thức số nhân tiền đầy đủ:

$$m = \frac{1 + c}{c + r + e}$$

Khi đó, tổng cung tiền $M1 = m \times MB$.

---

### 4. Ví dụ trực quan

Giả sử Ngân hàng Trung ương mua 1.000 USD trái phiếu chính phủ từ Ngân hàng A (bơm 1.000 USD tiền cơ sở $MB$ vào hệ thống). Giả định tỷ lệ dự trữ bắt buộc $r = 10\%$ (0,10), người dân không giữ thêm tiền mặt ($c = 0$), và ngân hàng không giữ dự trữ dôi dư ($e = 0$).

Hãy theo dõi hành trình tạo tiền qua các bước:

| Bước | Chủ thể | Tiền gửi nhận vào ($D$) | Dự trữ bắt buộc $10\%$ ($R$) | Cho vay mới ($\Delta \text{Loan}$) | Cung tiền M1 gia tăng |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Gốc** | Ngân hàng A | $1.000 USD | $100 USD | $900 USD | +$1.000 USD |
| **Vòng 1** | Ngân hàng B | $900 USD | $90 USD | $810 USD | +$900 USD |
| **Vòng 2** | Ngân hàng C | $810 USD | $81 USD | $729 USD | +$810 USD |
| **Vòng 3** | Ngân hàng D | $729 USD | $72,9 USD | $656,1 USD | +$729 USD |
| ... | ... | ... | ... | ... | ... |
| **TỔNG** | **Toàn hệ thống** | **$10.000 USD** | **$1.000 USD** | **$9.000 USD** | **$10.000 USD** |

**Ý nghĩa:**
Từ **1.000 USD tiền cơ sở ban đầu** do NHTW phát hành, thông qua 900 USD cho vay của ngân hàng A, 810 USD của ngân hàng B... tổng lượng tiền gửi thanh toán ($M1$) trong toàn nền kinh tế đã tăng lên thành **10.000 USD** (gấp $m = 1/0,1 = 10$ lần).

---

### 5. Tình huống thực tế

#### Tình huống: Bẫy thanh khoản và Cuộc hoảng loạn rút tiền (Bank Run) làm sụt giảm Cung tiền

Điều gì xảy ra khi nền kinh tế bước vào suy thoái, niềm tin suy giảm và xuất hiện nguy cơ đứt gãy tín dụng?

1. **Hành vi người dân:** Người dân lo sợ ngân hàng phá sản nên ồ ạt rút tiền mặt về két sắt cá nhân. Tỷ lệ giữ tiền mặt $c = C/D$ **tăng vọt**.
2. **Hành vi ngân hàng thương mại:** Ngân hàng sợ nợ xấu và đứt gãy thanh khoản nên dừng cho vay mới, ôm tiền mặt dự trữ dôi dư. Tỷ lệ $e = ER/D$ **tăng vọt**.

**Hệ quả vĩ mô:**
Dù Ngân hàng Trung ương có hạ lãi suất và cố gắng bơm thêm tiền cơ sở ($MB$), số nhân tiền $m = \frac{1+c}{c+r+e}$ bị sụt giảm nghiêm trọng do mẫu số $(c+r+e)$ tăng quá nhanh. 

Kết quả là **tăng trưởng cung tiền $M2$ bị tắc nghẽn (Credit Crunch)**, dẫn đến tình trạng "bẫy thanh khoản": Tiền nằm chết trong hệ thống ngân hàng mà không chảy được vào sản xuất kinh doanh thực tế. Đây chính là nguyên nhân khiến cuộc Đại Khủng hoảng 1929 tại Mỹ trở nên tàn khốc khi cung tiền bị co hẹp gần $30\%$.

---

### Kiến thức này có ích gì với tôi?

1. **Hiểu đúng bản tin kinh tế:** Khi đọc tin *"Tăng trưởng tín dụng đạt 14%"*, bạn hiểu rằng lượng tiền $M2$ trong nền kinh tế vừa được mở rộng tương ứng thông qua kênh cho vay của ngân hàng.
2. **Nhận diện nguy cơ Lạm phát:** Nếu cung tiền $M2$ tăng trưởng quá nhanh vượt xa tốc độ tăng trưởng hàng hóa thực tế ($GDP$), áp lực lạm phát sẽ xuất hiện sau 12 - 18 tháng (theo thuyết số lượng tiền tệ $M \cdot V = P \cdot Y$).
3. **Đánh giá sức khỏe ngân hàng cá nhân gửi tiền:** Bạn hiểu vì sao ngân hàng luôn đối mặt với rủi ro kỳ hạn (*maturity mismatch*): Ngân hàng dùng tiền gửi ngắn hạn để cho vay dài hạn, và chỉ giữ một phần dự trữ nhỏ ($r$). Việc rút tiền hàng loạt (*bank run*) có thể quật ngã cả một ngân hàng vững mạnh nếu thiếu sự hỗ trợ thanh khoản từ NHTW.

---

### Thuật ngữ

* **Tiền cơ sở (Base Money - MB/B):** Tổng tiền mặt lưu hành ngoài ngân hàng cộng với tiền dự trữ của các ngân hàng thương mại gửi tại Ngân hàng Trung ương.
* **Cung tiền M1 (M1 Money Supply):** Tổng tiền mặt lưu hành và tiền gửi thanh toán không kỳ hạn (tiền có thể chi tiêu tức thì).
* **Cung tiền M2 (M2 Money Supply):** Cung tiền $M1$ cộng với tiền gửi tiết kiệm có kỳ hạn và chứng chỉ tiền gửi ngắn hạn.
* **Dự trữ bắt buộc (Required Reserves - R):** Tỷ lệ tiền gửi tối thiểu mà ngân hàng thương mại buộc phải giữ lại tại NHTW theo quy định pháp luật.
* **Số nhân tiền (Money Multiplier - m):** Hệ số phản ánh mức độ mở rộng của cung tiền từ một đơn vị tiền cơ sở ban đầu.

---

### Nguồn tham khảo

1. **Mishkin, Frederic S.** (2021). *The Economics of Money, Banking and Financial Markets* (13th ed.). Pearson. (Giáo trình chuẩn quốc tế về Tiền tệ & Ngân hàng).
2. **Ngân hàng Nhà nước Việt Nam (SBV).** *Luật Ngân hàng Nhà nước Việt Nam năm 2010 & Luật các Tổ chức Tín dụng năm 2024*. (Quy định về dự trữ bắt buộc và công cụ điều hành cung tiền).
3. **Federal Reserve Bank of St. Louis.** *Page One Economics: Money and Missed Conceptions* (2021). (Tài liệu phân tích cơ chế tạo tiền và công cụ điều hành tiền tệ hiện đại).

---

### Liên kết kiến thức

* [`MACRO-001`](topics/macroeconomics-and-monetary/interest-rates-and-monetary-policy-transmission.md) *(⏳ Chưa học)*: Lãi suất điều hành & Kênh truyền dẫn chính sách tiền tệ.
* [`MACRO-002`](topics/macroeconomics-and-monetary/inflation-types-and-cpi-measurement.md) *(⏳ Chưa học)*: Lạm phát: Bản chất, Đo lường CPI và Mối liên hệ với Cung tiền $M2$.
* [`CORP-001`](topics/corporate-and-markets/cash-conversion-cycle.md) *(✅ Đã học)*: Chu kỳ chuyển đổi tiền mặt & Rủi ro Thanh khoản Doanh nghiệp.

---

### Điều đáng nhớ nhất

1. **Ngân hàng thương mại là nhà tạo tiền chính:** Ngân hàng không chỉ là trung gian tài chính chuyển tiền từ người tiết kiệm sang người vay, mà chính hành động cho vay đã mở rộng cung tiền $M1/M2$ của toàn bộ nền kinh tế.
2. **Số nhân tiền chịu ảnh hưởng bởi 3 chủ thể:** NHTW (ấn định $r$), Ngân hàng thương mại (quyết định dự trữ dôi dư $e$), và Người dân/Doanh nghiệp (quyết định thói quen giữ tiền mặt $c$).
3. **Dự trữ một phần tạo ra sự mong mỏng thanh khoản:** Vì ngân hàng chỉ giữ lại tỷ lệ dự trữ $r < 100\%$, rủi ro hoảng loạn rút tiền (*bank run*) luôn tồn tại nếu mất niềm tin hệ thống.

---

### Góc Phản xạ & Active Recall (Dành cho bạn)

> 💡 **Dạng 1 (Tóm tắt lại):** *"Hãy thử tự giải thích cho một người bạn không học kinh tế nghe: Tại sao khi ngân hàng thương mại duyệt một khoản vay 1 tỷ đồng cho khách hàng mua nhà, lượng tiền trong toàn nền kinh tế lại tăng thêm 1 tỷ đồng ngay lập tức?"*

*Gợi ý nhẹ cuối mục:* **Thang tự đánh giá (1-5):** Bạn tự thấy mức độ hiểu/nhớ cơ chế hôm nay ở mức nào (1 = Cần đọc lại sớm / 3 = Nắm vững / 5 = Rất tự tin)?
