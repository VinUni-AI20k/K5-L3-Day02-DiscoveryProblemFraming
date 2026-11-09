# Báo cáo cá nhân — 2A202603549_HoangVanBao

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Hoàng Văn Bảo
- MSSV: 2A202603549
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhóm 113
- Link repo nhóm: https://github.com/worryveem/K5-L3A-DAY02-113-DiscoveryProblemFraming/tree/main/report

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

|   # | Lăng kính                         | Job Story: Khi… tôi muốn… để…                                                                                                                   | Ai chịu ảnh hưởng?            | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)                                          |
| --: | --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------- | -------------------------------------------------------------------------------------------------- |
|   1 | Lặp lại                           | Khi có vị trí mới cần tuyển, tôi muốn có sẵn bản mô tả công việc theo form chuẩn của công ty, để đăng tin trong ngày thay vì viết lại từ đầu    | HR, trưởng bộ phận            | Mỗi vị trí mất khoảng 40 phút, 6 vị trí/tháng                                                      |
|   2 | Cần đọc tổng hợp nhiều thông tin  | Khi nhận 80 CV cho một vị trí, tôi muốn biết nhanh ai đáp ứng 3 tiêu chí bắt buộc, để chỉ gọi phỏng vấn đúng người                              | HR, trưởng bộ phận, ứng viên  | Đọc 80 CV mất khoảng 4 tiếng/vị trí, đếm lại tháng trước: 3 vị trí                                 |
|   3 | Pain từ người khác                | Khi trưởng bộ phận phỏng vấn xong, họ muốn có sẵn tóm tắt hồ sơ ứng viên trước giờ vào phòng, để không phải mở CV lúc đang ngồi với ứng viên    | Trưởng bộ phận, ứng viên      | Tháng trước 4/10 buổi phỏng vấn bị trưởng bộ phận nhắn xin CV hoặc hỏi lại thông tin trước giờ họp |
|   4 | Tốn thời gian                     | Khi chốt lịch phỏng vấn với ứng viên, tôi muốn thấy ngay giờ trống của người phỏng vấn, để không phải nhắn qua lại nhiều lần                    | HR, người phỏng vấn, ứng viên | Trung bình 6 tin nhắn/ứng viên để chốt lịch, khoảng 25 ứng viên/tháng (đếm từ Zalo)                |
|   5 | Lặp lại                           | Khi ứng viên không đạt, tôi muốn gửi thư từ chối lịch sự có nhắc đúng vị trí và vòng đã qua, để ứng viên không bị bỏ lơ                         | HR, ứng viên                  | Khoảng 70 thư/tháng, mỗi thư 3–4 phút; tháng trước 12 ứng viên nhắn hỏi kết quả vì chưa nhận thư   |
|   6 | Lặp lại                           | Khi ứng viên đã đồng ý nhận việc, tôi muốn có sẵn thư offer đúng mức lương, chức danh và ngày bắt đầu, để gửi trong ngày mà không sai thông tin | HR, ứng viên, kế toán         | Khoảng 25 phút/thư, 5 thư/tháng; quý trước sửa lại 2 thư vì sai ngày bắt đầu                       |
|   7 | Cần đọc, tổng hợp nhiều thông tin | Khi cuối tháng cần báo cáo tuyển dụng cho giám đốc, tôi muốn thấy số CV, số phỏng vấn và số offer ở một chỗ, để không phải gom từ 3 file Excel  | HR, giám đốc                  | Khoảng 90 phút/tháng, tự bấm giờ 2 tháng gần nhất                                                  |
|   8 |                                   |                                                                                                                                                 |                               |                                                                                                    |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-sau khi tự scan 5 ý, mình hỏi AI và giữ lại ý #6 (thư offer) và #7 (báo cáo tháng) vì đo được và là việc thật. Bỏ ý “trợ lý AI quản lý toàn bộ quy trình tuyển dụng” vì quá rộng và không có quy trình thật; bỏ “chatbot 24/7” vì là solution trá hình.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                            | Vì sao chọn                                                      | Điều còn chưa chắc                                                     |
| ---: | ---------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------------- |
|    1 | Sàng lọc CV (#2)                   | Actor rõ, quy trình vẽ được, bước đọc CV tốn nhiều giờ, có số đo | Thế nào là “chọn đúng người”? Tiêu chí của trưởng bộ phận có rõ không? |
|    2 | Thư từ chối ứng viên (#5)          | Việc lặp lại, dễ đo, vừa sức một buổi lab                        | Mail merge thường có thể giải quyết gần hết, AI có thật sự cần?        |
|    3 | Tóm tắt hồ sơ trước phỏng vấn (#3) | Pain thật từ người khác, có bằng chứng đếm được                  | Trưởng bộ phận có chịu đọc bản tóm tắt không?                          |

### Problem Card #1: Sàng lọc CV

| Trường                                    | Nội dung                                                                                                                                                                    |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi nhận 80 CV cho một vị trí, tôi muốn biết nhanh ai đáp ứng 3 tiêu chí bắt buộc, để chỉ gọi phỏng vấn đúng người                                                          |
| Actor                                     | HR tuyển dụng, làm việc với trưởng bộ phận                                                                                                                                  |
| Thời điểm / bối cảnh                      | 3–5 ngày sau khi đăng tin, trước khi chốt danh sách phỏng vấn                                                                                                               |
| Quy trình hiện tại (3–7 bước)             | 1. Gom CV từ email và web tuyển dụng · 2. Đọc lại yêu cầu vị trí và 3 tiêu chí · 3. Đọc từng CV · 4. Ghi đạt/không vào Excel · 5. Gửi danh sách cho trưởng bộ phận xác nhận |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, đọc từng CV: khoảng 160 phút, mỗi CV khoảng 2 phút, dễ mệt và bỏ sót ở CV thứ 50 trở đi                                                                             |
| Impact (nếu không giải thì sao)           | 240 phút/vị trí, 3 vị trí/tháng, khoảng 12 giờ/tháng cho 1 HR                                                                                                               |
| Success metric (baseline → target)        | Từ 240 phút xuống dưới 90 phút/vị trí; số ứng viên đạt tiêu chí bị bỏ sót không tăng (kiểm tra mẫu 20 CV)                                                                   |
| Phương án không dùng AI                   | Form ứng tuyển có câu hỏi bắt buộc + lọc từ khóa trong Excel: giảm CV không đạt, nhưng không đọc được CV viết tự do                                                         |
| Giả thuyết về AI (nếu có)                 | AI trích 3 tiêu chí từ mỗi CV vào bảng kèm câu trích dẫn làm bằng chứng; HR duyệt và quyết định                                                                             |
| Cảm nhận nhanh                            | Workflow                                                                                                                                                                    |

Quy trình nháp hiện tại: 240 phút / vị trí

[1 Gom CV: 20'] → [2 Đọc lại tiêu chí: 10'] → [3 Đọc từng CV: 160'] ← BOTTLENECK
→ [4 Ghi Excel: 30'] → [5 Gửi trưởng BP xác nhận: 20']

### Problem Card #2

| Trường                                    | Nội dung                                                                                                                                                    |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi ứng viên không đạt, tôi muốn gửi thư từ chối lịch sự có nhắc đúng vị trí và vòng đã qua, để ứng viên không bị bỏ lơ                                     |
| Actor                                     | HR tuyển dụng                                                                                                                                               |
| Thời điểm / bối cảnh                      | Sau mỗi vòng loại, thường dồn lại gửi cuối tuần                                                                                                             |
| Quy trình hiện tại (3–7 bước)             | Mỗi thư: 1. Tìm tên, vị trí, vòng trong Excel · 2. Mở và copy thư mẫu · 3. Sửa tên, vị trí, vòng, thêm lời nhắn riêng · 4. Gửi email · 5. Đánh dấu “đã gửi” |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, sửa và cá nhân hóa: khoảng 1,5 phút/thư; thư dồn nên ứng viên chờ lâu                                                                               |
| Impact (nếu không giải thì sao)           | 70 thư × 3,5 phút ≈ 245 phút/tháng; 12 ứng viên nhắn hỏi kết quả vì chưa nhận thư                                                                           |
| Success metric (baseline → target)        | Từ 3,5 xuống dưới 1 phút/thư; ứng viên nhắn hỏi còn tối đa 2/tháng; thư gửi trong 3 ngày sau quyết định                                                     |
| Phương án không dùng AI                   | Mail merge từ Excel: có thể xuống khoảng 1 phút/thư nhưng mất lời nhắn cá nhân hóa                                                                          |
| Giả thuyết về AI (nếu có)                 | AI soạn thư theo vòng và lý do chung; HR duyệt lô trước khi gửi                                                                                             |
| Cảm nhận nhanh                            | Workflow                                                                                                                                                    |

Quy trình nháp hiện tại:3,5 phút / thư

[1 Tìm thông tin: 0,5'] → [2 Copy thư mẫu: 0,5'] → [3 Sửa + cá nhân hóa: 1,5'] ← BOTTLENECK
→ [4 Gửi: 0,5'] → [5 Đánh dấu: 0,5']

### Problem Card #3

| Trường                                    | Nội dung                                                                                                                                                                           |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi trưởng bộ phận sắp phỏng vấn, họ muốn có sẵn tóm tắt hồ sơ ứng viên trước giờ vào phòng, để không phải mở CV lúc đang ngồi với ứng viên                                        |
| Actor                                     | Trưởng bộ phận (người phỏng vấn); HR là người chuẩn bị                                                                                                                             |
| Thời điểm / bối cảnh                      | 15–30 phút trước buổi phỏng vấn                                                                                                                                                    |
| Quy trình hiện tại (3–7 bước)             | 1. Trưởng BP nhắn xin CV, HR tìm trong email · 2. HR gửi file · 3. Trưởng BP đọc CV sát giờ · 4. Trưởng BP nhắn hỏi thêm (trường, lương mong muốn) · 5. Buổi phỏng vấn bắt đầu trễ |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, đọc CV 5 trang sát giờ: khoảng 8 phút, thường đọc dở                                                                                                                       |
| Impact (nếu không giải thì sao)           | Tháng trước 4/10 buổi bị nhắn xin CV hoặc hỏi lại; mỗi lần mất khoảng 4 phút của HR và trễ khoảng 5 phút                                                                           |
| Success metric (baseline → target)        | Từ 4/10 xuống dưới 1/10 buổi bị hỏi lại; buổi phỏng vấn bắt đầu đúng giờ                                                                                                           |
| Phương án không dùng AI                   | HR điền tay form tóm tắt 1 trang theo mẫu cố định: chắc nhưng tốn khoảng 10 phút/ứng viên                                                                                          |
| Giả thuyết về AI (nếu có)                 | AI soạn bản tóm tắt 1 trang theo form từ CV; HR kiểm tra số liệu rồi gửi                                                                                                           |
| Cảm nhận nhanh                            | Workflow                                                                                                                                                                           |

Quy trình nháp hiện tại: ~21 phút (cả HR và trưởng BP)

[1 Tìm CV: 3'] → [2 Gửi file: 1'] → [3 Đọc CV sát giờ: 8'] ← BOTTLENECK
→ [4 Hỏi lại, HR trả lời: 4'] → [5 Phỏng vấn trễ: 5']

### Card muốn pitch nhất

- Card số: #1 (Sàng lọc CV)
- Vì sao: impact lớn nhất (12 giờ/tháng) và có ranh giới rõ: AI chỉ trích bằng chứng, HR vẫn quyết định.
- Câu hỏi muốn nhóm phản biện: “Nếu AI sai, thì bỏ sót một ứng viên tốt hay mời nhầm một ứng viên không đạt, bên nào đáng sợ hơn? Và nhóm nghĩ HR nên kiểm tra lại bao nhiêu CV thì mới đủ yên tâm?”

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                                         | Đồng ý?         | Đã sửa gì                                                                          |
| -------------------------------------------------------------------------- | --------------- | ---------------------------------------------------------------------------------- |
| Baseline 240 phút chỉ dựa trên trí nhớ                                     | Đồng ý          | Bấm giờ thật 2 vị trí gần nhất: 225 và 250 phút, ghi lại vào card                  |
| 3 tiêu chí do trưởng bộ phận đặt, có thể mơ hồ nên AI và HR hiểu khác nhau | Đồng ý một phần | Đưa vào danh sách giả định cần kiểm chứng ở CP4: tiêu chí đã viết rõ, đo được chưa |
| Gợi ý để AI tự loại CV không đạt                                           | Không đồng ý    | Giữ “HR quyết định cuối” làm boundary; AI chỉ trích bằng chứng, không loại ai      |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì?         | Kết quả / ảnh hưởng tới bài nhóm |
| -------------------------- | ---------------------- | -------------------------------- |
| Pitch Problem Card         |                        |                                  |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:    |                                  |
| Nhận phản biện             | Câu hỏi tôi nhận được: | Tôi đã sửa gì:                   |
| Gom cluster / cây OST      |                        |                                  |
| Chọn candidate problem     |                        |                                  |
| Kiểm chứng / research      |                        |                                  |
| Quy trình nhóm             |                        |                                  |
| Problem Statement          |                        |                                  |
| Mức can thiệp AI           |                        |                                  |
| Quyết định                 |                        |                                  |

---

## 5. Dùng AI

| Checkpoint                     | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
| ------------------------------ | ---------------------- | ----------------- | -------------------------- | ----------------------------------- |
| CP1 Scan                       |                        |                   |                            |                                     |
| CP2 Problem Card               |                        |                   |                            |                                     |
| CP4 Research                   |                        |                   |                            |                                     |
| CP5 Quy trình                  |                        |                   |                            |                                     |
| CP5–6 Problem Statement        |                        |                   |                            |                                     |
| CP6 Mức can thiệp / quyết định |                        |                   |                            |                                     |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi _problem → quy trình → metric → boundary → mức can thiệp AI → quyết định_ của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
