# Báo cáo cá nhân — 2A202603943_NguyenDucHai

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Đức Hải
- MSSV: 2A202603943
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: LuckyTeam
- Link repo nhóm: https://github.com/ndhai255/K5-L3B-DAY02-LuckyTeam-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi nhận đề một lab mới, tôi muốn biết ngay mình cần nộp những file gì và đặt ở đâu, để bắt tay vào làm mà không phải đọc hết README, RULES, RUBRIC, SUBMISSION… | Học viên | Đề Day 02 có 9 file hướng dẫn (6 file ở thư mục gốc + 3 file trong `docs/`). Số phút đọc trước khi bắt tay vào làm: 45 phút/lab |
| 2 | Lặp lại | Khi chuẩn bị nộp bài lab trước deadline, tôi muốn biết bài đã đủ file và đặt tên đúng quy định chưa, để không bị trừ điểm vì sai format | Học viên; coach/TA chấm bài | Checklist trong SUBMISSION.md có 10 mục phải tự rà. Số phút rà mỗi lần nộp: 15 phút; số lần từng bị trừ điểm vì sai format: 0 lần |
| 3 | Tốn thời gian | Khi bắt đầu một lab mới, tôi muốn môi trường (thư viện, API key, phiên bản Python) chạy được ngay, để dành thời gian lab cho nội dung chính thay vì sửa lỗi cài đặt | Học viên; coach/TA phải hỗ trợ lỗi cài đặt | Số phút cài môi trường cho mỗi lab: 20 phút |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi ôn bài trước buổi học hoặc buổi kiểm tra tiếp theo, tôi muốn tìm được đúng phần cần ôn trong slide, video ghi hình và ghi chép cá nhân, để ôn đủ ý mà không phải mở từng nguồn một | Học viên | Số nguồn phải mở cho một chủ đề: 5 nguồn; số giờ ôn: 3 giờ/lần |
| 5 | Pain từ người khác | Khi làm bài nhóm đã chia phần cho từng người, tôi muốn biết ai đang làm phần nào và đã xong tới đâu, để không phải nhắn nhắc deadline hay hỏi lại từng thành viên | Người điều phối nhóm (nhóm trưởng); các thành viên nhóm | Số tin nhắc deadline hoặc hỏi ai đang làm phần nào trong nhóm chat: 12 tin/tuần |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Bỏ** ý cũ ở dòng 5: "Bạn cùng lớp hỏi đi hỏi lại một câu trong nhóm chat lớp". Lý do: chỉ đếm được 4 tin hỏi trùng/tuần, tín hiệu yếu. Các câu hỏi đó xoay quanh đề và cách nộp bài, trùng gốc với ý #1 và #2. Tôi cũng chỉ đứng ngoài quan sát, không nắm được người hỏi đang làm gì.
- **Thay bằng** ý mới ở dòng 5: "Phải nhắc thành viên deadline, hỏi ai đang làm phần nào". Lý do: tôi gặp trực tiếp khi làm bài nhóm, đếm được 12 tin/tuần trong nhóm chat (gấp 3 lần ý cũ), và có thể xem lại tin nhắn làm bằng chứng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Đọc đề lab để biết cần nộp gì (#1) | Gặp ở mọi buổi lab, mọi học viên đều gặp; quy trình rõ, có baseline 45 phút/lab | SUBMISSION.md đã có checklist 10 mục và README đã có bảng "Thứ tự đọc": có thể chỉ cần đọc đúng file trước là đủ, không cần AI |
| 2 | Ôn bài từ nhiều nguồn (#4) | Tốn thời gian nhất trong 5 ý: 3 giờ/lần, phải mở 5 nguồn | Chưa biết đo "ôn đủ ý" thế nào; chưa rõ có tải được video ghi hình không |
| 3 | Nhắc deadline, hỏi tiến độ trong nhóm (#5) | Bằng chứng đếm được ngay trong nhóm chat: 12 tin/tuần | Có thể chỉ cần một bảng phân công chung; chưa chắc thành viên chịu cập nhật bảng |

### Problem Card #1 — Đọc đề lab để biết cần nộp gì

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận đề một lab mới, tôi muốn biết ngay mình cần nộp những file gì và đặt ở đâu, để bắt tay vào làm mà không phải đọc hết README, RULES, RUBRIC, SUBMISSION… |
| Actor | Học viên K5 lớp L3B (tôi), làm lab có cả phần cá nhân và phần nhóm |
| Thời điểm / bối cảnh | Đầu mỗi buổi lab, ngay khi mở repo đề; buổi lab dài 240 phút |
| Quy trình hiện tại (3–7 bước) | 1. Đọc README để nắm tổng quan · 2. Đọc RULES để biết chỗ nào được dùng AI · 3. Đọc CHECKPOINTS và worksheet để biết từng CP làm gì · 4. Đọc RUBRIC và SUBMISSION để biết nộp gì, đặt tên ra sao · 5. Đối chiếu qua lại giữa các file vì cùng một quy định nằm ở nhiều nơi · 6. Tự ghi danh sách việc cần nộp |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5, đối chiếu qua lại giữa các file: khoảng 10 phút/lab. Ví dụ quy tắc đặt tên file báo cáo cá nhân được nhắc ở 4 nơi: README, SUBMISSION, `report/individual/README.md` và đầu file template |
| Impact (nếu không giải thì sao) | 45 phút/lab, gần 1/5 thời lượng buổi lab. Nếu đọc sót một yêu cầu thì mất điểm, ví dụ RUBRIC C1: dưới 5 problem chỉ được tối đa 3/8 điểm |
| Success metric (baseline → target) | Thời gian từ lúc mở đề tới lúc có danh sách việc cần nộp: 45 → dưới 15 phút/lab; không thiếu file bắt buộc nào khi rà checklist SUBMISSION |
| Phương án không dùng AI | Đọc checklist trong SUBMISSION.md trước rồi mới đọc các file khác; tự làm một mẫu checklist dùng lại cho mọi lab; đề nghị coach đặt mục "Cần nộp gì" ngay đầu README |
| Giả thuyết về AI (nếu có) | AI đọc toàn bộ file đề và trích ra danh sách việc cần nộp, mỗi dòng kèm tên file và đoạn gốc để tôi tự kiểm. AI không quyết định thay tôi phần nào được bỏ qua |
| Cảm nhận nhanh | Workflow (cần kiểm xem phương án không dùng AI đã đủ chưa) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 45 phút/lab

[1 Đọc README: 5'] → [2 Đọc RULES: 5'] → [3 Đọc CHECKPOINTS + worksheet: 12']
→ [4 Đọc RUBRIC + SUBMISSION: 8'] → [5 Đối chiếu qua lại giữa các file: 10'] ← BOTTLENECK
→ [6 Tự ghi danh sách việc cần nộp: 5']
```

### Problem Card #2 — Ôn bài từ nhiều nguồn

| Trường | Nội dung |
|---|---|
| Job Story | Khi ôn bài trước buổi học hoặc buổi kiểm tra tiếp theo, tôi muốn tìm được đúng phần cần ôn trong slide, video ghi hình và ghi chép cá nhân, để ôn đủ ý mà không phải mở từng nguồn một |
| Actor | Học viên (tôi), tự ôn ngoài giờ học |
| Thời điểm / bối cảnh | Trước buổi học tiếp theo hoặc buổi kiểm tra; nội dung một chủ đề nằm rải ở 5 nguồn: slide, video ghi hình, ghi chép cá nhân và các tài liệu khác |
| Quy trình hiện tại (3–7 bước) | 1. Xác định chủ đề cần ôn · 2. Mở slide, tìm phần liên quan · 3. Tua video ghi hình tìm đoạn giảng chủ đề đó · 4. Đối chiếu với ghi chép cá nhân và các nguồn còn lại · 5. Gom lại thành một ghi chú ôn tập · 6. Ôn và tự kiểm tra |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, tua video tìm đúng đoạn: khoảng 60 phút/lần, vì phải tua và nghe lại mới biết đoạn nào nói về chủ đề cần ôn |
| Impact (nếu không giải thì sao) | 3 giờ/lần ôn, trong đó khoảng 2 giờ (bước 2–4) là tìm và đối chiếu, chưa phải học. Nếu không giải: ôn thiếu ý hoặc bỏ qua luôn video |
| Success metric (baseline → target) | Thời gian tìm và đối chiếu (bước 2–4): 120 → dưới 40 phút/lần; tổng thời gian ôn: 3 giờ → dưới 2 giờ/lần |
| Phương án không dùng AI | Ghi chép theo mẫu cố định ngay trong buổi học, ghi kèm số slide và mốc thời gian video; nhóm học chia nhau làm mục lục cho video |
| Giả thuyết về AI (nếu có) | AI chuyển video thành bản ghi chữ có mốc thời gian, rồi tìm đoạn khớp chủ đề trong cả 5 nguồn, trả về link tới slide và mốc video. Tôi vẫn học từ nguồn gốc, không học từ bản tóm tắt của AI |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 180 phút/lần ôn

[1 Xác định chủ đề: 10'] → [2 Tìm trong slide: 30'] → [3 Tua video tìm đoạn: 60'] ← BOTTLENECK
→ [4 Đối chiếu ghi chép + nguồn khác: 30'] → [5 Gom ghi chú ôn tập: 30'] → [6 Ôn + tự kiểm tra: 20']
```

### Problem Card #3 — Nhắc deadline, hỏi tiến độ trong nhóm

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm bài nhóm đã chia phần cho từng người, tôi muốn biết ai đang làm phần nào và đã xong tới đâu, để không phải nhắn nhắc deadline hay hỏi lại từng thành viên |
| Actor | Tôi, người điều phối bài nhóm 3–4 người; các thành viên nhóm |
| Thời điểm / bối cảnh | Trong các bài nhóm (ví dụ CP3–CP6 của lab này), từ lúc chia việc tới deadline nộp |
| Quy trình hiện tại (3–7 bước) | 1. Chia việc bằng tin nhắn trong nhóm chat · 2. Kéo lại lịch sử chat để xem ai nhận phần nào · 3. Nhắn hỏi tiến độ từng người và theo dõi trả lời · 4. Nhắc deadline cho người chưa xong · 5. Gom phần của mọi người vào báo cáo chung |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, hỏi tiến độ từng người: khoảng 15 phút/lần, phải chờ từng người trả lời mới biết nhóm đang ở đâu |
| Impact (nếu không giải thì sao) | 12 tin nhắc hoặc hỏi tiến độ mỗi tuần. Nếu không giải: phần nhóm dễ trễ hoặc thiếu. Theo RULES, thành viên không có đóng góp thực tế sẽ không được tính điểm phần nhóm, nên không rõ ai làm gì thì ảnh hưởng cả tới điểm |
| Success metric (baseline → target) | Số tin nhắc deadline hoặc hỏi tiến độ: 12 → dưới 4 tin/tuần; số phần nộp trễ so với hạn nội bộ của nhóm: 0 |
| Phương án không dùng AI | Một bảng phân công chung có người phụ trách, hạn và trạng thái: dùng luôn bảng "Phân công theo checkpoint" trong TEAM.md hoặc GitHub Issues gán người và hạn |
| Giả thuyết về AI (nếu có) | Có thể không cần AI. Nếu bảng chung chưa đủ thì thêm rule nhắc tự động khi tới hạn mà trạng thái chưa đổi. AI chỉ đáng thử nếu cần tự đọc nhóm chat để biết ai đã báo xong, nhưng dễ đọc sai và đụng tới tin nhắn riêng |
| Cảm nhận nhanh | No AI hoặc Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — mỗi vòng kiểm tra tiến độ

[1 Chia việc qua chat: 10', một lần đầu bài] → [2 Kéo lại chat xem ai nhận gì: 5']
→ [3 Hỏi tiến độ từng người: 15'] ← BOTTLENECK → [4 Nhắc deadline người chưa xong: 5']
→ [5 Gom phần vào báo cáo chung: 20']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Cả lớp đều gặp ở mọi buổi lab nên CP4 dễ kiểm chứng bằng cách hỏi bạn ở nhóm khác. Quy trình rõ, có baseline 45 phút, và so sánh được đủ 4 mức No AI / Rule / Workflow / Agent.
- Câu hỏi muốn nhóm phản biện: SUBMISSION.md đã có checklist 10 mục. Vậy vấn đề thật là đề thiếu thông tin, hay là học viên không biết nên đọc file nào trước?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: 45 phút là con số nhớ lại, chưa bấm giờ thật; số phút từng bước mới là ước tính | | |
| Card #1: README đã có bảng "Thứ tự đọc" và SUBMISSION có checklist 10 mục, có thể đang nhảy sang AI quá sớm | | |
| Card #2: Metric chỉ đo thời gian, chưa đo được ôn có đủ ý hay không | | |
| Card #3: Bottleneck thật có thể là bước 1 (chia việc qua tin nhắn, không có chỗ ghi chung), không phải bước 3 | | |

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
