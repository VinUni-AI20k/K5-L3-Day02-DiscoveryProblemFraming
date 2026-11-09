# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Trọng Truyền
- MSSV: 225748020110258
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:HungTungTruyenHuy
- Link repo nhóm:https://github.com/huydn8816/K5-L3B-Day02-HungTungTruyenHuy-DiscoveryProblemFraming
---

## 2. Scan problem (CP1)

### Năm điểm nghẽn vận hành

| # | Lăng kính | Job Story (Khi… tôi muốn… để…) | Ai chịu ảnh hưởng? | Bước nghẽn và công sức ước tính |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | **Soạn bảng đáp ứng yêu cầu chào thầu.** Khi nhận hồ sơ có nhiều tiêu chí kỹ thuật, tôi muốn tìm đúng dòng thông số và tài liệu của từng model, để nộp bảng đáp ứng đúng hạn và có căn cứ. | Nhân viên kinh doanh dự án, kỹ sư giải pháp | Mở từng PDF, đối chiếu tiêu chí như PoE, số cổng và tốc độ, rồi chép thông số vào bảng. **6 hồ sơ/tháng × 4 giờ tra cứu và nhập lại = 24 giờ/tháng (3,6 triệu đồng).** |
| 2 | Lặp lại · Tốn thời gian | **Nhập đơn đặt hàng vào ERP.** Khi nhận đơn từ khách dưới dạng PDF hoặc Excel, tôi muốn xác định đúng mã hàng, số lượng và đơn vị tính, để kho soạn đúng và đơn kịp chuyến giao. | Nhân viên xử lý đơn, kho, khách hàng | Đọc từng dòng, tra mã theo tên hàng của khách và nhập lại vào ERP. Mã hoặc đơn vị tính sai khiến kho phải dừng để xác nhận. **600 đơn/tháng × 6 phút = 60 giờ/tháng (9 triệu đồng).** |
| 3 | Lặp lại · Pain từ người khác | **Gắn phiếu giao hàng đã ký vào đúng đơn.** Khi tài xế gửi ảnh phiếu giao hàng, tôi muốn biết phiếu thuộc chuyến nào và có ghi giao thiếu hay không, để chốt trạng thái giao hàng trong ngày. | Điều phối, tài xế, bộ phận đối soát | Mở ảnh trong nhóm chat, dò mã phiếu hoặc tên khách trong ERP và hỏi lại khi ảnh mờ hoặc thiếu mã. **240 phiếu ảnh/tháng × 5 phút = 20 giờ/tháng (3 triệu đồng).** |
| 4 | Cần đọc, tổng hợp nhiều thông tin · Pain từ người khác | **Kiểm tra hồ sơ bảo hành thiết bị.** Khi khách gửi ảnh tem và mô tả lỗi, tôi muốn tìm đúng số sê-ri, giao dịch bán và thời hạn bảo hành, để phản hồi khách ngay lần đầu hoặc yêu cầu đúng giấy tờ còn thiếu. | Nhân viên bảo hành, kỹ thuật viên, khách hàng | Gõ lại số sê-ri, tìm hóa đơn và tra chính sách của hãng. Nếu đọc nhầm ký tự, nhân viên phải dò lại hoặc yêu cầu khách chụp lại. **180 hồ sơ/tháng × 8 phút = 24 giờ/tháng (3,6 triệu đồng).** |
| 5 | Lặp lại · Tốn thời gian | **Xử lý hóa đơn nhà cung cấp bị lệch.** Khi hóa đơn lệch so với đơn mua hoặc phiếu nhập, tôi muốn biết dòng nào sai và còn thiếu chứng từ gì, để xác minh trước hạn thanh toán. | Kế toán công nợ, mua hàng, kho | Mở ba chứng từ, dò từng dòng và liên hệ kho hoặc mua hàng để xác nhận trường hợp giao từng phần hay sai đơn vị tính. **500 hóa đơn/tháng × 18% có ngoại lệ × 15 phút = 22,5 giờ/tháng (~3,38 triệu đồng).** |

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

