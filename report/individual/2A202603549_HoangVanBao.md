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

| Hoạt động                  | Tôi đã làm gì?                                                                                                                                                                                                                                                                                                                                                                                                               | Kết quả / ảnh hưởng tới bài nhóm                                                                                                                                                                                                                  |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pitch Problem Card         | Pitch 3 card: #1 Sàng lọc CV (đọc 80 CV mất 225–250 phút/vị trí), #2 Thư từ chối ứng viên (70 thư/tháng, 1,5 phút/thư), #3 Tóm tắt hồ sơ trước phỏng vấn (8 phút đọc CV sát giờ)                                                                                                                                                                                                                                             | Cả 3 card vào bảng Pitch (dòng 1–3). Card #1 vào shortlist chấm điểm (26 điểm, xếp cuối)                                                                                                                                                          |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: (1) Với #4 của Hoàng: "Nếu lúc họp ghi chép vội, viết tắt hay nói đùa thì AI có gán nhầm việc cho người khác không?"; (2) Với #8 của Hạ: "Tech Lead và PM Lead đã thống nhất được cách tính độ nghiêm trọng chưa, hay mỗi người một quan điểm?"; (3) Với #11 của Thành: "Thêm bước xác nhận cũng tốn thời gian chờ; nếu người giao trả lời chậm thì tổng thời gian có còn ít hơn 25 phút làm lại không?" | Câu hỏi (1) góp vào lý do loại card của Hoàng (rủi ro AI hiểu sai ngữ cảnh ghi chép). Câu hỏi (2) chỉ ra tiêu chí chưa rõ ở card của Hạ. Câu hỏi (3) làm rõ phải so sánh tổng thời gian trước/sau                                                 |
| Nhận phản biện             | Câu hỏi tôi nhận được: Hoàng hỏi #1: "Không có AI thì cách đơn giản nhất để giảm một nửa thời gian là gì? Có dùng form lọc trước được không?"; Thành hỏi #2: "Mail merge kết hợp template có sẵn đã giải được chưa mà phải cần AI?"; Hạ hỏi #3: "Ai ngoài bạn gặp vấn đề này? Có bằng chứng sếp phàn nàn vì không kịp đọc CV không?"                                                                                         | Tôi đã sửa gì: ghi thêm phương án không dùng AI cho #1 (form ứng tuyển + lọc từ khóa Excel) và #2 (mail merge, thừa nhận có thể giải được gần hết); với #3 thừa nhận mới có bằng chứng của riêng tôi, cần thêm người khác xác nhận **[xác nhận]** |
| Gom cluster / cây OST      | Đưa 3 card vào cluster: #1 vào B (Phân loại & xử lý yêu cầu định kỳ), #3 vào C (Tổng hợp & chuẩn hóa tài liệu), #2 vào D (Phản hồi & giao tiếp tự động)                                                                                                                                                                                                                                                                      | #2 đứng riêng một cluster (D) vì chưa trùng ai. Nhóm đưa 3 phương án solution đội lốt vào danh sách gạch bỏ khi dựng cây OST **[xác nhận phần bạn đóng góp ở bước này]**                                                                          |
| Chọn candidate problem     | Tham gia chấm điểm shortlist 4 candidate (7 tiêu chí, thang 1–5); card của tôi (#1) được 26/35, thấp nhất. Tôi đồng ý nhóm chọn bài của Thành (34/35)                                                                                                                                                                                                                                                                        | Nhóm chọn "Theo dõi ai đã nắm deadline". Lý do loại card #1: cần tập CV thật, liên quan chính sách tuyển dụng, nhóm ít hiểu domain nên khó kiểm chứng trong một buổi lab                                                                          |
| Kiểm chứng / research      | **[xác nhận]** Ví dụ: tham gia phỏng vấn theo The Mom Test (nhóm có 3 buổi: 2 nhóm trưởng, 1 thành viên) và/hoặc tìm hiểu công cụ có sẵn (Zalo poll, Trello/Notion, Geekbot)                                                                                                                                                                                                                                                 | Kết quả phỏng vấn: nhóm trưởng mất 30–40 phút/tuần nhắn riêng giục người; thành viên phản bác rằng có khi biết hạn nhưng bị dồn bài môn khác. Nhờ đó nhóm chuyển problem sang cơ chế xác nhận 2 chiều, không chỉ gửi tin nhắc                     |
| Quy trình nhóm             | **[xác nhận]** Ví dụ: tham gia vẽ quy trình hiện tại (5 bước, bottleneck là nhắn riêng từng người, 20 phút/đợt) và quy trình tương lai (Rule + AI + nhóm trưởng duyệt)                                                                                                                                                                                                                                                       | Quy trình trước/sau: 40–50 phút/tuần xuống 10–12 phút/tuần (kỳ vọng)                                                                                                                                                                              |
| Problem Statement          | **[xác nhận]** Ví dụ: góp ý trường Boundary hoặc Success Metric cho v0 và v1                                                                                                                                                                                                                                                                                                                                                 | v1 bổ sung điểm can thiệp AI (soạn nháp tin nhắn nhắc) và trường rủi ro và người kiểm tra                                                                                                                                                         |
| Mức can thiệp AI           | **[xác nhận]** Ví dụ: tham gia so sánh 4 mức (No AI, Rule, Workflow, Agent) và lập luận vì sao không chọn mức đơn giản hơn                                                                                                                                                                                                                                                                                                   | Nhóm chọn Workflow kết hợp Rule: AI chỉ soạn nháp, nhóm trưởng duyệt và gửi                                                                                                                                                                       |
| Quyết định                 | **[xác nhận]** Ví dụ: đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability) và thống nhất ngưỡng dừng                                                                                                                                                                                                                                                                                                                 | Quyết định: Go, phạm vi nhỏ (Pilot) 2 tuần; dừng nếu tỷ lệ bấm xác nhận dưới 50%                                                                                                                                                                  |

