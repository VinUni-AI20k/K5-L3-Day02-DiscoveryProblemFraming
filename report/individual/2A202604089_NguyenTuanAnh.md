# Báo cáo cá nhân — 2A202604089_NguyenTuanAnh

## 1. Thông tin học viên

- Họ tên: Nguyễn Tuấn Anh
- MSSV: 2A202604089
- Email trường (không bắt buộc, repo có thể để public):26ai.anhnt14@vinuni.edu.vn
- Tên nhóm: 4Ward
- Link repo nhóm: https://github.com/phungtr/K5-L3B-Day02-4Ward-DiscoveryProblemFraming.git

## 2. CP1 — Scan problems

| # | Lăng kính | Job Story | Dấu hiệu thật |
|---|---|---|---|
| 1 | Lặp lại | Khi cần tìm lại một thông báo hoặc quyết định cũ trong nhóm chat, tôi muốn thấy đúng tin đó ngay, để khỏi phải cuộn hàng trăm tin nhắn. | ~10 phút/lần, 3–4 lần/tuần, cả nhóm 5 người đều gặp |
| 2 | Tốn thời gian | Khi chuẩn bị nộp bài lúc 22h, tôi muốn biết bài còn thiếu mục nào, để không bị trừ điểm vì sai cấu trúc. | ~20 phút đối chiếu đề, 1–2 lần/tuần; từng bị trừ điểm 1 lần |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi ôn thi từ slide, ghi chú và tài liệu tiếng Anh rời rạc, tôi muốn gom ý chính của từng chương vào một chỗ, để ôn xong trong một buổi. | ~3 giờ/môn, mỗi kỳ 5–6 môn, 4/5 bạn trong lớp làm như vậy |
| 4 | Pain từ người khác | Khi làm bài nhóm, tôi muốn biết ai đang làm phần nào và hạn bao giờ, để khỏi phải nhắn hỏi lại. | Nhóm chat có ≥5 tin hỏi lại mỗi tuần, từng có 1 lần trùng phần việc |
| 5 | Tốn thời gian | Khi theo dõi chi tiêu trong tháng, tôi muốn thấy tổng theo từng loại, để biết mình vượt ngân sách ở đâu. | ~30 phút/tháng, dữ liệu ở 3 nơi (ngân hàng, ví điện tử, ghi chú) |
| 6 | Lặp lại | Khi ghi chép buổi học, tôi muốn có ghi chú đã gọn theo ý chính, để khỏi mất thời gian sắp xếp lại sau buổi học. | ~25 phút/buổi, 4 buổi/tuần |

## 3. CP2 — Top 3 Problem Card + quy trình nháp

