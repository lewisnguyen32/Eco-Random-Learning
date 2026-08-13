---
id: MACRO-001
title: "Lạm phát: Bản chất, Phương pháp Đo lường CPI và Các Kênh Truyền dẫn Vĩ mô"
category: macroeconomics
tags: [cpi, inflation, money-supply, purchasing-power, macroeconomics]
prerequisites: [MONEY-001]
difficulty: Fundamental
date: 2026-08-13
applicable_year: 2026
last_verified: 2026-08-13
---

# Lạm phát: Bản chất, Phương pháp Đo lường CPI và Các Kênh Truyền dẫn Vĩ mô

## 1. Chủ đề hôm nay

* **Tên tiếng Việt:** Lạm phát và Chỉ số Giá tiêu dùng (CPI)
* **Tên tiếng Anh:** Inflation and Consumer Price Index (CPI)

---

## 2. Vấn đề cốt lõi

Trong đời sống thường ngày, chúng ta thường nghe báo chí thông báo "lạm phát năm nay được kiểm soát ở mức 3.5%", nhưng khi đi chợ hay thanh toán hóa đơn sinh hoạt, nhiều người lại cảm thấy chi phí sống đã tăng lên 10-15%. Vì sao lại có sự chênh lệch này?

Bài học này giải quyết 3 câu hỏi trung tâm:
1. **Bản chất của lạm phát là gì?** Liệu lạm phát là sự tăng giá của một vài hàng hóa riêng lẻ hay là sự suy giảm sức mua mang tính hệ thống của đồng tiền?
2. **Chỉ số CPI được tính toán như thế nào** và sự khác biệt giữa *Lạm phát Tổng thể (Headline Inflation)* và *Lạm phát Cơ bản (Core Inflation)*?
3. **Cung tiền $M2$ chuyển hóa thành Lạm phát qua cơ chế nào**, và tại sao bơm tiền không phải lúc nào cũng gây lạm phát ngay lập tức trên rổ hàng hóa tiêu dùng?

---

## 3. Giải thích cơ chế

### 3.1. Phân định Mô hình Lý thuyết vs Cơ chế Thực tế

#### TEXTBOOK MODEL (Mô hình Giáo trình)

- `[Theoretical Model]` **Thuyết Số lượng Tiền tệ (Quantity Theory of Money - QTM):**
  Trong mô hình kinh tế cổ điển của Irving Fisher và Milton Friedman, mối quan hệ giữa cung tiền và mức giá được diễn tả qua Phương trình Trao đổi:

  $$M \cdot V = P \cdot Y$$

  *Trong đó:*
  * $M$: Cung tiền trong nền kinh tế ($M2$).
  * $V$: Tốc độ lưu thông tiền (Money Velocity - số lần trung bình 1 đơn vị tiền được dùng để mua hàng hóa/dịch vụ trong một kỳ).
  * $P$: Mức giá chung (Price Level).
  * $Y$: Sản lượng thực tế của nền kinh tế (Real Output / Real GDP).

- **Giả định của Mô hình Giáo trình:**
  1. Tốc độ lưu thông tiền $V$ là một hằng số cố định trong ngắn hạn do thói quen thanh toán không đổi.
  2. Sản lượng $Y$ luôn ở mức toàn dụng nhân công (Full-employment output $Y = Y_{\bar{N}}$) cố định bởi công nghệ và nguồn lực.

- **Kết luận của Mô hình Giáo trình:** 
  **Nằm trong phạm vi các giả định của mô hình giáo trình nêu trên**, khi $V$ và $Y$ được giữ cố định, sự gia tăng của cung tiền $M$ được giả định sẽ dẫn tới sự gia tăng tỷ lệ thuận trực tiếp của mức giá $P$:
  
  $$\frac{\Delta M}{M} \approx \frac{\Delta P}{P} = \pi \quad (\text{với } \pi \text{ là tỷ lệ lạm phát})$$

---

#### REAL-WORLD MECHANISM (Cơ chế Thực tế)

Trong thực tế thể chế và vận hành vĩ mô, phương trình $M \cdot V = P \cdot Y$ vẫn đúng về mặt đồng nhất thức, nhưng mối quan hệ $M2 \uparrow \to P \uparrow$ **không phải là quy luật cơ học, tức thời hay 1:1**:

1. `[Accounting Identity & Causal Mechanism]` **Phân biệt Tiền cơ sở ($MB$) vs Cung tiền mở rộng ($M2$) và Tốc độ lưu thông ($V$):**
   * **Tiền cơ sở (Monetary Base - $MB$):** Bao gồm tiền mặt lưu hành ngoài hệ thống ngân hàng cộng với dự trữ của các ngân hàng thương mại tại Ngân hàng Trung ương (reserve balances). Tiền gửi của hộ gia đình/doanh nghiệp không nằm trong $MB$ mà thuộc các chỉ tiêu rộng hơn như $M1/M2$.
   * Khi Ngân hàng Trung ương thực hiện nới lỏng tiền tệ hoặc QE, $MB$ tăng lên dưới dạng tiền dự trữ của ngân hàng thương mại tại NHTW. Việc này **không tự động biến thành quan hệ 1:1 với $M2$ hay tiền gửi tiêu dùng** nếu các ngân hàng thương mại không mở rộng cho vay.
   * Đồng thời, tốc độ lưu thông tiền $V$ biến động rất mạnh. Khi niềm tin kinh tế thấp hoặc ưa thích thanh khoản cao, người dân giữ tiền tiết kiệm thay vì chi tiêu, làm $V$ sụt giảm và triệt tiêu áp lực tăng giá $P$.

2. `[Causal Mechanism]` **Phản ứng của giá tài sản vs CPI (Asset Prices vs CPI):**
   Trong một số giai đoạn nới lỏng tiền tệ và tài chính, dòng tiền có thể phản ứng sớm hơn trên thị trường tài sản (chứng khoán, bất động sản) trước khi lan sang rổ hàng hóa tiêu dùng ($CPI$). Tuy nhiên, đây là hiện tượng phụ thuộc bối cảnh dòng tiền và môi trường lãi suất, không phải là một quy luật cố định luôn xảy ra theo thứ tự.

3. `[Causal Mechanism]` **Các kênh nguyên nhân lạm phát thực tế:**
   * `[Demand-Pull]` **Lạm phát Cầu kéo:** Tổng cầu trong nền kinh tế ($C + I + G + NX$) tăng nhanh hơn khả năng cung ứng của nền kinh tế ($Y < Y_{demand}$).
   * `[Cost-Push]` **Lạm phát Chi phí đẩy:** Giá nguyên vật liệu đầu vào nhập khẩu (dầu mỏ, phân bón, logistics) tăng vọt, hoặc tỷ giá mất giá làm tăng chi phí sản xuất bằng đồng nội tệ, buộc doanh nghiệp phải nâng giá bán dù tổng cầu không tăng.
   * `[Inflation Expectations]` **Kỳ vọng lạm phát:** Khi người dân và công đoàn kỳ vọng giá cả năm tới tăng, họ yêu cầu tăng lương. Doanh nghiệp trả lương cao hơn lại điều chỉnh giá bán để giữ biên lợi nhuận, tạo thành **Vòng xoáy Lương - Giá (Wage-Price Spiral)**.

---

### 3.2. Phương pháp Đo lường CPI & Phân loại Lạm phát

`[Definition]` **Chỉ số Giá tiêu dùng (CPI - Consumer Price Index)** là một **chỉ số giá** (price index) đo lường mức giá trung bình của một rổ hàng hóa và dịch vụ tiêu dùng đại diện cho hộ gia đình. Tỷ lệ phần trăm thay đổi của chỉ số CPI giữa các kỳ được sử dụng để xác định **tỷ lệ lạm phát**.

`[Theoretical Model]` **Công thức chỉ số giá Laspeyres dùng để tính CPI:**

$$\text{CPI}_t = \frac{\sum_{i=1}^{n} (P_{i,t} \cdot Q_{i,0})}{\sum_{i=1}^{n} (P_{i,0} \cdot Q_{i,0})} \times 100$$