---

## 5. Dùng AI

| Checkpoint                     | Tôi dùng AI để làm gì?                                                                                                               | AI hữu ích ở đâu?                                                                                                             | AI sai hoặc hời hợt ở đâu?                                                                                                                                                                          | Tôi sửa gì bằng nhận định của mình?                                                                                                                                                   |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CP1 Scan                       | Tự scan 5 problem trước, sau đó hỏi AI gợi ý thêm các việc lặp lại, tốn thời gian, hoặc gây pain cho người khác mà tôi có thể bỏ sót | Gợi ý thêm 2 ý đáng giữ: thư offer (#6) và báo cáo tuyển dụng cuối tháng (#7), đều đo được và là việc thật của HR             | Gợi ý "trợ lý AI quản lý toàn bộ quy trình tuyển dụng" (quá rộng, không có số đo), "chatbot trả lời ứng viên 24/7" (solution trá hình), "dự đoán ứng viên nghỉ việc" (không từ trải nghiệm của tôi) | Giữ #6, #7 sau khi tự hỏi "mình có thật sự gặp việc này và đo được chưa"; bỏ 4 ý còn lại và ghi lý do bỏ vào báo cáo                                                                  |
| CP2 Problem Card               | Nhờ AI đóng vai "PM hoài nghi" phản biện Problem Card #1 (Sàng lọc CV)                                                               | Chỉ ra 3 điểm yếu: baseline chỉ dựa trí nhớ, tiêu chí do trưởng bộ phận đặt có thể mơ hồ, và gợi ý để AI tự loại CV           | Gợi ý để AI tự loại CV không đạt đi ngược boundary "HR quyết định cuối"; baseline ban đầu là số ước lượng, chưa có phép đo thật                                                                     | Đồng ý sửa baseline: bấm giờ lại 2 vị trí gần nhất (225 và 250 phút); đưa "tiêu chí đã đủ rõ chưa" vào giả định cần kiểm chứng; không đồng ý cho AI tự loại, giữ "HR quyết định cuối" |
| CP4 Research                   | Ví dụ: nhờ AI lập khung Assumption Map và gợi ý câu hỏi phỏng vấn theo kiểu hỏi chuyện đã xảy ra                                     | Phân loại giả định theo Value / Usability / Feasibility / Viability, gợi ý ưu tiên giả định "quan trọng cao, bằng chứng thấp" | AI không có dữ liệu thật của tôi; lời phỏng vấn và số liệu AI viết chỉ là ví dụ minh họa, không phải kết quả kiểm chứng                                                                             | Thay bằng kết quả tôi tự hỏi và đo; dùng câu nói nguyên văn của người được phỏng vấn, không viết lại cho đẹp                                                                          |
| CP5 Quy trình                  | Ví dụ: nhờ AI gợi ý khung quy trình trước/sau và chỗ đặt bước Rule / AI / con người                                                  | Gợi ý tách rõ bước nào là Rule, bước nào AI, bước nào người duyệt và phương án quay về                                        | Ví dụ: ước lượng thời gian sau (10–12 phút/tuần) quá lạc quan, chưa có thử nghiệm                                                                                                                   | Ví dụ: ghi thời gian "sau" là kỳ vọng, chờ pilot kiểm chứng; thêm rủi ro mới "bấm xác nhận bừa"                                                                                       |
| CP5–6 Problem Statement        | Đưa Problem Statement v0 cho AI hoặc nhóm khác phản biện, rồi sửa thành v1                                                           | Gợi ý 2 phản biện: thành viên bấm "Đã nắm" cho xong mà không làm; có cần AI không hay template cố định (Rule) là đủ           | AI gợi ý hướng tự động hóa rộng hơn phạm vi một buổi lab, và có lúc đề xuất bước mà AI tự nhắn tin cho thành viên                                                                                   | Đồng ý thêm mốc cam kết nộp bản nháp trước hạn 1 ngày; đồng ý một phần về Rule: giữ Workflow kết hợp Rule; từ chối cho AI tự nhắn, giữ boundary AI chỉ soạn nháp                      |
| CP6 Mức can thiệp / quyết định | Ví dụ: nhờ AI so sánh 4 mức (No AI, Rule, Workflow, Agent) và soi 4 rủi ro                                                           | Liệt kê ưu nhược từng mức, nhắc 2 câu hỏi PAIR (hỗ trợ hay giao hẳn, báo nhầm hay bỏ sót tệ hơn)                              | AI có xu hướng chấm rủi ro "Thấp" cho cả 4 loại, chưa có bằng chứng đủ mạnh (mới phỏng vấn 3 người)                                                                                                 | Ví dụ: hạ độ tự tin của rủi ro Value và Viability, giữ quyết định Go phạm vi nhỏ (Pilot) kèm ngưỡng dừng: dưới 50% bấm xác nhận sau 2 tuần thì quay về Google Sheets                  |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5).

