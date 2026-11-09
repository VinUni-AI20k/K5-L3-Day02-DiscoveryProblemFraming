# Báo cáo cá nhân — 2A202604089_NguyenTuanAnh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Tuấn Anh
- MSSV: 2A202604089
- Email trường (không bắt buộc, repo có thể để public):26ai.anhnt14@vinuni.edu.vn
- Tên nhóm: 4Ward
- Link repo nhóm: https://github.com/phungtr/K5-L3B-Day02-4Ward-DiscoveryProblemFraming.git

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story | Dấu hiệu thật |
|---|---|---|---|
| 1 | Lặp lại | Khi cần tìm lại một thông báo hoặc quyết định cũ trong nhóm chat, tôi muốn thấy đúng tin đó ngay, để khỏi phải cuộn hàng trăm tin nhắn. | ~10 phút/lần, 3–4 lần/tuần, cả nhóm 5 người đều gặp |
| 2 | Tốn thời gian | Khi chuẩn bị nộp bài lúc 22h, tôi muốn biết bài còn thiếu mục nào, để không bị trừ điểm vì sai cấu trúc. | ~20 phút đối chiếu đề, 1–2 lần/tuần; từng bị trừ điểm 1 lần |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi ôn thi từ slide, ghi chú và tài liệu tiếng Anh rời rạc, tôi muốn gom ý chính của từng chương vào một chỗ, để ôn xong trong một buổi. | ~3 giờ/môn, mỗi kỳ 5–6 môn, 4/5 bạn trong lớp làm như vậy |
| 4 | Pain từ người khác | Khi làm bài nhóm, tôi muốn biết ai đang làm phần nào và hạn bao giờ, để khỏi phải nhắn hỏi lại. | Nhóm chat có ≥5 tin hỏi lại mỗi tuần, từng có 1 lần trùng phần việc |
| 5 | Tốn thời gian | Khi theo dõi chi tiêu trong tháng, tôi muốn thấy tổng theo từng loại, để biết mình vượt ngân sách ở đâu. | ~30 phút/tháng, dữ liệu ở 3 nơi (ngân hàng, ví điện tử, ghi chú) |
| 6 | Lặp lại | Khi ghi chép buổi học, tôi muốn có ghi chú đã gọn theo ý chính, để khỏi mất thời gian sắp xếp lại sau buổi học. | ~25 phút/buổi, 4 buổi/tuần |

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Card 1 — Tìm lại thông tin cũ trong chat nhóm

- **Job Story:** Khi cần tìm lại một thông báo hoặc quyết định cũ, tôi muốn thấy đúng tin đó ngay, để khỏi cuộn hàng trăm tin nhắn.
- **Actor:** Sinh viên trong nhóm 5 người.
- **Bottleneck:** Cuộn và tìm thủ công vì chat không có cấu trúc, ~6 phút/lần.
- **Impact:** ~10 phút × 4 lần × 5 người = ~200 phút/tuần cả nhóm.
- **Success metric:** Từ ~10 phút xuống dưới 2 phút/lần, tự bấm giờ trong 1 tuần.
- **Phương án không dùng AI:** Ghim tin quan trọng, tạo một file "Quyết định chung" cập nhật sau mỗi buổi họp.

```text
HIỆN TẠI — ~16 phút/lần

[Nhớ mang máng: 1'] → [Cuộn chat: 6'] ← BOTTLENECK
→ [Hỏi lại người khác: 3'] → [Chờ trả lời: 5'] → [Xác nhận: 1']
```

### Card 2 — Kiểm tra bài nộp trước deadline

- **Job Story:** Khi chuẩn bị nộp bài lúc 22h, tôi muốn biết bài còn thiếu mục nào, để không bị trừ điểm vì sai cấu trúc.
- **Actor:** Sinh viên làm bài lab.
- **Bottleneck:** Tự đối chiếu từng mục yêu cầu với bài làm bằng mắt, ~12 phút.
- **Impact:** ~20 phút/lần, 1–2 lần/tuần; từng mất điểm vì thiếu mục.
- **Success metric:** Từ ~12 phút xuống dưới 3 phút, và 0 lần thiếu mục trong 4 bài liên tiếp.
- **Phương án không dùng AI:** Checklist các mục bắt buộc của từng bài, tick trước khi nộp.

```text
HIỆN TẠI — ~21 phút/lần

[Mở đề: 2'] → [Mở bài làm: 1'] → [Đối chiếu từng mục: 12'] ← BOTTLENECK
→ [Sửa chỗ thiếu: 5'] → [Nộp: 1']
```

### Card 3 — Theo dõi phân công bài nhóm

- **Job Story:** Khi làm bài nhóm, tôi muốn biết ai đang làm phần nào và hạn bao giờ, để khỏi phải nhắn hỏi lại.
- **Actor:** Nhóm trưởng và 4 thành viên.
- **Bottleneck:** Nhóm trưởng phải nhắn hỏi từng người vì không có nơi ghi chung, ~8 phút/lần.
- **Impact:** ≥5 tin hỏi lại/tuần, từng có 1 lần trùng phần việc.
- **Success metric:** Từ ≥5 tin hỏi lại/tuần xuống ≤1, đếm trong nhóm chat 3 tuần.
- **Phương án không dùng AI:** Bảng Google Sheets có cột người, việc, hạn, trạng thái.

```text
HIỆN TẠI — ~22 phút/lần

[Chia việc trong buổi họp: 10'] → [Mỗi người tự nhớ phần mình: 0']
→ [Quên hoặc nhầm hạn: 0'] → [Nhóm trưởng nhắn hỏi từng người: 8'] ← BOTTLENECK
→ [Cập nhật lại: 4']
```

### Card chọn để pitch

- **Card:** Card 2.
- **Câu hỏi muốn nhóm phản biện:** "Checklist đã đủ giải quyết chưa, hay thật sự cần thêm gì nữa?"
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