### Bảng xếp hạng top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tìm lại thông tin cũ trong chat nhóm (#1) | Pain thật, cả nhóm đều gặp, impact rộng (~200 phút/tuần) | Thời gian tìm thật sự là bao nhiêu, mình có đang ước lượng quá cao? |
| 2 | Kiểm tra bài nộp trước deadline (#2) | Quy trình rõ, bottleneck cụ thể, có baseline đo thật (~12 phút, từng mất điểm) | Checklist đã đủ hay cần thêm công cụ khác? |
| 3 | Theo dõi phân công bài nhóm (#4) | Có dấu hiệu thật (≥5 tin hỏi lại/tuần), dễ đo | Nhóm có chịu cập nhật bảng chung không? |

### Problem Card #1 — Tìm lại thông tin cũ trong chat nhóm

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tìm lại một thông báo hoặc quyết định cũ trong nhóm chat, tôi muốn thấy đúng tin đó ngay, để khỏi phải cuộn hàng trăm tin nhắn |
| Actor | Sinh viên trong nhóm 5 người |
| Thời điểm / bối cảnh | Khi làm bài nhóm, cần nhớ lại hạn nộp hoặc quyết định đã chốt trước đó |
| Quy trình hiện tại | 1. Nhớ mang máng (1') · 2. Cuộn chat (6') · 3. Hỏi lại người khác (3') · 4. Chờ trả lời (5') · 5. Xác nhận (1') |
| Bottleneck | Bước 2, cuộn chat tìm thủ công: khoảng 6 phút/lần |
| Impact | ~10 phút/lần × 4 lần/tuần × 5 người = ~200 phút/tuần cả nhóm |
| Success metric | Thời gian tìm từ ~10 phút xuống dưới 2 phút/lần, tự bấm giờ trong 1 tuần |
| Phương án không dùng AI | Ghim tin quan trọng + file "Quyết định chung" cập nhật sau mỗi buổi họp |
| Giả thuyết về AI | Nếu ghim và file chung vẫn không đủ, AI tìm và tóm tắt tin cũ trong chat; người dùng tự kiểm tra lại tin gốc |
| Cảm nhận nhanh | No AI |

```text
HIỆN TẠI — ~16 phút/lần

[Nhớ mang máng: 1'] → [Cuộn chat: 6'] ← BOTTLENECK
→ [Hỏi lại người khác: 3'] → [Chờ trả lời: 5'] → [Xác nhận: 1']
```

### Problem Card #2 — Kiểm tra bài nộp trước deadline

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài lúc 22h, tôi muốn biết bài còn thiếu mục nào, để không bị trừ điểm vì sai cấu trúc |
| Actor | Sinh viên làm bài lab |
| Thời điểm / bối cảnh | Tối ngày deadline, ngay trước khi nộp bài |
| Quy trình hiện tại | 1. Mở đề (2') · 2. Mở bài làm (1') · 3. Đối chiếu từng mục (12') · 4. Sửa chỗ thiếu (5') · 5. Nộp (1') |
| Bottleneck | Bước 3, tự đối chiếu từng mục bằng mắt: khoảng 12 phút/lần |
| Impact | ~20 phút/lần, 1–2 lần/tuần; từng bị trừ điểm vì thiếu mục |
| Success metric | Thời gian đối chiếu từ ~12 phút xuống dưới 3 phút; 0 lần thiếu mục trong 4 bài liên tiếp |
| Phương án không dùng AI | Checklist các mục bắt buộc của từng bài, tick trước khi nộp |
| Giả thuyết về AI | Nếu checklist vẫn bỏ sót lỗi, AI đối chiếu bài với đề và liệt kê mục thiếu; sinh viên kiểm tra lại trước khi nộp |
| Cảm nhận nhanh | No AI |

```text
HIỆN TẠI — ~21 phút/lần

[Mở đề: 2'] → [Mở bài làm: 1'] → [Đối chiếu từng mục: 12'] ← BOTTLENECK
→ [Sửa chỗ thiếu: 5'] → [Nộp: 1']
```

### Problem Card #3 — Theo dõi phân công bài nhóm

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm bài nhóm, tôi muốn biết ai đang làm phần nào và hạn bao giờ, để khỏi phải nhắn hỏi lại |
| Actor | Nhóm trưởng và 4 thành viên |
| Thời điểm / bối cảnh | Trong tuần làm bài nhóm, sau buổi họp chia việc |
| Quy trình hiện tại | 1. Chia việc khi họp (10') · 2. Mỗi người tự nhớ phần mình (0') · 3. Quên hoặc nhầm hạn (0') · 4. Nhóm trưởng nhắn hỏi từng người (8') · 5. Cập nhật lại (4') |
| Bottleneck | Bước 4, nhắn hỏi từng người vì không có nơi ghi chung: khoảng 8 phút/lần |
| Impact | ≥5 tin hỏi lại/tuần; từng có 1 lần trùng phần việc |
| Success metric | Số tin hỏi lại từ ≥5 xuống ≤1 tin/tuần, đếm trong nhóm chat 3 tuần |
| Phương án không dùng AI | Bảng Google Sheets: người, việc, hạn, trạng thái |
| Giả thuyết về AI | Chưa thấy cần AI; chỉ xem xét nếu bảng chung vẫn không ai cập nhật |
| Cảm nhận nhanh | No AI |

```text
HIỆN TẠI — ~22 phút/lần

[Chia việc khi họp: 10'] → [Mỗi người tự nhớ: 0'] → [Quên/nhầm hạn: 0']
→ [Nhóm trưởng nhắn hỏi từng người: 8'] ← BOTTLENECK → [Cập nhật lại: 4']
```


### Card chọn để pitch

- **Card:** #2
- **Câu hỏi muốn nhóm phản biện:** Checklist đã đủ giải quyết chưa, hay thật sự cần thêm gì nữa?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #2: Actor "sinh viên làm bài lab" quá rộng, chưa rõ ai và nộp theo quy định nào | Đồng ý | Thu hẹp Actor thành sinh viên lớp này nộp bài lab theo cấu trúc giảng viên yêu cầu |
| Card #2: 12 phút đối chiếu có thể chỉ là cảm giác, chưa có baseline đo thật | Đồng ý | Ghi baseline là tự bấm giờ 3 bài lab gần nhất, thay vì ước lượng |
| Card #1: 10 phút/lần có thể bị thổi phồng; ghim tin hoặc file chung có thể đã đủ | Đồng ý một phần | Ghi rõ impact là ước lượng cần bấm giờ 1 tuần; giữ phương án không dùng AI là lựa chọn đầu tiên |
| Card #2: Đang nhảy sang AI quá sớm, checklist đã có thể đủ | Không | Giữ nguyên: giả thuyết AI chỉ xét sau khi checklist thử và vẫn bỏ sót lỗi, cảm nhận nhanh vẫn là No AI |