6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?
Nghe bài của Hoàng (họp xong gom việc, chuẩn hóa đồ án, ôn thi) và Hạ (họp Triage, phân loại bug), tôi nhận ra bài của mình và của Hạ cùng một dạng: đều là đọc một lượng lớn đầu mục (CV, ticket) rồi mới quyết định, và nhóm xếp chung vào Cluster B. Điều tôi học nhiều nhất là cách các bạn mô tả bottleneck bằng con số cụ thể. Hạ nói buổi họp 45 phút thường lố 15–20 phút, Thành nói 6 tin nhắc mỗi tuần và 2 lần phải nhắc lần hai. Pitch của tôi cũng có số (160 phút/vị trí), nhưng tôi chưa tự hỏi số đó đến từ đâu. Giờ tôi biết một con số chưa có nguồn thì chưa phải bằng chứng.

6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?
Có, và chính tôi cũng bị. Candidate #2 của tôi là “gửi thư từ chối lịch sự có nhắc đúng vị trí”, nghe như một nhu cầu nhưng thực ra tôi đã nghĩ sẵn đến việc AI viết thư. Khi Thành hỏi “mail merge kết hợp template đã giải được chưa mà phải cần AI?”, tôi nhận ra mình chưa chứng minh được template không đủ. Ở cấp nhóm, khi dựng Opportunity Solution Tree, các ý như “chatbot AI nhắn tin nhắc việc” hay “bảng Trello tự đổi màu” đều bị gạch vì là tính năng chứ không phải opportunity. Nhóm xử lý bằng cách viết lại mỗi nhánh thành một nỗi đau của người dùng.

6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.
Có. Với candidate #1 (lọc 80 CV), Hoàng hỏi: “Không có AI thì cách đơn giản nhất để giảm một nửa thời gian là gì? Có dùng form lọc trước được không?” Ban đầu tôi định bảo vệ, nhưng khi nghĩ lại thì form khảo sát 3 tiêu chí bắt buộc đặt ngay lúc ứng viên nộp hồ sơ có thể loại được rất nhiều người, không cần AI đọc CV. Với candidate #3, Hạ hỏi tôi có bằng chứng trưởng bộ phận từng phàn nàn vì không kịp đọc CV không, và tôi không có. Hai câu hỏi đó làm tôi đổi ý: đề tài của mình chưa đủ mạnh để đứng đầu shortlist.

6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?
Có. Tôi tưởng nguyên nhân trễ deadline gần như chỉ là quên hoặc trôi tin nhắn. Nhưng một thành viên phản bác thẳng: nhiều khi họ biết rõ hạn nộp, chỉ là bài môn khác dồn dập nên không kịp làm. Điều này làm giả định #2 của nhóm yếu đi nhiều hơn tôi dự đoán. Tôi cũng bất ngờ vì cả hai nhóm trưởng đều đòi được duyệt tin nhắn trước khi gửi. Tôi từng nghĩ người dùng sẽ thích tự động hóa tối đa, nhưng thực tế họ coi trọng việc giữ hòa khí hơn việc tiết kiệm vài phút.

