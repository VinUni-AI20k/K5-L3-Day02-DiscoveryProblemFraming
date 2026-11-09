# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: LuckyTeam
- Thành viên: xem `TEAM.md` (Nguyễn Đức Hải, Trần Tùng Lâm, Vũ Quang Hải, Nguyễn Anh Quân)
- Candidate problem được chọn (1 câu): Khi mở đề một lab mới, học viên K5 mất khoảng 45 phút đọc 6 file hướng dẫn và đối chiếu qua lại mới biết đủ điều kiện được và mất điểm của từng checkpoint, và vẫn làm sai những điều kiện có sẵn trong đề.
- Quyết định cuối: **No-Go cho AI.** Rule (lệnh gom điều kiện chấm + lệnh kiểm tên repo, tên file) cộng với đổi thứ tự đọc là đủ; thử ở 2 lab tiếp theo.

---

## 2. Hội tụ nhóm (CP3)

Nhóm 4 người, 12 candidate (mỗi người 3 card).

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Đức Hải | Khi nhận đề lab mới, tôi muốn biết ngay cần nộp gì, đặt ở đâu, để bắt tay làm mà không phải đọc hết các file hướng dẫn | Học viên K5 lớp L3B | Bước 5, đối chiếu qua lại giữa các file: ~10'/lab (tổng 45'/lab) | "SUBMISSION.md đã có checklist 10 mục. Vậy đề thiếu thông tin, hay chỉ là không biết đọc file nào trước?" (Nguyễn Anh Quân) · "45 phút là bấm giờ hay nhớ lại?" (Trần Tùng Lâm) |
| 2 | Nguyễn Đức Hải | Khi ôn bài trước buổi học/kiểm tra, tôi muốn tìm đúng phần cần ôn trong slide, video, ghi chép, để ôn đủ ý mà không mở từng nguồn | Học viên tự ôn ngoài giờ | Bước 3, tua video tìm đoạn: ~60'/lần (tổng 3 giờ/lần) | "Lớp có cho tải video ghi hình không? Không có video thì bước nghẽn này không giải được" (Vũ Quang Hải) |
| 3 | Nguyễn Đức Hải | Khi làm bài nhóm đã chia phần, tôi muốn biết ai làm phần nào, xong tới đâu, để không phải nhắn nhắc từng người | Người điều phối nhóm 3–4 người | Bước 3, hỏi tiến độ từng người: ~15'/lần; 12 tin/tuần | "Bảng phân công trong TEAM.md đã đủ chưa? Bottleneck thật có phải bước 1, chia việc qua chat mà không có chỗ ghi chung?" (Trần Tùng Lâm) |
| 4 | Trần Tùng Lâm | Khi nhận kết quả xét nghiệm trên MyVinmec, tôi muốn biết chỉ số nào bất thường và có cần khám sớm không, để khỏi lo trong 2 ngày chờ bác sĩ | Người khám ngoại trú Vinmec có xét nghiệm máu | Bước 3, tra từng chỉ số trên Google: ~30' (ước lượng, chưa đo) | "Nhóm không ai học y. Ai kiểm được lời giải thích là đúng? Có lấy được dữ liệu kết quả không?" (Nguyễn Đức Hải) |
| 5 | Trần Tùng Lâm | Khi lái VinFast về quê dịp lễ, tôi muốn biết nên sạc ở trạm nào, để không chờ trụ lâu hay lo hết pin | Chủ ô tô điện VinFast đi đường dài | Bước 3, chọn trạm: ~20', chọn sai dẫn tới chờ trụ ~45' | "App VinFast đã hiện trụ trống chưa? Nếu có thì chỉ còn phần dự đoán, mà phần đó cần dữ liệu của VinFast" (Vũ Quang Hải) |
| 6 | Trần Tùng Lâm | Khi đi VinBus tới trường, tôi muốn biết mấy phút nữa xe tới theo tình hình thực tế, để không đứng chờ lâu hay lỡ chuyến | Sinh viên đi VinBus tuyến cố định, ~5 lượt/tuần | Bước 4, đứng chờ ở trạm: 10–20'/lượt (~75'/tuần) | "Nhóm lấy được dữ liệu GPS và tình trạng giao thông của tuyến không? Không có thì làm sao so sánh Rule với AI?" (Nguyễn Anh Quân) |
| 7 | Vũ Quang Hải | Khi tổng hợp tài liệu nghiên cứu cho buổi họp nhóm cuối tuần, tôi muốn gom được các ý chính theo chủ đề, để không mất 2–3 tiếng lọc thủ công | Thành viên làm báo cáo tổng hợp | Bước 3–4, lọc ý trùng và gom nhóm: 90–120' | "Job Story gốc có chữ 'tự động gom nhóm': đó là giải pháp. Pain thật nằm ở bước đọc, bước lọc hay bước viết lại? 2,5 giờ/tuần là đo hay ước?" (Nguyễn Đức Hải) |
| 8 | Vũ Quang Hải | Khi làm slide thuyết trình mỗi tuần, tôi muốn bố cục thống nhất, để không phải căn chỉnh lại từng slide | Các thành viên nhóm thuyết trình | Bước 4, căn lề, font, hình: 45–60' | "Slide Master hoặc template có sẵn đã giảm được bao nhiêu phút? Bài này có phải No AI là đủ không?" (Trần Tùng Lâm) |
| 9 | Vũ Quang Hải | Khi cần tìm lại quyết định cũ trong chat nhóm, tôi muốn thấy ngay các điều đã thống nhất, để không phải cuộn lại hàng trăm tin | Nhóm trưởng, thành viên nhóm dự án | Bước 2–3, cuộn và đọc lướt tin nhắn: 15–20'/lần | "Trùng pattern với card #3 của Đức Hải. Đọc lịch sử chat nhóm có đụng tin nhắn riêng của thành viên không?" (Nguyễn Anh Quân) |
| 10 | Nguyễn Anh Quân | Khi ứng tuyển nhiều nơi, tôi muốn quản lý vị trí đã nộp, hạn và phản hồi, để không lỡ lịch phỏng vấn hay nộp trùng | Sinh viên năm cuối ứng tuyển thực tập/việc làm | Bước 3, đối chiếu phản hồi với hồ sơ đã gửi: 6'/lần (tổng 15'/lần, số minh họa) | "15 phút/lần là số minh họa. Đã có lần nào lỡ lịch thật chưa? Một bảng tính có đủ không?" (Vũ Quang Hải) |
| 11 | Nguyễn Anh Quân | Khi hoàn thiện báo cáo, tôi muốn trình bày đúng quy định của khoa, để không phải sửa định dạng nhiều lần | Sinh viên làm bài tập lớn, đồ án, khóa luận | Bước 3, sửa tay tiêu đề, bảng, hình: 50'/đợt (tổng 120'/đợt) | "Template chính thức cộng Styles của Word đã giải phần lớn. Còn lại phần nào thật sự cần giải?" (Nguyễn Đức Hải) |
| 12 | Nguyễn Anh Quân | Khi đọc tài liệu cho khóa luận, tôi muốn nắm phương pháp, kết quả và điểm khác giữa các nghiên cứu, để viết phần tổng quan | Sinh viên năm cuối làm nghiên cứu | Bước 2, đọc hiểu phương pháp: 20'/bài (tổng 60'/bài) | "Trùng pattern với card #7 của Quang Hải, gộp được không? Chậm vì đọc chậm hay vì thiếu kiến thức nền?" (Trần Tùng Lâm) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Đọc và đối chiếu nhiều tài liệu | #1 Đọc đề lab, #2 Ôn bài nhiều nguồn, #7 Tổng hợp tài liệu nhóm, #12 Đọc tài liệu nghiên cứu | Thông tin cần dùng nằm rải ở nhiều tài liệu dài. Thời gian mất ở bước tìm và đối chiếu, chưa phải ở việc chính |
| B — Theo dõi việc trong tin nhắn, email | #3 Hỏi tiến độ nhóm, #9 Tìm quyết định cũ trong chat, #10 Theo dõi ứng tuyển | Không có một chỗ ghi chung, phải kéo lại lịch sử chat/email hoặc hỏi lại người khác |
| C — Thiếu thông tin đúng lúc để quyết định | #4 Kết quả xét nghiệm, #5 Trạm sạc VinFast, #6 Chờ VinBus | Dữ liệu nằm ở hệ thống của tổ chức khác (Vinmec, VinFast, VinBus); người dùng phải chờ hoặc tự đoán |
| D — Trình bày đúng quy chuẩn | #8 Layout slide, #11 Định dạng báo cáo của khoa | Quy tắc định dạng đã rõ nhưng phải sửa tay; phần lớn giải được bằng template |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm số phút học viên mất để tìm và đối chiếu thông tin trước khi bắt tay vào việc chính
         của một bài lab hoặc bài học
