# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: LÊ QUANG TRƯỜNG
- MSSV:2A202603663
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:PhungTruongThanh
- Link repo nhóm:https://github.com/okuminhphen/K5-L3A-Day02-PhungTruongThanh-DiscoveryProblemFraming/tree/main

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

|   # | Lăng kính                         | Job Story: Khi… tôi muốn… để…                                                                                                                                                    | Ai chịu ảnh hưởng?                           | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)                                                                                     |
| --: | --------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
|   1 | Cần đọc, tổng hợp nhiều thông tin | Khi kênh Discord của lớp có hơn 100 tin chưa đọc sau một ngày bận, tôi muốn thấy ngay tin nào có hạn nộp hoặc đổi lịch, để không bỏ sót việc cần làm.                            | Học viên lớp L3A (~40 người dùng chung kênh) | Lướt lại ~15 phút/ngày, 5 ngày/tuần = ~75 phút/tuần. Từng bỏ sót 1 tin đổi lịch học. Bằng chứng: ảnh chụp số tin chưa đọc, link tin đổi lịch. |
|   2 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận đề lab trên GitHub gồm 4–5 file (README, CHECKPOINTS, RUBRIC, SUBMISSION), tôi muốn biết ngay mình phải nộp gì, lúc nào và ở đâu, để không phải mở đi mở lại từng file. | Học viên mới làm lab, người chưa quen GitHub | Đọc hết ~20 phút. Trong 1 buổi lab mở lại SUBMISSION.md ≥3 lần để kiểm tra deadline. Bằng chứng: lịch sử tab đã mở, ghi chú tay.              |
|   3 | Lặp lại                           | Khi mỗi buổi lab có deadline khác nhau (sáng 23h59 cùng ngày, chiều/tối 11h59 hôm sau), tôi muốn deadline tự có sẵn trong lịch cá nhân, để không phải chép tay và tính lại giờ.  | Học viên học nhiều buổi mỗi tuần             | Chép tay ~5 phút/buổi, ~3 buổi/tuần = ~15 phút/tuần. Từng nhập nhầm múi giờ 1 lần. Bằng chứng: sự kiện lịch bị sửa lại, ảnh chụp.             |
|   4 | Tốn thời gian                     | Khi 3–4 bạn cùng sửa một file báo cáo rồi `git push`, tôi muốn push một lần là xong, để không bị conflict và phải ngồi gỡ.                                                       | Nhóm 3–4 người làm chung một repo            | Conflict ~2 lần/buổi lab, mỗi lần gỡ ~10 phút = ~20 phút/buổi (trên 240 phút). Bằng chứng: thông báo lỗi Git, commit "merge" trong lịch sử.   |
|   5 | Pain từ người khác                | Khi bạn cùng nhóm chưa biết dùng Git và hỏi lại cách clone, commit, push, tôi muốn bạn ấy tự làm được sau vài phút, để cả nhóm khỏi đứng chờ.                                    | Bạn cùng nhóm chưa quen Git (2/4 người)      | Mỗi lần chỉ ~10 phút, mỗi bạn hỏi lại ~2 lần. Bằng chứng: tin nhắn nhóm kiểu "push sao vậy", ảnh chụp lỗi bạn gửi.                            |
|   6 | Tốn thời gian                     | Khi sắp thi hoặc sắp có bài kiểm tra và tôi có ghi chú rải rác ở nhiều nơi (vở, Discord, Google Docs), tôi muốn gom lại thành một bản ôn, để không mất cả buổi tối đi tìm.       | Học viên ôn bài trước bài kiểm tra           | Gom ghi chú ~60–90 phút mỗi lần, ~1 lần/tháng. Bằng chứng: danh sách ghi chú ở 3 nơi, ảnh chụp.                                               |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- ***

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                                                                               | Vì sao chọn                                                                                        | Điều còn chưa chắc                                                                   |
| ---: | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
|    1 | Hơn 100 tin chưa đọc trên Discord lớp, khó thấy tin có hạn nộp hoặc đổi lịch (CP1 #1) | Actor rõ (~40 học viên), mất ~75 phút/tuần, từng bỏ sót 1 tin đổi lịch, có ảnh chụp làm bằng chứng | Chưa rõ lọc bằng từ khóa có đủ không, hay cần AI để hiểu ngữ cảnh                    |
|    2 | Phải chép tay deadline từng buổi lab vào lịch cá nhân (CP1 #3)                        | Quy trình ngắn, vẽ được, ~15 phút/tuần, từng nhập nhầm múi giờ                                     | Chưa biết deadline có nguồn cố định để lấy tự động không, hay mỗi buổi viết một kiểu |
|    3 | Conflict khi cả nhóm cùng sửa một file rồi `git push` (CP1 #4)                        | Bottleneck rất cụ thể (~20 phút/buổi lab), có thông báo lỗi và lịch sử commit làm bằng chứng       | Chưa chắc nguyên nhân là thiếu kỹ năng Git hay do cách chia việc trong nhóm          |

### Problem Card #1

| Trường                                    | Nội dung                                                                                                                                                       |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi kênh Discord của lớp có hơn 100 tin chưa đọc sau một ngày bận, tôi muốn thấy ngay tin nào có hạn nộp hoặc đổi lịch, để không bỏ sót việc cần làm.          |
| Actor                                     | Học viên lớp L3A (~40 người dùng chung kênh)                                                                                                                   |
| Thời điểm / bối cảnh                      | Cuối ngày hoặc sáng hôm sau, khi mở Discord sau lúc bận học, làm lab hoặc đi làm thêm                                                                          |
| Quy trình hiện tại (3–7 bước)             | Mở Discord → cuộn lên đầu chỗ chưa đọc → đọc lướt từng tin → tự nhận ra tin nào liên quan hạn nộp/đổi lịch → ghi lại vào lịch hoặc ghi chú → quay lại đọc tiếp |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước "đọc lướt từng tin" và "tự nhận ra tin nào quan trọng": ~15 phút/ngày                                                                                     |
| Impact (nếu không giải thì sao)           | Mất ~75 phút/tuần. Có thể bỏ sót thông báo đổi lịch hoặc hạn nộp (đã xảy ra 1 lần)                                                                             |
| Success metric (baseline → target)        | Thời gian xử lý tin chưa đọc: 15 phút/ngày → dưới 3 phút/ngày. Số thông báo quan trọng bị bỏ sót: 1 lần/tháng → 0                                              |
| Phương án không dùng AI                   | Ghim tin quan trọng, quy ước tag `[HẠN NỘP]` / `[ĐỔI LỊCH]` trong tiêu đề tin nhắn, mở bộ lọc thông báo chỉ khi được nhắc tên                                  |
| Giả thuyết về AI (nếu có)                 | AI đọc kênh và tóm tắt mỗi ngày: liệt kê tin có hạn nộp/đổi lịch kèm link tin gốc. Con người vẫn kiểm tra lại link gốc trước khi tin                           |
| Cảm nhận nhanh                            | Workflow                                                                                                                                                       |

Quy trình nháp hiện tại:

```text
[Mở Discord] -> [Cuộn tới chỗ chưa đọc] -> [Đọc lướt từng tin] -> [Tự nhận ra tin quan trọng] -> [Ghi vào lịch/ghi chú] -> [Đọc tiếp]

                                              NGHẼN: ~15 phút/ngày, dễ sót
```

### Problem Card #2

| Trường                                    | Nội dung                                                                                                                                                                        |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi mỗi buổi lab có deadline khác nhau (sáng 23h59 cùng ngày, chiều/tối 11h59 hôm sau), tôi muốn deadline tự có sẵn trong lịch cá nhân, để không phải chép tay và tính lại giờ. |
| Actor                                     | Học viên học nhiều buổi mỗi tuần                                                                                                                                                |
| Thời điểm / bối cảnh                      | Đầu mỗi buổi lab hoặc khi nhận lịch học mới của tuần                                                                                                                            |
| Quy trình hiện tại (3–7 bước)             | Đọc lịch/đề → xác định buổi sáng hay chiều/tối → tính giờ nộp theo múi giờ GMT+7 → mở Google Calendar → tạo sự kiện thủ công → đặt nhắc                                         |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước "tính giờ nộp" và "tạo sự kiện thủ công": ~5 phút/buổi, ~3 buổi/tuần                                                                                                       |
| Impact (nếu không giải thì sao)           | Mất ~15 phút/tuần. Nhập sai giờ hoặc múi giờ thì nộp trễ (đã nhập nhầm 1 lần)                                                                                                   |
| Success metric (baseline → target)        | Thời gian thiết lập deadline: 5 phút/buổi → dưới 30 giây/buổi. Số lần nhập sai giờ: 1 lần/tháng → 0                                                                             |
| Phương án không dùng AI                   | Giáo vụ gửi một file lịch `.ics` chung có sẵn deadline. Học viên chỉ cần bấm "Thêm vào lịch"                                                                                    |
| Giả thuyết về AI (nếu có)                 | Không cần AI. Đây là bài toán quy tắc: buổi sáng = 23h59 cùng ngày, buổi chiều/tối = 11h59 hôm sau                                                                              |
| Cảm nhận nhanh                            | Rule                                                                                                                                                                            |

Quy trình nháp hiện tại:

```text
[Đọc lịch/đề] -> [Xác định sáng hay chiều/tối] -> [Tính giờ nộp GMT+7] -> [Mở Calendar] -> [Tạo sự kiện thủ công] -> [Đặt nhắc]
                                                  ^^^^^^^^^^^^^^^^^^^^^^   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
                                                  NGHẼN: ~5 phút/buổi, dễ nhầm giờ
```

### Problem Card #3

| Trường                                    | Nội dung                                                                                                                                                                    |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi 3–4 bạn cùng sửa một file báo cáo rồi `git push`, tôi muốn push một lần là xong, để không bị conflict và phải ngồi gỡ.                                                  |
| Actor                                     | Nhóm 3–4 người làm chung một repo                                                                                                                                           |
| Thời điểm / bối cảnh                      | Trong buổi lab 4 tiếng, khi cả nhóm cùng viết `group_report.md` và `TEAM.md`                                                                                                |
| Quy trình hiện tại (3–7 bước)             | Mỗi người sửa file trên máy → `git add`/`commit` → `git push` bị từ chối vì người khác đã push → `git pull` → mở file, thấy dấu conflict → ngồi gỡ tay → commit lại và push |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước "thấy dấu conflict và gỡ tay": ~10 phút/lần, ~2 lần/buổi                                                                                                               |
| Impact (nếu không giải thì sao)           | Mất ~20 phút/buổi (khoảng 8% của 240 phút). Có nguy cơ mất nội dung nếu gỡ sai                                                                                              |
| Success metric (baseline → target)        | Số lần conflict mỗi buổi: 2 → 0. Thời gian gỡ lỗi: 20 phút/buổi → 0                                                                                                         |
| Phương án không dùng AI                   | Quy ước: mỗi người chỉ sửa mục của mình, luôn `git pull` trước khi sửa, push ngay sau mỗi lần sửa nhỏ. Hoặc chia mỗi người một file riêng rồi gộp                           |
| Giả thuyết về AI (nếu có)                 | Không cần AI. Nguyên nhân là cách phối hợp, nên giải bằng quy ước nhóm                                                                                                      |
| Cảm nhận nhanh                            | No AI                                                                                                                                                                       |

Quy trình nháp hiện tại:

```text
[Sửa file] -> [add/commit] -> [push bị từ chối] -> [pull] -> [Thấy dấu conflict] -> [Gỡ tay] -> [Commit lại và push]

                                                                NGHẼN: ~10 phút/lần, ~2 lần/buổi
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Ảnh hưởng nhiều người nhất (~40 học viên), mất nhiều thời gian nhất (~75 phút/tuần), đã gây hậu quả thật (bỏ sót 1 thông báo đổi lịch), và là card duy nhất có chỗ hợp lý cho AI.
- Câu hỏi muốn nhóm phản biện: Nếu chỉ lọc theo từ khóa như "deadline", "nộp", "đổi lịch" thì đã đủ chưa? AI chỉ đáng dùng khi từ khóa bỏ sót hoặc nhận nhầm nhiều. Điều đó có đúng không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                                                  | Đồng ý?         | Đã sửa gì                                                                                     |
| ----------------------------------------------------------------------------------- | --------------- | --------------------------------------------------------------------------------------------- |
| Con số 15 phút/ngày chỉ là ước lượng, chưa đo thật                                  | Đồng ý          | Sẽ tự bấm giờ 3 ngày liên tiếp rồi ghi lại số thật                                            |
| Chưa chứng minh phương án không AI (quy ước tag, ghim tin) đã thử và không hiệu quả | Đồng ý          | Thêm bước thử quy ước tag 1 tuần rồi đo lại thời gian                                         |
| AI tóm tắt có thể bỏ sót hoặc hiểu sai tin quan trọng, nguy hiểm hơn việc đọc tay   | Đồng ý một phần | Thêm điều kiện: mỗi mục tóm tắt phải kèm link tin gốc và con người kiểm tra lại trước khi tin |

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
