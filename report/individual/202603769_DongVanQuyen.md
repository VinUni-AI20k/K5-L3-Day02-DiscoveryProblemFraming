# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đồng Văn Quyến
- MSSV: 2A202603769
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: d3
- Link repo nhóm: https://github.com/congnt180263/K5-L3B-Day02-D3-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi vừa meeting với team xong, tôi muốn có 1 bản báo cáo các vấn đề đã họp, cách giải quyết, công việc cần làm và hạn chót để không ai bỏ sót việc | team member | 30-40p/ buổi, 2 buổi/tuần  |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi cần biết vì sao lại chọn phương án A, tôi cần phải đọc nhiều tài liệu liên quan, hỏi nhiều người để có thể nắm bắt được thông tin | team member | 10-20 phút /mail, 5 lần/tuần |
| 3 | Pain từ người khác | Khách hàng gửi cùng 1 loại câu hỏi về đơn hàng/ dịch vụ qua nhiều kênh tới cskh, họ cần được trả lời nhanh chóng, chính xác, nhất quán | khách hàng, cskh | khoảng 40% ticket/tuần là câu hỏi trùng, phản hồi trung bình 4 giờ |
| 4 | Cần tổng hợp nhiều thông tin | Khi làm bài lab, tôi cần tổng hợp nhiều file, nắm rõ các rule, yêu cầu, quy tắc chấm điểm để đạt được kết quả tốt nhất | Học viên | 2 lần / ngày,  5 ngày / tuần |
| 5 | Pain từ người khác · Cần đọc, tổng hợp nhiều thông tin · Lặp lại | Khi nhận bàn giao ca trực của bệnh nhân, bác sĩ cần phải nắm được tình hình sức khỏe, kết quản đang chờ, các công việc còn tồn đọng để đảm bảo sức khỏe bệnh nhân, không bỏ sót công việc | Bác sĩ, điều dưỡng | Bàn giao mất 15–45 phút/lần, 2–3 lần/ngày |
| 6 | Tốn thời gian | Khi cả nhóm cần chốt lịch họp ngoài giờ, tôi muốn tìm được khung giờ mọi người đều rảnh, để không phải nhắn qua lại nhiều lần | Team member |15–20 tin nhắn qua lại/lần chốt lịch, 2 lần/tuần |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- bỏ ý chốt lịch họp ngoài giờ, vì đây là pain nhỏ, gg calendar đã có thể giải quyết được

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Báo cáo sau meeting | Đây là 1 quy trình lặp lại hàng tuần, và cũng quan trọng để có thể kịp tiến độ hoàn thành công việc của team | Biên bản "đủ tốt" đo thế nào, có cần rv lại báo cáo không |
| 2 | Bàn giao ca trực | Vấn đề lớn ảnh hưởng tới sức khỏe của bệnh nhân | Chỉ research trên internet nên chưa thể nắm rõ quy trình |
| 3 | Trả lời CSKH | Quy trình rõ ràng, đa số câu hỏi trùng lặp, đã có sẵn kịch bản trả lời | Đã có nhiều công cụ như chatbot trả lời tự động phục vụ việc giải quyết những vấn đề đơn giản |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa họp team xong, tôi muốn có bản tóm tắt các vấn đề đã bàn, cách giải quyết, việc cần làm, người phụ trách và hạn chót, để không ai bỏ sót việc |
| Actor | Người phụ trách ghi biên bản, team member |
| Thời điểm / bối cảnh | ngay sau buổi họp |
| Quy trình hiện tại (3–7 bước) | 1. Ghi chú tay trong lúc họp · 2. Nghe lại ghi âm hoặc hỏi lại người khác chỗ chưa rõ · 3. Viết lại biên bản (vấn đề, quyết định) · 4. Tách danh sách việc cần làm, gán người và hạn · 5. Gửi lên group/email · 6. Nhắc lại việc khi gần tới hạn |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: viết lại và tách việc mất khoảng 20 phút/buổi, dễ ghi nhầm người phụ trách hoặc thiếu hạn chót |
| Impact (nếu không giải thì sao) | 30–40 phút/buổi × 2 buổi/tuần ≈ 70 phút/tuần cho 1 người; việc bị quên phải bàn lại ở buổi sau |
| Success metric (baseline → target) | Thời gian làm biên bản giảm xuống còn 10p/ lần, phân việc đúng người, deadline được báo trước 2 ngày, số việc bị quên gần bằng 0 |
| Phương án không dùng AI | teamplate biên bản cố định  |
| Giả thuyết về AI (nếu có) | sử dụng stt và ai tự tổng hợp sau đó điền vào form các nội dung, danh sách việc, người thư ký review và chốt biên bản trước khi gửi |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |  Workflow

Quy trình nháp hiện tại: HIỆN TẠI — khoảng 35 phút/buổi

