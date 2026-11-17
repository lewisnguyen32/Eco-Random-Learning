---
id: VIET-001
title: "Tỷ giá và giá tiêu dùng: VND mất giá truyền vào CPI như thế nào?"
category: vietnam-economy
tags: [exchange-rates, vietnam, pass-through, inflation, cpi]
prerequisites: [MACRO-001, MONEY-002]
difficulty: Intermediate
date: 2026-11-18
last_verified: 2026-11-18
---

# VIET-001 – Tỷ giá và giá tiêu dùng

## 1. Chủ đề hôm nay

**Truyền dẫn tỷ giá vào giá cả** (*exchange rate pass-through*, ERPT) ở Việt Nam. Bài học nối cách đo CPI trong [MACRO-001](../macroeconomics/inflation-cpi-and-macro-transmission.md) với kênh tỷ giá trong [MONEY-002](../monetary-and-banking/policy-rates-and-monetary-transmission.md).

## 2. Vấn đề cốt lõi

Nếu mua một USD tốn thêm 10% tiền đồng, một doanh nghiệp có hóa đơn USD cố định sẽ cần thêm 10% VND để trả hóa đơn theo tỷ giá mới. Qua những bước nào áp lực đó mới đến giá bán lẻ? Vì sao một dịch vụ trong nước cũng có thể tăng giá, trong khi một món hàng nhập khẩu vẫn giữ giá?

## 3. Giải thích cơ chế

### Các đại lượng đang đo

**[Definition]** Gọi $E$ là **tỷ giá danh nghĩa song phương** (*bilateral nominal exchange rate*), đo bằng số VND đổi một USD. $E$ tăng nghĩa là cần nhiều VND hơn để mua một USD, tức VND mất giá so với USD. Bài dùng phần trăm thay đổi của $E$ khi định lượng biến động. Nếu đọc báo giá nghịch đảo, mẫu số đổi và độ lớn phần trăm cũng đổi.

