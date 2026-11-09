# Báo cáo cá nhân — 2A202603914_TranGiaBao

> Đổi tên file theo quy tắc `2A202603914_TranGiaBao.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Gia Bảo
- MSSV: 2A202603914
- Email trường: không công khai
- Tên nhóm: HEHEHE
- Link repo nhóm: https://github.com/hoangvu1806/K5-L3B-DAY02-HEHEHE-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (cần bổ sung) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi khách hàng gửi nhiều đợt yêu cầu chỉnh sửa website, tôi muốn tổng hợp đủ yêu cầu và trạng thái xử lý để không bỏ sót khi bàn giao. | Developer, khách hàng | [Số lần/tuần, số phút tổng hợp; bằng chứng ẩn danh] |
| 2 | Tốn thời gian | Khi test web app có nhiều vai trò, tôi muốn ghi rõ bước tái hiện lỗi để developer sửa đúng ngay từ lần đầu. | Tester, developer | [Số lỗi, phút viết ticket; bản ghi bug thật] |
| 3 | Đọc / tổng hợp | Khi khách gửi brief dự án còn mơ hồ, tôi muốn làm rõ phạm vi và luồng nghiệp vụ trước khi báo giá để tránh hiểu sai yêu cầu. | Freelancer, khách hàng | [Số lượt hỏi lại, phút xử lý brief] |
| 4 | Pain từ người khác | Khi khách hàng muốn biết dự án đang ở giai đoạn nào, tôi muốn cung cấp thông tin tiến độ đã xác nhận để họ không phải hỏi nhiều lần. | Khách hàng, PM | [Số lần khách hỏi; tin nhắn đã ẩn danh] |
| 5 | Lặp lại | Khi developer sửa lỗi xong, tôi muốn biết chính xác case nào phải kiểm tra lại để tránh bỏ sót lỗi cũ. | Tester, developer | [Số vòng retest, phút kiểm tra; ticket thật] |

**Ghi chú quá trình chọn vấn đề:** Tôi tập trung vào các khâu thường gặp trong công việc phát triển và kiểm thử website: tiếp nhận yêu cầu, làm rõ phạm vi, theo dõi chỉnh sửa và kiểm thử. Các số liệu ở cột bằng chứng cần được đối chiếu với dự án thực tế. Khi hoàn thiện, tôi sẽ phân biệt vấn đề tự quan sát với ý bổ sung nhờ công cụ hỗ trợ.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp yêu cầu chỉnh sửa website | Luồng công việc rõ, dễ kiểm chứng qua dự án | Tần suất và mức thiệt hại thực tế? |
| 2 | Làm rõ brief trước báo giá | Có tác động trực tiếp tới phạm vi, thời gian | Nguyên nhân nằm ở brief hay cách hỏi khách? |
| 3 | Ghi nhận bug và retest | Có thể đo số phút / ticket và số vòng sửa | Bước nào chậm nhất thực sự? |

### Problem Card #1 — Theo dõi yêu cầu chỉnh sửa

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận feedback nhiều đợt, tôi muốn theo dõi từng yêu cầu và trạng thái để bàn giao không thiếu hạng mục. |
| Actor | Freelancer developer / PM |
| Thời điểm / bối cảnh | Khách gửi feedback sau mỗi bản demo website |
| Quy trình hiện tại | Nhận feedback → đọc/phân loại → đối chiếu yêu cầu cũ → tạo task → sửa web → khách xác nhận |
| Bottleneck | Bước đối chiếu yêu cầu cũ; thời gian: [điền sau khi đo] |
| Impact | Có thể sót feedback, phải xác nhận lại |
| Success metric | Baseline [phút/đợt feedback] → target giảm 25%; đo ít nhất 5 đợt tương đương |
| Phương án không dùng AI | Bảng feedback chuẩn, mã task, người phụ trách, trạng thái |
| Giả thuyết về AI | Gợi ý trích và phân loại yêu cầu từ văn bản đã nhập, có duyệt thủ công |
| Cảm nhận nhanh | Rule hoặc Workflow; cần kiểm chứng |

```text
Nhận feedback [? phút]
  → Đọc/phân loại [? phút]
  → Đối chiếu task cũ [? phút]  ← bước cần đo
  → Ghi task [? phút]
  → Thực hiện sửa [? phút]
  → Gửi khách xác nhận [? phút]
