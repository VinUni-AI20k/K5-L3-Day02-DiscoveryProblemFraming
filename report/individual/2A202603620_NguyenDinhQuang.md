# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Nguyễn Đình Quang  
- MSSV:2A202603620
- Email trường (không bắt buộc, repo có thể để public):26ai.quangnd@vinuni.edu.vn
- Tên nhóm:PhuongHoang
- Link repo nhóm:https://github.com/VinUni-AI20k/K5-L3-Day02-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi bắt đầu mỗi tiết học, tôi muốn biết nhanh ai có mặt mà không phải gọi tên từng em, để dành thời gian cho bài giảng | Giáo viên, trợ giảng | Bấm giờ điểm danh 5 tiết liên tiếp; đếm số tiết/ngày; số phút/tuần cộng dồn |
| 2 | Lặp lại | Khi mỗi tiết đổi giáo viên, tôi muốn biết em nào vắng từ tiết trước, để không phải hỏi lại cả lớp | Giáo viên bộ môn, học sinh | Đếm số lần phải hỏi lại trong 1 ngày học; số phút mỗi lần |
| 3 | Tốn thời gian | Khi có em vào lớp muộn, tôi muốn ghi nhận đúng giờ mà không ngắt bài giảng, để không ghi nhầm thành vắng | Giáo viên, học sinh đến muộn | Số em muộn/tiết; số lần bị ngắt bài/tiết; số ca ghi vắng sai thực ra là muộn trong học kỳ |
| 4 | Tốn thời gian | Khi cuối tuần hoặc cuối kỳ, tôi muốn có số liệu chuyên cần của cả lớp, để không phải nhập lại từ sổ giấy vào Excel | Giáo viên, giáo vụ | Bấm giờ một lần nhập và tổng hợp; số lớp/số sổ phải xử lý; số lỗi nhập phát hiện được |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi có em vắng nhiều bất thường, tôi muốn nhận ra sớm từ dữ liệu chuyên cần, để kịp hỏi thăm trước khi quá muộn | Giáo viên chủ nhiệm, học sinh | Hỏi giáo viên: lần gần nhất phát hiện em bỏ học dần là khi nào, bằng cách nào, sớm hay muộn mấy tuần |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi có khiếu nại "em có đi mà", tôi muốn kiểm chứng nhanh bằng dữ liệu, để không phải tranh cãi dựa vào trí nhớ | Giáo viên, giáo vụ, học sinh | Số khiếu nại/học kỳ; mất bao lâu để giải quyết một ca; cần đối chiếu mấy nguồn (sổ, Excel, tin nhắn) |
| 7 | Pain từ người khác | Khi bị ghi vắng dù có đi học, tôi muốn được xác nhận lại nhanh, để không bị trừ điểm oan | Học sinh | Hỏi 3-5 em: lần gần nhất bị ghi sai là khi nào, chuyện gì xảy ra sau đó, mất mấy ngày để sửa |
| 8 | Pain từ người khác | Khi con vắng mặt ở trường, tôi muốn biết sớm, để không phải lo hoặc chờ đến cuối ngày mới biết | Phụ huynh, giáo viên chủ nhiệm | Hỏi 3-5 phụ huynh: lần gần nhất biết con vắng muộn, họ đã làm gì; đo thời gian từ lúc vắng đến lúc phụ huynh biết |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Điểm danh đầu tiết, kể cả ghi nhận em đến muộn  | Việc lặp mỗi tiết, bấm giờ được ngay. Có nhiều phía để phỏng vấn (giáo viên, trợ giảng, học sinh). Đây là chỗ để so camera với gọi tên theo sơ đồ chỗ ngồi, QR, thẻ quẹt. | Đau nhất ở mất thời gian, ký hộ hay ghi nhầm người đến muộn thành vắng? Nếu chỉ là mất thời gian thì QR hoặc sơ đồ chỗ ngồi đã đủ. Camera cần đồng ý của phụ huynh và nhà trường vì dữ liệu khuôn mặt học sinh là dữ liệu nhạy cảm. |
| 2 | Phụ huynh biết con vắng quá muộn | Đo được độ trễ từ lúc vắng đến lúc phụ huynh biết. Có 3 phía để phỏng vấn (giáo viên chủ nhiệm, văn phòng, phụ huynh). | Chậm ở khâu nhận diện ai vắng hay ở khâu nhắn tin? Nếu là khâu nhắn tin thì camera không giải quyết được. Phụ huynh có thật sự muốn được báo ngay không? |
| 3 | Khiếu nại ghi vắng sai "em có đi mà"  | Có hậu quả cụ thể (bị trừ điểm oan), có hai phía (học sinh và giáo viên/giáo vụ). | Số khiếu nại có đủ nhiều để đáng giải không? Nguyên nhân chính là ký hộ, đến muộn hay nhập sai? Dữ liệu cũ có còn để đối chiếu không? |

