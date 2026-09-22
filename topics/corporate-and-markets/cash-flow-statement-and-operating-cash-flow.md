---
id: CORP-002
title: "Báo cáo lưu chuyển tiền tệ: Vì sao có lợi nhuận vẫn thiếu tiền?"
category: corporate-and-markets
tags: [cash-flow-statement, operating-cash-flow, accrual-accounting, working-capital]
prerequisites: [CORP-001]
difficulty: Intermediate
date: 2026-09-23
last_verified: 2026-09-23
---

# Báo cáo lưu chuyển tiền tệ: Vì sao có lợi nhuận vẫn thiếu tiền?

## 1. Chủ đề hôm nay

**Báo cáo lưu chuyển tiền tệ (statement of cash flows)** cho biết tiền và các khoản tương đương tiền đã đi vào, đi ra doanh nghiệp trong một kỳ như thế nào. Trọng tâm bài này là **dòng tiền thuần từ hoạt động kinh doanh (operating cash flow, OCF)**.

> 🔄 **Ôn tập Ngắt quãng (Delayed Active Recall):** *Trước khi đọc tiếp, bạn còn nhớ vì sao chu kỳ chuyển đổi tiền mặt ở [CORP-001](cash-conversion-cycle.md) có thể khiến doanh nghiệp bán được hàng mà vẫn phải tìm vốn trả nhà cung cấp không? Hãy thử nhớ lại một ý cốt lõi.*

## 2. Vấn đề cốt lõi