```

### Problem Card #2 — Làm rõ brief trước báo giá

| Trường | Nội dung |
|---|---|
| Job Story | Khi brief dự án thiếu thông tin, tôi muốn xác định câu hỏi và phạm vi cần làm rõ để báo giá có cơ sở. |
| Actor | Freelancer / BA / khách hàng |
| Thời điểm / bối cảnh | Trước khi ký hợp đồng triển khai website/phần mềm |
| Quy trình hiện tại | Nhận brief → đọc → liệt kê điểm thiếu → hỏi khách → chốt phạm vi → ước lượng |
| Bottleneck | Bước phát hiện thông tin thiếu và chờ phản hồi; [điền thời gian đo được] |
| Impact | Nguy cơ sai phạm vi, phải sửa báo giá |
| Success metric | Baseline [lượt hỏi lại/brief] → target giảm 20%; đánh giá trên ít nhất 3 brief so sánh được |
| Phương án không dùng AI | Checklist discovery và biểu mẫu xác nhận phạm vi |
| Giả thuyết về AI | Tìm điểm mơ hồ trong brief và đề xuất câu hỏi, không tự chốt yêu cầu |
| Cảm nhận nhanh | No AI hoặc Workflow |

```text
Nhận brief [? phút]
  → Đọc/ghi chú [? phút]
  → Phát hiện điểm thiếu [? phút]  ← bước cần đo
  → Trao đổi/chờ khách [? phút hoặc giờ]
  → Xác nhận phạm vi [? phút]
  → Báo giá [? phút]
```

### Problem Card #3 — Bug report & retest

| Trường | Nội dung |
|---|---|
| Job Story | Khi kiểm thử sản phẩm nhiều luồng, tôi muốn ghi lỗi tái hiện được và theo dõi lịch sử sửa để không bỏ sót khi retest. |
| Actor | Tester/QA và developer |
| Thời điểm / bối cảnh | Trước nghiệm thu, sau các bản fix |
| Quy trình hiện tại | Chọn case → thao tác → tái hiện lỗi → chụp bằng chứng → viết ticket → dev sửa → retest |
| Bottleneck | Bước tái hiện lỗi và viết ticket; [điền thời gian đo được] |
| Impact | Tốn thời gian trao đổi và nguy cơ bug bị reopen |
| Success metric | Baseline [phút/ticket, % ticket phải làm rõ] → target giảm 20% phút/ticket; đo trên mẫu lỗi tương đương |
| Phương án không dùng AI | Template bug report bắt buộc Steps / Expected / Actual / Evidence |
| Giả thuyết về AI | Hỗ trợ tóm tắt log và soạn draft bug report, tester xác nhận |
| Cảm nhận nhanh | Rule / Workflow |

```text
Chọn case [? phút]
  → Chạy test [? phút]
  → Tái hiện lỗi [? phút]  ← bước cần đo
  → Lưu ảnh/video [? phút]
  → Viết ticket [? phút]
  → Developer fix [? phút]
  → Retest [? phút]
```

### Card muốn pitch nhất

- Card số: **1**
- Vì sao: Việc quản lý feedback có điểm bắt đầu và kết thúc rõ, dễ đối chiếu với lịch sử task và các lần bàn giao.
- Câu hỏi muốn nhóm phản biện: **"Nếu chuẩn hóa cách ghi nhận feedback bằng một bảng task chung, vấn đề bỏ sót yêu cầu còn xảy ra ở bước nào?"**

### Phản biện của AI đối với Problem Cards (theo yêu cầu CP2)

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa có số liệu chứng minh tốn thời gian | Cần tự xác minh | Để trống baseline, yêu cầu đo từ case thật |
| Chưa chứng minh AI cần thiết | Cần kiểm chứng | Thêm phương án checklist/bảng task không AI |
| Chưa tách thời gian làm và thời gian chờ phản hồi | Cần tự xác minh | Tách hai loại thời gian trong Card #2 |

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

- [Đề bài CHECKPOINTS](../../CHECKPOINTS.md)
- [Quy định sử dụng AI](../../RULES.md)
- [Rubric](../../RUBRIC.md)
- [Bổ sung nguồn tài liệu thực tế sau khi xác minh]