Ưu tiên bài toán có người chịu trách nhiệm rõ, bước nghẽn đo được, dữ liệu để kiểm tra kết quả và phương án đơn giản có thể thử trong một buổi lab. Khối lượng và thời gian gốc lấy từ kịch bản CP1. Thời lượng các bước còn lại và các ngưỡng mục tiêu là giả định để thiết kế phép thử.

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | CP1 #2 — Nhập đơn đặt hàng vào ERP | Bước nhập chiếm 60 giờ/tháng theo kịch bản, cao nhất trong năm bài toán. Đơn gốc, danh mục hàng và bản ghi ERP cho phép so thời gian và lỗi trên cùng bộ đơn. | Bao nhiêu đơn dùng mẫu cố định hoặc có mã khách hàng ánh xạ được? Sai mã, sai số lượng và lỡ chuyến giao hiện xảy ra bao nhiêu lần? |
| 2 | CP1 #5 — Xử lý hóa đơn nhà cung cấp bị lệch | Có ba chứng từ để đối chiếu và quy tắc nghiệp vụ rõ cho nhiều trường hợp. Bỏ sót một khoản lệch có thể dẫn đến thanh toán sai hoặc thanh toán chậm. | Hóa đơn có trường tham chiếu đơn mua hay phải dò tay? ERP có ghi giao từng phần, đơn vị quy đổi và dung sai đã duyệt không? |
| 3 | CP1 #3 — Gắn phiếu giao hàng đã ký vào đúng đơn | Mã lần giao có thể gắn ngay khi tài xế gửi ảnh. Thử được với một tuyến giao và đo trực tiếp tỷ lệ phiếu chốt đúng ngày. | Tài xế có thể gửi qua biểu mẫu trên tuyến không? Bao nhiêu đơn giao nhiều lần và bao nhiêu phiếu có ghi giao thiếu? |

Hai bài toán còn lại được giữ làm ứng viên sau. Với **#1 chào thầu**, danh mục thông số có cấu trúc và mẫu bảng theo model có thể điền các tiêu chí lặp lại bằng quy tắc. Tiêu chí viết tự do vẫn cần kỹ sư thẩm định, nên phải đo riêng phần tra cứu có thể chuẩn hóa. Với **#4 bảo hành**, biểu mẫu bắt buộc số sê-ri và bảng chính sách theo hãng có thể xử lý hồ sơ đủ dữ liệu bằng tra cứu chính xác. Cần xác minh hệ thống có liên kết số sê-ri với hóa đơn bán và lưu đúng phiên bản chính sách trước khi chọn.

### Problem Card #1 — Nhập đơn đặt hàng vào ERP

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách gửi đơn đặt hàng qua email, tôi muốn đưa đúng mã hàng, số lượng và đơn vị tính vào ERP, để kho soạn đúng và kịp chuyến giao. |
| Actor | Nhân viên xử lý đơn là người nhập và kiểm. Nhân viên kho nhận đơn đã xác nhận để soạn hàng. |
| Thời điểm / bối cảnh | Khi đơn PDF hoặc Excel đến gần giờ chốt chuyến, tên hàng trên đơn có thể khác tên trong danh mục nội bộ. |
| Quy trình hiện tại (3–7 bước) | Mở email và đơn gốc → xác định khách và báo giá → đọc dòng hàng, tra mã, nhập ERP → so lại bản nháp với đơn gốc → lưu đơn để kho nhận. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 mất khoảng 6 phút/đơn theo CP1. Nhân viên phải dò tên viết tắt, mã và quy cách trước khi nhập từng dòng. |
| Impact (nếu không giải thì sao) | 600 đơn × 6 phút = 60 giờ/tháng tại bước 3. Sai mã hoặc đơn vị tính khiến kho phải dừng để xác nhận, có thể lỡ chuyến. Chưa có số đo về tần suất lỡ chuyến. |
| Success metric (baseline → target) | Thời gian công trung bình từ lúc bắt đầu đọc dòng hàng đến khi đã so và sửa xong bản nháp (bước 3–4) **8 phút giả định → ≤5 phút/đơn**. Tính cả đơn phải nhập tay. Theo dõi tỷ lệ đơn kịp giờ chốt chuyến. Trên cùng tập đơn, tỷ lệ sai mã, số lượng hoặc đơn vị sau khi lưu phải bằng hoặc thấp hơn phương án nhập tay. |
| Phương án không dùng AI | Cung cấp mẫu Excel có mã và đơn vị tính bắt buộc, đọc các mẫu có cấu trúc bằng bộ nhập, ánh xạ tên hàng theo từng khách. ERP kiểm tra mã, quy đổi đơn vị và chặn trùng theo khách + số đơn. Đưa trường hợp thiếu dữ liệu hoặc có nhiều mã khả dĩ về hàng chờ xử lý tay. |
| Giả thuyết về AI (nếu có) | Chỉ thử trích xuất hoặc gợi ý mã cho phần PDF nhiều bố cục hay tên hàng chưa có trong bảng ánh xạ. Đo phần cải thiện thêm so với phương án quy tắc, gồm thời gian người duyệt và sửa lỗi. |
| Cảm nhận nhanh | **Rule trước.** Nếu đầu vào chuẩn hoặc tra được bằng bảng mã, kết quả có thể kiểm lại từng dòng và dùng lại ở lần sau. |