**[Definition]** Truyền dẫn tỷ giá mô tả mức giá phản ứng khi tỷ giá thay đổi. Một hệ số truyền dẫn cần ghi rõ giá nào được đo, tỷ giá nào được dùng và phản ứng được xét sau bao lâu. Giá nhập khẩu, giá bán lẻ một mặt hàng và CPI là ba đối tượng đo khác nhau. Ước lượng từ dữ liệu quan sát còn phụ thuộc cách tách cú sốc tỷ giá khỏi các biến động cùng lúc. [ECB, mục 2.1](https://www.ecb.europa.eu/press/economic-bulletin/articles/2020/html/ecb.ebart202003_01~7fc0abdec2.en.html).

### Mô hình giáo trình (Textbook Model) — quy đổi một hóa đơn

**[Theoretical Model]** Giả sử nhà cung cấp giữ giá ghi trên hóa đơn bằng USD, nhà nhập khẩu mua đủ USD theo tỷ giá giao ngay tại lúc thanh toán, và bỏ qua phí đổi tiền, thuế và chi phí vận chuyển. Khoản thanh toán quy đổi cho một đơn vị hàng là:

$$
P_{\mathrm{VND}} = E \times P_{\mathrm{USD}}.
$$

$P_{\mathrm{USD}}$ là số USD trên mỗi đơn vị hàng. Nhân với số VND cần cho mỗi USD cho ra số VND cần cho một đơn vị hàng. Khi giá USD giữ nguyên, $E$ tăng 10% làm giá trị hóa đơn tính bằng VND tăng đúng 10%. Nếu nhà cung cấp đồng thời hạ giá USD 10%, hai thay đổi nhân với nhau: $1{,}10 \times 0{,}90 = 0{,}99$. Khi đó số VND cần trả giảm 1%. Kết quả chỉ mô tả khoản thanh toán trong các điều kiện trên.

### Cơ chế thực tế (Real-World Mechanism) — từ hợp đồng đến CPI

1. **[Causal Mechanism] Đồng tiền ghi hóa đơn (*invoicing currency*) quyết định tỷ giá nào đi vào phép quy đổi.** Một nhà cung cấp ở Hàn Quốc có thể định giá bằng USD. Khi mức giá USD còn cố định, người nhập khẩu tại Việt Nam cần nhìn tỷ giá VND trên một USD để tính số tiền phải đổi. Nếu hợp đồng khóa giá bằng VND, số tiền trong hóa đơn giữ nguyên cho đến khi điều khoản cho phép đổi giá. Nhà cung cấp có thể điều chỉnh giá khi đàm phán lại. [ECB, mục 3.3](https://www.ecb.europa.eu/press/economic-bulletin/articles/2020/html/ecb.ebart202003_01~7fc0abdec2.en.html).

   **[Empirical Relationship]** Nghiên cứu của Boz và cộng sự trên dữ liệu thương mại nhiều nước tìm thấy mức truyền dẫn từ tỷ giá với USD vào giá nhập khẩu cao hơn ở các nước dùng USD nhiều hơn để ghi hóa đơn. [Boz và cộng sự, 2020](https://www.imf.org/en/publications/wp/issues/2020/07/17/patterns-in-invoicing-currency-in-global-trade-49574).
2. **[Causal Mechanism] Chi phí nhập khẩu và giá trên kệ đổi theo những lịch khác nhau.** Doanh nghiệp có thể mua USD trước hoặc dùng hợp đồng kỳ hạn (*FX forward*) để chốt tỷ giá cho số USD và ngày thanh toán xác định. Việc đó giới hạn biến động của khoản chi đã phòng hộ. Hàng tồn kho mua trước cú sốc cho phép doanh nghiệp tiếp tục bán từ lô có chi phí cũ, dù họ có thể điều chỉnh giá ngay nếu dự kiến chi phí nhập lô thay thế sẽ cao hơn. Khi chi phí tăng, nhà bán lẻ cân nhắc giữa giữ giá để giữ khách và tăng giá để giữ phần chênh còn lại sau chi phí. Chi phí phân phối trong nước như thuê kho và giao hàng cũng góp vào giá bán, nên giá của một món hàng có thể tăng theo tỷ lệ nhỏ hơn giá trị hóa đơn nhập. [ECB, mục 3.4](https://www.ecb.europa.eu/press/economic-bulletin/articles/2020/html/ecb.ebart202003_01~7fc0abdec2.en.html).
3. **[Causal Mechanism] Giá từng món đi vào CPI qua quyền số và hai đường truyền.** Hàng nhập bán thẳng cho hộ gia đình tạo kênh trực tiếp. Nguyên liệu, phụ tùng hay nhiên liệu nhập khẩu tạo kênh gián tiếp nếu chi phí tăng và nhà sản xuất hoặc đơn vị vận tải chuyển một phần vào giá hàng hóa, dịch vụ trong nước. Giá một nhóm hàng tác động lên CPI theo mức biến động và quyền số chi tiêu của nhóm đó. Ở chiều ngược lại, nếu cú sốc khiến hộ gia đình giảm mua sắm, sức cầu yếu có thể khiến doanh nghiệp giữ giá và chấp nhận phần chênh thấp hơn. Nguồn gốc của biến động tỷ giá vì thế ảnh hưởng đến kết quả quan sát được. [ECB, mục 3–4](https://www.ecb.europa.eu/press/economic-bulletin/articles/2020/html/ecb.ebart202003_01~7fc0abdec2.en.html).

## 4. Ví dụ trực quan — từ 10% ở tỷ giá đến 0,625% ở rổ giá

**[Theoretical Model]** Giả sử một nhà bán lẻ nhập một bộ lọc với giá 20 USD, thanh toán ngay theo tỷ giá giao ngay. Chi phí nội địa là 200.000 VND mỗi bộ và giữ nguyên. Tỷ giá, giá bán, cấu trúc chi phí và rổ tiêu dùng dưới đây đều là giả định.

| Tỷ giá và số tiền mỗi bộ | Trước khi tỷ giá đổi | Sau khi tỷ giá đổi |
| :--- | ---: | ---: |
| Tỷ giá (VND cho 1 USD) | 25.000 | 27.500 |
| Hóa đơn nhập khẩu (VND quy đổi) | 500.000 | 550.000 |
| Tổng chi phí giả định (VND) | 700.000 | 750.000 |
| Giá bán lẻ (VND) | 800.000 | 825.000 |
| Phần chênh giá bán trừ chi phí giả định (VND) | 100.000 | 75.000 |

Trong 50.000 VND chi phí tăng thêm, người mua chịu 25.000 VND qua giá bán và nhà bán lẻ chịu 25.000 VND qua phần chênh mỗi bộ giảm đi. Giá bán tăng $25\,000 / 800\,000 = 3{,}125\%$. Nếu giữ nguyên giá 800.000 VND, nhà bán lẻ còn 50.000 VND mỗi bộ trước các chi phí khác. Thay đổi số lượng bán sẽ ảnh hưởng đến kết quả của cả cửa hàng.

Giả sử trong một rổ có lượng mua cố định, bộ lọc chiếm 20% chi tiêu gốc và giá các món còn lại giữ nguyên. Khi đó, chi phí mua rổ tăng $0{,}20 \times 3{,}125\% = 0{,}625\%$, đưa chỉ số giá của rổ từ 100 lên 100,625. Quyền số 20% là tỷ trọng chi tiêu của mặt hàng trong rổ gốc, còn tỷ trọng hàng nhập trong chi phí của doanh nghiệp là một đại lượng khác. Nếu mọi giá giữ nguyên ở kỳ kế tiếp, mức giá của rổ vẫn là 100,625 và lạm phát so với kỳ liền trước bằng 0%.

## 5. Tình huống thực tế — đọc dữ liệu Việt Nam 2010–2011

**[Historical Claim]** Theo báo cáo IMF năm 2023, VND mất giá khoảng 13% so với USD từ tháng 1 đến tháng 12/2010, theo thước đo tỷ giá liên ngân hàng của báo cáo. [IMF, Phụ lục IV, chú thích 3](https://www.imf.org/-/media/files/publications/cr/2023/english/1vnmea2023003.pdf#page=47).

**[Empirical Relationship]** Với dữ liệu 2010–2011, IMF ghép mức thay đổi so với cùng kỳ của tỷ giá liên ngân hàng bình quân tháng với lạm phát CPI so với cùng kỳ ở cùng tháng và ở các tháng sau. Trong mẫu này, tương quan dương với lạm phát CPI chung mạnh nhất khi tỷ giá đi trước khoảng sáu tháng. Tương quan cũng nổi bật ở các nhóm vận tải, nhà ở, thực phẩm và dịch vụ ăn uống. Báo cáo nêu các đường truyền có thể giải thích mẫu hình này qua nhiên liệu, phân bón, thức ăn chăn nuôi và vận chuyển. Muốn quy một phần lạm phát riêng cho tỷ giá cần tách biến động đồng thời của giá hàng hóa thế giới, sức cầu và những yếu tố khác. [IMF, Phụ lục IV, Hình 1](https://www.imf.org/-/media/files/publications/cr/2023/english/1vnmea2023003.pdf#page=48).

**[Empirical Relationship]** Trong một phân tích riêng trên tám nước ASEAN, gồm Việt Nam, IMF dùng dữ liệu tháng với mẫu Việt Nam từ 2000 đến 2022. Với mức tăng 10% so với cùng kỳ của tỷ giá nội tệ trên một USD, mô hình ước lượng lạm phát CPI so với cùng kỳ ở tháng thứ 12 cao hơn khoảng 0,3 điểm phần trăm theo đặc tả cơ sở và 1,7 điểm phần trăm theo đặc tả chỉ xét các đợt mất giá. Đây là hai ước lượng điểm cho mẫu gộp. Tháng thứ 12 là mốc đọc kết quả trong mô hình. Mức tác động cho riêng Việt Nam hoặc cho một đợt mất giá khác cần bằng chứng riêng. [IMF, Phụ lục IV, chú thích 4 và Hình 2 ở trang kế tiếp](https://www.imf.org/-/media/files/publications/cr/2023/english/1vnmea2023003.pdf#page=48).

## 6. Kiến thức này có ích gì với tôi?

- **Đọc bản tin.** Khi thấy “USD tăng, hàng nhập đắt lên”, hãy xác định bản tin đang nói về tỷ giá nào và giá nào. Nếu bản tin nêu thêm giá dầu bằng USD, xét hai thay đổi cùng một lúc để biết liệu chi phí dầu quy đổi có thực sự tăng. Khi chuyển sang CPI, xét thêm quyền số, giá bán lẻ và kỳ so sánh.
- **Dự trù khoản chi bằng ngoại tệ.** Với một khoản học phí cố định bằng USD chưa thanh toán, hãy tính ngân sách VND theo tỷ giá bán USD mà ngân hàng áp dụng và phí chuyển tiền, rồi thử vài kịch bản tỷ giá tại ngày đến hạn. Khoản này nhạy trực tiếp với tỷ giá giao dịch. Khi mua một thiết bị nhập khẩu đã niêm yết bằng VND, mức giá bạn gặp còn phụ thuộc thời điểm cửa hàng nhập lô mới và quyết định giữ hay chỉnh giá.
- **Hiểu phản ứng của doanh nghiệp.** Hai cửa hàng nhập cùng một mẫu hàng có thể đổi giá vào các thời điểm khác nhau vì lịch nhập, hợp đồng và sức ép giữ khách khác nhau. Đọc số liệu CPI cùng với cơ cấu chi tiêu của gia đình giúp nhận ra vì sao một cú sốc có thể tác động lên ngân sách nhà mình mạnh hơn hoặc nhẹ hơn chỉ số chung.

## 7. Liên kết kiến thức

- [CPI và quyền số chi tiêu](../macroeconomics/inflation-cpi-and-macro-transmission.md) (MACRO-001) giúp giải thích vì sao cùng một mức tăng giá của một nhóm hàng có thể tác động khác nhau lên chỉ số chung và từng hộ.
- [Lạm phát chi phí đẩy](../macroeconomics/supply-shocks-cost-push-inflation-and-stagflation.md) (MACRO-003) mở rộng cách đọc kênh đầu vào và phân biệt một lần tăng mức giá với lạm phát dai dẳng.
- **Phòng hộ tỷ giá** (*FX hedging*) giúp hiểu cách doanh nghiệp quản lý dòng tiền ngoại tệ theo số tiền và ngày đến hạn.
- **Tỷ giá hữu hiệu danh nghĩa** (*nominal effective exchange rate*, NEER) tổng hợp các tỷ giá song phương theo quyền số. Khi đọc chi phí của một hợp đồng cụ thể, đồng tiền trên hóa đơn cho biết tỷ giá song phương nào cần theo dõi.

## 8. Điều đáng nhớ nhất

- Hóa đơn có giá USD cố định phản ứng ngay khi được quy đổi theo tỷ giá mới. Giá trên kệ còn qua chi phí nội địa, lịch đổi giá và quyết định chia sẻ chi phí giữa người bán với người mua.
- Để hiểu tác động lên CPI, lần theo cả hàng nhập bán cho hộ và đầu vào nhập dùng trong nước, rồi xét quyền số và kỳ đo. Một lần tăng mức giá chỉ duy trì lạm phát trong các kỳ so sánh còn bao trùm lần tăng đó, nếu các giá sau đó giữ nguyên.

## 9. Góc Phản xạ & Active Recall (Dành cho bạn)

Bạn sẽ giải thích bằng 2–3 câu thế nào cho một người bạn khi hóa đơn USD của cửa hàng đắt thêm 10% tính bằng VND nhưng giá trên kệ chỉ tăng khoảng 3%?

**Thang tự đánh giá (1–5).** Chọn 1 nếu cần đọc lại sớm, 3 nếu nắm vững, hoặc 5 nếu rất tự tin. Mức 1–2 giúp ưu tiên ôn lại sớm hơn.

## 10. Nguồn tham khảo

1. Ngân hàng Trung ương châu Âu (ECB), *Economic Bulletin*, số 3/2020. [The transmission of exchange rate changes to euro area inflation](https://www.ecb.europa.eu/press/economic-bulletin/articles/2020/html/ecb.ebart202003_01~7fc0abdec2.en.html).
2. Emine Boz và cộng sự, *IMF Working Paper* 2020/126, 17/07/2020. [Patterns in Invoicing Currency in Global Trade](https://www.imf.org/en/publications/wp/issues/2020/07/17/patterns-in-invoicing-currency-in-global-trade-49574).
3. Quỹ Tiền tệ Quốc tế (IMF), *Vietnam: 2023 Article IV Consultation*, Country Report 23/338, 09/2023, tr. 43–45. [Annex IV. Exchange Rate Pass-Through to Inflation in Vietnam](https://www.imf.org/-/media/files/publications/cr/2023/english/1vnmea2023003.pdf#page=47).