*Trong đó:*
* $P_{i,t}$: Giá của mặt hàng $i$ tại thời điểm kỳ tính toán $t$.
* $P_{i,0}$: Giá của mặt hàng $i$ tại thời điểm kỳ gốc $0$.
* $Q_{i,0}$: Lượng tiêu dùng của mặt hàng $i$ tại kỳ gốc $0$ (xác định trọng số của rổ hàng hóa).

`[Definition]` **Tỷ lệ lạm phát ($\pi_t$)** giữa kỳ $t$ và kỳ $t-1$:

$$\pi_t = \frac{\text{CPI}_t - \text{CPI}_{t-1}}{\text{CPI}_{t-1}} \times 100\%$$

---

#### Phân biệt Lạm phát Tổng thể vs Lạm phát Cơ bản

| Tiêu chí | Lạm phát Tổng thể (Headline Inflation) | Lạm phát Cơ bản (Core Inflation) |
| :--- | :--- | :--- |
| **Phạm vi tính toán** | Bao gồm toàn bộ danh mục rổ hàng hóa và dịch vụ tiêu dùng trong chỉ số CPI. | Trừ bỏ một số nhóm mặt hàng biến động ngắn hạn mạnh. Một cách đo phổ biến (như tại Mỹ) là loại bỏ **lương thực - thực phẩm và năng lượng**. Tại Việt Nam, chỉ số lạm phát cơ bản do cơ quan thống kê tính toán còn loại trừ thêm các mặt hàng do Nhà nước quản lý giá (như dịch vụ y tế, giáo dục). |
| **Đặc điểm** | Phản ánh biến động giá ngắn hạn, nhạy cảm với thời tiết, thiên tai và giá năng lượng thế giới. | Loại bỏ các cú shock ngắn hạn để phản ánh xu hướng giá nền tảng dài hạn của nền kinh tế. |
| **Ý nghĩa chính sách** | Phản ánh trực tiếp chi phí sinh hoạt thực tế của hộ gia đình. | Là **một chỉ báo quan trọng** giúp Ngân hàng Trung ương đánh giá áp lực lạm phát nền tảng (*underlying inflation pressure*) cùng với các chỉ báo vĩ mô khác. |

---

### 3.3. Tác động của Lạm phát lên Lợi suất Thực (Real Return)

`[Accounting Identity]` **Phương trình Fisher (Fisher Equation):**
Mối quan hệ **ex-ante** (trước kỳ đầu tư, dựa trên tỷ lệ lạm phát kỳ vọng $\pi^e$) giữa Lãi suất Danh nghĩa ($r_{nominal}$), Lãi suất Thực kỳ vọng ($r_{real}$) và Lạm phát Kỳ vọng ($\pi^e$):

$$1 + r_{nominal} = (1 + r_{real})(1 + \pi^e)$$

Khi tính toán **sau kỳ đầu tư (ex-post)** với tỷ lệ lạm phát thực tế $\pi$ đo lường qua CPI:

1. **Công thức xấp xỉ tuyến tính (Linear Approximation):**
   $$r_{real} \approx r_{nominal} - \pi$$

2. **Công thức chính xác (Exact Ex-post Real Return):**
   $$1 + r_{real} = \frac{1 + r_{nominal}}{1 + \pi} \implies r_{real} = \frac{1 + r_{nominal}}{1 + \pi} - 1$$

* **Lưu ý:** Công thức xấp xỉ $r_{nominal} - \pi$ thường được dùng cho các phép tính nhanh khi lạm phát thấp. Khi tỷ lệ lạm phát cao, cần áp dụng công thức chính xác để tránh sai lệch đáng kể.

---

## 4. Ví dụ trực quan

Hãy xét một nền kinh tế giả định đơn giản với rổ CPI gồm 3 nhóm mặt hàng cơ bản được theo dõi trong 2 năm ($t_0$ và $t_1$):

