# Báo cáo cá nhân — 2A202603563_NguyenDucMinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Đức Minh
- MSSV: 2A202603563
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: 3AE
- Link repo nhóm: https://github.com/hoangtukhoi/K5-L3A-Day02-Nhom3AE-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Pain từ người khác | Khi nhận ca, tôi muốn biết ngay ca trước để lại việc gì dở và tiền két có khớp không, để không sót việc hay gánh khoản lệch không phải của mình | Nhân viên ca sau, quản lý cửa hàng | [x] phút/lần giao ca; [x] lần/tháng sót việc hoặc lệch tiền (hỏi [x] người) |
| 2 | Tốn thời gian | Khi hết ca, tôi muốn báo cáo doanh thu, hàng bán và sự cố trong ca cho quản lý, để quản lý nắm tình hình mà không phải gọi hỏi | Trưởng ca, quản lý | [x] phút/báo cáo; [x] lần/tuần quản lý nhắn hỏi lại |
| 3 | Pain từ người khác | Khi có nhân viên mới vào làm, tôi muốn họ tự tra được quy trình (pha chế, thu ngân, đóng cửa), để không phải hỏi lại người cũ nhiều lần | Nhân viên mới, nhân viên kèm | [x] câu hỏi lặp lại/ngày trong tuần đầu; [x] ngày đến khi làm được một mình |
| 4 | Lặp lại | Khi đầu ca có người báo nghỉ đột xuất, tôi muốn tìm nhanh người làm thay, để ca không bị thiếu người | Quản lý, nhân viên trong ca | [x] lần/tháng; [x] phút nhắn gọi tìm người |
| 5 | Lặp lại | Khi khách hỏi cùng một câu (giờ mở cửa, khuyến mãi, đổi trả), tôi muốn trả lời nhanh và đúng, để không làm chậm hàng đợi | Nhân viên thu ngân, khách | [x] lần/ca bị hỏi câu giống nhau |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi cuối tháng tính lương, tôi muốn đối chiếu giờ làm thực tế với lịch ca và đơn xin nghỉ, để trả lương đúng và không bị khiếu nại | Quản lý, nhân viên | [x] giờ/tháng đối chiếu; [x] lần nhân viên khiếu nại sai giờ |