### Problem Card #1 (bổ sung quy trình nháp)

Quy trình nháp hiện tại:

```text
[Bắt đầu tiết]
   -> Gọi tên / chuyền danh sách
   -> Học sinh đáp "có" / ký
   -> Em đến muộn vào sau: giáo viên ghi chú tay (hoặc quên)
   -> Nghi ngờ ký hộ? -> Có: đối chiếu thủ công
   -> Nhập lại vào Excel / hệ thống trường
   -> Cuối kỳ tổng hợp chuyên cần, xử lý khiếu nại
Bottleneck giả định: bước "gọi tên / ký" (mất ___ phút/tiết) và bước "em đến muộn" (ghi nhầm thành vắng)
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi con vắng mặt ở trường, tôi muốn biết sớm, để không phải lo hoặc chờ đến cuối ngày mới biết |
| Actor | Phụ huynh (người cần biết); giáo viên chủ nhiệm (người báo); văn phòng/giám thị (người tổng hợp) |
| Thời điểm / bối cảnh | Đầu buổi sáng và đầu mỗi tiết, ngay sau khi giáo viên phát hiện em vắng; trường hợp em đi học nhưng không vào lớp |
| Quy trình hiện tại (3–7 bước) | 1. Giáo viên điểm danh, phát hiện em vắng · 2. Ghi vào sổ đầu bài · 3. Cuối buổi văn phòng thu sổ, tổng hợp danh sách vắng · 4. Giáo viên chủ nhiệm nhắn hoặc gọi phụ huynh · 5. Phụ huynh phản hồi lý do (hoặc không phản hồi) · 6. Ghi nhận có phép / không phép |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả định, cần xác minh: khoảng chờ giữa bước 1 và bước 4 (từ lúc phát hiện vắng đến lúc phụ huynh biết) mất ___ phút/giờ. Chưa biết chậm ở khâu thu sổ hay khâu nhắn tin. |
| Impact (nếu không giải thì sao) | [Bạn tự đo]: ___ giờ trung bình từ lúc vắng đến lúc phụ huynh biết; ___ trường hợp phụ huynh không biết con vắng trong ngày/tháng; ___ giáo viên chủ nhiệm mất bao nhiêu phút/ngày để nhắn. Nếu không giải: phụ huynh lo lắng, em trốn học khó phát hiện sớm, giáo viên mất thời gian nhắn thủ công. |
| Success metric (baseline → target) | Thời gian từ lúc phát hiện vắng đến lúc phụ huynh biết từ ___ → dưới ___ phút; số phụ huynh không biết con vắng trong ngày giảm; không tăng số tin nhắn gây phiền cho phụ huynh |
| Phương án không dùng AI | Giáo viên nhắn phụ huynh ngay sau điểm danh qua nhóm Zalo/app liên lạc của trường; mẫu tin nhắn có sẵn; tin nhắn tự động từ phần mềm quản lý của trường khi giáo viên đánh dấu vắng |
| Giả thuyết về AI (nếu có) | Gần như không cần AI: khâu thông báo là Rule (đánh dấu vắng -> gửi tin theo mẫu). AI chỉ xét nếu cần soạn tin theo từng hoàn cảnh hoặc phân loại lý do phụ huynh trả lời. Boundary: AI không tự gửi tin khi giáo viên chưa xác nhận em vắng thật. |
| Cảm nhận nhanh | Rule (nghiêng về No AI). Camera không giải quyết được nếu nút thắt nằm ở khâu nhắn tin. |

Quy trình nháp hiện tại:

```text
[Giáo viên điểm danh] -> phát hiện em vắng
   -> Ghi vào sổ đầu bài
   -> Cuối buổi: văn phòng thu sổ, tổng hợp danh sách vắng
   -> Giáo viên chủ nhiệm nhắn / gọi phụ huynh
   -> Phụ huynh phản hồi lý do (hoặc im lặng)
   -> Ghi nhận có phép / không phép