├── Opportunity A: Yêu cầu và điều kiện chấm của một lab nằm rải ở nhiều file, phải đối chiếu qua lại
│                  mới biết đủ (#1)
├── Opportunity B: Nội dung cần ôn hoặc cần nghiên cứu nằm trong nhiều nguồn dài, khó tìm đúng đoạn
│                  (#2, #7, #12)
├── Opportunity C: Ai làm phần nào, nhóm đã thống nhất gì chỉ nằm trong lịch sử chat (#3, #9)
└── Opportunity D: Quy định trình bày phải tự dò bằng mắt rồi sửa tay (#8, #11)

     ✗ "Chatbot hỏi đáp đề lab"            ← solution, gạch khỏi tầng này
     ✗ "Tự động gom nhóm ý chính" (#7)     ← solution nằm sẵn trong Job Story gốc
     ✗ "Bot AI tóm tắt lịch sử chat" (#9)  ← solution
     ✗ "Template layout tự động" (#8)      ← solution
```

Cluster C (#4, #5, #6) không nằm dưới outcome này: đó là chuyện đi lại và sức khỏe, không phải chuyện học. Nhóm vẫn đưa #6 vào shortlist để so sánh vì đây là card chính của Trần Tùng Lâm.

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "Chatbot hỏi đáp đề lab": ý đầu tiên khi nghe card #1, nhưng là công cụ, không phải pain.
- "Tự động tổng hợp tài liệu và gom nhóm ý chính" (#7): pain là mất 90–120' lọc và gom ý, còn "tự động gom nhóm" là một cách giải.
- "Bot AI quét lịch sử chat" (#9): pain là mất 15–20' cuộn tìm, còn bot là một cách giải.
- "Sinh layout slide tự động" (#8): pain là mất 45–60' căn chỉnh tay.
- "Tô màu giao thông trên bản đồ" (#6): phương án không dùng AI của card, không phải opportunity.

### 2.4. Chấm điểm shortlist (1–5)

Shortlist lấy từ 2 cluster: #1 và #7 + #12 cùng thuộc cluster A nhưng nằm ở 2 opportunity khác nhau trong cây OST (A và B); #6 thuộc cluster C. #7 và #12 được gộp thành một candidate vì cùng pattern; dùng quy trình của #12 vì có đủ bước và số phút hơn.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #1 Đọc đề lab để biết cần nộp gì | 5 | 5 | 4 | 4 | 5 | 5 | 5 | **33** |
| #6 Chờ VinBus ở trạm | 5 | 4 | 3 | 4 | 2 | 4 | 3 | 25 |
| #7 + #12 Đọc và tổng hợp tài liệu nghiên cứu | 4 | 4 | 2 | 4 | 3 | 4 | 3 | 24 |

Lý do các ô điểm thấp:

- #1, Pain 4: con số 45' mới là tự ghi của 1 người, nhưng độ dài đề và chỗ đặt yêu cầu thì đếm được ngay trong repo. Impact 4: chỉ tốn ở đầu mỗi lab, không phải hằng ngày.
- #6, Vừa sức lab 2: cần dữ liệu GPS và giao thông của VinBus/Xanh SM, nhóm không có quyền truy cập và không kiểm chứng được trong 4 tiếng. Domain 3: chỉ Tùng Lâm đi tuyến này. Pain 3: mới có 1 người, chưa ghi giờ thật.
- #7 + #12, Pain 2: cả hai card đều dùng số minh họa hoặc ước lượng. Vừa sức lab 3: cần bài báo thật, và "tóm đúng phương pháp" phụ thuộc chuyên ngành từng đề tài, khó chấm trong lab.

**Candidate được chọn:** #1 Đọc đề lab để biết cần nộp gì (Nguyễn Đức Hải).

**Vì sao chọn:** điểm cao nhất; bằng chứng lấy được ngay trong repo đề và trên GitHub; actor là cả lớp; card đã tự nghi "có thể không cần AI", đúng dịp để thử nguyên tắc chọn mức đơn giản nhất.

**Vì sao loại các candidate còn lại:**

- #6 Chờ VinBus: dữ liệu vị trí xe và giao thông nằm ở hệ thống Xanh SM/VinBus, nhóm không lấy được; phương án chính (tô màu giao thông) là việc của đơn vị vận hành app, người dùng không tự làm được. Không kiểm chứng và không so sánh 4 mức được trong 1 buổi lab.
- #7 + #12 Tổng hợp tài liệu nghiên cứu: chưa có số liệu đo thật; khó viết tiêu chí "ý chính đúng" khi mỗi người một đề tài; Job Story #7 còn chứa giải pháp.
- #4 Kết quả xét nghiệm: lĩnh vực y tế, sai thì hại thật; nhóm không ai đủ chuyên môn để kiểm, và không có dữ liệu của Vinmec.
- #3 Hỏi tiến độ nhóm và #11 Định dạng báo cáo: đã có phương án No AI rõ ràng (bảng phân công trong TEAM.md; template + Styles), chưa thấy phần nào cần hơn thế.

**Xử lý bất đồng (nếu có):** card chính của Trần Tùng Lâm (#6) và Vũ Quang Hải (#7) không được chọn. Nhóm thống nhất chọn bài kiểm chứng được ngay trong buổi. #6 ghi vào hướng tiếp theo: Tùng Lâm ghi giờ ra trạm và giờ lên xe trong 1 tuần để có baseline thật.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Học viên khác cũng mất từ 30 phút trở lên đọc đề trước khi biết cần làm và nộp gì | Value | 5 | 3 | ✅ Phỏng vấn 2 người, kết quả trái chiều: SV-01 mất 35' đối chiếu 3 nguồn, SV-02 chỉ 14' |
| 2 | Một quy định nằm ở nhiều file nên phải đối chiếu qua lại mới chắc | Value | 5 | 4 | ✅ Review tài liệu đề + phỏng vấn SV-01 |
| 3 | Học viên thật sự làm sai những yêu cầu đã có trong đề | Value | 5 | 3 | ✅ Phỏng vấn: 2/2 người từng sót 1 yêu cầu có sẵn |
| 4 | Đề các lab khác dùng cùng cách viết (ô `- [ ]`, bảng RUBRIC có chữ "trừ", "tối đa") nên một Rule dùng lại được | Feasibility | 4 | 2 | Kiểm ở lab Day 03 |
| 5 | Học viên chạy được vài lệnh tìm kiếm (Git Bash hoặc ô tìm kiếm VS Code) | Usability | 3 | 4 | — |
| 6 | Dùng công cụ để đọc đề không trái RULES và không lộ dữ liệu | Viability | 3 | 4 | — |

Bằng chứng hiện có: #5, lab đã bắt mọi người dùng GitHub và repo đã clone về máy; #6, RULES mục 2 không cấm dùng công cụ để đọc đề, và đề là tài liệu công khai.

Giả định nhóm kiểm chứng: #1, #2 và #3 (quan trọng cao, lúc đầu ít bằng chứng), bằng phỏng vấn 2 người và review tài liệu đề. Cột "Đã có bằng chứng" ghi mức sau kiểm chứng.

### 3.2. Kiểm chứng

Cách đã dùng: **Phỏng vấn 2 người** và **review tài liệu đề Day 02**. Hai người được hỏi không thuộc nhóm, đều là sinh viên năm cuối; báo cáo chỉ ghi mã SV-01, SV-02. Chi tiết review tài liệu và lệnh chạy lại: [report/assets/cp4-doc-review.md](../assets/cp4-doc-review.md).

Interview snapshot #1 — sinh viên năm cuối, đã thực tập phát triển phần mềm:

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | SV-01: sinh viên năm cuối ngành CNTT, đã thực tập phát triển phần mềm |
| Cách hỏi | Phỏng vấn trực tiếp, ghi chép ngay sau buổi hỏi |
| Câu nói đáng nhớ nhất (nguyên văn) | "Mình biết phải nộp báo cáo, nhưng lúc so lại tiêu chí mới nhận ra còn thiếu phần giải thích lựa chọn." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Trong một đồ án học phần: yêu cầu sản phẩm nằm trong đề, tiêu chí chấm nằm ở file riêng, hướng dẫn nộp nằm trên LMS. SV-01 đọc đề trước, làm xong mới đối chiếu tiêu chí, rồi bổ sung phần giải thích quyết định thiết kế |
| Quy trình người được hỏi kể lại | Đọc đề → mở tiêu chí chấm → xem hướng dẫn nộp → tự ghi các mục phải làm → đối chiếu với bản báo cáo |
| Hiện đang xử lý bằng cách nào (workaround)? | Tự lập checklist theo từng phần, đánh dấu nguồn của mỗi yêu cầu, hỏi giảng viên khi có điểm chưa rõ |
| Mất bao lâu, bao lần? | 35 phút đối chiếu 3 nguồn, thêm 20 phút bổ sung nội dung; tổng 55 phút cho lần này |
| Insight / opportunity rút ra | Nghẽn nằm ở bước đối chiếu giữa các nguồn (35'), đúng bước nghẽn của card #1. Tiêu chí chấm được đọc sau khi đã làm, nên phần thiếu chỉ lộ ra lúc cuối và tốn thêm 20' bổ sung. Gom tiêu chí chấm vào một chỗ và đọc **trước** khi làm sẽ tránh được phần này |

Interview snapshot #2 — sinh viên năm cuối, đã thực tập kiểm thử phần mềm:

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | SV-02: sinh viên năm cuối ngành phần mềm, đã thực tập kiểm thử |
| Cách hỏi | Phỏng vấn trực tuyến, ghi chép theo các bước người được hỏi kể lại |
| Câu nói đáng nhớ nhất (nguyên văn) | "Nếu có checklist rõ thì mình kiểm khá nhanh. Có lần sai tên file là do mình quên đổi tên, chứ không phải không biết quy định." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Khi nộp báo cáo thực tập, SV-02 đọc mẫu nộp trước và đối chiếu từng mục. Một bản file cũ còn giữ nguyên tên mặc định; SV-02 phát hiện và đổi tên ở bước kiểm cuối |
| Quy trình người được hỏi kể lại | Mở mẫu nộp → đối chiếu nội dung → kiểm tra tên file → kiểm tra nơi nộp → gửi báo cáo |
| Hiện đang xử lý bằng cách nào (workaround)? | Dùng checklist cá nhân; mở lại file đã tải lên để xác nhận đúng phiên bản |
| Mất bao lâu, bao lần? | 12 phút kiểm tra, thêm 2 phút đổi tên file; tổng 14 phút cho lần này |
| Insight / opportunity rút ra | Đọc mẫu nộp trước và có checklist rõ thì bước kiểm chỉ mất 12'. Lỗi tên file là lỗi quên lúc làm, không phải do không biết quy định, và chỉ bị bắt nhờ có bước kiểm cuối. Đọc kỹ hơn không giúp; cái giúp là một bước kiểm sau khi làm |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn | 2 người | 2/2 từng sót 1 yêu cầu đã có sẵn (SV-01 thiếu phần giải thích lựa chọn, SV-02 để tên file mặc định) và chỉ phát hiện ở bước đối chiếu cuối. 2/2 tự lập checklist cá nhân để khỏi sót. SV-01 mất 35' đối chiếu 3 nguồn, đúng bước nghẽn của card #1 | SV-02 chỉ mất 14', dưới mốc 30' của giả định #1, nhờ đọc mẫu nộp trước và có checklist rõ. Cả 2 kể về đồ án học phần và báo cáo thực tập, không phải lab K5. Số phút là người được hỏi kể lại, không phải bấm giờ |
| Review tài liệu đề Day 02 | 10 file, 15.919 từ | 6 file đọc ở bước 1–4 dài 10.012 từ. RUBRIC có 25 điều kiện làm mất hoặc giới hạn điểm; **6/25 không có ô nào** trong 32 ô tự kiểm. Ví dụ: thiếu thời gian từng bước (C8, trừ 2), thiếu 3–5 tiêu chí đánh giá (C9, trừ 3), reflection dưới 200 từ (C4, tối đa 4/10) | Đề **không thiếu**: danh sách file phải nộp đã gom ở 1 chỗ (SUBMISSION, mục "Cấu trúc và file phải nộp"); quy tắc đặt tên file nhắc ở 5 nơi và nói giống nhau; README đã có bảng "Thứ tự đọc" |
| Thử Rule (2 lệnh `grep`) | 1 lần chạy trên đề Day 02 | Gom được 56 dòng (1.687 từ), chứa đủ **25/25** điều kiện | 5/56 dòng nhiễu; đầu ra chưa xếp theo CP; mới thử trên 1 đề |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

- **Bỏ** nửa "biết cần nộp những file gì và đặt ở đâu": SUBMISSION đã gom đủ ở 1 chỗ, và SV-02 đọc mẫu nộp trước thì chỉ mất 14'. Chỉ cần đọc SUBMISSION trước (No AI).
- **Giữ và làm rõ** nửa "biết **đủ điều kiện được và mất điểm** của từng checkpoint trước khi làm": 25 điều kiện nằm rải ở 3 file, 6 điều kiện không có ô tự kiểm. SV-01 đọc tiêu chí sau khi làm nên mất thêm 20' bổ sung.
- **Thêm** phần "**tự kiểm được ngay** mình đã làm đúng các điều kiện máy kiểm được (tên repo, tên file báo cáo)". Lý do: SV-02 biết quy định mà vẫn để tên file mặc định vì quên đổi. Đọc nhiều hơn không giúp; cần một bước kiểm ngay sau khi làm.
- **Trả lời câu hỏi phản biện của Anh Quân:** đề không thiếu thông tin. Cái khó là điều kiện chấm và ô tự kiểm không khớp hết (6/25 điều kiện không có ô), người học hay đọc tiêu chí chấm sau khi đã làm (SV-01), và có chỗ chính đề tự lệch (`Day02` so với `DAY02`).
- **Giữ baseline 45' nhưng ghi rõ còn yếu:** 1/2 người chỉ mất 14'. Tín hiệu này không làm đổi problem, vì SV-02 nhanh nhờ đã có checklist rõ, và checklist rõ chính là thứ Rule tạo ra cho người chưa có. Ngưỡng dừng ở mục 8.2 (từ 2/3 người dưới 15' thì bỏ lệnh gom) giữ nguyên.
- **Đổi cảm nhận mức can thiệp** từ Workflow (card cá nhân) sang Rule: Rule gom bắt đủ 25/25 điều kiện; cả 2 người được hỏi đều tự xử lý bằng checklist, không cần AI; lỗi SV-02 gặp là sai tên file, đúng việc của biểu thức so mẫu (regex).

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Chính đề Day 02: bảng "Thứ tự đọc" (README) và "Checklist trước khi nộp" (SUBMISSION) | [README.md](../../README.md), [SUBMISSION.md](../../SUBMISSION.md) | Bước 1–4 và 6: chỉ thứ tự đọc, liệt kê file phải nộp | Có sẵn, do coach viết nên đúng | Checklist 10 mục chỉ nói về file, tên file và cách nộp; không nhắc 6/25 điều kiện mất điểm. Thứ tự đọc đặt RUBRIC và SUBMISSION ở cuối (#5, #6) | Đọc SUBMISSION và RUBRIC **trước** là phương án No AI rẻ nhất |
| TILT, Transparent Assignment Design (Mary-Ann Winkelmes; trang hướng dẫn của University of Oregon) | https://teaching.uoregon.edu/transparent-assignment-design · https://tilthighered.com/ | Bước 5, nhìn từ phía người ra đề: ghi Purpose, Task, Criteria ngay trong đề | Có nghiên cứu dẫn kèm (Winkelmes 2013; Winkelmes và cộng sự 2019): đề minh bạch giúp sinh viên, nhất là sinh viên thế hệ đầu | Cần coach sửa đề, học viên không tự làm được. Trang không đưa con số cụ thể | Đề Day 02 có Purpose (README) và Task (CHECKPOINTS), còn Criteria nằm riêng ở RUBRIC. Đề nghị coach ghi "bị trừ nếu…" ngay cạnh từng ô tự kiểm |
| NotebookLM (nay đổi tên thành Gemini Notebook) | https://support.google.com/notebooklm/answer/16179559 · https://support.google.com/notebooklm/answer/16215270 | Bước 1–6: nạp file `.md` của đề, hỏi "liệt kê điều kiện được/mất điểm theo từng CP" | Câu trả lời dựa trên nguồn đã nạp, có trích dẫn bấm vào ra đúng đoạn gốc; nhận file Markdown; gói Free 50 nguồn, mỗi nguồn tới 500.000 từ | Trang trợ giúp nói trích dẫn để "kiểm độ chính xác", tức vẫn phải tự kiểm. Chat có chế độ tìm web nên có thể lẫn nguồn ngoài. Mỗi lab phải nạp lại file | Mức Workflow làm được bằng công cụ có sẵn, không cần tự xây. Chỉ đáng dùng nếu Rule bắt thiếu |
| GitHub Classroom autograding | https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/use-autograding | Bước rà bài trước khi nộp (không phải bước đọc đề): test chạy bằng GitHub Actions mỗi lần push | Rule thuần, tự động, kiểm được có đủ file và đúng tên file | Trang ghi GitHub Classroom ngừng hoạt động ngày 28/08/2026, tức đã ngừng. Chỉ kiểm được thứ máy kiểm được (file, tên), không kiểm được "metric có baseline" | Kiểm tên repo và tên file giải được bằng Rule. SV-02 cho thấy lỗi tên là lỗi quên lúc làm, nên lệnh kiểm phải chạy sau khi làm. Không dựa vào công cụ đã ngừng: dùng lệnh kiểm tự chạy |

**Kết luận research:**

```text
Đề đã có sẵn một nửa lời giải: Thứ tự đọc + checklist nộp bài.
Nửa còn thiếu là gom điều kiện chấm vào một chỗ và kiểm tên ngay sau khi làm. Cả hai làm được bằng Rule.
AI có trích dẫn (NotebookLM) là phương án dự phòng nếu Rule bắt thiếu. Không có lý do tự xây công cụ.
```

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 6 bước, 45 phút/lab, 6/6 bước thủ công (học viên tự ghi, 1 người)

[1 Đọc README, fork + đặt tên repo: 5'] → [2 Đọc RULES: 5'] → [3 Đọc CHECKPOINTS + worksheet: 12']
→ [4 Đọc RUBRIC + SUBMISSION: 8'] → [5 Đối chiếu qua lại giữa các file: 10'] ← BOTTLENECK
→ [6 Tự ghi danh sách việc cần nộp: 5'] → (chuyển cho nhóm ở CP3)

Không có bước nào kiểm lại tên repo, tên file sau khi đặt.
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Học viên (nhóm trưởng fork) | README.md (1.343 từ) | Nắm tổng quan; repo fork đã đặt tên | 5' / mỗi lab | Không có bước kiểm lại tên sau khi đặt; SV-02 biết quy định mà vẫn quên đổi tên file |
| 2 | Học viên | RULES.md (898 từ) | Biết chỗ nào được dùng AI, quy định nhóm | 5' / mỗi lab | |
| 3 | Học viên | CHECKPOINTS.md + docs/01-worksheet.md (5.592 từ) | Biết từng CP làm gì | 12' / mỗi lab | Bước dài nhất, nhưng phần lớn chỉ cần khi làm tới CP đó |
| 4 | Học viên | RUBRIC.md + SUBMISSION.md (2.179 từ) | Biết file phải nộp, tên file, cách chấm | 8' / mỗi lab | |
| 5 | Học viên | Ghi chú bước 1–4, mở lại các file | Danh sách điều kiện đã khớp giữa các file | 10' / mỗi lab | **Bottleneck.** 1 điều kiện có thể nằm ở 2–5 nơi; 6/25 điều kiện mất điểm không có ô tự kiểm |
| 6 | Học viên | Kết quả bước 5 | Danh sách việc cần nộp (giấy hoặc ghi chú) | 5' / mỗi lab | Handoff: dùng để chia việc cho nhóm ở CP3 |

**Bottleneck chính:** bước 5, đối chiếu qua lại (~10'). Bước 3 dài hơn (12') nhưng không phải nghẽn: phần lớn nội dung CHECKPOINTS và worksheet chỉ cần khi làm tới CP đó, nên dời sang lúc làm được. Bước 5 thì không dời được. Đây là chỗ học viên sót điều kiện chấm, và mỗi điều kiện bị sót mất 2–5 điểm (thiếu thời gian từng bước trừ 2, thiếu tiêu chí đánh giá trừ 3, sai tên repo/file trừ 5).

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 6 bước, khoảng 18 phút/lab (ước tính, đo lại ở lab sau), 4/6 bước thủ công
(Trước đó: fork + clone theo README "Bắt đầu", như cũ)

[1 Chạy 2 lệnh gom ô tự kiểm + điều kiện chấm: 1']          ← RULE (lệnh trong report/assets/cp4-doc-review.md, mục 4)
→ [2 Đọc SUBMISSION mục "Cấu trúc và file phải nộp": 3']     ← CON NGƯỜI (No AI: đổi thứ tự đọc)
→ [3 Đọc danh sách gom (~56 dòng), xếp vào từng CP: 8']      ← CON NGƯỜI
→ [4 Mở đoạn gốc theo số dòng cho dòng chưa rõ;
     kiểm mỗi tiêu chí C1–C11 có ít nhất 1 dòng: 3']         ← CON NGƯỜI KIỂM (HITL)
→ [5 Chạy 2 lệnh kiểm tên repo + tên file báo cáo: 1']      ← RULE (mục 5 của file trên)
     báo sai → sửa ngay (Settings → General → Repository name; đổi tên file)
→ [6 Chốt danh sách việc cần nộp, đưa nhóm xem ở CP3: 2']    ← CON NGƯỜI

Chạy lại bước 5 trước khi nộp, cùng lúc rà checklist SUBMISSION.
Đọc CHECKPOINTS + worksheet: chuyển sang lúc làm từng CP, không tính vào thời gian trên.
Không có bước AI.

BOUNDARY: lệnh chỉ trích nguyên văn các dòng có trong đề, không tóm tắt, không suy ra yêu cầu mới.
          Lệnh kiểm tên chỉ báo đúng/sai, không tự đổi tên. Học viên tự quyết làm phần nào trước.
          File đề gốc luôn là nguồn cuối cùng.
PHƯƠNG ÁN QUAY VỀ: lệnh gom ra 0 dòng, hoặc có tiêu chí C1–C11 không có dòng nào (đề lab khác không dùng
          ô "- [ ]" hay chữ "trừ/tối đa") → đọc theo thứ tự SUBMISSION → RUBRIC → CHECKPOINTS và tự ghi
          checklist như cũ. Lệnh kiểm tên lỗi hoặc đề đổi mẫu tên → so tên bằng mắt với SUBMISSION.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 | 6 | Bỏ bước đọc trước CHECKPOINTS + worksheet, thêm bước kiểm tên |
| Tổng thời gian | 45' | khoảng 18' | Ước tính; target chính ≤ 20', đo bằng bấm giờ ở 2 lab tiếp theo |
| Số bước thủ công | 6/6 | 4/6 | Bước 1 và 5 là Rule |
| Lượng chữ phải đọc để biết điều kiện chấm | 10.012 từ (6 file) | 1.687 từ (56 dòng) + đoạn gốc khi cần | Đếm bằng `wc -w` |
| Kiểm tên repo, tên file | Không có bước kiểm; dễ quên đổi tên (SV-02) | Lệnh báo ngay sau khi làm; kỳ vọng 0 lỗi khi nộp | Lệnh đã báo đúng 8/8 tên repo thử và 5/5 tên file thử |
| Bottleneck chính | Đối chiếu qua lại (10') | Đọc danh sách gom (8') | Chấp nhận được: đây là lúc học viên hiểu điều kiện chấm |
| Rủi ro mới phát sinh | — | Lệnh gom bắt thiếu khi đề đổi cách viết; lệnh kiểm tên báo cả tên `Day02` (chữ thường), có thể không bị tính là sai | Xử lý ở bước 4 (kiểm C1–C11) và phương án quay về |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Học viên K5 lớp L3B mở đề một lab mới có cả phần cá nhân và phần nhóm |
| **Quy trình** | Đầu buổi lab: đọc README → RULES → CHECKPOINTS + worksheet → RUBRIC + SUBMISSION → đối chiếu qua lại giữa các file → tự ghi danh sách việc cần nộp |
| **Bottleneck** | Bước đối chiếu qua lại (~10'): 25 điều kiện được/mất điểm nằm rải ở RUBRIC, CHECKPOINTS và SUBMISSION; 6 điều kiện không có trong 32 ô tự kiểm |
| **Impact** | 45'/lab, gần 1/5 buổi lab 240'. Sót yêu cầu là chuyện có thật: 2/2 người được phỏng vấn từng sót 1 yêu cầu có sẵn (thiếu phần giải thích lựa chọn; để tên file mặc định). Sai tên repo hoặc tên file bị trừ 5 điểm (RUBRIC), dù quy tắc có trong checklist SUBMISSION |
| **Success Metric** (baseline → target, cách đo) | Thời gian từ lúc mở đề tới lúc có danh sách việc cần nộp: 45' (tự ghi, 1 người, Day 02) → ≤ 20'. Đo bằng bấm giờ ở lab tiếp theo |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Công cụ (AI hay không) không được tự quyết bỏ qua yêu cầu nào, không được thêm yêu cầu không có trong đề, không thay học viên đọc đoạn gốc khi chưa rõ. HITL: học viên đối chiếu mọi dòng chưa rõ với đoạn gốc trước khi chốt danh sách |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

Nhóm đưa v0 cho AI với prompt "chỉ ra lỗ hổng, không viết lại".

- AI: metric chỉ đo thời gian; nhanh hơn mà sót điều kiện thì sao? → **Đồng ý.** Thêm metric độ phủ và số lỗi tên ở v1.
- AI: baseline 45' là của 1 người tự ghi → **Đồng ý.** Đây là giả định #1; phỏng vấn 2 người cho kết quả trái chiều (SV-01 mất 35' đối chiếu, SV-02 chỉ 14'). Pilot sẽ bấm giờ lại và poll thêm người.
- AI: Impact dẫn lỗi đặt tên, nhưng lỗi đó xảy ra lúc fork và đặt tên, mà quy trình không ghi bước này; Impact và quy trình đang lệch nhau → **Đồng ý.** Ở v1, thêm bước fork + đặt tên vào quy trình, và thêm metric 0 lỗi tên.
- AI: bước 3 (12') dài hơn bước 5 (10'), sao chọn bước 5 làm bottleneck? → **Đồng ý cần giải thích.** Ghi lý do vào v1: bước 3 dời được sang lúc làm từng CP, bước 5 thì không.
- AI: boundary viết chung cho "công cụ" vì chưa chọn mức → **Đồng ý.** Viết lại cụ thể ở v1 sau khi chọn Rule.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **độ mơ hồ thấp × độ phức tạp thấp** → Rule hoặc Workflow đơn giản thường đủ.

Vì sao:

- **Độ mơ hồ thấp:** mỗi điều kiện có đúng/sai rõ. Nó có hoặc không có trong đề, và trích nguyên văn được. Tên repo, tên file thì đúng hoặc sai theo một mẫu cố định. Không cần "viết hay", chỉ cần đủ và đúng.
- **Độ phức tạp thấp:** chỉ 3 file chứa điều kiện (RUBRIC, CHECKPOINTS, SUBMISSION), các bước cố định, không rẽ nhánh, bước sau không cần suy luận từ bước trước.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Đổi thứ tự đọc: SUBMISSION → RUBRIC → CHECKPOINTS. Đề nghị coach ghi "bị trừ nếu…" cạnh từng ô tự kiểm (TILT, phần Criteria) và nói rõ `DAY02` có phân biệt hoa/thường không | Đủ cho phần "nộp file gì, đặt ở đâu" (SUBMISSION đã gom) | Vẫn phải tự đối chiếu 25 điều kiện; không giúp lỗi lúc làm như quên đổi tên (SV-02: biết quy tắc mà vẫn sai). Phần đề nghị coach không nằm trong tay học viên | **Dùng kèm** (bước 2) |
| **Rule** | 2 lệnh `grep` gom 32 ô tự kiểm và 24 dòng điều kiện của RUBRIC vào 1 danh sách (56 dòng, 1.687 từ thay vì 10.012 từ), cộng 2 lệnh kiểm tên repo và tên file bằng regex | Đề dùng ô `- [ ]` và các chữ "trừ / tối đa / bị 0"; mẫu tên cố định. Thử trên Day 02: lệnh gom bắt 25/25 điều kiện, lệnh kiểm tên báo đúng 8/8 tên repo thử và 5/5 tên file thử | Đề lab khác đổi cách viết thì bắt thiếu; 5 dòng nhiễu; báo cả tên `Day02` | **Chọn** |
| **Workflow** | Nạp file `.md` của đề vào NotebookLM → prompt cố định "liệt kê điều kiện được/mất điểm theo CP, kèm trích dẫn" → học viên kiểm từng trích dẫn | Đề không có cấu trúc cố định để Rule bắt | Bỏ sót hoặc diễn giải sai điều kiện; mỗi lab phải nạp lại; tốn thời gian kiểm trích dẫn; vẫn cần Rule để kiểm tên | Dự phòng, nếu chạm ngưỡng dừng |
| **Agent** | AI tự mở repo, tự quyết đọc file nào, tự theo dõi tiến độ, tự đổi tên repo | Khi bước tiếp theo không đoán trước được, không đúng với bài này | Quá rộng; có thể tự quyết bỏ qua yêu cầu hoặc tự đổi tên repo; khó kiểm | Không chọn |

**Mức chọn:** Rule (kèm thay đổi No AI ở bước đọc).

**Vì sao không chọn mức đơn giản hơn:** chỉ đổi thứ tự đọc (No AI) thì biết được file phải nộp, nhưng không gom được 6 điều kiện nằm ngoài ô tự kiểm, nên học viên vẫn kẹt ở đúng bước nghẽn. Phỏng vấn còn cho thấy đọc thôi là chưa đủ: SV-02 biết quy định đặt tên mà vẫn quên đổi tên file, chỉ bắt được nhờ bước kiểm cuối. Cần một bước kiểm tự động sau khi làm, và đó là Rule.

**Vì sao không cần mức cao hơn:** Rule chạy thử đã bắt 25/25 điều kiện của Day 02 và báo đúng 8/8 tên repo thử. Cả 2 người được phỏng vấn đều tự xử lý bằng checklist, không ai cần đến AI. Đầu ra cần có là những câu đã có sẵn trong đề và phép so mẫu tên, nên không cần AI tạo nội dung. Thêm AI là thêm rủi ro diễn giải sai, mà bước kiểm của con người vẫn phải giữ nguyên.

### 6.3. AI Canvas rút gọn

Không bắt buộc vì nhóm chọn Rule. Lý do bài không cần AI: đầu ra là câu nguyên văn có sẵn trong đề và kết quả so mẫu tên, có đúng/sai rõ; Rule đã bắt đủ 25/25 điều kiện ở Day 02 và báo đúng 8/8 tên repo thử.

Nhóm vẫn điền nhanh cho **phương án dự phòng (Workflow)**, để nếu chạm ngưỡng dừng thì biết ngay cần gì:

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Danh sách điều kiện được/mất điểm xếp theo CP, mỗi dòng kèm trích dẫn tới đoạn gốc |
| **Judgment** — con người cân nhắc, quyết định gì? | Dòng nào đúng là điều kiện; dòng nào AI diễn giải sai; làm phần nào trước |
| **Action** — hành động cuối cùng là gì, ai làm? | Học viên chốt danh sách việc cần nộp và đưa nhóm xem ở CP3 |
| **Outcome** — đo kết quả bằng gì? | Phút từ lúc mở đề tới lúc có danh sách; số điều kiện bị sót; số điểm bị trừ vì sót |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Các file `.md` của đề lab. Có sẵn, công khai, NotebookLM nhận Markdown |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Dòng học viên phải sửa hoặc xóa; điều kiện bị sót phát hiện khi nhận điểm |

### 6.4. Hai câu hỏi của Google PAIR

Không bắt buộc vì nhóm chọn Rule. Ghi lại vì câu trả lời vẫn ảnh hưởng tới thiết kế Rule:

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: nghiêng về augment, nhưng bằng chứng còn mỏng. Card #1 ghi "AI không quyết định thay tôi phần nào được bỏ qua"; cả 2 người được phỏng vấn đều tự lập checklist và tự đối chiếu, SV-01 hỏi giảng viên khi chưa rõ. Vì vậy lệnh kiểm tên chỉ báo, không tự đổi tên.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: **bỏ sót tệ hơn.** Sót 1 điều kiện mất 2–5 điểm, còn 1 dòng báo nhầm chỉ tốn vài giây đọc lướt. Vì vậy mẫu tìm của lệnh gom được đặt rộng (chấp nhận 5 dòng nhiễu), bước 4 kiểm mỗi tiêu chí C1–C11 có ít nhất 1 dòng, và lệnh kiểm tên báo cả tên `Day02` (chữ thường) dù chưa chắc bị tính là sai.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Học viên K5 lớp L3B mở đề một lab mới có cả phần cá nhân và phần nhóm |
| **Quy trình** | Đầu buổi lab: đọc README và fork, đặt tên repo theo bước "Bắt đầu" → RULES → CHECKPOINTS + worksheet → RUBRIC + SUBMISSION → đối chiếu qua lại giữa các file → tự ghi danh sách việc cần nộp. Không có bước kiểm lại tên repo, tên file |
| **Bottleneck** | Bước đối chiếu qua lại (~10'): 25 điều kiện được/mất điểm nằm rải ở 3 file, 6 điều kiện không có ô tự kiểm. Bước đọc CHECKPOINTS + worksheet (12') dài hơn nhưng dời được sang lúc làm từng CP, nên không phải nghẽn |
| **Impact** | 45'/lab, gần 1/5 buổi lab 240'. Sót 1 điều kiện có thể mất 2–5 điểm; 2/2 người được phỏng vấn từng sót 1 yêu cầu có sẵn |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian từ lúc mở đề tới lúc có danh sách việc cần nộp: 45' → ≤ 20', bấm giờ ở 2 lab tiếp theo. (2) Danh sách bắt được 100% điều kiện được/mất điểm (Day 02: 25/25), đo bằng đối chiếu với bảng điều kiện lập theo mẫu [cp4-doc-review.md](../assets/cp4-doc-review.md). (3) 0 lỗi tên repo và tên file báo cáo lúc nộp, đo bằng lệnh kiểm ở bước 5; 0 điểm bị trừ vì sót một yêu cầu có trong đề, đo bằng kết quả chấm |
| **Boundary** | Lệnh chỉ trích nguyên văn dòng có trong đề kèm tên file và số dòng; không tóm tắt, không suy ra yêu cầu mới, không quyết bỏ qua yêu cầu nào. Lệnh kiểm tên chỉ báo, không tự đổi tên. File đề gốc là nguồn cuối cùng. HITL: học viên mở đoạn gốc cho mọi dòng chưa rõ và kiểm mỗi tiêu chí C1–C11 có ít nhất 1 dòng; nhóm xem lại danh sách ở CP3 trước khi chia việc |
| **AI intervention point** | Không có. Đầu ra là câu có sẵn trong đề và phép so mẫu tên, có đúng/sai rõ; Rule đã bắt đủ 25/25 điều kiện ở Day 02 và báo đúng 8/8 tên repo thử. Thêm AI chỉ thêm rủi ro diễn giải sai |
| **Mức chọn** | Rule (kèm No AI: đổi thứ tự đọc SUBMISSION → RUBRIC → CHECKPOINTS) |
| **Rủi ro & người kiểm tra** | Đề lab sau đổi cách viết, lệnh gom bắt thiếu mà không báo → học viên kiểm ở bước 4 (mỗi tiêu chí C1–C11 phải có ít nhất 1 dòng). Lệnh kiểm tên báo nhầm tên `Day02` → học viên đọc lại SUBMISSION hoặc hỏi coach. Người điều phối nhóm xem lại danh sách trước CP3 |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Quy trình | Không ghi bước fork và đặt tên repo | Thêm bước fork + đặt tên repo, ghi rõ không có bước kiểm lại | Phản biện: Impact dẫn lỗi đặt tên mà quy trình không có bước đó; SV-02 cho thấy lỗi tên xảy ra lúc làm, không phải lúc đọc đề |
| Success Metric | Chỉ đo thời gian: 45' → ≤ 20' | Thêm (2) độ phủ 100% điều kiện và (3) 0 lỗi tên, 0 điểm bị trừ vì sót | Phản biện: nhanh hơn mà sót điều kiện thì không đạt |
| Boundary | Viết chung cho "công cụ (AI hay không)" | Viết riêng cho Rule: chỉ trích nguyên văn, kèm số dòng; lệnh kiểm tên chỉ báo; HITL ở bước kiểm C1–C11 và ở CP3 | Đã chọn mức Rule ở CP6 |
| Bottleneck | Đối chiếu qua lại ~10' | Thêm lý do không chọn bước 3 (12') | Phản biện: bước 3 dài hơn, cần giải thích |

**Tiêu chí đánh giá đầu ra của giải pháp (Rule, 5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đủ điều kiện | Mỗi tiêu chí C1–C11 và mỗi quy tắc chấm của RUBRIC có ít nhất 1 dòng trong danh sách | Có tiêu chí hoặc quy tắc chấm không xuất hiện dòng nào |
| 2 | Nguyên văn, có vị trí | Mỗi dòng giữ nguyên chữ của đề, kèm tên file và số dòng | Dòng bị sửa chữ, cắt mất phần điều kiện, hoặc không có số dòng |
| 3 | Ít nhiễu | Dòng không phải điều kiện ≤ 10% tổng số dòng (Day 02: 5/56, khoảng 9%) | Dòng nhiễu > 10% |
| 4 | Nhanh | Chạy lệnh + đọc xong danh sách ≤ 12' (bước 1 + 3 của quy trình tương lai) | Hơn 12' |
| 5 | Kiểm tên đúng | Lệnh báo "sai" cho mọi tên lệch mẫu và "đúng" cho mọi tên đúng mẫu. Đã chạy trên 8 tên repo thử (2 đúng, 6 kiểu sai hay gặp): khớp 8/8; trên 5 tên file mẫu: khớp 5/5 | Bỏ qua một tên sai, hoặc báo sai một tên đúng |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

Chấm cho giải pháp được chọn: Rule + đổi thứ tự đọc.

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | TB | Pain có bằng chứng hành vi: 2/2 người được phỏng vấn từng sót 1 yêu cầu có sẵn; 6/25 điều kiện không có ô tự kiểm. Nhưng mới có 2 người, cả 2 kể về môn học khác chứ không phải lab K5; thời gian trái chiều (35' và 14'); con số 45' mới của 1 người; chưa biết học viên có chịu chạy lệnh không |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Thấp | Lệnh copy-paste; đầu ra là văn bản thuần có số dòng, hoặc một câu "đúng/sai". Không chạy được terminal thì dùng ô tìm kiếm regex của VS Code |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | TB | Chạy được ở Day 02 (25/25 điều kiện, 8/8 tên repo thử), với cả GNU grep và ugrep. Chưa biết đề các lab khác có cùng cách viết không (giả định #4) |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Thấp | Không tốn tiền; đề nằm sẵn trên máy, không gửi dữ liệu ra ngoài; không trái RULES. Mỗi học viên tự chạy, không cần ai vận hành |

### 8.2. Kết luận

**Quyết định:** No-Go cho AI. Dùng Rule + đổi thứ tự đọc.

**Lý do:** theo worksheet, chọn No-Go khi No AI hoặc Rule đã đủ, và đây là trường hợp đó. Bài có độ mơ hồ thấp; Rule chạy thử đã bắt đủ 25/25 điều kiện và báo đúng 8/8 tên repo thử. Giải pháp Rule không có rủi ro mức Cao; hai rủi ro TB (Value, Feasibility) kiểm được ngay ở 2 lab tiếp theo.

**Nếu Go — pilot nhỏ nhất:** không áp dụng (không dùng AI).

**Nếu Not Yet — cần kiểm chứng gì trước:** không áp dụng.

**Nếu No-Go — nên làm gì thay AI:**

- Ở lab Day 03, 4 thành viên nhóm cùng làm theo quy trình tương lai ở mục 4.2: chạy lệnh gom, đọc SUBMISSION trước, chạy lệnh kiểm tên, bấm giờ từ lúc mở đề tới lúc có danh sách.
- Mỗi người chấm đầu ra theo 5 tiêu chí đánh giá ở mục 7; ghi số tiêu chí RUBRIC không có dòng nào.
- Poll 5–10 bạn nhóm khác bằng bộ câu hỏi ở mục 9, để có baseline thời gian của người khác (giả định #1).
- Gửi coach 2 đề nghị: (1) ghi "bị trừ nếu…" cạnh từng ô tự kiểm (TILT, phần Criteria); (2) nói rõ `DAY02` có phân biệt hoa/thường không, vì chính repo đề đang tên `Day02`.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

- Nếu sau 2 lab (Day 03 và Day 04) mà lệnh gom vẫn để sót ít nhất 1 tiêu chí của RUBRIC, hoặc tổng thời gian vẫn trên 20' → chuyển lên phương án dự phòng **Workflow** (NotebookLM có trích dẫn, mục 6.2–6.3).
- Nếu poll cho thấy từ 2/3 người trở lên chỉ mất dưới 15' đọc đề → bỏ lệnh gom, chỉ giữ đổi thứ tự đọc (**No AI**) và lệnh kiểm tên.
- Nếu đã chạy lệnh kiểm tên mà nhóm vẫn nộp sai tên → xem lại bước 5 (có chạy thật không, hay mẫu trong lệnh đã cũ so với đề).

---

## 9. Hạn chế và hướng tiếp theo

- **Mới phỏng vấn 2 người, cả 2 kể về đồ án học phần và báo cáo thực tập, không phải lab K5.** Số phút là người được hỏi kể lại. Giả định #1 (thời gian của người khác) có tín hiệu trái chiều: 35' và 14'. Bộ câu hỏi poll 5–10 bạn trong lớp ở lab sau, hỏi về chuyện đã xảy ra:
  1. Từ lúc mở repo đề tới lúc bắt đầu làm checkpoint đầu tiên, bạn mất khoảng bao nhiêu phút?
  2. Bạn đã mở những file nào, theo thứ tự nào?
  3. Bạn đọc RUBRIC.md vào lúc nào: trước khi làm, giữa chừng, gần lúc nộp, hay chưa đọc?
  4. Ở lab trước, có lần nào bạn phát hiện mình thiếu hoặc làm sai một yêu cầu không? Là yêu cầu gì?
  5. Hiện bạn làm gì để khỏi sót yêu cầu?
- Lệnh kiểm tên mới thử trên 8 tên repo do nhóm tự đặt và repo của nhóm, chưa thử trên tên thật của các nhóm khác.
- Chưa rõ tên `Day02` (chữ thường) có bị tính là sai không; lệnh kiểm tên hiện báo là sai để người dùng tự xem lại.
- Rule mới thử trên 1 đề (Day 02). Giả định #4 (các lab khác cùng cách viết) chỉ kiểm được ở lab sau.
- 25 điều kiện là nhóm tự tách từ RUBRIC; tách hoặc gộp khác thì con số có thể đổi nhẹ.
- Thời gian quy trình tương lai (18') là ước tính, chưa bấm giờ.
- Hướng tiếp theo: #6 Chờ VinBus (Trần Tùng Lâm ghi giờ 1 tuần để có baseline); #7 + #12 Tổng hợp tài liệu nghiên cứu (Vũ Quang Hải, Nguyễn Anh Quân) nếu đo được thời gian thật.

## 10. Tài liệu tham khảo

- Review tài liệu và thử Rule của nhóm: [report/assets/cp4-doc-review.md](../assets/cp4-doc-review.md)
- Đề Day 02: [README.md](../../README.md), [RULES.md](../../RULES.md), [CHECKPOINTS.md](../../CHECKPOINTS.md), [RUBRIC.md](../../RUBRIC.md), [SUBMISSION.md](../../SUBMISSION.md), [docs/01-worksheet.md](../../docs/01-worksheet.md)
- University of Oregon, Transparent Assignment Design: https://teaching.uoregon.edu/transparent-assignment-design
- TILT Higher Ed (Mary-Ann Winkelmes): https://tilthighered.com/
- Google, Use chat in NotebookLM / Gemini Notebook: https://support.google.com/notebooklm/answer/16179559
- Google, Add or discover new sources for your notebook: https://support.google.com/notebooklm/answer/16215270
- GitHub Docs, Use autograding: https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/use-autograding
- Teresa Torres, Opportunity Solution Trees: https://www.producttalk.org/opportunity-solution-trees/
- Rob Fitzpatrick, The Mom Test: https://www.momtestbook.com/
- Strategyzer, Assumptions Mapping: https://www.strategyzer.com/library/how-assumptions-mapping-can-focus-your-teams-on-running-experiments-that-matter
- Anthropic, Building effective agents: https://www.anthropic.com/research/building-effective-agents
- Google PAIR, User Needs + Defining Success: https://pair.withgoogle.com/chapter/user-needs/
- Marty Cagan (SVPG), The Four Big Risks: https://www.svpg.com/four-big-risks/
