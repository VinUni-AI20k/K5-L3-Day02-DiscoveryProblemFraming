# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Phạm Duy Thành
- MSSV: 2A202604075
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: 4Ward
- Link repo nhóm: https://github.com/phungtr/K5-L3B-Day02-4Ward-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi bắt đầu làm một bài tập mới, tôi muốn biết rõ yêu cầu và tiêu chí chấm nằm ở đâu, để không bỏ sót đầu việc quan trọng. | Sinh viên làm bài cá nhân | Phải mất khoảng 20-30 phút để tìm hiểu tất cả tiêu chí và yêu cầu |
| 2 | Tốn thời gian | Khi tìm thông tin về deadline hoặc yêu cầu bài trong nhiều kênh, tôi muốn tìm được thông tin mới nhất, để bắt đầu làm đúng việc mà không phải hỏi lại. | Sinh viên trong lớp/nhóm | Mất khoảng 15-20p để tìm thông tin |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi ôn một chủ đề từ slide, ghi chú và tài liệu đọc, tôi muốn nhận ra các ý liên quan và phần còn thiếu, để chuẩn bị bài có trọng tâm. | Sinh viên đang ôn tập | Tốn khoảng 10_15p để tìm đúng slide cho từng nội dung |
| 4 | Tốn thời gian | Khi chuẩn bị nộp bài, tôi muốn rà soát đủ các mục bắt buộc, để giảm nguy cơ thiếu nội dung hoặc sai định dạng. | Người làm bài và người chấm | Tốn khoảng 30-45p để kiểm tra lại |
| 5 | Lặp lại | Khi làm việc nhóm, tôi muốn biết ai đang phụ trách việc gì và hạn hoàn thành, để tránh hỏi tiến độ nhiều lần hoặc bỏ sót phần việc. | Thành viên nhóm và người điều phối | Mất khoảng 2-3p để đi hỏi |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận góp ý cho bài, tôi muốn gom các nhận xét theo phần cần sửa và mức độ ưu tiên, để chỉnh sửa có thứ tự và không bỏ qua góp ý quan trọng. | Người viết bài; người góp ý | Có thể lên tới 1-2h để tổng hợp và đánh giá các thông tin |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.
- AI chưa đưa ra được các con số cụ thể về dấu hiệu thật
- AI đưa ra 1 số vấn đề không thực tế
---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tìm đúng yêu cầu và deadline mới nhất khi thông tin nằm ở nhiều kênh (#2)| Bối cảnh và actor cụ thể; có thể quan sát thời gian tìm, số kênh phải kiểm tra và lần phải hỏi lại. | Chưa xác nhận vấn đề xảy ra thường xuyên với mình; chưa biết kênh nào gây mất thời gian nhất. |
| 2 | Tổng hợp nội dung ôn tập từ slide, ghi chú và tài liệu đọc (#3)| Có quy trình nhiều bước, bottleneck dự kiến nằm ở việc đối chiếu ý giữa các nguồn; có thể thử đo thời gian cho một chủ đề. | Thời lượng dưới đây chỉ là ước tính; chưa kiểm tra mức độ ảnh hưởng tới kết quả ôn tập. |
| 3 | Gom và ưu tiên góp ý để lập danh sách chỉnh sửa bài (#6)| Có đầu vào/đầu ra rõ (góp ý → danh sách việc cần sửa); có thể đo thời gian và số góp ý được xử lý. | Chưa có ví dụ góp ý gần nhất để xác nhận số nguồn, số nhận xét và thời gian thực tế. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị bắt đầu một bài tập và yêu cầu/deadline có thể nằm ở LMS, tin nhắn nhóm hoặc tài liệu lớp, tôi muốn tìm và xác nhận được thông tin mới nhất, để bắt đầu đúng việc mà không bỏ sót yêu cầu. |
| Actor | Sinh viên làm bài cá nhân; bạn cùng lớp có thể bị ảnh hưởng nếu thông tin được chia sẻ không thống nhất. |
| Thời điểm / bối cảnh | Lúc nhận bài mới hoặc trước khi bắt tay làm/nộp bài; cần xác nhận bằng một tình huống gần nhất của bản thân. |
| Quy trình hiện tại (3–7 bước) | 1) Mở đề bài trên LMS. 2) Tìm thông báo liên quan trong chat. 3) Mở rubric/tài liệu hướng dẫn. 4) So sánh các thông tin và xác định bản mới nhất. 5) Hỏi bạn/giảng viên nếu còn điểm chưa rõ. 6) Ghi lại việc cần làm và deadline. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–4: tìm và đối chiếu thông tin giữa các nguồn, ước tính 10–15 phút/lần; chưa bấm giờ, cần đo ở lần làm bài tiếp theo. Thời gian chờ câu trả lời chưa tính. |
| Impact (nếu không giải thì sao) | Có thể bắt đầu sai yêu cầu, phải sửa lại hoặc nộp thiếu mục; cần ghi nhận số lần sửa/thiếu mục thực tế trước khi kết luận mức độ ảnh hưởng. |
| Success metric (baseline → target) | Baseline: đo thời gian từ lúc bắt đầu tìm đến khi ghi được yêu cầu/deadline đã xác nhận trong 3 lần; hiện chưa có số đo. Target thử nghiệm: giảm trung vị thời gian ít nhất 30% so với baseline và không bỏ sót yêu cầu bắt buộc trong 3 lần kiểm tra tiếp theo. |
| Phương án không dùng AI | Dùng checklist cố định để kiểm tra LMS, thông báo mới nhất và rubric; ghi link nguồn, ngày cập nhật và deadline vào một nơi. |
| Giả thuyết về AI (nếu có) | AI có thể hỗ trợ trích yêu cầu/deadline từ tài liệu đã chọn và chỉ ra điểm chưa nhất quán; người học phải mở nguồn gốc để xác nhận, không để AI tự quyết định bản nào đúng. |
| Cảm nhận nhanh | Rule / Workflow trước; chưa có bằng chứng cho thấy cần AI. |

