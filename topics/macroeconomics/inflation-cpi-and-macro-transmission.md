---
id: MACRO-001
title: "Lạm phát: Bản chất, Phương pháp Đo lường CPI và Các Kênh Truyền dẫn Vĩ mô"
category: macroeconomics
tags: [cpi, inflation, money-supply, purchasing-power, macroeconomics]
prerequisites: [MONEY-001]
difficulty: Fundamental
date: 2026-08-13
applicable_year: 2026
last_verified: 2026-09-22
---

# Lạm phát, CPI và các kênh truyền dẫn vĩ mô

## 1. Chủ đề hôm nay

**Lạm phát (Inflation)**, **chỉ số giá tiêu dùng (Consumer Price Index – CPI)** và **lợi suất thực (Real return)**.

## 2. Vấn đề cốt lõi

Giả sử CPI tăng 3,5% nhưng chi tiêu của gia đình tăng 10%: hai con số có nhất thiết mâu thuẫn không? Vì sao cung tiền tăng không cho phép dự báo ngay một tỷ lệ lạm phát? Và gửi tiết kiệm có lãi danh nghĩa có bảo đảm sức mua tăng không?

Cần tách **mức giá**, **tốc độ tăng giá**, **số lượng/chất lượng hàng mua** và **sức mua của khoản tiền**.

## 3. Giải thích cơ chế

### 3.1. Định nghĩa và những khác biệt dễ nhầm

[Definition] Lạm phát là mức tăng của mặt bằng giá chung trong một khoảng thời gian. Một mặt hàng tăng giá chưa đủ đại diện cho toàn bộ mặt bằng giá.

**Giảm lạm phát (disinflation)** là tốc độ tăng giá chậm lại; **giảm phát (deflation)** là mặt bằng giá giảm. Giả sử chỉ số giá từ 100 lên 110 rồi lên 115,5: lạm phát giảm từ 10% xuống 5%, nhưng giá vẫn cao hơn trước.