Quy trình nháp hiện tại:

```text
[1. Mở email và đơn gốc: 1 phút]
→ [2. Tìm hồ sơ khách và báo giá: 1 phút]
→ [3. Đọc dòng hàng, tra mã và nhập ERP: 6 phút] ← BƯỚC NGHẼN
→ [4. So bản nháp với đơn gốc: 2 phút]
→ [5. Lưu đơn và chuyển kho: 1 phút]
```

### Problem Card #2 — Xử lý hóa đơn nhà cung cấp bị lệch

| Trường | Nội dung |
|---|---|
| Job Story | Khi hóa đơn không khớp đơn mua hoặc phiếu nhập, tôi muốn thấy dòng chênh lệch và chứng từ còn thiếu, để xác minh trước hạn thanh toán. |
| Actor | Kế toán công nợ xử lý ngoại lệ, mua hàng và kho xác nhận đơn mua và số thực nhận. |
| Thời điểm / bối cảnh | Khi ghi nhận hóa đơn, nhất là giao từng phần hoặc hóa đơn và phiếu nhập dùng đơn vị tính khác nhau. |
| Quy trình hiện tại (3–7 bước) | Mở hóa đơn đã bị đánh dấu lệch → tìm đơn mua và phiếu nhập → rà từng dòng và so chênh lệch → gửi yêu cầu xác minh → cập nhật kết quả khi có phản hồi. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 mất khoảng 15 phút công/hóa đơn ngoại lệ theo CP1. Kế toán phải dò từng dòng để tìm lệch số lượng, đơn giá hoặc chứng từ. Thời gian đợi phản hồi được ghi riêng. |
| Impact (nếu không giải thì sao) | 500 hóa đơn × 18% ngoại lệ × 15 phút = 22,5 giờ/tháng cho bước rà lệch theo giả định. Một khoản lệch bị bỏ qua có thể dẫn đến trả tiền cho hàng chưa nhận hoặc giữ lại nhầm hóa đơn hợp lệ. |
| Success metric (baseline → target) | Thời gian công trung bình để phát hiện và ghi lý do lệch **15 phút giả định → ≤8 phút/hóa đơn ngoại lệ đã xác minh**. Kiểm tra trên cả hóa đơn khớp và lệch. Báo riêng tỷ lệ ngoại lệ bị bỏ sót và tỷ lệ hồ sơ khớp bị giữ nhầm, theo bộ đáp án kế toán xác nhận. Không bỏ sót sai lệch trọng yếu trong bộ thử theo ngưỡng do kế toán xác định trước. |
| Phương án không dùng AI | Đối chiếu ba bên theo mã đơn mua, mã dòng hàng và đơn vị quy đổi. Cộng số đã nhận và trừ phần đã lập hóa đơn theo từng dòng để xử lý giao từng phần. Áp dụng dung sai số lượng và đơn giá đã duyệt. Ghi trường lệch, dữ liệu gốc và quy tắc bị vi phạm. Thiếu tham chiếu hoặc nhiều dòng có thể khớp thì chuyển kế toán xác minh. |
| Giả thuyết về AI (nếu có) | Nếu nhiều chứng từ chỉ có ảnh hoặc mô tả không có mã, thử đọc trường và gợi ý dòng có thể liên quan. Quy tắc vẫn tính chênh lệch, kế toán xác nhận chứng từ và quyết định thanh toán. |
| Cảm nhận nhanh | **Rule.** Khi có dữ liệu có cấu trúc, phép đối chiếu và dung sai cho kết quả nhất quán, giải thích được khi kiểm toán. |