Quy trình nháp hiện tại:

```text
[Mở đề bài LMS: ~3'] → [Tìm thông báo trong chat: ~5'] → [Đọc rubric/tài liệu: ~5']
→ [Đối chiếu phiên bản, deadline và yêu cầu: ~5–10'] ← BOTTLENECK
→ [Hỏi lại nếu còn điểm chưa rõ: ~?'] → [Ghi checklist việc cần làm: ~2']
Tổng thời gian thao tác ước tính: ~20–25 phút, chưa tính thời gian chờ phản hồi; cần đo thực tế.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi ôn một chủ đề bằng slide, ghi chú và tài liệu đọc, tôi muốn tổng hợp các ý liên quan và nhận ra phần chưa hiểu, để phân bổ thời gian ôn tập đúng trọng tâm. |
| Actor | Sinh viên đang tự ôn tập một chủ đề có nhiều tài liệu. |
| Thời điểm / bối cảnh | Trước buổi kiểm tra hoặc khi cần chuẩn bị bài; cần ghi lại chủ đề và buổi ôn cụ thể để xác nhận. |
| Quy trình hiện tại (3–7 bước) | 1) Tìm slide, ghi chú và tài liệu đọc. 2) Mở và đọc từng nguồn. 3) Ghi các ý chính. 4) So sánh các ý trùng/khác nhau. 5) Đánh dấu phần chưa hiểu. 6) Chọn nội dung cần ôn lại. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: ghi chú rồi đối chiếu nội dung giữa các nguồn, ước tính 20–30 phút cho một chủ đề; chưa bấm giờ, số nguồn và độ dài tài liệu có thể làm thời gian thay đổi nhiều. |
| Impact (nếu không giải thì sao) | Có thể mất thời gian đọc lặp lại hoặc bỏ qua phần chưa hiểu; chưa có bằng chứng để khẳng định ảnh hưởng đến điểm số. |
| Success metric (baseline → target) | Baseline: bấm giờ cho một chủ đề, ghi số nguồn và tổng thời gian đến khi có danh sách ý chính/phần chưa hiểu. Target thử nghiệm: giảm ít nhất 25% thời gian tổng hợp ở chủ đề tương đương, đồng thời tự rà lại để bảo đảm không bỏ sót ý quan trọng. |
| Phương án không dùng AI | Dùng mẫu ghi chú thống nhất (ý chính, nguồn/trang, câu hỏi còn mở) và bảng so sánh giữa các nguồn. |
| Giả thuyết về AI (nếu có) | AI có thể gợi ý nhóm các ý tương tự và trích dẫn nguồn/trang nếu tài liệu cho phép; người học phải kiểm tra lại nội dung và tự xác định phần cần ôn. |
| Cảm nhận nhanh | Workflow; thử mẫu ghi chú và cách tổ chức tài liệu trước khi cân nhắc AI. |

Quy trình nháp hiện tại:

```text
[Tìm và mở 3 nguồn: ~10'] → [Đọc/đánh dấu từng nguồn: ~30–45'] → [Ghi ý chính: ~15']
→ [Đối chiếu ý giữa nguồn, tìm điểm chưa hiểu: ~20–30'] ← BOTTLENECK
→ [Lập danh sách nội dung cần ôn: ~10']
Tổng thời gian ước tính: ~85–110 phút/chủ đề; cần thay bằng số đo của một buổi ôn thực tế.
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận góp ý từ giảng viên hoặc bạn học cho một bài làm, tôi muốn gom góp ý theo phần cần sửa và mức độ ưu tiên, để chỉnh sửa có thứ tự và kiểm tra được mình đã xử lý góp ý nào. |
| Actor | Sinh viên viết/chỉnh sửa bài; người góp ý có thể cần biết phản hồi đã được tiếp nhận. |
| Thời điểm / bối cảnh | Sau khi nhận phản hồi cho bản nháp hoặc bài thuyết trình; cần dùng một bộ góp ý thực tế để xác nhận. |
| Quy trình hiện tại (3–7 bước) | 1) Mở các nguồn nhận góp ý. 2) Đọc và ghi lại từng nhận xét. 3) Gộp nhận xét trùng nhau. 4) Gắn nhận xét với phần tương ứng trong bài. 5) Chọn thứ tự ưu tiên và lập danh sách chỉnh sửa. 6) Sửa bài và đánh dấu góp ý đã xử lý/chưa xử lý. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: phân loại, gắn góp ý vào phần bài và xác định thứ tự, ước tính 15–25 phút/bộ góp ý; chưa đo trên một bộ phản hồi thật. |
| Impact (nếu không giải thì sao) | Có thể bỏ sót hoặc sửa sai thứ tự, dẫn đến phải rà lại phản hồi; mức độ xảy ra cần xác minh bằng lịch sử chỉnh sửa/bài gần nhất. |
| Success metric (baseline → target) | Baseline: đo thời gian từ lúc mở góp ý đến khi có danh sách chỉnh sửa, đồng thời đếm tổng góp ý và số góp ý được ghi nhận. Target thử nghiệm: giảm ít nhất 25% thời gian lập danh sách và đối chiếu để 100% góp ý được đánh dấu đã xử lý/cần hỏi lại/bỏ qua có lý do. |
| Phương án không dùng AI | Tạo bảng gồm góp ý, vị trí trong bài, mức ưu tiên, trạng thái và lý do; tự gộp các nhận xét trùng. |
| Giả thuyết về AI (nếu có) | AI có thể đề xuất nhóm góp ý tương tự và liên kết với đoạn bài liên quan; người viết xác nhận cách diễn giải, ưu tiên và quyết định có áp dụng hay không. |
| Cảm nhận nhanh | Rule / Workflow trước; AI chỉ là giả thuyết hỗ trợ phân loại, không tự sửa bài. |

