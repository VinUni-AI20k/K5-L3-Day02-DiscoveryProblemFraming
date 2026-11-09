# Báo cáo cá nhân — 2A202603671_PhamQuynhAnh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Phạm Quỳnh Anh 
- MSSV:2A202603671
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:xyz
- Link repo nhóm:https://github.com/ducminh03/K5-L3A-DAY02-xyz-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc tổng hợp nhiều thông tin  |Khi ôn thi cuối kì tôi cần tổng hợp lại toàn bộ kiến thức cốt lõi để có thể ghi nhớ nhanh chóng   |Sinh viên đại học |mất 4-5 tiếng để ngồi xem lại toàn bộ slide bài giảng để tổng hợp công thức |
| 2 |Lặp lại| Khi phát sinh các khoản chi tiêu nhỏ lẻ trong ngày(tiền ăn, tiền gửi xe, tiền mua đồ), tôi muốn ghi nhận lại số tiền và phân loại vào các khoản mục, để kiểm soát chi tiêu hàng tháng mà không phải nhớ lại và cộng trừ lại vào cuối ngày|Cá nhân |Mất khoảng 15-20p mỗi ngày để tổng hợp lại chi tiêu |
| 3 |Lặp lại |Khi khách hàng muốn hỏi thông tin sản phẩm(giá, kích thước,...)tôi muốn cung cấp thông tin cho khách hàng mà không phải trực page  |Chủ cửa hàng | Tỷ lệ rớt đơn khoảng 40% vào khung giờ 22-7h sáng do khách hàng đợi quá lâu không thấy trả lời|
| 4 |Lặp lại |Khi tập gym/giảm cân, tôi muốn ước tính nhanh lượng calo và protein của suất ăn để điều chỉnh lượng chế độ ăn trong ngày   |Cá nhân  | Mất khoảng 15p mỗi bữa ăn để tra cứu calo cho từng món|
| 5 | Cần đọc, tổng hợp nhiều thông tin|Khi đăng ký tín chỉ vào ngày mở cổng, tôi muốn so sánh nhanh thời khóa biểu của 8‑10 lớp để tránh trùng lịch, để có lịch học hợp lý mà không phải ngồi 2 đêm trên Excel.| Sinh viên| Mất ≈ 4 giờ (2 đêm) dò danh sách lớp; 1 lần trùng giờ → phải đổi lớp, gây lãng phí 1 tuần học.|
| 6 |Pain từ người khác | Khi đối chiếu đơn hàng COD với báo cáo vận chuyển hàng tuần, tôi muốn so khớp nhanh mã đơn và số tiền thực nhận để phát hiện sai lệch, để không để mất tiền công ty.| Chủ shop, nhân viên kế toán|Mất 3‑4 giờ mỗi tuần kiểm tra 500 đơn; 2‑3 đơn có sai lệch > 5 % giá trị. |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Trả lời thông tin sản phẩm và tư vấn khách hàng ngoài giờ hành chính (bán hàng online)	 |ảnh hưởng trực tiếp đến doanh thu cửa hàng |Chưa chắc mức độ sẵn sàng mua hàng thực tế của khách|
| 2 |Ghi nhận và phân loại chi tiêu nhỏ lẻ hàng ngày	 |vấn đề ai cũng từng gặp | Chưa chắc người dùng có duy trid thói quen nhập liệu lâu dài hay không |
| 3 |Tổng hợp kiến thức và công thức cốt lõi từ slide bài giảng khi ôn thi| nhu cầu cấp thiết của sinh viên| dữ liệu slide bài giảng nhiều thông tin, lộn xộn|

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | KKhi khách hàng nhắn tin hỏi thông tin sản phẩm (giá, kích thước, tình trạng còn hàng) ngoài giờ hành chính (22h–7h), tôi (chủ shop) muốn cung cấp thông tin chính xác và tư vấn tức thì cho khách, để giữ chân khách mua hàng mà tôi không phải thức đêm trực page.|
| Actor |Chủ cửa hàng online, nhân viên trực page, khách mua hàng ban đêm |
| Thời điểm / bối cảnh |Khung giờ từ 22h đêm đến 7h sáng hôm sau, khi chủ shop ngủ hoặc không có nhân viên trực ca |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

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