| Nhóm hàng hóa | Lượng tiêu dùng kỳ gốc ($Q_0$) | Giá năm $t_0$ ($P_0$) | Giá năm $t_1$ ($P_1$) | Chi phí kỳ gốc ($P_0 \cdot Q_0$) | Chi phí kỳ $t_1$ ($P_1 \cdot Q_0$) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Gạo & Thực phẩm** | 100 kg | 20.000 VNĐ | 24.000 VNĐ | 2.000.000 VNĐ | 2.400.000 VNĐ |
| **Xăng dầu (Năng lượng)** | 50 lít | 22.000 VNĐ | 27.500 VNĐ | 1.100.000 VNĐ | 1.375.000 VNĐ |
| **Dịch vụ giáo dục & y tế**| 10 đơn vị | 100.000 VNĐ | 105.000 VNĐ | 1.000.000 VNĐ | 1.050.000 VNĐ |
| **TỔNG CỘNG** | - | - | - | **4.100.000 VNĐ** | **4.825.000 VNĐ** |

### Các bước tính toán:

1. **Tính CPI năm $t_0$ (Kỳ gốc):**
   $$\text{CPI}_0 = \frac{4.100.000}{4.100.000} \times 100 = 100$$

2. **Tính CPI năm $t_1$:**
   $$\text{CPI}_1 = \frac{4.825.000}{4.100.000} \times 100 = 117,68$$

3. **Tính Tỷ lệ Lạm phát năm $t_1$ ($\pi_1$):**
   $$\pi_1 = \frac{117,68 - 100}{100} \times 100\% = 17,68\%$$

4. **Phân tích Lợi suất Thực tế (Ex-post Real Return):**
   * Giả sử đầu năm $t_0$, bạn gửi 10.000.000 VNĐ vào ngân hàng với lãi suất danh nghĩa $r_{nominal} = 7\%$/năm.
   * Đến năm $t_1$, bạn nhận được cả gốc và lãi là $10.700.000$ VNĐ.
   * **Nếu tính theo công thức xấp xỉ:** 
     $$r_{real} \approx 7\% - 17,68\% = -10,68\%$$
   * **Nếu tính theo công thức chính xác (Exact Ex-post Real Return):**
     $$1 + r_{real} = \frac{1 + 0,07}{1 + 0,1768} = \frac{1,07}{1,1768} \approx 0,909245 \implies r_{real} \approx -9,08\%$$
   * **Kết luận:** Mặc dù số tiền danh nghĩa tăng 700.000 VNĐ, sức mua thực tế của khoản tiền gửi đã giảm khoảng **9.08%** (thay vì mức xấp xỉ -10.68%). Ví dụ này minh họa tầm quan trọng của việc phân biệt giữa mức xấp xỉ tuyến tính và kết quả chính xác khi lạm phát ở mức cao.

---

## 5. Tình huống thực tế

### Tình huống phân tích

> **Câu hỏi:** *"Giai đoạn 2020–2021, US Fed thực hiện nới lỏng định lượng (QE), bơm lượng lớn tiền cơ sở (MB) vào hệ thống ngân hàng. Tại sao trong năm 2020 lạm phát CPI ở Mỹ vẫn ở mức thấp (dưới 1.5%), nhưng đến tháng 6/2022, lạm phát CPI lại đạt đỉnh tới 9.1% YoY (mức cao nhất trong 40 năm) trước khi hạ nhiệt trong năm 2023?"*

### Phân tích chi tiết chuỗi truyền dẫn:

1. `[Causal Mechanism]` **Giai đoạn 2020 - Đầu 2021: Tăng trưởng Tiền cơ sở ($MB$) chưa lan nhanh sang Cầu tiêu dùng**
   * Các chương trình QE làm tăng tiền cơ sở $MB$ (dưới dạng dự trữ của ngân hàng thương mại gửi tại Fed). Tuy nhiên, lượng dự trữ này không lập tức biến thành sự bùng nổ tín dụng hay tiền gửi tiêu dùng ($M1/M2$) do dịch bệnh gây gián đoạn hoạt động kinh doanh.
   * Tốc độ lưu thông tiền $V$ giảm mạnh do tâm lý thận trọng của hộ gia đình và doanh nghiệp. Trong môi trường lãi suất thấp, dòng thanh khoản dễ tiếp cận giá tài sản (như chứng khoán và bất động sản) có xu hướng phản ứng sớm hơn CPI tiêu dùng.