[1 Ghi chú trong họp: (trong giờ họp)] → [2 Nghe lại/hỏi lại: 8']
→ [3 Viết lại biên bản: 12'] → [4 Tách việc + gán người/hạn: 8'] ← BOTTLENECK (3+4 = 20')
→ [5 Format + gửi group: 5'] → [6 Nhắc việc khi tới hạn: 2']

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận bàn giao ca trực, cần nắm đầy đủ diễn biến sức khỏe, thuốc đã dùng, chỉ định đang thực hiện, kết quả đang chờ và việc còn tồn của từng bệnh nhân, để chăm sóc tiếp chính xác và không bỏ sót việc của ca trước |
| Actor | điều dưỡng, bác sĩ |
| Thời điểm / bối cảnh | Giờ giao ca (khoảng 6h30–7h30 và 16h–17h) |
| Quy trình hiện tại (3–7 bước) | 	1. Ca giao ghi sổ bàn giao/hồ sơ · 2. Bàn giao miệng tại phòng trực · 3. Ca nhận đọc lại hồ sơ, y lệnh, kết quả xét nghiệm · 4. Đi buồng kiểm tra bệnh nhân · 5. Gọi/nhắn hỏi lại ca trước chỗ thiếu · 6. Ký nhận bàn giao |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: đọc và đối chiếu hồ sơ, y lệnh, kết quả đang chờ từ nhiều nguồn, khoảng 15–20 phút; hay sót kết quả đang chờ và thay đổi thuốc |
| Impact (nếu không giải thì sao) | 15–45 phút/lần, 2–3 lần/ngày, mọi điều dưỡng đều làm; khoảng 80% sai sót y khoa nghiêm trọng liên quan đến trao đổi thông tin khi bàn giao |
| Success metric (baseline → target) | Số lần phải hỏi lại ca trước/ca giảm, số việc bị đo sót giảm|
| Phương án không dùng AI |Áp dụng bảng kiểm SBAR/I-PASS giấy + bàn giao tại giường. |
| Giả thuyết về AI (nếu có) | AI tóm tắt hồ sơ điện tử của từng bệnh nhân thành mẫu SBAR, đánh dấu kết quả đang chờ và việc tồn; điều dưỡng kiểm tra lại tại giường |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết | Rule

Quy trình nháp hiện tại:
HIỆN TẠI — khoảng 40 phút/lần giao ca (18 bệnh nhân)

[1 Ca giao ghi sổ: 8'] → [2 Bàn giao miệng: 10']
→ [3 Đọc hồ sơ, y lệnh, kết quả chờ: 15'] ← BOTTLENECK
→ [4 Đi buồng kiểm tra: (song song/sau giao ca)] → [5 Hỏi lại ca trước: 5'] → [6 Ký nhận: 2']

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story |	Khi khách hàng gửi cùng một loại câu hỏi về đơn hàng/dịch vụ qua nhiều kênh, họ muốn được trả lời nhanh, chính xác và nhất quán, để không phải hỏi lại hoặc chờ lâu |
| Actor | Nhân viên cskh |
| Thời điểm / bối cảnh | Suốt giờ làm việc, cao điểm khi có đợt sale |
| Quy trình hiện tại (3–7 bước) | 1. Nhận tin nhắn từ nhiều kênh · 2. Đọc và phân loại câu hỏi · 3. Tra cứu đơn hàng trên hệ thống · 4. Tìm câu trả lời mẫu · 5. Soạn và gửi trả lời · 6. Đóng ticket |
| Bottleneck (bước nào, mất bao nhiêu phút) | 	Bước 3–4: tra đơn và tìm câu trả lời đúng chính sách mất khoảng 5–7 phút/ticket, dù 40% là câu hỏi trùng |
| Impact (nếu không giải thì sao) | Khoảng 40% ticket/tuần là câu hỏi trùng; phản hồi trung bình 4 giờ; khách hỏi lại qua kênh khác làm tăng số ticket |
| Success metric (baseline → target) | Thời gian phản hồi trung bình từ 4 giờ xuống dưới 1 giờ với nhóm câu hỏi trùng; tỉ lệ khách hỏi lại giảm |
| Phương án không dùng AI | Bộ câu trả lời mẫu (FAQ/macro) theo 10 loại câu hỏi hay gặp + trang tra cứu đơn hàng cho khách tự xem |
| Giả thuyết về AI (nếu có) | AI phân loại câu hỏi và soạn nháp trả lời từ dữ liệu đơn hàng + chính sách; nhân viên duyệt trước khi gửi |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết | Rule

Quy trình nháp hiện tại:
HIỆN TẠI — khoảng 10 phút/ticket (chưa tính thời gian chờ trong hàng đợi)

[1 Nhận tin nhiều kênh: 1'] → [2 Đọc + phân loại: 1']
→ [3 Tra cứu đơn hàng: 3'] → [4 Tìm câu trả lời/hỏi trưởng nhóm: 3'] ← BOTTLENECK (3+4 = 6')
→ [5 Soạn + gửi: 2'] → [6 Đóng ticket: 0,5']

```text

```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Công việc hàng ngày đểu cần họp mặt với team để có thể cập nhật tiến độ dự án, hoàn thành công việc dự án theo tiến độ
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|  | | |

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