Quy trình nháp hiện tại:

```text
[1. Mở hóa đơn ngoại lệ: 1 phút]
→ [2. Tìm đơn mua và phiếu nhập: 3 phút]
→ [3. Rà từng dòng, xác định khoản lệch: 15 phút] ← BƯỚC NGHẼN
→ [4. Gửi yêu cầu xác minh: 2 phút]
→ [5. Ghi kết quả sau phản hồi: 2 phút]
```

### Problem Card #3 — Gắn phiếu giao hàng đã ký vào đúng đơn

| Trường | Nội dung |
|---|---|
| Job Story | Khi tài xế gửi ảnh phiếu giao có chữ ký, tôi muốn xác định đúng lần giao và biết có giao thiếu hay không, để chốt trạng thái trong ngày. |
| Actor | Nhân viên điều phối đối soát phiếu, tài xế nộp ảnh và ghi tình trạng giao thực tế. |
| Thời điểm / bối cảnh | Cuối chuyến, ảnh được gửi vào nhóm chat. Một đơn có thể chia nhiều lần giao và ảnh đôi khi thiếu mã phiếu. |
| Quy trình hiện tại (3–7 bước) | Tài xế chụp và gửi ảnh → điều phối mở ảnh, dò lần giao trong ERP và hỏi lại nếu thiếu mã → kiểm chữ ký và tình trạng giao thiếu → gắn ảnh và cập nhật trạng thái. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 mất khoảng 5 phút công/ảnh theo CP1. Thiếu mã lần giao khiến điều phối phải tìm theo tên khách hoặc hỏi lại tài xế. |
| Impact (nếu không giải thì sao) | 240 ảnh × 5 phút = 20 giờ/tháng cho bước tìm và ghép. Gắn sai phiếu hoặc chốt muộn khiến bộ phận đối soát thiếu bằng chứng giao đúng chuyến. |
| Success metric (baseline → target) | Thời gian công trung bình cho việc dò và gắn ảnh (bước 2 và 4, kể cả trường hợp cần thao tác tay) **6 phút giả định → ≤3 phút/phiếu**. Đo thêm tổng phút của tài xế và điều phối để phát hiện chuyển việc sang tài xế, cùng tỷ lệ lần giao đủ hồ sơ trước giờ chốt ngày. Không có phiếu gắn nhầm trong bộ thử đã đối chiếu với dữ liệu chuyến. |
| Phương án không dùng AI | Sinh mã duy nhất cho mỗi lần giao và gửi tài xế liên kết có điền sẵn mã. Bắt buộc ảnh và trạng thái giao đủ/thiếu. Xác thực mã và tuyến theo dữ liệu phân công, chặn nộp trùng, chuyển phiếu giao thiếu hoặc thiếu bằng chứng sang điều phối kiểm. |
| Giả thuyết về AI (nếu có) | Thử đọc mã và ghi chú viết tay trên ảnh cũ hoặc ảnh từ đối tác chưa dùng được biểu mẫu. Điều phối xác nhận khi thiếu mã, ảnh mờ hoặc nhiều lần giao có thể khớp. |
| Cảm nhận nhanh | **No AI + Rule.** Ghi mã có cấu trúc ngay lúc nộp ảnh giúp bỏ bước dò tên và giảm rủi ro nhầm hai chuyến của cùng khách. |