Quy trình nháp hiện tại:

```text
[Mở các nguồn góp ý: ~5'] → [Đọc và ghi từng nhận xét: ~10–15'] → [Gộp nhận xét trùng: ~5–10']
→ [Gắn góp ý vào phần bài và ưu tiên: ~10–15'] ← BOTTLENECK
→ [Lập checklist sửa: ~5'] → [Sửa và đánh dấu trạng thái: ~20–30']
Tổng thời gian ước tính: ~55–80 phút/bộ góp ý; cần đo bằng một lần chỉnh sửa thực tế.
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Actor và tình huống tìm thông tin khá cụ thể; có thể kiểm tra bằng cách bấm giờ và xem có phải hỏi lại hay không. Đây mới là lựa chọn tạm thời, chưa phải kết luận đã kiểm chứng.
- Câu hỏi muốn nhóm phản biện: Bottleneck có thực sự là việc thông tin nằm ở nhiều kênh, hay chủ yếu do yêu cầu chưa rõ? Cách đo nào giúp phân biệt hai nguyên nhân này?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Các thời lượng và mục tiêu phần trăm chưa có dữ liệu thực tế; nếu ghi như kết quả đã quan sát sẽ gây hiểu nhầm. | Đồng ý. | Ghi rõ các phút là ước tính, baseline chưa đo và nêu cách đo trước khi so với target. |
| Một số vấn đề có thể đang mô tả quy trình mong muốn hơn là pain đã xảy ra; các card cũng chưa có bằng chứng về tần suất và hậu quả. | Đồng ý. | Giữ nội dung dưới dạng giả thuyết cần xác minh; thêm điều còn chưa chắc và không khẳng định ảnh hưởng tới kết quả khi chưa có bằng chứng. |
| Giả thuyết AI có thể khiến nhóm nhảy sang giải pháp trước khi thử cách đơn giản hơn. | Đồng ý. | Bổ sung phương án không dùng AI và đặt Rule/Workflow trước; chỉ xem xét AI nếu thử nghiệm cho thấy cách tổ chức thủ công chưa xử lý được bottleneck. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Báo cáo nhóm ghi tên tôi ở 3 candidate: tìm yêu cầu/deadline; tổng hợp tài liệu ôn tập; phân loại feedback. Tôi chưa đặt câu hỏi trực tiếp trong lớp do thời gian hạn chế. | Candidate tìm yêu cầu/deadline đang được xem xét làm hướng tiếp tục; chưa có ghi nhận về phần pitch/thảo luận trực tiếp của tôi. |
| Phản biện bài của bạn khác | Tôi chưa đặt câu hỏi phản biện trực tiếp. | Không có câu hỏi do tôi đặt để ghi nhận. |
| Nhận phản biện | Tôi chưa có trải nghiệm phản biện trực tiếp đủ để ghi lại câu hỏi cụ thể. | Chưa ghi nhận thay đổi do phản biện của bạn khác. |
| Gom cluster / cây OST | Tôi chưa có thông tin về đóng góp trực tiếp của mình ở phần này. | Chưa có kết quả cá nhân để ghi nhận. |
| Chọn candidate problem | Candidate nhóm đang xem xét: sinh viên làm bài cá nhân cần tìm đúng yêu cầu/deadline mới nhất nằm rải rác ở LMS, chat nhóm và tài liệu lớp. | Hướng giải quyết dự kiến là bắt đầu bằng checklist Rule/Workflow; chưa có quyết định Go / Not Yet / No-Go. |
| Kiểm chứng / research | Tôi chưa phỏng vấn và chưa thực hiện kiểm chứng/research. | Chưa có bằng chứng xác nhận hoặc bác bỏ pain, tần suất và thời lượng. |
| Quy trình nhóm | Tôi ghi lại quy trình giả thuyết gồm 6 bước: mở đề trên LMS → tìm thông báo trong chat → mở rubric/tài liệu → đối chiếu bản mới nhất → hỏi lại nếu chưa rõ → ghi checklist và deadline. | Bottleneck dự kiến ở bước 2–4, ước tính 10–15 phút/lần; chưa bấm giờ và chưa xác nhận với người dùng. |
| Problem Statement | Tôi đã mô tả actor, quy trình, bottleneck, metric thử nghiệm và boundary dự kiến theo thông tin hiện có. | Baseline chưa đo; cần đo 3 lần. Chưa có Problem Statement v0/v1 hoàn chỉnh của nhóm để so sánh. |
| Mức can thiệp AI | Mức dự kiến là Rule/Workflow trước, dùng checklist cố định; chưa có bằng chứng cho thấy cần AI. | Nếu sau này thử AI, AI chỉ trích yêu cầu/deadline từ tài liệu đã chọn và báo chỗ chưa nhất quán; người học phải xác nhận với nguồn gốc. |
| Quyết định | Chưa có quyết định cuối của nhóm. | Bước tiếp theo là đo baseline và phân biệt bottleneck do thông tin nhiều kênh hay do yêu cầu chưa rõ. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Dùng AI để gợi ý/diễn đạt 7 Job Story từ bối cảnh học tập và làm việc nhóm. | Gợi ý actor, bối cảnh và cách đo cho các ý tưởng. | AI không biết tần suất, thời gian hay bằng chứng thật của tôi; một số ý có thể không đúng trải nghiệm. | Ghi rõ đây là bản nháp cần xác nhận; bỏ ý nào không đúng và thay dấu hiệu thật trước khi nộp. |
| CP2 Problem Card | Dùng AI để phát triển 3 card và quy trình nháp từ các ý scan. | Giúp cấu trúc quy trình, bottleneck, metric thử nghiệm và phương án không AI. | Các thời lượng, target và quy trình là ước tính, chưa được đo hoặc xác nhận. | Đánh dấu ước tính/chưa đo và nêu cách lấy baseline; không xem là kết quả thực tế. |
| CP4 Research | Không dùng AI; tôi chưa phỏng vấn và chưa làm research. | — | Chưa có dữ liệu kiểm chứng hay nguồn research. | Ghi rõ chưa thực hiện, không tạo kết quả giả định. |
| CP5 Quy trình | Không dùng AI ở checkpoint này. | — | Quy trình và 10–15 phút/lần hiện chỉ là giả thuyết/ước tính, chưa quan sát thực tế. | Ghi rõ ước tính; cần đo 3 lần và xác nhận quy trình với người thực hiện. |
| CP5–6 Problem Statement | Không dùng AI ở checkpoint này. | — | Chưa có bản v0/v1 hoàn chỉnh của nhóm để đối chiếu. | Ghi nhận nội dung hiện tại là hướng nháp, không coi là kết quả nhóm đã xác nhận. |
| CP6 Mức can thiệp / quyết định | Không dùng AI; nhóm dự kiến bắt đầu với Rule/Workflow, chưa chốt quyết định cuối. | — | Chưa có bằng chứng kiểm chứng để kết luận mức này đủ hoặc cần AI. | Đề xuất đo baseline và thử checklist trước; quyết định Go / Not Yet / No-Go vẫn để nhóm thống nhất. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Mình cảm thấy hầu như vấn đề nằm rất nhiều ở việc soạn báo cáo theo tuần/tháng hay việc soạn tài liệu học tập rất mất thời gian

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có, và lúc đó nhóm em cảm thấy đã đi sai hướng và đã ngay lập tức đóng băng giải pháp và lùi lại 5p để làm rõ lại vấn đề cốt lõi mà ý tưởng đang giải quyết

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Em không vì nhận ra ngay sai lầm của mình

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Kết quả kiểm chứng thì em chưa có cơ hội để phỏng vấn các bạn xung quanh vì bạn nhóm trưởng đại diện cho toàn nhóm để lên phản biện với các nhóm khác ạ

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất đó chính là khó khăn trong việc cưỡng lại sự cám dỗ của việc lồng ghép giải pháp vào vấn đề

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Em nghĩ nhóm em làm khá ổn và mình cũng đã làm tròn trách nhiệm nên chưa nghĩ ra cần phản biện mạnh phần nào nữa

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán nhóm đang xem xét là sinh viên làm bài cá nhân phải tìm và xác nhận yêu cầu/deadline mới nhất khi thông tin nằm rải ở LMS, chat nhóm và tài liệu lớp. Quy trình giả thuyết gồm mở đề trên LMS, tìm thông báo trong chat, mở rubric/tài liệu, đối chiếu phiên bản, hỏi lại khi chưa rõ, rồi ghi checklist và deadline. Bottleneck dự kiến là tìm và đối chiếu thông tin ở bước 2–4, ước tính 10–15 phút/lần nhưng chưa được bấm giờ. Baseline sẽ được đo trong 3 lần tìm; target thử nghiệm là giảm trung vị thời gian ít nhất 30% và không bỏ sót yêu cầu bắt buộc. Boundary dự kiến là nếu dùng AI thì AI chỉ trích yêu cầu/deadline từ tài liệu đã chọn và chỉ ra điểm chưa nhất quán, còn người học phải kiểm tra nguồn gốc. Mức can thiệp dự kiến là Rule/Workflow trước vì chưa có bằng chứng cần AI. Nhóm chưa đưa ra quyết định cuối; cần đo baseline và xác định bottleneck trước khi chốt.
---

## 7. Tài liệu tham khảo

- Template và prompt mẫu của lớp: docs/01-worksheet.md (repo K5-L3B-Day02-4Ward-DiscoveryProblemFraming).