2. `[Causal Mechanism]` **Giai đoạn 2021 - 2023: Sự tổng hòa giữa Cầu kéo, Chi phí đẩy và Cắt giảm nới lỏng**
   * **Tài khóa & Tổng cầu:** Các gói hỗ trợ tài khóa trực tiếp thúc đẩy sức mua của hộ gia đình, kết hợp với nhu cầu dồn nén khi mở cửa trở lại (*reopening*) làm tổng cầu tiêu dùng tăng nhanh.
   * **Nguồn cung & Địa chính trị:** Đứt gãy chuỗi cung ứng toàn cầu cùng với căng thẳng địa chính trị đẩy giá năng lượng và lương thực tăng vọt (chi phí đẩy).
   * **Diễn biến số liệu & Phản ứng chính sách:** CPI Mỹ đạt đỉnh **9.1% YoY vào tháng 6/2022**, sau đó hạ nhiệt dần trong năm 2023 khi Fed thắt chặt tiền tệ mạnh mẽ (tăng lãi suất điều hành và thu hẹp bảng cân đối kế toán) kết hợp với chuỗi cung ứng dần phục hồi.

---

## 6. Kiến thức này có ích gì với tôi?

### 1. Đọc và giải mã tin tức kinh tế chính xác
* Nhận biết CPI là chỉ số giá, còn tỷ lệ % thay đổi CPI giữa các kỳ là tỷ lệ lạm phát. Phân biệt được sự khác nhau giữa biến động ngắn hạn của giá năng lượng/thực phẩm (lạm phát tổng thể) và áp lực tăng giá dài hạn (lạm phát cơ bản).

### 2. Định hình tư duy quản trị tài sản cá nhân
* **Phân biệt Lãi suất thực Ex-ante vs Ex-post:** Đánh giá rủi ro lạm phát kỳ vọng trước khi gửi tiết kiệm hay đầu tư, và hiểu sự khác biệt giữa công thức xấp xỉ và công thức chính xác khi lạm phát cao.
* **Tư duy về tài sản bảo vệ sức mua (Inflation Hedge):** Trong một số bối cảnh lạm phát cao kéo dài, các tài sản thực hoặc cổ phiếu của những doanh nghiệp có sức mạnh ấn định giá (*pricing power*) có thể có khả năng bảo hộ sức mua tốt hơn việc nắm giữ tiền mặt cố định, dù vẫn chịu các rủi ro biến động giá riêng. Đây là nguyên lý tư duy vĩ mô, không phải lời khuyên đầu tư cụ thể.

### 3. Hiểu hành vi điều hành của Ngân hàng Trung ương
* Nhận diện lạm phát cơ bản là một chỉ báo quan trọng (bên cạnh tăng trưởng, việc làm và tỷ giá) để Ngân hàng Trung ương hoạch định lãi suất điều hành và thanh khoản thị trường.

---

## 7. Thuật ngữ

* **Lạm phát (Inflation):** Sự gia tăng liên tục và kéo dài của mức giá chung trong nền kinh tế theo thời gian, làm suy giảm sức mua của đồng tiền.
* **Chỉ số Giá tiêu dùng (Consumer Price Index - CPI):** Chỉ số giá đo lường mức giá trung bình của một rổ hàng hóa và dịch vụ tiêu dùng đại diện cho hộ gia đình. Tỷ lệ % thay đổi của CPI giữa các kỳ được dùng để đo tỷ lệ lạm phát.
* **Lạm phát Tổng thể (Headline Inflation):** Tỷ lệ lạm phát tính toán trên toàn bộ danh mục rổ CPI (bao gồm cả thực phẩm và năng lượng).
* **Lạm phát Cơ bản (Core Inflation):** Chỉ báo lạm phát nền tảng đã loại bỏ một số nhóm mặt hàng biến động ngắn hạn mạnh (như thực phẩm, năng lượng, hoặc hàng hóa do Nhà nước quản lý giá).
* **Lạm phát Cầu kéo (Demand-Pull Inflation):** Lạm phát phát sinh khi tổng cầu trong nền kinh tế vượt quá khả năng cung ứng hàng hóa dịch vụ.
* **Lạm phát Chi phí đẩy (Cost-Push Inflation):** Lạm phát phát sinh khi chi phí sản xuất đầu vào (nguyên vật liệu, tiền lương, vận tải) tăng cao, buộc doanh nghiệp nâng giá bán.
* **Lợi suất Thực (Real Return):** Tỷ lệ tăng trưởng sức mua thực tế của một khoản đầu tư sau khi đã trừ đi lạm phát. Phân biệt *ex-ante real return* (dựa trên lạm phát kỳ vọng $\pi^e$) và *ex-post real return* (dựa trên lạm phát thực tế $\pi$).
* **Tốc độ lưu thông tiền (Money Velocity - $V$):** Số lần trung bình một đơn vị tiền tệ chuyển tay để thực hiện giao dịch hàng hóa/dịch vụ cuối cùng trong một thời kỳ.