Quy trình nháp hiện tại:

```text
[1. Chụp và gửi ảnh vào nhóm chat: 2 phút]
→ [2. Mở ảnh và dò đúng lần giao: 5 phút] ← BƯỚC NGHẼN
→ [3. Kiểm chữ ký và ghi chú giao thiếu: 1 phút]
→ [4. Gắn ảnh và cập nhật ERP: 1 phút]
```

### Card muốn pitch nhất

- **Card số 1 — Nhập đơn đặt hàng vào ERP.**
- **Vì sao:** Có khối lượng lớn và dữ liệu gốc để so ba cách trên 50 đơn chia theo loại đầu vào. Nếu đạt mức 8 → 5 phút trên toàn bộ đơn, kịch bản 600 đơn cho khoảng 30 giờ công giải phóng mỗi tháng. Đây là cơ sở để đánh giá lợi ích trước khi tính chi phí triển khai và vận hành.
- **Câu hỏi muốn nhóm phản biện:** Nếu phần lớn đơn nhập được bằng mẫu chuẩn và bảng ánh xạ tên hàng, nhóm sẽ dùng kết quả nào trên phần đơn còn lại để chứng minh AI giúp giảm công mà vẫn giữ đúng mã, số lượng và đơn vị tính?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| **1. Logic tài chính — CFO:** 22,6 triệu đồng/tháng của CP1 là giá trị quy đổi từ giờ công giả định. Dùng toàn bộ số đó làm lợi ích của AI sẽ tính luôn thời gian bắt buộc phải rà soát và bỏ qua chi phí triển khai, duy trì bảng mã, sửa lỗi. Thời gian giải phóng cũng chỉ chuyển thành tiền khi giảm được chi thực tế hoặc có cách sử dụng công suất đó. | Có | Ghi rõ số nào là giả định. Tính giờ giải phóng từ chênh lệch thời gian trước và sau trên cùng phạm vi, gồm công kiểm tra và xử lý tay. Khi xét ROI, quy đổi phần công suất thực sự dùng được rồi trừ chi phí triển khai phân bổ và vận hành. |
| **2. Metric vận hành — Trưởng phòng Vận hành:** Phút trung bình không cho biết đơn có kịp giờ chốt, hàng có bị soạn sai hay phiếu có gắn đúng chuyến. Chỉ đo hồ sơ hệ thống xử lý được sẽ bỏ qua ngoại lệ. Giảm công của điều phối bằng cách tăng công của tài xế cũng dễ tạo ra số đẹp trên một bộ phận. | Có | Xác định điểm bắt đầu và kết thúc theo từng card. Dùng cùng mẫu có cả ca thường và ngoại lệ, tính cả xử lý tay, theo dõi thời gian công và chỉ số lỗi riêng. Mẫu 50 đơn dùng để sàng lọc cách làm, cần dữ liệu rộng hơn để kết luận về lỗi hiếm. |
| **3. Logic giải pháp — CFO và Trưởng phòng Vận hành:** CP1 mô tả AI có thể hỗ trợ nhưng chưa chứng minh cần AI ở bước gây tốn công. Các thao tác có khóa định danh, phép tính và điều kiện nghiệp vụ ổn định có thể xử lý bằng mã quy tắc. Kết quả có thể tái hiện và truy vết từng quyết định, thuận tiện khi sửa lỗi hoặc kiểm toán. | Có | Mỗi card có phương án quy tắc để so: bảng mã và kiểm tra trường khi nhập đơn, mã lần giao có sẵn khi nộp phiếu, đối chiếu ba chứng từ khi xử lý hóa đơn. Đo độ bao phủ và chi phí duy trì trước. Chỉ thử AI trên nhóm dữ liệu khó chuẩn hóa còn tốn công sau bước này. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
