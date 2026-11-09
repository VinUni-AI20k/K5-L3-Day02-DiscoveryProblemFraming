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
| Card #1: 45 phút là con số nhớ lại, chưa bấm giờ thật; số phút từng bước mới là ước tính | Đồng ý | Không bấm giờ lại được trong buổi nên vẫn giữ 45' làm baseline, nhưng ghi rõ đây là số tự ghi của 1 người. Metric ở Problem Statement v1 đo lại bằng bấm giờ ở 2 lab tiếp theo |
| Card #1: README đã có bảng "Thứ tự đọc" và SUBMISSION có checklist 10 mục, có thể đang nhảy sang AI quá sớm | Đồng ý | Ghi vào "Điều còn chưa chắc" ở bảng top 3 và đưa thành câu hỏi muốn nhóm phản biện. Sau kiểm chứng CP4: bỏ nửa "nộp file gì, đặt ở đâu" vì SUBMISSION đã gom đủ; hạ cảm nhận từ Workflow xuống Rule |
| Card #2: Metric chỉ đo thời gian, chưa đo được ôn có đủ ý hay không | Đồng ý | Chưa sửa metric vì chưa biết đo "ôn đủ ý" thế nào; ghi vào "Điều còn chưa chắc" ở bảng top 3. Card không được chọn ở CP3 nên không làm tiếp |
| Card #3: Bottleneck thật có thể là bước 1 (chia việc qua tin nhắn, không có chỗ ghi chung), không phải bước 3 | Đồng ý | Không sửa card. Ở CP3 Tùng Lâm hỏi đúng ý này; tôi chấp nhận bảng phân công trong TEAM.md là phương án No AI đủ dùng, nhóm loại #3 khỏi shortlist |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch 3 card: #1 Đọc đề lab để biết cần nộp gì, #2 Ôn bài từ nhiều nguồn, #3 Hỏi tiến độ nhóm | Card #1 được chọn làm candidate problem của nhóm: 33 điểm, cao nhất shortlist (group_report mục 2.4) |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: (1) Card #4 của Tùng Lâm: "Nhóm không ai học y. Ai kiểm được lời giải thích là đúng? Có lấy được dữ liệu kết quả không?" (2) Card #7 của Quang Hải: "Job Story gốc có chữ 'tự động gom nhóm': đó là giải pháp. Pain thật nằm ở bước đọc, bước lọc hay bước viết lại? 2,5 giờ/tuần là đo hay ước?" (3) Card #11 của Anh Quân: "Template chính thức cộng Styles của Word đã giải phần lớn. Còn lại phần nào thật sự cần giải?" | #4 bị loại: lĩnh vực y tế, nhóm không ai đủ chuyên môn để kiểm, không có dữ liệu Vinmec. "Tự động gom nhóm" của #7 bị gạch khỏi tầng opportunity trong cây OST; #7 + #12 bị chấm Pain 2 vì chưa có số đo thật. #11 bị loại vì đã có phương án No AI (template + Styles) |
| Nhận phản biện | Câu hỏi tôi nhận được: (1) Anh Quân, card #1: "SUBMISSION.md đã có checklist 10 mục. Vậy đề thiếu thông tin, hay chỉ là không biết đọc file nào trước?" (2) Tùng Lâm, card #1: "45 phút là bấm giờ hay nhớ lại?" (3) Tùng Lâm, card #3: "Bảng phân công trong TEAM.md đã đủ chưa? Bottleneck thật có phải bước 1?" | Tôi đã sửa gì: (1) Sau kiểm chứng, bỏ nửa "nộp file gì, đặt ở đâu" vì SUBMISSION đã gom đủ ở 1 chỗ; giữ và làm rõ nửa "biết đủ điều kiện được và mất điểm" (25 điều kiện rải ở 3 file, 6 điều kiện không có ô tự kiểm). (2) Giữ baseline 45' nhưng ghi rõ đây là số của 1 người, còn yếu; metric ở Problem Statement v1 đo lại bằng bấm giờ ở 2 lab tiếp theo. (3) Chấp nhận bảng phân công là phương án No AI đủ dùng; nhóm loại #3 khỏi shortlist |
| Gom cluster / cây OST | Người chính CP3: điều phối nhóm gom 12 card thành 4 cluster (A Đọc và đối chiếu nhiều tài liệu, B Theo dõi việc trong tin nhắn, C Thiếu thông tin đúng lúc để quyết định, D Trình bày đúng quy chuẩn) và dựng cây OST với 1 outcome, 4 opportunity | Gạch 5 ý là solution đội lốt opportunity: chatbot hỏi đáp đề lab, "tự động gom nhóm" (#7), bot quét chat (#9), layout slide tự động (#8), tô màu giao thông (#6). Cluster C (#4–#6) không nằm dưới outcome vì là chuyện đi lại và sức khỏe, không phải chuyện học (group_report mục 2.2–2.3) |
| Chọn candidate problem | Điều phối chấm shortlist 3 candidate theo 7 tiêu chí (thang 1–5), ghi lý do cho từng ô điểm thấp và lý do loại #6, #7 + #12, #4, #3, #11 | #1 (card của tôi) được chọn với 33 điểm, hơn #6 (25) và #7 + #12 (24). Ghi phần xử lý bất đồng: card chính của Tùng Lâm (#6) và Quang Hải (#7) không được chọn; #6 đưa vào hướng tiếp theo (group_report mục 2.4) |
| Kiểm chứng / research | Hỗ trợ Vũ Quang Hải ở bảng research: dùng AI gợi ý công cụ đã có, rồi tự mở từng link để kiểm (xem mục 5) | Bảng research 4 nguồn, link đều mở được; ghi rõ GitHub Classroom đã ngừng và NotebookLM đã đổi tên. Sau kiểm chứng, problem bỏ nửa "nộp file gì, đặt ở đâu", giữ nửa "biết đủ điều kiện được/mất điểm" (group_report mục 3.2–3.3) |
| Quy trình nhóm | Không phải người chính (Anh Quân). Quy trình nháp 6 bước, 45' của card #1 được dùng làm khung cho quy trình hiện tại | Mục 4.1 giữ 6 bước và số phút của card #1, thêm "fork + đặt tên repo" vào bước 1. Quy trình tương lai khoảng 18', 4/6 bước thủ công, 2 bước Rule (group_report mục 4) |
| Problem Statement | Hỗ trợ Trần Tùng Lâm viết Problem Statement v0 | v0 nhận 5 điểm phản biện từ AI, nhóm đồng ý cả 5. v1 thêm 2 metric (độ phủ 100% điều kiện, 0 lỗi tên), thêm bước fork vào quy trình, viết lại boundary riêng cho Rule (group_report mục 5, 7) |
| Mức can thiệp AI | Card #1 ban đầu tôi ghi cảm nhận Workflow. Nhờ AI phản biện lựa chọn mức; AI nghiêng về Workflow, tôi phản biện lại bằng kết quả Rule bắt đủ 25/25 điều kiện (xem mục 5) | Nhóm chọn Rule kèm đổi thứ tự đọc; Workflow (NotebookLM có trích dẫn) giữ làm phương án dự phòng khi chạm ngưỡng dừng (group_report mục 6.2) |
| Quyết định | Hỗ trợ Nguyễn Anh Quân ở mục 8; ghi quyết định cuối vào TEAM.md và mục 1 của group_report; tổng hợp, biên tập toàn bộ group_report | No-Go cho AI, dùng Rule. Ngưỡng dừng: sau Day 03 và Day 04 mà lệnh gom còn sót tiêu chí hoặc vẫn trên 20' thì lên Workflow; từ 2/3 người được poll mất dưới 15' thì bỏ lệnh gom (group_report mục 8.2) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Sau khi tự scan, nhờ AI gợi ý thêm problem | Gợi ý thêm một ý cho lăng kính "Pain từ người khác": bạn cùng lớp hỏi đi hỏi lại một câu trong nhóm chat lớp | Ý này tín hiệu yếu (tôi chỉ đếm được 4 tin hỏi trùng/tuần), trùng gốc với ý #1 và #2, và tôi chỉ đứng ngoài quan sát, không biết người hỏi đang làm gì | Bỏ ý của AI, thay bằng ý tôi gặp trực tiếp: nhắc deadline, hỏi tiến độ nhóm (12 tin/tuần, xem lại được trong nhóm chat) |
| CP2 Problem Card | Nhờ AI đóng vai PM hoài nghi phản biện 3 Problem Card | Chỉ ra 45' của card #1 là số nhớ lại, chưa bấm giờ; README và SUBMISSION đã có thứ tự đọc và checklist nên có thể đang nhảy sang AI quá sớm | Phản biện hời hợt: chưa phân biệt việc đề thiếu thông tin với việc sinh viên chưa biết đọc file nào trước | Làm rõ pain nằm ở việc tìm kiếm và tổng hợp điều kiện, không phải đề thiếu dữ liệu |
| CP4 Research | Nhờ AI gợi ý công cụ và case đã có cho việc đọc đề, nộp bài | Gợi ý NotebookLM và GitHub Classroom autograding, hai hướng nhóm đưa vào bảng research (Workflow có trích dẫn; Rule kiểm file và tên) | Thông tin cũ: AI không biết GitHub Classroom đã ngừng hoạt động ngày 28/08/2026 và NotebookLM đã đổi tên thành Gemini Notebook | Tự mở từng link để kiểm, ghi rõ hai điểm này vào bảng research (group_report mục 3.3). Không dựa vào công cụ đã ngừng mà dùng lệnh kiểm tên tự chạy |
| CP5 Quy trình | Không dùng | — | — | — |
| CP5–6 Problem Statement | Không dùng | — | — | — |
| CP6 Mức can thiệp / quyết định | Nhờ AI phản biện lựa chọn mức can thiệp cho card #1 | Đưa ra phương án Workflow cụ thể (NotebookLM có trích dẫn tới đoạn gốc), nhóm giữ làm phương án dự phòng | Nghiêng về Workflow chỉ vì có dùng AI, không tính tới việc Rule đã chạy thử trên đề thật | Phản biện lại bằng kết quả Rule bắt đủ 25/25 điều kiện và báo đúng 8/8 tên repo thử → giữ Rule, để Workflow làm dự phòng khi chạm ngưỡng dừng |
| CP3–CP6 Rà soát báo cáo nhóm | Nhờ Claude Code đối chiếu `group_report.md` với RUBRIC, chạy lại các lệnh `grep` và mở 6 link research | Phát hiện câu "Shortlist lấy từ 3 cluster khác nhau" ở mục 2.4 là sai (#1 và #7 + #12 cùng cluster A); xác nhận số từ, số dòng và 6 link đều khớp với báo cáo | Chỉ kiểm được những gì đếm hoặc chạy lại được (số từ, số dòng, link, lệnh `grep`); không đánh giá được lập luận chọn Rule và No-Go có đủ chặt không | Sửa mục 2.4 thành "Shortlist lấy từ 2 cluster"; tự đọc lại mục 6–8 để kiểm lập luận |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
- Card khiến tôi bất ngờ nhất là nhóm card của Tùng Lâm vì cả ba đều phụ thuộc vào dữ liệu từ tổ chức bên ngoài. Tôi nhận ra một problem dù có pain lớn nhưng nếu phụ thuộc vào dữ liệu, quyền truy cập và nhiều bên liên quan thì sẽ khó triển khai trong phạm vi nhỏ. Card #9 của Quang Hải trùng pattern với card #3 của tôi cho thấy pain này không phải vấn đề cá nhân mà có thể xuất hiện ở nhiều người.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
- Ở card #1, ý tưởng chatbot hỏi đáp đề lab xuất hiện khá sớm và tôi thấy nó hấp dẫn vì có thể ứng dụng AI trực tiếp. Tuy nhiên, khi phân tích sâu hơn, nhóm nhận ra chưa xác định rõ vấn đề thực sự cần giải quyết. Câu hỏi khiến nhóm gạch ý này: "Chatbot có thực sự giải quyết pain hay chỉ là giải pháp được nghĩ ra trước khi xác định problem?" Card #7 cũng vậy, cụm từ "tự động gom nhóm" đã mô tả cách giải quyết thay vì nhu cầu. Card #1 ban đầu ghi "Workflow" cũng cho thấy tôi đã phần nào nghĩ đến giải pháp trước khi hiểu rõ pain.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
- Lần chuyển từ Workflow sang Rule khiến tôi thay đổi cách nhìn về problem. Ban đầu tôi muốn bảo vệ Workflow, tức mức can thiệp AI gồm các bước viết sẵn bằng code, AI thực hiện một số bước. Tuy nhiên, bằng chứng cho thấy Rule đơn giản có thể xử lý vấn đề, không cần AI. Tôi chuyển mức can thiệp từ Workflow xuống Rule, nhưng vẫn giữ baseline 45 phút vì đó là dữ liệu quan sát ban đầu cần được kiểm chứng thêm.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
- Con số 14 phút của SV-02 khiến tôi hơi lo problem chưa đủ lớn. Tuy nhiên, việc bạn ấy biết quy định nhưng vẫn quên đổi tên file giúp tôi hiểu rằng vấn đề không đơn giản là đọc đề. Đáng bất ngờ nhất là đề không thiếu thông tin, 6/25 điều kiện không có ô tự kiểm và chỉ cần hai lệnh grep đã gom đủ 25/25 điều kiện.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
- Khó nhất là xây dựng metric vừa đo thời gian vừa đo độ phủ điều kiện. Tôi không thể chỉ nói làm nhanh hơn mà phải đảm bảo không bỏ sót yêu cầu. Baseline 45 phút chỉ đến từ một người nên tôi cần ghi rõ giới hạn dữ liệu, không khái quát thành kết luận chung. Việc ghi AI intervention point là "Không có" ban đầu hơi tiếc, nhưng tôi nghĩ trung thực quan trọng hơn cố gắng đưa AI vào mọi vấn đề.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
- Nếu làm lại, tôi sẽ bấm giờ thực tế ngay từ CP1 và phỏng vấn thêm sinh viên trong lớp K5 để có dữ liệu trực tiếp. Vì vừa là nhóm trưởng vừa có card được chọn, tôi nghĩ mình đôi lúc chưa phản biện đủ mạnh, đặc biệt ở điểm Pain 4 khi dữ liệu còn ít. Tôi cũng sẽ kiểm tra kỹ các con số ước tính như 18 phút và xác định rõ ngưỡng dừng dựa trên bằng chứng.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
- Problem của nhóm tôi là sinh viên mất thời gian xử lý đề lab và có nguy cơ bỏ sót các điều kiện yêu cầu. Quy trình hiện tại chủ yếu dựa vào việc đọc đề, tự ghi nhớ và kiểm tra thủ công; bước nghẽn là tìm đúng file và tổng hợp các điều kiện của đề. Metric thời gian có target ≤ 20 phút, cùng hai metric khác là độ phủ 100% điều kiện và 0 lỗi tên file. Boundary của bài toán là hỗ trợ kiểm tra yêu cầu, không thay thế việc sinh viên tự đọc hiểu và thực hiện bài lab. Qua kiểm chứng, chúng tôi nhận thấy AI chưa thực sự cần thiết vì các điều kiện có thể được kiểm tra bằng những quy tắc và lệnh grep đơn giản. Vì vậy, mức can thiệp nhóm chọn là Rule. Quyết định của nhóm là No-Go cho AI.

---

## 7. Tài liệu tham khảo

- Đề Day 02: [README.md](../../README.md), [RULES.md](../../RULES.md), [CHECKPOINTS.md](../../CHECKPOINTS.md), [RUBRIC.md](../../RUBRIC.md), [SUBMISSION.md](../../SUBMISSION.md), [docs/01-worksheet.md](../../docs/01-worksheet.md)
- Báo cáo nhóm: [report/team/group_report.md](../team/group_report.md)
- Review tài liệu đề và thử Rule của nhóm: [report/assets/cp4-doc-review.md](../assets/cp4-doc-review.md)
- Teresa Torres, Opportunity Solution Trees: https://www.producttalk.org/opportunity-solution-trees/
- Google, Use chat in NotebookLM / Gemini Notebook: https://support.google.com/notebooklm/answer/16179559
- GitHub Docs, Use autograding: https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/use-autograding