---

## 8. Tin tức và tính cập nhật

`[Current Fact]` **Bối cảnh đo lường và Quy định tại Việt Nam (năm 2026):**

1. **Cơ quan công bố dữ liệu:** 
   Tại Việt Nam, **Cục Thống kê (Bộ Tài chính)** – cơ quan thống kê quốc gia – thực hiện thu thập, tính toán và công bố Chỉ số giá tiêu dùng (CPI) định kỳ hàng tháng, hàng quý và hàng năm.

2. **Cấu trúc rổ hàng hóa CPI Việt Nam:**
   * Rổ hàng hóa tính CPI tại Việt Nam hiện gồm 11 nhóm hàng hóa và dịch vụ chính.
   * Trong **kỳ quyền số hiện hành**, nhóm **"Hàng ăn và dịch vụ ăn uống"** chiếm trọng số lớn nhất (khoảng **33.56%** tổng rổ CPI). Trọng số này được cơ quan thống kê cập nhật định kỳ dựa trên kết quả khảo sát mức sống hộ gia đình.
   * Nhóm **"Giao thông"** (chiếm khoảng **9.67%**) chịu ảnh hưởng trực tiếp từ biến động của giá xăng dầu thế giới và trong nước.

3. **Mục tiêu Kiểm soát Lạm phát:**
   Hàng năm, Quốc hội Việt Nam đề ra mục tiêu kiểm soát lạm phát CPI (thường ở mức khoảng 4.0% – 4.5%). Ngân hàng Nhà nước Việt Nam (SBV) phối hợp các công cụ chính sách tiền tệ (lãi suất điều hành, nghiệp vụ thị trường mở OMO, tỷ lệ dự trữ bắt buộc) để đạt mục tiêu vĩ mô này.

---

## 9. Nguồn tham khảo và độ tin cậy

1. **Cục Thống kê (Bộ Tài chính):** Phương pháp điều tra và tính toán chỉ số giá tiêu dùng tại Việt Nam (*gso.gov.vn / mof.gov.vn*).
2. **Ngân hàng Nhà nước Việt Nam (SBV):** Báo cáo thường niên và Định hướng Điều hành Chính sách Tiền tệ (*sbv.gov.vn*).
3. **Frederic S. Mishkin:** *The Economics of Money, Banking and Financial Markets* (13th Edition) – Chương về Money Supply and Inflation.
4. **International Monetary Fund (IMF):** *Consumer Price Index Manual: Concepts and Methods* (2020).

---

## 10. Liên kết kiến thức

### 🔗 Bài học đã qua:
* [`MONEY-001`](topics/monetary-and-banking/money-supply-and-bank-money-creation.md): Cung tiền M1, M2 và Cơ chế Tạo tiền của Ngân hàng Thương mại (Hiểu cách cung tiền được tạo ra trước khi tìm hiểu cách cung tiền tác động đến mức giá $P$).

### 💡 Khái niệm gợi mở cho bài học tiếp theo (RELATE.md):
* **Lãi suất điều hành & Kênh truyền dẫn chính sách tiền tệ:** NHTW dùng công cụ gì để kiềm chế khi lạm phát vượt mục tiêu?
* **Hiệu ứng Fisher & Đường cong Lãi suất (Yield Curve):** Lạm phát kỳ vọng làm thay đổi lãi suất trái phiếu và giá tài sản như thế nào?
* **Lạm phát chi phí đẩy và Hiện tượng Đình lạm (Stagflation):** Điều gì xảy ra khi nền kinh tế vừa bị lạm phát cao vừa bị suy thoái/thất nghiệp?