[Definition] CPI là chỉ số theo dõi biến động giá một rổ tiêu dùng đại diện. CPI bằng 110 không có nghĩa “lạm phát 110%”. Phải xác định kỳ gốc hoặc kỳ so sánh. [IMF và các tổ chức thống kê quốc tế, CPI Manual: Concepts and Methods, 2020](https://www.imf.org/en/data/statistics/cpi-manual).

### 3.2. TEXTBOOK MODEL – rổ hàng cố định

[Theoretical Model] Mô hình Laspeyres giữ nguyên lượng hàng kỳ gốc:

$$CPI_t = \frac{\sum_i P_{i,t}Q_{i,0}}{\sum_i P_{i,0}Q_{i,0}}\times100$$

P là giá, Q là lượng; tổng ở tử số là chi phí mua **cùng một rổ** theo giá mới. Trọng số phản ánh tỷ trọng chi tiêu ở kỳ gốc, không phải mọi mặt hàng đều quan trọng như nhau.

[Definition] Tỷ lệ thay đổi CPI:

$$\pi_{t,s}=\left(\frac{CPI_t}{CPI_s}-1\right)\times100\%$$

- So tháng trước: s là tháng liền trước.
- So cùng kỳ (YoY): s là cùng tháng năm trước.
- Bình quân năm: so trung bình các mức CPI tháng của năm này với năm trước trên chuỗi tương thích; không lấy riêng tháng 12 đại diện cả năm.

Mô hình giúp hiểu quyền số và kỳ so sánh. Nó không bao quát toàn bộ cách thu thập và tổng hợp CPI chính thức.

### 3.3. REAL-WORLD MECHANISM – đo giá không đơn giản là cộng hóa đơn

Cơ quan thống kê phải xử lý thay đổi chất lượng, sản phẩm biến mất, hàng mới, giá khuyến mại và cập nhật quyền số. CPI thực tế có nhiều cấp tổng hợp; không phải mọi cấp đều dùng duy nhất công thức Laspeyres đơn giản ở trên. CPI cũng không trùng hoàn toàn với chi phí duy trì một mức sống hoặc trải nghiệm của từng hộ. [IMF, CPI Manual 2020, chương 1](https://www.elibrary.imf.org/display/book/9781484354841/ch01.xml).

[Causal Mechanism] Hộ dành phần lớn ngân sách cho thực phẩm chịu tác động mạnh hơn khi thực phẩm tăng giá. Hộ vừa đổi sang căn nhà lớn hơn có chi tiêu tăng do cả **giá lẫn lượng/chất lượng**, nên mức tăng hóa đơn không phải phép đo lạm phát riêng thuần túy.

| Chỉ tiêu | Diễn giải đúng |
| :--- | :--- |
| Lạm phát tổng thể (Headline inflation) | Biến động CPI toàn rổ theo kỳ so sánh đã nêu. |
| Lạm phát cơ bản (Core inflation) | Chỉ báo lọc một số biến động nhằm xem xu hướng nền; danh mục loại trừ tùy cơ quan và phương pháp. |
| Lạm phát riêng của hộ | Ước lượng theo cơ cấu tiêu dùng hộ; cần giữ cách đo giá và lượng nhất quán. |

Lạm phát cơ bản không phải “lạm phát thật”, không bảo đảm luôn thấp hơn tổng thể và không có nghĩa khoản chi bị loại trừ là không quan trọng.

### 3.4. Tiền và giá: đồng nhất thức khác mô hình nhân quả

[Accounting Identity] Với Y là GDP thực, P là **chỉ số giảm phát GDP được chuẩn hóa phù hợp**, PY là GDP danh nghĩa. Định nghĩa tốc độ lưu thông thu nhập $V=PY/M$ cho ta:

$$MV=PY$$

M là chỉ tiêu tiền tệ lựa chọn và V tương ứng; **không thay P bằng CPI rồi mặc định đẳng thức vẫn đúng với GDP**. CPI đo giá tiêu dùng, còn giảm phát GDP đo giá sản lượng trong nước. [Federal Reserve Bank of St. Louis, The velocity of money, 2015](https://fredblog.stlouisfed.org/2015/01/the-velocity-of-money/).

[Theoretical Model] Nếu giả định M được thay đổi ngoại sinh, V không đổi và Y không đổi, thì P tỷ lệ thuận với M. Đây là mô hình số lượng tiền với ràng buộc cụ thể, không phải mô tả mặc định ngắn hạn.

Dạng tăng trưởng chính xác:

$$1+g_P = \frac{(1+g_M)(1+g_V)}{1+g_Y}$$

Khi các tốc độ đủ nhỏ: $g_P \approx g_M+g_V-g_Y$. Các tốc độ viết dạng thập phân, cùng kỳ đo.

Ví dụ tự xây dựng: M tăng 10%, V giảm 5%, Y tăng 3% thì:

$$g_P=\frac{1{,}10\times0{,}95}{1{,}03}-1\approx1{,}46\%$$

Đây là phép tính theo giả định, **không phải dự báo CPI**. Hơn nữa, V tính bằng PY/M không phải một nguyên nhân độc lập có thể quan sát mà không cần xét hành vi; tiền, chi tiêu và chính sách cùng phản ứng với điều kiện kinh tế.

### 3.5. Từ chính sách đến chi tiêu và giá

[Causal Mechanism] Điều kiện vay thuận lợi hơn có thể làm doanh nghiệp đầu tư, hộ mua hàng lâu bền và người giữ tài sản điều chỉnh danh mục. Nếu tổng chi tiêu tăng nhanh hơn khả năng đáp ứng, doanh nghiệp có thể tăng giá. Nếu còn năng lực nhàn rỗi, sản lượng có thể tăng trước hoặc cùng với giá.

Phải phân biệt các giao dịch:

- NHTW mua tài sản **từ ngân hàng**: dự trữ tăng, chưa tự tăng tiền gửi công chúng.
- NHTW mua **từ chủ thể phi ngân hàng đủ điều kiện thống kê**: tiền gửi người bán và dự trữ ngân hàng có thể cùng tăng ngay, dù chưa có khoản vay mới.
- Tiền gửi tăng không buộc chủ sở hữu chi tiêu ngay; họ có thể giữ tiền hoặc trả nợ.

Vì vậy, không được nói “QE chỉ tăng M2 khi ngân hàng cho vay”. Bút toán đã phân tích ở [MONEY-001](../monetary-and-banking/money-supply-and-bank-money-creation.md); đối chiếu [Bank of England, QE: functioning and effectiveness, 2022](https://www.bankofengland.co.uk/quarterly-bulletin/2022/2022-q1/qe-at-the-bank-of-england-a-perspective-on-its-functioning-and-effectiveness).

[Causal Mechanism] Các lực tác động khác gồm:

1. **Cầu kéo:** chi tiêu tăng so với năng lực cung ứng, tạo áp lực tăng giá.
2. **Chi phí đẩy:** năng lượng, đầu vào hoặc tỷ giá làm chi phí tăng; mức chuyển vào giá bán còn phụ thuộc cạnh tranh, biên lợi nhuận và sức mua.
3. **Kỳ vọng:** dự báo giá/lương tương lai ảnh hưởng đàm phán và định giá hôm nay. Vòng xoáy lương–giá là khả năng có điều kiện, không phải mọi tăng lương đều tạo vòng xoáy.

Giá tài sản có thể phản ứng nhanh qua kỳ vọng và chiết khấu; không có thứ tự bắt buộc “tiền vào chứng khoán trước, rồi mới vào CPI”. Giao dịch mua cổ phiếu cũ thường chuyển tiền giữa người mua và người bán, không làm tiền biến mất khỏi nền kinh tế.

### 3.6. Lợi suất thực: chính xác sau kỳ, xấp xỉ trước kỳ

[Accounting Identity] Với lợi suất danh nghĩa i và lạm phát thực tế π **cùng khoảng thời gian**, sức mua sau kỳ thay đổi:

$$r_{\text{thực, ex-post}} = \frac{1+i}{1+\pi}-1$$

Đây là phép chia mức tăng tiền cho mức tăng giá. Thuế và phí cần trừ trong i nếu muốn tính sức mua ròng.

[Theoretical Model] Trước kỳ, cách ước lượng thường dùng là:

$$r_{\text{thực, ex-ante}}\approx i-E(\pi)$$

Không coi $1+i=(1+r)(1+E\pi)$ là đồng nhất thức kỳ vọng tổng quát khi lạm phát bất định. Với i cố định, kỳ vọng chính xác là $E[(1+i)/(1+\pi)]-1$, nhìn chung khác $(1+i)/(1+E\pi)-1$. Nếu phân tích hình thành lãi suất thị trường còn cần xét phần bù rủi ro lạm phát, thanh khoản và kỳ hạn.

Với lạm phát dương, công thức xấp xỉ $i-\pi$ phóng đại **độ lớn** của lợi suất thực so với phép chia chính xác: phóng đại khoản lỗ nếu $i<\pi$, hoặc phóng đại khoản lãi nếu $i>\pi$. Không phải lúc nào nó cũng “phóng đại sụt giảm sức mua”.

## 4. Ví dụ trực quan

**Ví dụ giả định**, rổ hàng giữ nguyên trong một năm:

| Nhóm hàng | Lượng kỳ gốc | Giá đầu năm | Giá cuối năm | Chi phí đầu năm | Chi phí cuối năm |
| :--- | ---: | ---: | ---: | ---: | ---: |
| Thực phẩm | 100 kg | 20.000 | 24.000 | 2.000.000 | 2.400.000 |
| Năng lượng | 50 lít | 22.000 | 27.500 | 1.100.000 | 1.375.000 |
| Dịch vụ | 10 đơn vị | 100.000 | 105.000 | 1.000.000 | 1.050.000 |
| **Tổng (đồng)** | | | | **4.100.000** | **4.825.000** |

CPI đầu kỳ bằng 100; cuối kỳ bằng $100\times4.825.000/4.100.000 \approx117{,}6829$. Lạm phát cả kỳ khoảng 17,6829%.

Gửi 10 triệu với lãi 7%/năm, bỏ qua thuế/phí, cuối kỳ có 10,7 triệu. Sức mua tính theo rổ đầu kỳ:

$$\frac{10{,}7}{4{,}825/4{,}1}\approx9{,}0922\ \text{triệu đồng}$$

$$r_{\text{thực}}=\frac{1{,}07}{4{,}825/4{,}1}-1\approx-9{,}08\%$$

Phép xấp xỉ cho $7\%-17{,}6829\%\approx-10{,}68\%$. Dùng tỷ lệ chưa làm tròn khi tính, chỉ làm tròn kết quả cuối.

## 5. Tình huống thực tế: lạm phát Mỹ trong đại dịch

[Historical Claim] CPI-U Mỹ tháng 6/2022 tăng **9,1% so cùng kỳ**, chưa điều chỉnh mùa vụ; đây là biến động 12 tháng, không phải bình quân cả năm. [BLS, công bố ngày 13/07/2022](https://www.bls.gov/news.release/archives/cpi_07132022.htm).

[Causal Mechanism / diễn giải có nguồn] Trong bài phát biểu ngày 23/08/2024, Chủ tịch Fed Jerome Powell giải thích giai đoạn này bằng sự kết hợp của cầu phục hồi mạnh và lệch sang hàng hóa, cung bị hạn chế, thị trường lao động và giá nguyên liệu. Việc áp lực giá giảm sau đó liên quan cả phục hồi nguồn cung, điều tiết tổng cầu và kỳ vọng. Đây là cách diễn giải của người phát biểu, không phải phép phân rã duy nhất được mọi nghiên cứu thống nhất. [Fed, Review and Outlook](https://www.federalreserve.gov/newsevents/speech/powell20240823a.htm).

Không thể nhìn hai đường M2 và CPI rồi suy ra toàn bộ lạm phát do QE, hoặc gán độ trễ cố định. Cần tách kế toán tạo tiền gửi khỏi quyết định chi tiêu và khả năng sản xuất hàng hóa.

## 6. Kiến thức này có ích gì với tôi?

- **Đọc tin:** xác định chỉ số, kỳ so sánh, điều chỉnh mùa vụ và phạm vi địa lý trước khi so hai con số.
- **Đánh giá khoản tiết kiệm:** dùng lạm phát kỳ vọng cho kế hoạch, lạm phát thực tế để đánh giá sau kỳ; thu nhập danh nghĩa tăng chưa chắc sức mua tăng.
- **Hiểu hành vi:** doanh nghiệp có thể hấp thụ chi phí bằng giảm biên lợi nhuận thay vì tăng toàn bộ vào giá; người lao động đòi tăng lương không có nghĩa lạm phát tất yếu tăng tương ứng.
- **Tránh kết luận đầu tư máy móc:** một tài sản có khả năng tăng dòng tiền theo giá chung vẫn có thể giảm giá vì lãi suất, rủi ro hoặc mức giá mua ban đầu.

## 7. Thuật ngữ

- **CPI:** chỉ số giá tiêu dùng; phân biệt mức chỉ số với tỷ lệ thay đổi.
- **Headline/Core inflation:** tổng thể/cơ bản; phạm vi loại trừ phải theo phương pháp công bố.
- **GDP deflator:** chỉ số giảm phát GDP; không phải CPI.
- **Money velocity:** trong bài là GDP danh nghĩa chia chỉ tiêu tiền tệ tương ứng.
- **Ex-ante / Ex-post:** dự kiến trước kỳ / quan sát sau kỳ.
- **Disinflation / Deflation:** lạm phát chậm lại / mặt bằng giá giảm.

## 8. Phạm vi Việt Nam và tính cập nhật

[Current Fact – đối chiếu 22/09/2026] Tên cơ quan hiện dùng là **Cục Thống kê, Bộ Tài chính**. Quyết định 384/QĐ-BTC ngày 26/02/2025 và những thay đổi tổ chức sau đó được cơ quan ghi nhận trong [Lịch sử phát triển](https://www.nso.gov.vn/gioi-thieu/lich-su-phat-trien/). Không dùng tên “Tổng cục Thống kê thuộc Bộ Kế hoạch và Đầu tư” như hiện trạng năm 2026.

[Historical Claim] Tài liệu phương pháp do cơ quan thống kê đăng năm 2025 mô tả **752 mặt hàng cho giai đoạn 2020–2025** và việc chuyển năm gốc từ 2019 sang 2024. Vì vậy, số mặt hàng và quyền số cũ không được mặc định là rổ hiện hành năm 2026. [Cục Thống kê, Chỉ số giá tiêu dùng và phương pháp đo lường tại Việt Nam, 2025](https://www.nso.gov.vn/default/2025/11/chi-so-gia-tieu-dung-va-phuong-phap-do-luong-tai-viet-nam/).

[Current Fact – phạm vi công bố tháng 02/2026] Chú thích lạm phát cơ bản trong báo cáo giá của Cục Thống kê loại trừ lương thực, thực phẩm tươi sống, năng lượng và mặt hàng Nhà nước quản lý gồm dịch vụ y tế, giáo dục. [Báo cáo CPI tháng 02/2026, chú thích 2](https://www.nso.gov.vn/wp-content/uploads/2026/03/Tong-quan-CPI-thang-02-nam-2026-1.pdf). Đợt kiểm tra đọc được chú thích qua chỉ mục tìm kiếm của PDF chính thức; công cụ mở toàn văn gặp lỗi, nên không dùng nguồn này để xác nhận thêm số liệu ngoài chú thích.

Bài không khẳng định số mặt hàng, bộ quyền số đầy đủ hoặc mục tiêu CPI cả năm 2026 khi chưa có văn bản tương ứng được đối chiếu. Phần cơ chế vẫn sử dụng được độc lập với những số liệu cập nhật đó.

## 9. Nguồn tham khảo

Năm nguồn trọng tâm; nguồn cho dữ kiện bổ sung đã đặt tại đoạn liên quan:

1. **IMF và các tổ chức thống kê quốc tế (2020)**, [Consumer Price Index Manual: Concepts and Methods](https://www.imf.org/en/data/statistics/cpi-manual).
2. **Federal Reserve Bank of St. Louis (2015)**, [The velocity of money](https://fredblog.stlouisfed.org/2015/01/the-velocity-of-money/).
3. **BLS (13/07/2022)**, [Consumer Price Index – June 2022](https://www.bls.gov/news.release/archives/cpi_07132022.htm).
4. **Jerome H. Powell – Federal Reserve (23/08/2024)**, [Review and Outlook](https://www.federalreserve.gov/newsevents/speech/powell20240823a.htm).
5. **Cục Thống kê (2025)**, [Chỉ số giá tiêu dùng và phương pháp đo lường tại Việt Nam](https://www.nso.gov.vn/default/2025/11/chi-so-gia-tieu-dung-va-phuong-phap-do-luong-tai-viet-nam/).

## Liên kết kiến thức

- [MONEY-001](../monetary-and-banking/money-supply-and-bank-money-creation.md): tạo tiền gửi và phân biệt tiền cơ sở (✅ Đã học).
- [MONEY-002](../monetary-and-banking/policy-rates-and-monetary-transmission.md): lãi suất và truyền dẫn tiền tệ (✅ Đã học).
- **Hiệu ứng Fisher và đường cong lợi suất:** từ kỳ vọng lạm phát đến lãi suất thị trường (⏳ Chưa học riêng).
- **Đình lạm (Stagflation):** giá tăng trong bối cảnh hoạt động kinh tế yếu (⏳ Chưa học riêng).

## Điều đáng nhớ nhất

1. CPI là chỉ số; lạm phát là tỷ lệ thay đổi theo kỳ xác định. Chi tiêu riêng còn bị ảnh hưởng bởi lượng hàng và cơ cấu mua sắm.
2. MV = PY không tự chứng minh M gây ra CPI, và P trong đồng nhất thức GDP không phải CPI.
3. Lợi suất thực sau kỳ tính bằng phép chia mức tăng tiền cho mức tăng giá; kỳ vọng trước kỳ không phải kết quả chắc chắn.

## Góc Phản xạ & Active Recall (Dành cho bạn)

Nếu lạm phát giảm từ 10% xuống 5%, tại sao gia đình vẫn có thể phải chi nhiều hơn để mua cùng rổ hàng?

**Thang tự đánh giá (1–5):** 1 = cần đọc lại sớm; 3 = nắm vững; 5 = giải thích được CPI, đồng nhất thức tiền tệ và lợi suất thực.
