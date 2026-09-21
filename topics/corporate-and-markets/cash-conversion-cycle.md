---
id: CORP-001
title: "Chu kỳ chuyển đổi tiền mặt (Cash Conversion Cycle - CCC) & Quản trị Rủi ro Thanh khoản"
category: corporate-and-markets
tags: [cash-conversion-cycle, liquidity, working-capital, ocf, cash-flow]
prerequisites: []
difficulty: Intermediate
date: 2026-08-04
last_verified: 2026-09-22
---

# Chu kỳ chuyển đổi tiền mặt & Quản trị rủi ro thanh khoản

## 1. Chủ đề hôm nay

**Chu kỳ chuyển đổi tiền mặt (Cash Conversion Cycle – CCC):** vì sao doanh nghiệp có lãi vẫn có thể thiếu tiền trả nợ?

## 2. Vấn đề cốt lõi

Bán hàng, ghi nhận lợi nhuận và thu tiền là những thời điểm có thể khác nhau. Trong khi chờ khách hàng trả tiền, doanh nghiệp vẫn phải thanh toán nhà cung cấp, lương và các khoản nợ đến hạn. Bài học nối ba thứ: thời gian thu hồi tiền, số vốn nằm trong hoạt động và lịch thanh toán thực tế.

## 3. Giải thích cơ chế

### 3.1. Lợi nhuận khác tiền mặt

[Definition] **Kế toán dồn tích (Accrual accounting)** ghi nhận doanh thu và chi phí khi đáp ứng điều kiện ghi nhận, không đơn thuần khi thu hoặc chi tiền. Không phải cứ xuất hóa đơn hoặc khách hàng hứa thanh toán là đương nhiên đủ điều kiện ghi nhận doanh thu.

Ví dụ giả định: doanh nghiệp giao hàng và đủ điều kiện ghi nhận doanh thu 100 triệu, giá vốn 70 triệu; người mua chưa trả tiền. Lãi gộp là 30 triệu nhưng tiền thu từ giao dịch lúc này bằng 0. Nếu doanh nghiệp đã trả nhà cung cấp 70 triệu, dòng tiền của giao dịch đến thời điểm đó là âm 70 triệu.

Dòng tiền từ hoạt động kinh doanh phải điều chỉnh các khoản dồn tích và phi tiền mặt; nó không thể suy ra chỉ từ lợi nhuận. [IFRS Foundation, IAS 7, mục tổng quan](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/).

### 3.2. TEXTBOOK MODEL – CCC đo thời gian, không trực tiếp đo số tiền

[Definition] Với dữ liệu một năm và giả định hoạt động đủ ổn định để dùng số dư bình quân:

$$CCC = DIO + DSO - DPO$$

$$DIO = \frac{\text{Tồn kho bình quân}}{\text{Giá vốn hàng bán năm}} \times 365$$

$$DSO = \frac{\text{Phải thu thương mại bình quân}}{\text{Doanh thu bán chịu năm}} \times 365$$

$$DPO = \frac{\text{Phải trả nhà cung cấp bình quân}}{\text{Giá trị mua chịu năm}} \times 365$$

- **DIO (Days Inventory Outstanding):** thời gian vốn nằm trong tồn kho.
- **DSO (Days Sales Outstanding):** thời gian chờ thu tiền bán chịu.
- **DPO (Days Payable Outstanding):** thời gian được nhà cung cấp cho trả chậm.