6.5. Điều khó nhất khi viết Problem Statement là gì?
Với tôi, khó nhất là buộc mình viết bottleneck mà không nhắc đến giải pháp. Khi viết các candidate, tôi quen mở đầu bằng “tôi muốn AI giúp...”, nên khi viết Problem Statement phải kiềm lại để chỉ mô tả ai đang làm gì, mất bao lâu, kẹt ở đâu. Phần Boundary cũng khó: phải quyết định AI không được làm gì (không tự gửi tin, không tự đổi deadline), trong khi theo bản năng tôi thường nghĩ AI càng làm được nhiều càng tốt. Đặt giới hạn trước rồi mới nghĩ mức can thiệp là cách làm ngược với thói quen của tôi.

6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?
Nếu làm lại, tôi sẽ mang đề tài của mình đi phỏng vấn ít nhất 2–3 người làm HR thật trước khi pitch, để có bằng chứng thay vì số ước lượng. Khi nhóm chọn bài của Thành, tôi sẽ phản biện mạnh hơn hai điểm. Thứ nhất, metric “0 lần trễ hạn” quá tuyệt đối và nằm ngoài tầm kiểm soát của công cụ. Thứ hai, nhóm chỉ đồng ý một phần với câu hỏi “Rule template có đủ chưa?”, nên tôi sẽ đề nghị thử so sánh tin nhắn mẫu với tin AI soạn trước khi kết luận cần AI. Tôi cũng sẽ hỏi kỹ hơn về việc đo baseline 45 phút/tuần vì hiện chỉ mới ước lượng.

6.7. Hiểu bài: giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi _problem → quy trình → metric → boundary → mức can thiệp AI → quyết định_ của bài nhóm mình.
Nhóm trưởng sinh viên (4 người) giao việc xong nhưng không biết ai đã thực sự nắm deadline, vì tin nhắn trong nhóm chat bị trôi. Quy trình hiện tại gồm 5 bước, từ giao việc trên nhóm chat đến kiểm tra bài nộp, và tốn khoảng 40–50 phút/tuần của nhóm trưởng. Nút thắt nằm ở bước 3, khi nhóm trưởng phải nhắn riêng từng bạn (khoảng 20 phút/đợt, 2–3 đợt/tuần) và thường phải giục lần hai mới có phản hồi. Vì vậy nhóm đo thành công bằng việc giảm thời gian theo dõi từ 45 xuống dưới 12 phút/tuần và có tỷ lệ xác nhận nắm deadline cao trong 24h đầu. Ranh giới an toàn là AI chỉ soạn nháp tin nhắc, không tự gửi tin và không được đổi deadline, nên nhóm trưởng luôn là người duyệt và bấm gửi. Nhóm chọn mức Workflow kết hợp Rule: Rule ghi nhận ai đã bấm xác nhận, còn AI chỉ can thiệp ở bước soạn tin nhắc cho người chưa bấm sau 24h. Mức này được chọn thay vì thuần Rule vì tin nhắn mẫu lặp lại dễ bị coi là spam, và thay vì Agent vì nhắn nhầm hoặc nhắn thô lỗ sẽ làm mất hòa khí trong nhóm. Với bốn rủi ro được đánh giá thấp, quyết định là Go ở phạm vi nhỏ: pilot 2 tuần, và quay về Google Sheets nếu tỷ lệ xác nhận dưới 50% hoặc việc duyệt tin tốn thời gian hơn tự gõ.

---

## 7. Tài liệu tham khảo

Savoia, A. (2019). The Right It: Why So Many Ideas Fail and How to Make Sure Yours Succeed. HarperOne. → Mục 8.2 (pilot nhỏ nhất, ngưỡng dừng)

Fitzpatrick, R. (2013). The Mom Test: How to Talk to Customers & Learn If Your Business Is a Good Idea When Everyone Is Lying to You. CreateSpace. → Mục 3.2 (phỏng vấn kiểm chứng)

Torres, T. (2021). Continuous Discovery Habits. Product Talk LLC. → Mục 2.3 (Opportunity Solution Tree)

Cagan, M. (2017). Inspired: How to Create Tech Products Customers Love (2nd ed.). Wiley. → Mục 8.1 (bốn rủi ro)

Google PAIR. People + AI Guidebook. https://pair.withgoogle.com/guidebook → Mục 6.4 (augment vs automate, báo nhầm vs bỏ sót)

-