**Dùng AI:** trao đổi với Claude để chọn bối cảnh vận hành cửa hàng/quán. Giữ ý giao ca vì ai cũng hiểu và dễ hỏi người từng làm ca. Bỏ bối cảnh ở xưởng sản xuất vì hôm nay chưa có người để kiểm chứng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Giao ca (#1) | Lặp mỗi ngày, quy trình rõ, dễ hỏi người thật | Pain là sót việc hay lệch tiền? |
| 2 | Báo cáo cuối ca (#2) | Lặp mỗi ca, đo được thời gian | Quản lý có đọc kỹ báo cáo không? |
| 3 | Nhân viên mới hỏi lại quy trình (#3) | Pain từ cả người mới và người kèm | Chỉ nặng ở tuần đầu |

### Problem Card #1 — Giao ca

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận ca, tôi muốn biết ngay ca trước để lại việc gì dở và tiền két có khớp không, để không sót việc hay gánh khoản lệch không phải của mình |
| Actor | Nhân viên bán thời gian ca sau |
| Thời điểm / bối cảnh | Lúc đổi ca, cửa hàng vẫn có khách |
| Quy trình hiện tại | 1. Ca trước đếm két · 2. Kiểm hàng · 3. Ghi sổ / nhắn nhóm chat · 4. Ca sau đọc lại · 5. Đếm lại két · 6. Hỏi lại chỗ chưa rõ |
| Bottleneck | Bước 4–6 (dự đoán): tin quan trọng trôi trong nhóm chat, [x] phút |
| Impact | Sót đơn đặt trước, khách phàn nàn; lệch tiền không rõ ca nào |
| Success metric | Số lần hỏi lại: [x]/tuần → [x]; lệch tiền không rõ nguyên nhân: [x]/tháng → 0 |
| Phương án không dùng AI | Mẫu sổ giao ca cố định, ca sau ký xác nhận |
| Giả thuyết về AI | Chưa cần |
| Cảm nhận nhanh | Rule |

```text
[Đếm két x'] → [Kiểm hàng x'] → [Ghi sổ x'] → [Ca sau đọc x'] ← BOTTLENECK → [Đếm lại x'] → [Hỏi lại x']
```

### Problem Card #2 — Báo cáo cuối ca

| Trường | Nội dung |
|---|---|
| Job Story | Khi hết ca, tôi muốn báo cáo doanh thu, hàng bán và sự cố trong ca cho quản lý, để quản lý nắm tình hình mà không phải gọi hỏi |
| Actor | Trưởng ca |
| Thời điểm / bối cảnh | 10–15 phút cuối ca |
| Quy trình hiện tại | 1. Xem số trên máy bán hàng · 2. Đếm hàng tồn · 3. Nhớ lại sự cố trong ca · 4. Viết tin nhắn báo cáo · 5. Gửi quản lý · 6. Trả lời câu hỏi lại |
| Bottleneck | Bước 3–4: nhớ và viết lại sự cố, [x] phút |
| Impact | Quản lý thiếu thông tin, phải gọi hỏi; sự cố lặp lại không ai ghi nhận |
| Success metric | [x] phút/báo cáo → [x]; số lần quản lý hỏi lại: [x]/tuần → [x] |
| Phương án không dùng AI | Mẫu báo cáo cố định; số liệu lấy thẳng từ máy bán hàng |
| Giả thuyết về AI | Nếu phần sự cố dài, có thể tóm tắt từ ghi chú trong ca |
| Cảm nhận nhanh | Rule / Workflow |

```text
[Xem số x'] → [Đếm tồn x'] → [Nhớ sự cố x'] → [Viết báo cáo x'] ← BOTTLENECK → [Gửi 1'] → [Trả lời hỏi lại x']
```

### Problem Card #3 — Nhân viên mới hỏi lại quy trình

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhân viên mới vào làm, tôi muốn họ tự tra được quy trình (pha chế, thu ngân, đóng cửa), để không phải hỏi lại người cũ nhiều lần |
| Actor | Nhân viên mới và người kèm |
| Thời điểm / bối cảnh | 1–2 tuần đầu đi làm |
| Quy trình hiện tại | 1. Người cũ chỉ miệng · 2. Người mới làm thử · 3. Quên thì hỏi lại · 4. Người cũ dừng việc để chỉ · 5. Lặp lại đến khi thuộc |
| Bottleneck | Bước 3–4: hỏi lại và người cũ phải dừng việc, [x] lần/ngày |
| Impact | Chậm phục vụ giờ đông khách; người cũ mệt; người mới làm sai |
| Success metric | Số câu hỏi lại/ngày: [x] → [x]; số ngày đến khi làm một mình: [x] → [x] |
| Phương án không dùng AI | Sổ tay quy trình ngắn có ảnh, dán tại quầy |
| Giả thuyết về AI | Chưa cần |
| Cảm nhận nhanh | No AI |

```text
[Chỉ miệng x'] → [Làm thử] → [Quên, hỏi lại x'] ← BOTTLENECK → [Người cũ dừng việc chỉ x'] → [Lặp lại]
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: ai cũng hiểu, dễ phỏng vấn người thật, quy trình giống giao ca ở xưởng sản xuất.
- Câu hỏi muốn nhóm phản biện: mẫu sổ giao ca cố định đã đủ chưa?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: quy trình và số phút đang là đoán, chưa hỏi người làm ca thật | | |
| Card #1: bottleneck có thể là "quên ghi" ở bước 3, không phải "đọc lại" | | |
| Card #2: chưa chắc quản lý đọc phần sự cố hay chỉ xem doanh thu | | |

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