Trong thực hành, có thể dùng doanh thu thuần thay doanh thu bán chịu và COGS thay mua chịu khi thiếu số liệu; đó là **phép xấp xỉ**, phải nêu rõ. Đặc biệt, mua hàng khác giá vốn khi tồn kho biến động. Dữ liệu theo quý cần số ngày của quý và mẫu số cùng kỳ. [ACCA, Working capital management, mục Liquidity ratios và Cash operating cycle](https://www.accaglobal.com/gb/en/student/exam-support-resources/fundamentals-exams-study-resources/f9/technical-articles/wcm.html).

[Theoretical Model] Với một lô hàng giả định:

    Ngày 0: nhập hàng → Ngày 30: trả nhà cung cấp
                      → Ngày 60: bán hàng → Ngày 90: thu tiền

Ở đây DIO = 60, DSO = 30, DPO = 30 nên CCC = 60 ngày. Khoảng cần tài trợ bắt đầu **từ ngày 30 đến ngày 90**, không phải từ lúc nhập hàng.

Mô hình cho thấy thời gian thu tiền có thể dài hơn thời gian được hoãn trả. Nó không mô tả hết thuế, lương, đầu tư máy móc, vay đến hạn, mùa vụ hoặc các khoản khách hàng ứng trước.

### 3.3. Từ ngày sang số tiền: phải giữ đúng cơ sở đo lường

[Accounting Identity] Phân biệt:

$$NWC = \text{Tài sản ngắn hạn} - \text{Nợ ngắn hạn}$$

với vốn lưu động hoạt động đơn giản hóa:

$$W = \text{Tồn kho} + \text{Phải thu thương mại} - \text{Phải trả nhà cung cấp}$$

NWC có thể gồm tiền mặt và nợ vay ngắn hạn; W ở đây chỉ gồm ba khoản hoạt động. Không được dùng hai đại lượng thay nhau trong công thức dòng tiền.

Từ định nghĩa các chỉ số trên, số dư bình quân thỏa:

$$W =
\frac{COGS}{365}DIO
+\frac{\text{Doanh thu bán chịu}}{365}DSO
-\frac{\text{Mua chịu}}{365}DPO$$

Do ba mẫu số khác nhau, **COGS/ngày × CCC không phải công thức tổng quát cho W**. Ngay cả W cũng không phải hạn mức vay cần có: kế hoạch tiền mặt còn phụ thuộc ngày thu/chi, vốn chủ, lợi nhuận giữ lại, thuế và những nghĩa vụ khác.

### 3.4. Dòng tiền hoạt động và vốn lưu động

[Theoretical Model] Nếu giả định chỉ có khấu hao là khoản phi tiền mặt, W bao quát toàn bộ khoản dồn tích hoạt động và không có điều chỉnh phân loại khác:

$$OCF = \text{Lợi nhuận ròng} + \text{Khấu hao} - \Delta W$$

Đây là **mô hình rút gọn**, không phải công thức đầy đủ áp dụng cho mọi báo cáo. Khi đọc báo cáo thực tế, còn phải đối chiếu dự phòng, lãi/lỗ thanh lý, thuế, lãi vay và cách phân loại theo chuẩn mực áp dụng. Biến động W trong mô hình là chênh lệch **cuối kỳ trừ đầu kỳ**, khác với số dư bình quân dùng trong CCC. [ACCA, Cash flow statements, phần phương pháp gián tiếp](https://www.accaglobal.com/uk/en/student/exam-support-resources/fundamentals-exams-study-resources/f3/technical-articles/cashflow-statements.html).

[Ví dụ giả định] Lợi nhuận ròng 10 tỷ, khấu hao 2 tỷ, W tăng 15 tỷ thì OCF trong mô hình bằng −3 tỷ. Lãi kế toán không ngăn được tiền bị giữ lại trong tồn kho và khoản phải thu.

### 3.5. REAL-WORLD MECHANISM – động cơ và ràng buộc

[Causal Mechanism] Doanh nghiệp muốn bán nhanh, thu sớm và trả nhà cung cấp muộn; khách hàng và nhà cung cấp lại có động cơ ngược lại. Tăng DPO chỉ có ích nếu lợi ích giữ tiền lớn hơn chi phí mất chiết khấu, phạt chậm trả hoặc đứt nguồn cung.

Ngân hàng nhìn vào dòng tiền dự kiến, tài sản bảo đảm, sức khỏe khách hàng và điều kiện hợp đồng để quyết định tài trợ. Một ngân hàng giảm hạn mức cho một doanh nghiệp không đủ để kết luận có **credit crunch** trên toàn thị trường.

[Theoretical Model] Nếu doanh thu và giá vốn cùng tăng gấp đôi, biên lợi nhuận cùng các số ngày DIO/DSO/DPO giữ nguyên, W cũng tăng gấp đôi. Kết quả này phụ thuộc giả định; doanh nghiệp thu tiền trước hoặc đàm phán được tín dụng nhà cung cấp có thể tăng trưởng mà không cần vốn theo tỷ lệ đó.

CCC âm có nghĩa doanh nghiệp thường thu tiền trước khi trả nhà cung cấp. Điều này không bảo đảm an toàn: tiền vay đến hạn, hoàn tiền cho khách hàng, đầu tư tài sản cố định hoặc bán hàng suy giảm vẫn có thể gây thiếu tiền.

## 4. Ví dụ trực quan

**Toàn bộ tên và số liệu sau là giả định**, đơn vị tỷ đồng. Công ty Nam Hà có:

| Đại lượng | Giá trị |
| :--- | ---: |
| Doanh thu năm, giả định toàn bộ là bán chịu | 120 |
| Giá vốn hàng bán | 90 |
| Mua chịu trong năm, giả định bằng giá vốn | 90 |
| Tồn kho bình quân | 22,5 |
| Phải thu thương mại bình quân | 30 |
| Phải trả nhà cung cấp bình quân | 15 |

Suy ra DIO = 91,25 ngày; DSO = 91,25 ngày; DPO ≈ 60,83 ngày và **CCC ≈ 121,67 ngày**.

Vốn nằm trong ba khoản hoạt động:

$$W = 22{,}5 + 30 - 15 = 37{,}5\ \text{tỷ đồng}$$

Nếu lấy $90/365 \times CCC$, kết quả chỉ là 30 tỷ. Chênh lệch 7,5 tỷ đến từ việc định giá khoảng chờ thu tiền theo **giá vốn**, trong khi khoản phải thu ghi theo **giá bán**. Con số 30 tỷ có thể dùng như một phép ước lượng theo cơ sở chi phí với giả định bổ sung, nhưng không được gọi là W hay số tiền bắt buộc phải vay.

Giả sử kế hoạch tiền mặt riêng của Nam Hà cho thấy công ty cần duy trì dư nợ vay bình quân 20 tỷ với lãi suất 8%/năm, chi phí lãi là 1,6 tỷ/năm. Khoản vay 20 tỷ là giả định tài trợ riêng, không suy ra tự động từ CCC.

## 5. Tình huống thực tế

**Tình huống giả định:** Một chuỗi bán lẻ có lợi nhuận tăng 50% nhưng thiếu tiền trả lương sau khi mở thêm cửa hàng.

1. Nhập thêm hàng cho cửa hàng mới khiến tồn kho bằng tiền tăng; nếu tốc độ bán chậm, DIO còn tăng từ 30 lên 45 ngày.
2. Nới điều kiện bán chịu và khách trả chậm khiến DSO tăng từ 15 lên 75 ngày.
3. Nhà cung cấp thấy rủi ro nên giảm thời gian cho nợ, DPO từ 45 xuống 20 ngày.
4. CCC tăng từ $30+15-45=0$ lên $45+75-20=100$ ngày. CCC ban đầu bằng 0 không có nghĩa mọi nhu cầu vốn hoặc chi phí tài trợ đều bằng 0.
5. Tiền thu không đủ trang trải tiền hàng, lương và nợ đến hạn; nếu không có nguồn tài trợ hoặc điều chỉnh hoạt động kịp thời, doanh nghiệp mất khả năng thanh toán.

Lợi nhuận tăng không tự gây thiếu tiền. Nguyên nhân nằm ở **lịch thu/chi, vốn bị giữ lại và khả năng tài trợ**. OCF âm cũng chưa tự chứng minh gian lận: phải xem tuổi nợ, khả năng thu hồi và lý do tích hàng.

## 6. Kiến thức này có ích gì với tôi?

- **Đọc báo cáo:** đối chiếu lợi nhuận với OCF, tồn kho, tuổi nợ phải thu và lịch trả nợ; so sánh cùng ngành và cùng mùa kinh doanh.
- **Kinh doanh nhỏ:** lập lịch tiền mặt theo tuần/tháng trước khi nhận đơn lớn. Có lãi trên đơn hàng vẫn có thể cần tiền ứng trước.
- **Tài chính cá nhân:** khoản thu đã hứa nhưng chưa nhận không thể trả hóa đơn hôm nay. Quy mô tiền dự phòng phụ thuộc chi tiêu bắt buộc, độ ổn định thu nhập và nguồn tiền có thể tiếp cận; không có một số tháng phù hợp cho tất cả.
- **Tránh hiểu lầm:** DSO tăng là tín hiệu cần điều tra, không phải bằng chứng tự đủ về doanh thu giả. Thiếu thanh khoản khác tài sản ròng âm; “phá sản” là tình trạng pháp lý, không đồng nhất với một thời điểm thiếu tiền mặt.

## 7. Thuật ngữ

| Thuật ngữ | Ý nghĩa trong bài |
| :--- | :--- |
| Chu kỳ chuyển đổi tiền mặt (CCC) | Thời gian thu tiền từ bán hàng sau khi trừ khoảng được nhà cung cấp tài trợ. |
| Vốn lưu động ròng (NWC) | Tài sản ngắn hạn trừ nợ ngắn hạn; không đồng nhất W. |
| Vốn lưu động hoạt động (Operating working capital) | Trong mô hình này là tồn kho + phải thu thương mại − phải trả nhà cung cấp. |
| Dòng tiền hoạt động (OCF) | Dòng tiền thuần từ hoạt động kinh doanh theo cách phân loại của báo cáo. |
| Tăng trưởng quá sức (Overtrading) | Quy mô hoạt động vượt khả năng tài trợ và quản trị dòng tiền. |
| Thanh khoản tài trợ (Funding liquidity) | Khả năng thu xếp tiền để thanh toán nghĩa vụ đúng hạn. |

## 8. Nguồn tham khảo

1. **ACCA**, *Working capital management* (trang không ghi năm; truy cập 22/09/2026): [CCC, tỷ số và giả định mẫu số](https://www.accaglobal.com/gb/en/student/exam-support-resources/fundamentals-exams-study-resources/f9/technical-articles/wcm.html).
2. **ACCA**, *Cash flow statements* (trang không ghi năm; truy cập 22/09/2026): [điều chỉnh lợi nhuận sang dòng tiền](https://www.accaglobal.com/uk/en/student/exam-support-resources/fundamentals-exams-study-resources/f3/technical-articles/cashflow-statements.html).
3. **IFRS Foundation**, *IAS 7 – Statement of Cash Flows* (trang tổng quan chuẩn mực; truy cập 22/09/2026): [phân loại dòng tiền và phương pháp gián tiếp](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/).

Các ví dụ là mô hình tự xây dựng để kiểm tra số học, không phải số liệu doanh nghiệp thực. Bài không hướng dẫn lập báo cáo theo một chế độ kế toán Việt Nam cụ thể.

## 9. Liên kết kiến thức

- **Báo cáo lưu chuyển tiền tệ:** đi từ lợi nhuận đến tiền thu/chi thực tế (⏳ Chưa học riêng).
- **Mất khả năng thanh toán và tài sản ròng âm:** phân biệt thời điểm đến hạn với giá trị bảng cân đối (⏳ Chưa học riêng).
- **Quản trị tồn kho Just-In-Time:** đánh đổi vốn tồn kho với rủi ro thiếu hàng (⏳ Chưa học riêng).
- **Tín dụng thương mại và chiết khấu thanh toán:** tính chi phí giữ tiền khi bỏ qua chiết khấu trả sớm (⏳ Chưa học riêng).

## Điều đáng nhớ nhất

1. CCC đo số ngày; W đo số tiền; kế hoạch tiền mặt mới xác định nhu cầu tài trợ theo thời điểm.
2. Không nhân toàn bộ CCC với giá vốn/ngày rồi coi đó là nhu cầu vay chính xác.
3. Doanh nghiệp có lãi vẫn có thể thiếu tiền nếu thu chậm, trả sớm hoặc mở rộng nhanh hơn khả năng tài trợ.

## Góc Phản xạ & Active Recall (Dành cho bạn)

Nếu doanh thu tăng gấp đôi nhưng CCC không đổi, vì sao doanh nghiệp vẫn có thể cần thêm vốn?

**Thang tự đánh giá (1–5):** 1 = cần đọc lại sớm; 3 = nắm vững; 5 = có thể giải thích và tự kiểm tra ví dụ.