Bottleneck giả định: khoảng chờ từ "phát hiện vắng" đến "phụ huynh biết" (___ phút/giờ)
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi bị ghi vắng dù có đi học, tôi muốn được xác nhận lại nhanh bằng dữ liệu đáng tin, để không bị trừ điểm oan và giáo viên không phải tranh cãi dựa vào trí nhớ |
| Actor | Học sinh (người bị ảnh hưởng); giáo viên, giáo vụ (người xử lý khiếu nại) |
| Thời điểm / bối cảnh | Khi công bố chuyên cần giữa kỳ hoặc cuối kỳ; khi học sinh phát hiện mình bị ghi vắng |
| Quy trình hiện tại (3–7 bước) | 1. Học sinh thấy bị ghi vắng · 2. Báo giáo viên ("em có đi mà") · 3. Giáo viên nhớ lại, lục sổ hoặc hỏi bạn cùng lớp · 4. Đối chiếu nhiều nguồn (sổ, Excel, tin nhắn) · 5. Quyết định sửa hoặc giữ nguyên · 6. Cập nhật lại hệ thống, thông báo học sinh |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả định, cần xác minh: bước 3-4 (tìm lại bằng chứng) mất ___ phút/ca, và nhiều ca không có bằng chứng để kết luận. Chưa biết nguyên nhân chính là ký hộ, đến muộn hay nhập sai. |
| Impact (nếu không giải thì sao) | [Bạn tự đo]: ___ khiếu nại/học kỳ; ___ ngày để giải quyết một ca; ___ % ca không có bằng chứng để kết luận. Nếu không giải: học sinh bị trừ điểm oan, mất niềm tin vào số liệu, giáo viên tốn thời gian tranh luận. |
| Success metric (baseline → target) | Thời gian giải quyết một khiếu nại từ ___ → dưới ___ phút; tỷ lệ ca có bằng chứng đối chiếu tăng từ ___ → ___; số khiếu nại do ghi sai giảm |
| Phương án không dùng AI | Lưu điểm danh dạng số có dấu thời gian (Google Sheet, QR có khung giờ); chốt và công bố chuyên cần hằng tuần để học sinh kiểm tra sớm; quy trình khiếu nại có mẫu và hạn xử lý rõ |
| Giả thuyết về AI (nếu có) | Có thể không cần AI: gốc rễ là dữ liệu điểm danh không có dấu vết. AI chỉ xét ở việc gắn cờ bất thường (vắng lẻ tẻ, mẫu ký hộ) để giáo viên xem lại. Boundary: AI không tự quyết ai đúng ai sai; không dùng làm bằng chứng duy nhất. |
| Cảm nhận nhanh | No AI / Rule (chuẩn hóa cách ghi nhận và lưu vết). Chưa biết nếu cần AI phát hiện bất thường. |

Quy trình nháp hiện tại:

```text
[Học sinh thấy bị ghi vắng]
   -> Báo giáo viên "em có đi mà"
   -> Giáo viên nhớ lại / lục sổ / hỏi bạn cùng lớp
   -> Đối chiếu nhiều nguồn (sổ, Excel, tin nhắn)
   -> Quyết định sửa hoặc giữ nguyên
   -> Cập nhật hệ thống, thông báo học sinh
Bottleneck giả định: bước "tìm lại bằng chứng" (___ phút/ca, nhiều ca không có bằng chứng)
```

### Card muốn pitch nhất

- Card số: 1 (Điểm danh đầu tiết, kể cả em đến muộn)
- Vì sao: Đo được ngay bằng bấm giờ, có nhiều phía để phỏng vấn, và là chỗ rõ nhất để so sánh camera với QR, sơ đồ chỗ ngồi, thẻ quẹt. Dù kết luận là No AI/Rule, lập luận so sánh vẫn chặt.
- Câu hỏi muốn nhóm phản biện: Nếu QR có khung giờ đã đủ cho phần lớn lớp học, thì có tình huống nào (lớp đông, học sinh nhỏ tuổi chưa có điện thoại, trốn tiết giữa giờ) khiến camera đếm số người thật sự đáng đầu tư? Hay chúng ta đang chọn camera vì nó hấp dẫn chứ không vì bằng chứng?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|


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