Doanh nghiệp báo lãi 100 triệu đồng nhưng số tiền sẵn có cuối kỳ lại giảm. Tiền đang nằm ở khoản phải thu, tồn kho, máy móc hay đã dùng để trả nợ? Báo cáo kết quả kinh doanh không tự trả lời được câu hỏi này, vì lợi nhuận được ghi nhận theo cơ sở dồn tích. Báo cáo lưu chuyển tiền tệ nối kết quả kinh doanh với biến động tiền. [SEC, *Beginners' Guide to Financial Statements*, mục “Cash Flow Statements”](https://www.sec.gov/about/reports-publications/investorpubsbegfinstmtguide).

## 3. Giải thích cơ chế

### 3.1. Ba nhóm dòng tiền và các chủ thể

[Definition] Theo IAS 7, báo cáo chia dòng tiền thành **hoạt động kinh doanh** (operating: hoạt động tạo doanh thu chính và các hoạt động không thuộc hai nhóm còn lại), **đầu tư** (investing: mua, bán tài sản dài hạn và một số khoản đầu tư), và **tài trợ** (financing: thay đổi vốn góp và các khoản vay). Khách hàng trả tiền, nhà cung cấp nhận tiền, ngân hàng cấp hoặc thu hồi khoản vay và chủ sở hữu góp vốn đều tác động đến các nhóm khác nhau. Cách phân loại một số dòng tiền cụ thể phải theo chuẩn mực áp dụng và bản chất hoạt động của doanh nghiệp; không suy từ tên giao dịch đơn lẻ. [IFRS Foundation, *IAS 7 Statement of Cash Flows*, mục “About”](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/).

| Nhóm | Câu hỏi cần hỏi | Ví dụ trong doanh nghiệp thương mại giả định |
| :--- | :--- | :--- |
| Hoạt động kinh doanh | Hoạt động thường xuyên tạo hay dùng bao nhiêu tiền? | Thu từ khách; trả nhà cung cấp, nhân viên |
| Đầu tư | Tiền đã dùng để mua tài sản tạo năng lực tương lai? | Mua máy móc bằng tiền |
| Tài trợ | Tiền đến từ hoặc trả lại người cấp vốn? | Vay mới, trả gốc vay |

[Accounting Identity] Trong ví dụ đơn giản **không có ảnh hưởng tỷ giá hoặc khoản đối chiếu khác**:

$$\Delta\text{Tiền và tương đương tiền}=OCF+ICF+CFF,$$

Ở đây $ICF$ là dòng tiền đầu tư và $CFF$ là dòng tiền tài trợ. Đây là phép đối chiếu ba luồng tiền để ra chênh lệch số dư đầu và cuối kỳ. Nó không nói doanh nghiệp khỏe hay yếu nếu đứng riêng lẻ. **Tiền và tương đương tiền** gồm tiền và khoản đầu tư ngắn hạn, thanh khoản cao, dễ chuyển thành số tiền xác định và ít rủi ro thay đổi giá trị; không phải mọi khoản đầu tư ngắn hạn đều đủ điều kiện. [IFRS Foundation, *IAS 7 Statement of Cash Flows*, mục “About”](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/).

### 3.2. TEXTBOOK MODEL — từ lợi nhuận đến OCF

[Theoretical Model] Với doanh nghiệp phi tài chính đơn giản, giả sử không có khoản lãi/lỗ bán tài sản, giao dịch phi tiền khác, chênh lệch tỷ giá hay khoản dồn tích ngoài ba khoản dưới đây; lãi vay và thuế đã trả bằng đúng chi phí ghi trong lợi nhuận và được xếp trong hoạt động kinh doanh của ví dụ:

$$OCF=\text{Lợi nhuận sau thuế}+\text{Khấu hao}-\Delta W,$$

trong đó [Definition] $W=\text{Tồn kho}+\text{Phải thu thương mại}-\text{Phải trả nhà cung cấp}$ là **vốn lưu động hoạt động** được thu hẹp vào ba khoản. $\Delta W=W_{\text{cuối kỳ}}-W_{\text{đầu kỳ}}$, dùng **biến động số dư đầu/cuối kỳ**, không dùng số dư bình quân tính DIO, DSO, DPO ở [CORP-001](cash-conversion-cycle.md). $W$ cũng khác **vốn lưu động ròng kế toán** $NWC=\text{Tài sản ngắn hạn}-\text{Nợ ngắn hạn}$, vốn có thể chứa chính tiền và nợ vay. Công thức là mô hình rút gọn để đọc dấu của dòng tiền, không phải mẫu tính OCF áp cho mọi báo cáo.

**Phạm vi áp dụng:** Cách xếp lãi vay đã trả vào OCF trong ví dụ phù hợp với một lựa chọn theo IAS 7 trước khi áp dụng sửa đổi đi kèm IFRS 18. IFRS 18 có hiệu lực cho kỳ báo cáo năm bắt đầu từ ngày 01/01/2027 (được phép áp dụng sớm). Khi áp dụng sửa đổi này, doanh nghiệp thương mại thông thường xếp lãi vay đã trả vào dòng tiền tài trợ và bắt đầu phương pháp gián tiếp từ lợi nhuận hoạt động; vì vậy không dùng nguyên công thức rút gọn trên làm mẫu trình bày cho các kỳ đó. [IFRS Foundation, *IFRS 18 Presentation and Disclosure in Financial Statements*, mục “About”](https://www.ifrs.org/issued-standards/list-of-standards/ifrs-18-presentation-and-disclosure-in-financial-statements/); [IASB, *Effects Analysis: IFRS 18*, mục 2.5](https://www.ifrs.org/content/dam/ifrs/publications/amendments/english/2024/effect-analysis-ifrs18-april2024.pdf#page=27).

- [Causal Mechanism] **Phải thu tăng**: doanh thu và lợi nhuận có thể đã ghi nhận, nhưng khách chưa trả phần tiền đó; trừ phần tăng khi đối chiếu.
- [Causal Mechanism] **Tồn kho tăng**: doanh nghiệp bỏ thêm tiền vào hàng chưa bán hoặc chưa ghi vào giá vốn; trừ phần tăng nếu các khoản khác giữ nguyên.
- [Causal Mechanism] **Phải trả nhà cung cấp tăng**: hàng đã nhận nhưng chưa trả hết tiền; cộng phần tăng. Đây là nguồn tài trợ tạm thời, kèm nghĩa vụ thanh toán về sau.
- [Accounting Identity] **Khấu hao** làm giảm lợi nhuận kỳ này nhưng bản thân khoản ghi chi phí không tạo dòng tiền ra kỳ này, nên được cộng lại khi đối chiếu gián tiếp. Tiền mua máy, nếu đã trả, xuất hiện trong dòng tiền đầu tư.

IAS 7 cho phép trình bày OCF theo **phương pháp trực tiếp (direct method)**, liệt kê các khoản thu chi tiền chủ yếu, hoặc **phương pháp gián tiếp (indirect method)**, điều chỉnh kết quả kinh doanh cho khoản phi tiền, dồn tích và khoản thuộc đầu tư/tài trợ. Hai cách là hai lối trình bày cùng một OCF, không phải hai loại tiền khác nhau. [IFRS Foundation, *IAS 7 Statement of Cash Flows*, mục “About”](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/); [ACCA, *Cash flow statements*, mục “Operating activities”](https://www.accaglobal.com/uk/en/student/exam-support-resources/fundamentals-exams-study-resources/f3/technical-articles/cashflow-statements.html).

### 3.3. REAL-WORLD MECHANISM — đọc báo cáo thực tế

Một báo cáo thật có thể thêm ứng trước của khách hàng, chi phí trả trước, thuế phải nộp, dự phòng, lãi/lỗ bán tài sản, giao dịch mua tài sản chưa trả tiền hoặc tác động tỷ giá. Khi đó phải đối chiếu **từng khoản phù hợp với chuẩn mực đang áp dụng**, chứ không lấy một công thức bốn hạng tử để thay cho báo cáo. Giao dịch đầu tư/tài trợ không dùng tiền được trình bày riêng thay vì đưa vào tổng tiền thu chi; IAS 7 cũng yêu cầu đối chiếu thành phần tiền và tương đương tiền với báo cáo tình hình tài chính. [IFRS Foundation, *IAS 7 Statement of Cash Flows*, mục “About”](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/).

[Causal Mechanism] OCF thấp hơn lợi nhuận trong một kỳ **không tự chứng minh** gian lận hay kinh doanh sa sút: doanh nghiệp tăng trưởng có thể phải giữ thêm hàng và cho khách trả chậm. Ngược lại, OCF tăng nhờ kéo dài thời hạn trả nhà cung cấp có thể đi kèm áp lực trả tiền kỳ sau. Cần xem nhiều kỳ, biến động phải thu/tồn kho/phải trả, đầu tư cần thiết và lịch nợ đến hạn. [SEC, *Beginners' Guide to Financial Statements*, mục “Bringing It All Together”](https://www.sec.gov/about/reports-publications/investorpubsbegfinstmtguide) cũng lưu ý rằng một báo cáo riêng lẻ không kể hết tình hình.

## 4. Ví dụ trực quan — kiểm tra bằng hai phương pháp

**Toàn bộ số liệu sau là giả định, đơn vị triệu đồng, cho cùng một kỳ.** Doanh nghiệp thương mại bán hàng ghi nhận doanh thu 500, giá vốn 300, chi phí vận hành trả tiền 60, khấu hao 20 và lãi vay cùng thuế đã trả 20. Lợi nhuận sau thuế là $500-300-60-20-20=100$. Trong kỳ, phải thu tăng 70, tồn kho tăng 40 và phải trả nhà cung cấp tăng 25. Giả sử không có khoản điều chỉnh nào khác.

| Đối chiếu gián tiếp | Triệu đồng |
| :--- | ---: |
| Lợi nhuận sau thuế | 100 |
| Cộng khấu hao phi tiền | +20 |
| Trừ phải thu tăng | −70 |
| Trừ tồn kho tăng | −40 |
| Cộng phải trả nhà cung cấp tăng | +25 |
| **OCF** | **35** |

$\Delta W=70+40-25=85$, nên công thức rút gọn cũng cho $OCF=100+20-85=35$. **Kiểm tra trực tiếp:** tiền thu khách hàng $=500-70=430$; tiền trả nhà cung cấp $=300+40-25=315$ (vì mua hàng $=300+40=340$); các khoản chi tiền khác $=60+20=80$. Vậy $430-315-80=35$. Ở đây hàng mua và bán chỉ phục vụ hoạt động thương mại, không có biến động khác trong giá vốn, tồn kho và phải trả.

Giả sử thêm doanh nghiệp trả **80** mua máy, vay mới **60**, trả gốc vay **20**. Khi đó dòng tiền đầu tư $=-80$; dòng tiền tài trợ $=60-20=40$; biến động tiền $=35-80+40=-5$. Nếu đầu kỳ có **30** tiền và tương đương tiền, cuối kỳ còn **25**. Báo lãi **100** và OCF dương **35** vẫn có thể đi cùng số dư tiền giảm **5** vì chi mua máy vượt phần tiền hoạt động và tài trợ ròng. Đây là phép đối chiếu giao dịch giả định, không phải số liệu của doanh nghiệp thật.

[Accounting Identity] Kiểm tra thêm bảng cân đối với giả định không có giao dịch hay thay đổi vốn chủ khác: tài sản thay đổi $-5$ tiền $+70$ phải thu $+40$ tồn kho $+60$ giá trị máy ròng ($80$ mua mới trừ $20$ khấu hao) $=+165$. Nguồn vốn thay đổi $+25$ phải trả $+40$ nợ vay ròng $+100$ lợi nhuận giữ lại $=+165$. Hai vế khớp nhau; khoản vay mới không bị tính vào lợi nhuận.

## 5. Tình huống thực tế

**Nếu một doanh nghiệp công bố lợi nhuận tăng nhưng OCF âm, điều gì cần xem?** Trước tiên kiểm tra tiền thu khách: phải thu tăng do doanh số tăng theo mùa, điều khoản trả chậm, hay khách hàng chậm thanh toán? Tiếp đó xem tồn kho: doanh nghiệp đang chuẩn bị cho đơn hàng đã có hay hàng bán chậm? Cuối cùng xem dòng tiền tài trợ và số dư tiền: doanh nghiệp có đang dùng vay mới để bù tiền hoạt động trong khi khoản vay cũ sắp đến hạn không? Cùng một OCF âm có thể có ý nghĩa khác nhau tùy nguyên nhân, thời điểm thu tiền và khả năng tiếp cận vốn. Không thể suy ra trực tiếp tình trạng mất khả năng thanh toán chỉ từ dấu âm của một kỳ.

## Kiến thức này có ích gì với tôi?

Khi đọc tin “doanh nghiệp lãi lớn”, hãy tìm **OCF**, biến động phải thu/tồn kho/phải trả và dòng tiền mua tài sản. Bạn sẽ phân biệt được tiền do khách hàng trả với tiền do vay mới đem vào; vay mới tăng tiền cuối kỳ nhưng cũng tạo nghĩa vụ trả gốc về sau. Nếu cân nhắc mua cổ phiếu hoặc cho một doanh nghiệp vay, cách đọc này giúp đặt câu hỏi về khả năng trả tiền đúng hạn mà không biến một chỉ tiêu thành kết luận đầu tư. Khi quản lý dòng tiền cá nhân, nguyên lý tương tự là ghi cả **ngày tiền thực vào/ra**, thay vì chỉ cộng thu nhập đã kiếm và chi phí đã phát sinh.

## Thuật ngữ cần phân biệt

- **Lợi nhuận sau thuế (net income/profit after tax):** kết quả theo kế toán dồn tích trong kỳ; không phải số dư tiền.
- **Dòng tiền hoạt động (operating cash flow):** tiền thuần từ hoạt động kinh doanh theo phân loại báo cáo; khác lợi nhuận và khác **tổng biến động tiền**.
- **Dòng tiền đầu tư (investing cash flow):** tiền thuần từ mua, bán tài sản dài hạn và khoản đầu tư thuộc nhóm này; không đồng nghĩa mọi khoản “đầu tư” trong lời nói thường ngày.
- **Dòng tiền tài trợ (financing cash flow):** tiền thuần từ giao dịch với người cấp vốn; tiền vay vào là dòng tiền dương nhưng không phải doanh thu.
- **Vốn lưu động hoạt động (operating working capital):** trong mô hình bài này chỉ gồm tồn kho, phải thu thương mại và phải trả nhà cung cấp; khác NWC tổng quát.

## Liên kết kiến thức

- **Chu kỳ chuyển đổi tiền mặt [CORP-001](cash-conversion-cycle.md):** giải thích vì sao dòng tiền bị giữ trong tồn kho và phải thu theo thời gian.
- **Chất lượng lợi nhuận:** xem lợi nhuận được hỗ trợ bởi thu tiền thế nào qua nhiều kỳ.
- **Rủi ro thanh khoản và lịch đáo hạn nợ:** OCF và số dư tiền phải đặt cạnh nghĩa vụ trả tiền theo ngày.

## Điều đáng nhớ nhất

1. Lợi nhuận đo kết quả dồn tích; OCF đo tiền thuần thuộc hoạt động kinh doanh. Chênh lệch thường đi qua khấu hao và các khoản phải thu, tồn kho, phải trả.
2. Tổng tiền còn tăng hay giảm còn phụ thuộc đầu tư và tài trợ. Tiền vay mới có thể che áp lực tiền hoạt động trong ngắn hạn.
3. Công thức $OCF=\text{lợi nhuận}+\text{khấu hao}-\Delta W$ chỉ đúng với các giả định đã nêu; khi đọc báo cáo thật cần xem từng dòng và thuyết minh.

## Góc Phản xạ & Active Recall (Dành cho bạn)

*Hãy thử giải thích cho một người bạn bằng 2–3 câu: vì sao doanh nghiệp ghi lợi nhuận 100 nhưng dòng tiền hoạt động chỉ 35 trong ví dụ này?*

**Thang tự đánh giá (1–5):** Bạn thấy mình hiểu/nhớ cơ chế hôm nay ở mức nào (1 = cần đọc lại sớm; 3 = nắm vững; 5 = rất tự tin)? Nếu chọn 1–2, hãy ưu tiên ôn lại sau ít ngày.

## Nguồn tham khảo

1. IFRS Foundation, [*IAS 7 Statement of Cash Flows*](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/), trang tổng quan chuẩn mực (không ghi ngày công bố trang; truy cập 2026-09-23). Hỗ trợ định nghĩa ba nhóm, tiền và tương đương tiền, hai phương pháp trình bày OCF và giao dịch phi tiền.
2. U.S. Securities and Exchange Commission, [*Beginners' Guide to Financial Statements*](https://www.sec.gov/about/reports-publications/investorpubsbegfinstmtguide), 2007 (truy cập 2026-09-23). Hỗ trợ cách phân biệt lợi nhuận với dòng tiền và đọc kết hợp các báo cáo.
3. ACCA, [*Cash flow statements*](https://www.accaglobal.com/uk/en/student/exam-support-resources/fundamentals-exams-study-resources/f3/technical-articles/cashflow-statements.html), tài liệu học thuật trực tuyến (trang không ghi ngày công bố; truy cập 2026-09-23). Hỗ trợ dấu điều chỉnh tồn kho, phải thu, phải trả và đối chiếu phương pháp trực tiếp/gián tiếp.
4. IFRS Foundation, [*IFRS 18 Presentation and Disclosure in Financial Statements*](https://www.ifrs.org/issued-standards/list-of-standards/ifrs-18-presentation-and-disclosure-in-financial-statements/) và IASB, [*Effects Analysis: IFRS 18*, mục 2.5](https://www.ifrs.org/content/dam/ifrs/publications/amendments/english/2024/effect-analysis-ifrs18-april2024.pdf#page=27), 2024 (truy cập 2026-09-23). Hỗ trợ ngày hiệu lực, thay đổi điểm bắt đầu phương pháp gián tiếp và phân loại lãi vay đã trả.
