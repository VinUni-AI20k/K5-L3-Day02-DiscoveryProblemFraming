# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: 113
- Thành viên: Đỗ Minh Hoàng (2A202603554), Bùi Xuân Thành (2A202603521), Lê Xuân Hạ (2A202603571), Hoàng Văn Bảo (2A202603549) — xem chi tiết tại `TEAM.md`
- Candidate problem được chọn (1 câu): Khi giao deadline, tôi muốn biết ai đã nắm deadline, để chủ động theo dõi tiến độ mà không phải nhắn tin giục riêng từng người.
- Quyết định cuối: Go, phạm vi nhỏ (Pilot)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Bảo | Khi nhận 80 CV cho một vị trí, tôi muốn biết nhanh ai đáp ứng 3 tiêu chí bắt buộc, để chỉ gọi phỏng vấn đúng người | HR tuyển dụng | Đọc từng CV: khoảng 160 phút/vị trí (tổng 225-250 phút) | Không có AI thì cách đơn giản nhất để giảm một nửa thời gian là gì? Có dùng form lọc trước được không? (Hoàng hỏi) |
| 2 | Bảo | Khi ứng viên không đạt, tôi muốn gửi thư từ chối lịch sự có nhắc đúng vị trí và vòng đã qua, để ứng viên không bị bỏ lơ | HR tuyển dụng | Sửa và cá nhân hóa thư: 1,5 phút/thư, 70 thư/tháng | Mail merge kết hợp template có sẵn đã giải được bài này chưa mà phải cần AI? (Thành hỏi) |
| 3 | Bảo | Khi trưởng bộ phận sắp phỏng vấn, họ muốn có sẵn tóm tắt hồ sơ trước giờ vào phòng, để không phải mở CV lúc đang ngồi với ứng viên | Trưởng bộ phận (HR chuẩn bị) | Đọc CV 5 trang sát giờ: khoảng 8 phút | Ai ngoài bạn gặp vấn đề này? Có bằng chứng sếp phàn nàn vì không kịp đọc CV không? (Hạ hỏi) |
| 4 | Hoàng | Khi kết thúc buổi họp nhóm, tôi muốn lọc nhanh các ý vừa bàn thành danh sách việc cần làm, để cả nhóm nắm được việc và không bị trôi task | Nhóm trưởng / Thư ký | Đọc lại ghi chú thô và viết lại to-do list: mất 15-20 phút (tổng 30 phút) | Nếu lúc họp ghi chép vội, viết tắt hay nói đùa thì AI có gán nhầm việc cho người khác không? (Bảo hỏi) |
| 5 | Hoàng | Khi sắp nộp bài tập lớn/đồ án, tôi muốn chuẩn hóa lại lề trang, font chữ và trích dẫn, để bài nộp đúng mẫu không bị trừ điểm oan | Bạn ghép bài cuối cùng | Mò mẫm đối chiếu trích dẫn với danh mục tài liệu cuối bài: mất 35 phút | Dùng template Word mẫu với Zotero quản lý trích dẫn từ đầu có giải quyết triệt để mà không cần AI không? (Thành hỏi) |
| 6 | Hoàng | Khi ôn thi cuối kỳ, tôi muốn gom kiến thức trọng tâm từ slide, sách và câu hỏi thảo luận, để ôn trúng trọng tâm không bị sót | Sinh viên ôn thi | Đọc hàng trăm trang slide và sách chép công thức: mất 180 phút | Tài liệu mỗi môn một kiểu (chữ, hình vẽ, công thức toán), gom tự động có bị lỗi vỡ định dạng không? (Hạ hỏi) |
| 7 | Hạ | Khi họp Triage, Tech Lead muốn danh sách bug xếp sẵn theo độ nghiêm trọng, để quyết định fix hay hoãn | Tech Lead, PM Lead | Buổi họp 45 phút thường lố giờ 15–20 phút vì đọc từng ticket | Họp lố 15–20 phút là do chưa xếp sẵn thứ tự bug, hay do vào họp hai Lead mới bắt đầu ngồi đọc từng ticket và bàn cách sửa lỗi? (Hoàng hỏi) |
| 8 | Hạ | Khi có bug mới tạo trên Jira, tôi muốn bug tự phân loại mức độ ưu tiên, để không mất công phân loại thủ công | QA / Tester | Ngồi đọc mô tả bug và chọn mức độ nghiêm trọng: 10 phút/ngày | Tech Lead và PM Lead đã thống nhất được cách tính "độ nghiêm trọng" chưa, hay mỗi người một quan điểm? (Bảo hỏi) |
| 9 | Hạ | Khi chuẩn bị họp duyệt lỗi, tôi muốn lọc nhanh các lỗi trùng lặp, để không mất thời gian bàn lại lỗi cũ | Tech Lead | Rà soát tìm các ticket bị trùng nội dung: mất 20 phút trước họp | Chỉ cần bắt buộc người tạo bug chọn Priority trên Jira rồi bấm sort trước giờ họp là xong, có thực sự cần làm công cụ tự động hay dùng AI không? (Thành hỏi) |
| 10 | Thành | Khi giao deadline, tôi muốn biết ai đã nắm deadline, để chủ động theo dõi tiến độ | Nhóm trưởng | Nhắn riêng và nhắc lại từng người: 6 tin nhắc/tuần, 2 lần phải nhắc lần 2 mới có phản hồi | Nếu cả nhóm đều react "đã nhận" mà vẫn làm trễ, thì việc giảm số tin nhắc có còn chứng minh vấn đề đã được giải không? (Hoàng hỏi) |
| 11 | Thành | Khi nhận chỉ dẫn thiếu ngữ cảnh, tôi muốn xác nhận đúng ý trước khi làm, để không phải làm lại | Thành viên nhận việc | Làm luôn mà không xác nhận: 3 lượt hỏi để làm rõ, mỗi lần hiểu sai mất ~25 phút làm lại | Thêm bước xác nhận cũng tốn thời gian chờ người giao trả lời; nếu họ trả lời chậm thì tổng thời gian có còn ít hơn 25 phút làm lại không? (Bảo hỏi) |
| 12 | Thành | Khi một câu hỏi bị hỏi lại, tôi muốn biết nó đã được trả lời chưa, để không phải trả lời lại | Người hay phải trả lời (nhóm trưởng) | Tìm lại thông tin rải giữa Zalo và Discord: trước hạn ~30 phút có 1 câu hỏi lặp, ~3 phút mỗi lần trả lời | Thành viên đã ngại kéo chat tìm lại, vậy điều gì đảm bảo họ chịu mở FAQ hoặc hỏi bot thay vì hỏi thẳng vào nhóm? (Hạ hỏi) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Theo dõi tiến độ & Giao việc | #4 (Gom việc sau họp - Hoàng), #10 (Biết ai nắm deadline - Thành), #11 (Xác nhận rõ chỉ dẫn trước khi làm - Thành) | Sau khi bàn bạc/giao việc, thông tin bị trôi hoặc thiếu sự cam kết 2 chiều, dẫn đến trễ hạn hoặc làm sai |
| B — Phân loại & Xử lý yêu cầu định kỳ | #1 (Lọc 80 CV theo 3 tiêu chí - Bảo), #7 (Xếp thứ tự bug trước họp - Hạ), #8 (Tự phân loại độ ưu tiên bug - Hạ), #9 (Lọc bug trùng lặp - Hạ) | Phải đọc lướt qua một lượng lớn đầu mục (CV, bug ticket) để phân loại/xếp thứ tự trước khi đưa ra quyết định |
| C — Tổng hợp & Chuẩn hóa tài liệu | #3 (Tóm tắt hồ sơ ứng viên trước phỏng vấn - Bảo), #5 (Chuẩn hóa lề/trích dẫn đồ án - Hoàng), #6 (Gom kiến thức ôn thi từ slide - Hoàng), #12 (Tìm câu trả lời cho câu hỏi bị lặp - Thành) | Gom góp, bóc tách và định dạng lại thông tin từ nhiều nguồn rải rác để người khác dễ đọc và sử dụng |
| D — Phản hồi & Giao tiếp tự động | #2 (Gửi thư từ chối ứng viên cá nhân hóa - Bảo) | Tốn thời gian sửa tay câu chữ lặp đi lặp lại để gửi phản hồi lịch sự cho từng người |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian lãng phí và đảm bảo 100% công việc/deadline được các thành viên nắm rõ và hoàn thành đúng hạn
├── Opportunity A: Nhóm trưởng không biết thành viên đã thực sự đọc và nắm deadline hay chưa sau khi giao việc
├── Opportunity B: Thành viên nhận chỉ dẫn mơ hồ, không dám hỏi lại hoặc hỏi đi hỏi lại làm mất thời gian đôi bên
├── Opportunity C: Nhóm trưởng mất nhiều thời gian đi nhắn tin riêng giục từng người trước mỗi hạn chót
└── Opportunity D: Việc đã bàn trong cuộc họp bị trôi và không có người đứng ra nhận trách nhiệm rõ ràng
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ "Chatbot AI tự động nhắn tin nhắc việc qua Zalo/Discord" (Gạch bỏ vì đây là giải pháp/công cụ, không phải nhu cầu cốt lõi của người dùng).
- ✗ "Bảng Trello/Notion tự động đổi màu cảnh báo" (Gạch bỏ vì là tính năng công cụ).
- ✗ "Hệ thống AI tự chấm điểm và phân chia task cho thành viên" (Gạch bỏ vì là solution trá hình).

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Theo dõi ai nắm deadline (Thành) | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| Gom việc sau họp nhóm thành to-do list (Hoàng) | 5 | 4 | 4 | 4 | 5 | 4 | 5 | 31 |
| Xếp thứ tự bug trước họp Triage (Hạ) | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 28 |
| Lọc CV đáp ứng tiêu chí bắt buộc (Bảo) | 4 | 4 | 4 | 4 | 3 | 4 | 3 | 26 |

**Candidate được chọn:** Theo dõi ai đã nắm deadline khi giao việc (Đề tài của Thành).

**Vì sao chọn:**
- Nỗi đau cực kỳ thực tế và nhức nhối với mọi nhóm sinh viên/team làm việc: giao việc xong không biết ai đã đọc, ai đã nắm, nhóm trưởng phải đi nhắn riêng từng người (6 tin nhắc/tuần, nhiều lần phải giục lần 2 mới trả lời).
- Quy trình rất gọn, các bước rõ ràng (giao việc -> chờ xác nhận -> nhắn nhắc -> kiểm tra tiến độ).
- Rất vừa sức một buổi lab, nhóm hiểu sâu domain và dễ dàng mang ra thử nghiệm, so sánh rõ ràng giữa các mức No AI, Rule, Workflow và Agent.

**Vì sao loại các candidate còn lại:**
- *Gom việc sau họp nhóm (Hoàng)*: Quy trình tốt nhưng phụ thuộc nhiều vào chất lượng ghi chép lúc họp (dễ bị viết tắt, nói đùa), rủi ro AI hiểu sai ngữ cảnh cao hơn.
- *Xếp thứ tự bug trước họp Triage (Hạ)*: Việc buổi họp lố giờ một phần do văn hóa và cách điều phối cuộc họp (hai Lead mải bàn giải pháp kỹ thuật) chứ chưa hẳn do thiếu công cụ xếp bug tự động; chỉ cần áp dụng luật cứng (timebox 2 phút/bug) là giải quyết được phần lớn vấn đề mà chưa cần đến AI.
- *Lọc CV tuyển dụng (Bảo)*: Cần tập dữ liệu CV thật và liên quan đến chính sách tuyển dụng doanh nghiệp, sinh viên trong nhóm ít hiểu sâu domain này nên khó kiểm chứng ngay trong buổi lab.

**Xử lý bất đồng (nếu có):**
- Ban đầu Hoàng và Hạ đều muốn bảo vệ đề tài của mình (Hoàng muốn làm gom việc sau họp, Hạ muốn làm tối ưu họp Triage). Tuy nhiên, sau khi cả nhóm phân tích các câu hỏi phản biện, nhóm nhận thấy bài của Hạ có thể giải quyết bằng luật cứng điều phối buổi họp (No-tech), còn bài của Hoàng thì bước tiếp theo vẫn là phải có người nhận deadline. Do đó, cả nhóm đồng thuận chọn bài của Thành vì giải quyết đúng khâu then chốt và dễ đo lường nhất. Đề tài của Hoàng và Hạ được lưu lại làm hướng phát triển tiếp theo.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Các nhóm trưởng khác cũng mất nhiều thời gian và ức chế vì phải nhắn tin giục riêng từng người để biết ai đã nắm deadline | Value | 5 | 2 | Có (phỏng vấn ngay) |
| 2 | Thành viên nộp bài trễ phần lớn là do quên hoặc trôi tin nhắn deadline, chứ không phải do cố tình phớt lờ | Value | 5 | 2 | Có (phỏng vấn ngay) |
| 3 | Thành viên chịu chủ động bấm nút xác nhận 'đã nắm deadline' nếu có công cụ hỗ trợ tiện lợi | Usability | 4 | 2 | Có |
| 4 | Có thể dùng các tính năng có sẵn (poll/bot nhắc việc trên Zalo, Discord, Notion) để tự động hóa khâu nhắc mà không cần tự code hệ thống mới | Feasibility | 4 | 4 | Research công cụ |
| 5 | Nhóm trưởng và các thành viên sẵn sàng duy trì việc dùng công cụ xác nhận trong suốt cả học kỳ | Viability | 4 | 2 | Thử nghiệm pilot |

Giả định nhóm kiểm chứng trong buổi này: Giả định #1 và #2 (Nỗi đau nhắn giục deadline có thật không và nguyên nhân trễ là do trôi tin/quên hay do cố tình).

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn theo bộ câu hỏi The Mom Test (phỏng vấn nhanh bạn học ở nhóm khác).

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Bạn Nam (Nhóm trưởng môn Phát triển ứng dụng Web, nhóm 5 người) |
| Câu nói đáng nhớ nhất (nguyên văn) | "Nhiều đứa thả tim tin nhắn giao việc trong nhóm cho có, đến sát hạn 2 tiếng mình hỏi bài đâu thì mới ngớ người bảo tưởng deadline là tuần sau." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước nộp báo cáo sprint 2, hạn là 23h chủ nhật. Đến 20h bạn ấy mở Google Drive vẫn chưa thấy phần code của 1 bạn. Nhắn tin riêng thì 30 phút sau bạn đó mới trả lời là đang đi ăn và chưa làm xong phần test. Nhóm trưởng phải ngồi tự gánh và làm thay đến 2h sáng mới nộp bài được. |
| Hiện đang xử lý bằng cách nào (workaround)? | Lập file Google Sheets ghi deadline, tag tên từng người trên nhóm Zalo và trước hạn 1 ngày phải tự vào nhắn tin riêng cho từng bạn để hỏi 'làm đến đâu rồi'. |
| Mất bao lâu, bao lần? | Mỗi tuần mất tầm 30-40 phút chỉ để đi rà soát và nhắn tin riêng giục 4 thành viên; tuần nào cũng phải nhắn ít nhất 2 lượt. |
| Insight / opportunity rút ra | Chỉ tag tên hoặc nhắn chung trong nhóm chat là vô tác dụng vì tin nhắn bị trôi. Cái nhóm trưởng cần không phải là tin nhắn nhắc chung chung, mà là một cơ chế xác nhận rõ ràng: thành viên phải ấn cam kết 'đã nắm hạn chót và đang làm' để nhóm trưởng biết ai chưa phản hồi mà xử lý sớm. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn sâu nhóm trưởng & thành viên nhóm khác | 3 người (2 nhóm trưởng, 1 thành viên) | Cả 2 nhóm trưởng đều xác nhận cực kỳ ngán việc phải đi nhắn tin riêng giục từng người; thành viên thừa nhận nếu chỉ nhắn trong group chat chung thì hay lướt qua rồi quên bẵng mất. | Thành viên phản bác: 'Nhiều khi tao biết rõ deadline nhưng do bài tập môn khác dồn dập quá nên không kịp làm, chứ không hẳn là do không biết hạn nộp'. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
- Nhóm nhận ra rằng giải pháp không chỉ đơn thuần là "gửi tin nhắn nhắc nhở tự động" (vì gửi nhiều quá sẽ bị coi là spam và người ta vẫn lờ đi).
- Vấn đề cốt lõi chuyển thành: Cần một cơ chế **xác nhận 2 chiều (Acknowledgment)** gọn nhẹ ngay khi giao deadline (thành viên xác nhận đã nắm + chọn thời điểm sẽ nộp bản nháp). Nếu ai chưa bấm xác nhận sau 24h thì hệ thống mới cảnh báo cho nhóm trưởng biết để can thiệp kịp thời.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Tính năng Bình chọn / Nhắc hẹn Zalo | https://zalo.me | Nhắc nhở hạn nộp và tạo bình chọn xác nhận trong nhóm chat | Có sẵn ngay trong ứng dụng chat hàng ngày của sinh viên, không cần cài thêm app mới | Phải tạo tay từng bình chọn; không tự động thống kê xem ai chưa bấm và không tự động nhắc lại | Tận dụng kênh Zalo quen thuộc nhưng cần cách gom và theo dõi trạng thái tự động hơn |
| Trello / Notion Due Date Reminder | https://trello.com | Đặt deadline cho từng thẻ công việc và tự đổi màu khi sắp đến hạn | Giao diện kéo thả trực quan, rõ ràng ai làm task nào | Chỉ là thông báo một chiều, người dùng lờ đi thì nhóm trưởng vẫn không biết họ đã bắt đầu làm chưa | Cần bước phản hồi tương tác (người làm bấm xác nhận) chứ không chỉ hiện ngày tháng tĩnh |
| Geekbot / Standuply (Bot nhắc việc trên Discord/Slack) | https://geekbot.com | Tự động hỏi thành viên tiến độ định kỳ và tổng hợp lại cho nhóm trưởng | Tự động hỏi theo lịch trình, gom câu trả lời về một nơi | Phức tạp, thường tính phí bản nâng cao và sinh viên hay ngại trả lời các câu hỏi dài dòng của bot | Chỉ cần thiết kế tương tác 1 chạm (bấm nút xác nhận) cực nhanh, không bắt gõ báo cáo dài dòng |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ:

```text
HIỆN TẠI — Mất khoảng 40–50 phút/tuần cho việc theo dõi

[1. Giao task & hạn nộp trên nhóm chat: 5'] 
→ [2. Chờ phản hồi tự giác (tin nhắn bị trôi): 1–2 ngày]
→ [3. Nhắn riêng từng người để hỏi 'đã nắm deadline chưa': 20'] ← BOTTLENECK
→ [4. Chờ trả lời & giải thích lại yêu cầu: 15']
→ [5. Đến sát giờ mở Drive kiểm tra xem ai nộp: 10']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Nhóm trưởng | Nội dung công việc sau họp | Tin nhắn giao việc trên nhóm Zalo/Discord | 5 phút / sau mỗi buổi họp | Tin nhắn thường bị trôi nhanh do các bạn tán gẫu |
| 2 | Thành viên | Tin nhắn trong nhóm | Lướt qua hoặc thả tim biểu tượng cảm xúc | 1–2 ngày chờ đợi | Không có gì đảm bảo là thành viên đã đọc kỹ hạn nộp |
| 3 | Nhóm trưởng | Danh sách việc chưa có xác nhận | Nhắn tin riêng cho từng bạn (4 người) | 20 phút / 2-3 lần mỗi tuần | Bước mệt mỏi nhất, phải giục lần 2 mới có người trả lời |
| 4 | Thành viên & Nhóm trưởng | Thắc mắc / lý do bận việc | Xác nhận lại thời gian nộp bài | 15 phút / tuần | Thành viên hay hỏi lại những chi tiết đã nói trong cuộc họp |
| 5 | Nhóm trưởng | Link thư mục nộp bài chung | Kiểm tra ai đã nộp, ai chưa nộp | 10 phút sát hạn nộp | Phát hiện trễ thì đã quá muộn để nhóm trưởng xoay sở |

**Bottleneck chính:** Bước 3 — Nhóm trưởng phải tốn 20 phút mỗi đợt để đi nhắn tin riêng cho từng thành viên hỏi xem đã nắm deadline chưa, tuần nào cũng phải lặp lại 2-3 đợt nhắn tin giục.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — Rút xuống còn 10–12 phút/tuần

[1. Nhóm trưởng nhập tóm tắt task vào template: 3' - Người]
→ [2. Hệ thống gửi tin nhắn giao việc kèm nút bấm xác nhận 1-chạm: 0' - Rule]
→ [3. Thành viên bấm 'Đã nắm & Cam kết nộp' (lưu trạng thái tự động): 1' - Người/Rule]
→ [4. AI quét danh sách ai chưa bấm sau 24h, soạn nháp tin nhắc lịch sự: 1' - AI]
→ [5. Nhóm trưởng duyệt nhanh tin nhắn nháp và gửi nhắc: 2' - Người duyệt (HITL)]
```

- **Bước 1 (Con người)**: Nhóm trưởng điền task, tên người làm và deadline vào form/template chuẩn.
- **Bước 2 (Rule)**: Hệ thống tự động tạo tin nhắn giao việc kèm nút tương tác xác nhận (Acknowledgment) trên Zalo/Discord/Notion.
- **Bước 3 (Người & Rule)**: Thành viên bấm nút xác nhận. Hệ thống tự cập nhật trạng thái "Đã nắm" vào bảng theo dõi.
- **Bước 4 (AI)**: Với những bạn chưa bấm xác nhận sau 24h hoặc sát hạn nộp 1 ngày, AI tự động soạn một đoạn tin nhắn nhắc nhở khéo léo, lịch sự có chèn đúng tên task và hạn nộp cụ thể.
- **Bước 5 (Con người duyệt - Human-in-the-loop)**: Nhóm trưởng liếc mắt duyệt qua tin nhắn nháp của AI rồi bấm gửi.
- **Boundary (Ranh giới an toàn)**: AI **không được phép** tự động gửi tin nhắn giục vào nhóm hay nhắn riêng cho thành viên; AI **không được** tự ý thay đổi deadline đã chốt. Nhóm trưởng là người bấm nút gửi cuối cùng.
- **Phương án quay về (Fallback)**: Nếu bot/AI bị lỗi mạng, nhóm trưởng mở bảng Google Sheets/Notion có sẵn trạng thái để tag tên trực tiếp các bạn chưa xác nhận bằng tay như cũ.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 bước rời rạc | 5 bước có phối hợp công cụ | Quy trình mới rõ ràng, minh bạch |
| Tổng thời gian | 40–50 phút/tuần | 10–12 phút/tuần | Giảm được ~75% thời gian theo dõi của nhóm trưởng |
| Số bước thủ công | 5 bước (100% làm tay) | 2 bước làm tay + 1 bước duyệt | Nhóm trưởng chỉ cần nhập đầu vào và duyệt cuối |
| Bottleneck chính | Nhắn tin riêng giục từng người (20p) | Duyệt tin nhắn nhắc nhở (2p) | Nút thắt được gỡ bỏ nhờ nút xác nhận tự động |
| Rủi ro mới phát sinh | Trôi tin nhắn, thành viên quên hạn | Thành viên bấm xác nhận bừa nhưng vẫn không làm | Cần bước cam kết giờ nộp bản nháp để kiểm chứng |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Nhóm trưởng sinh viên phụ trách quản lý tiến độ bài tập lớn/đồ án nhóm (3–5 người) |
| **Quy trình** | Giao việc trên nhóm chat -> Chờ phản hồi -> Nhắn tin riêng giục từng người -> Giải thích lại yêu cầu -> Kiểm tra bài nộp sát hạn |
| **Bottleneck** | Khâu nhắn tin riêng cho từng bạn để hỏi xem đã nắm deadline chưa (mất 20 phút/đợt, phải nhắn 2 lượt/tuần) vì tin nhắn chung trong nhóm bị trôi |
| **Impact** | Tốn 40-50 phút/tuần của nhóm trưởng; 1-2 lần mỗi tháng phát hiện thành viên chưa làm sát giờ nộp, buộc nhóm trưởng phải làm thay đến đêm muộn |
| **Success Metric** | Giảm thời gian theo dõi deadline từ 45 phút xuống dưới 12 phút/tuần; 100% thành viên bấm xác nhận nắm deadline trong 24h đầu; số lần bị trễ hạn nộp bài giảm về 0 |
| **Boundary** | AI chỉ hỗ trợ phát hiện ai chưa xác nhận và soạn nháp tin nhắn nhắc việc lịch sự; AI tuyệt đối không tự động nhắn tin cho thành viên và không được tự đổi deadline |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **Phản biện 1**: "Nếu thành viên cứ bấm nút 'Đã nắm' cho xong chuyện mà thực tế vẫn không chịu làm thì sao?"
  - *Nhóm đồng ý:* Đã bổ sung vào quy trình: khi bấm xác nhận, thành viên phải chọn kèm mốc thời gian cam kết gửi bản nháp (draft) trước ngày nộp chính thức 1 ngày.
- **Phản biện 2**: "Có cần thiết phải dùng AI để soạn tin nhắn nhắc nhở không, hay chỉ cần dùng 1 template tin nhắn cố định (Rule)?"
  - *Nhóm đồng ý một phần:* Với các lần nhắc thông thường, Rule dạng template là đủ. AI chỉ hữu ích khi cần tạo lời nhắc linh hoạt, khéo léo theo từng ngữ cảnh (ví dụ: nhắc bạn đang bận thi môn khác hoặc nhắc lần 2 mà không gây khó chịu). Nhóm giữ mức can thiệp là Workflow kết hợp Rule.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ thấp × Độ phức tạp thấp đến trung bình**

Vì sao:
- Quy trình giao việc và theo dõi deadline rất tường minh: có danh sách người làm, tên việc và thời hạn cụ thể (không bị mơ hồ).
- Độ phức tạp thấp: không cần suy luận logic nhiều bước phức tạp, chỉ cần bắt đúng trạng thái (đã bấm nút xác nhận hay chưa) và tạo nội dung nhắc nhở đúng người.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Bắt buộc họp xong ai cũng phải tự gõ vào bảng Excel/Notion chung và tự đặt báo thức điện thoại | Khi nhóm có ý thức tự giác cực cao, không ai quên việc | Mọi người hay quên cập nhật bảng chung, nhóm trưởng vẫn phải đi giục bằng tay | Không |
| **Rule** | Dùng bot tự động gửi poll/form Zalo, ai chưa vote sau 24h thì bot gửi 1 tin nhắn mẫu cố định để tag tên | Khi chỉ cần nhắc cứng nhắc, không quan tâm tới sắc thái ngữ cảnh | Tin nhắn mẫu lặp đi lặp lại dễ bị coi là spam, gây khó chịu hoặc bị tắt thông báo (mute) | Không (chỉ dùng làm nền) |
| **Workflow** | Rule tự bắt trạng thái ai chưa xác nhận -> AI soạn nháp tin nhắn nhắc nhở khéo léo theo từng người -> Nhóm trưởng duyệt và bấm gửi | Khi cần cá nhân hóa lời nhắc nhẹ nhàng, giữ hòa khí nhóm và nhóm trưởng vẫn kiểm soát 100% | Tốn thêm 1-2 phút của nhóm trưởng để duyệt tin nhắn trước khi gửi | **CHỌN** |
| **Agent** | AI tự động quyết định khi nào nhắn, tự nhắn tin riêng giục thành viên, tự động dời deadline hoặc phạt nếu trễ | Khi có hệ thống tích hợp sâu và AI hiểu hết mọi mối quan hệ xã hội | AI bịa chuyện (hallucination), nhắn tin thô lỗ gây mất đoàn kết nội bộ | Không |

**Mức chọn:** **Workflow kết hợp Rule**

**Vì sao không chọn mức đơn giản hơn:**
Nếu chỉ dùng thuần Rule (tin nhắn mẫu cố định), thành viên nhận vài lần sẽ bị nhờn và coi như spam, bấm tắt thông báo nhóm. Cần chút hỗ trợ của AI để biến đổi câu từ nhắc nhở cho tự nhiên, khéo léo theo ngữ cảnh (ví dụ: biết bạn đó đang thi môn khác để nhắc nhẹ nhàng), nhưng vẫn giữ chi phí cực thấp và con người duyệt cuối.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Tạo ra bản nháp tin nhắn nhắc nhở thân thiện, cá nhân hóa theo từng thành viên chưa bấm xác nhận task |
| **Judgment** — con người cân nhắc, quyết định gì? | Nhóm trưởng đọc xem câu từ có phù hợp không, có đúng người đúng việc không, có quá gắt gao hay quá lỏng lẻo không |
| **Action** — hành động cuối cùng là gì, ai làm? | Nhóm trưởng bấm nút gửi tin nhắn nhắc nhở đến thành viên qua kênh Zalo/Discord |
| **Outcome** — đo kết quả bằng gì? | 100% thành viên phản hồi/bấm xác nhận sau khi nhận tin nhắc; thời gian nhóm trưởng phải bận tâm giảm xuống dưới 12 phút/tuần |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Tên thành viên, tên task, deadline, số ngày còn lại đến hạn, trạng thái xác nhận (lấy từ bảng theo dõi của nhóm - có sẵn) |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Tỷ lệ thành viên phản hồi tích cực và bấm xác nhận sau khi nhận tin nhắn nhắc |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
  - Người dùng muốn **được hỗ trợ (augment)**. 
  - Bằng chứng: Cả 2 nhóm trưởng khi được phỏng vấn đều kiên quyết đòi phải được xem qua tin nhắn trước khi gửi. Trong môi trường làm việc nhóm sinh viên, việc giao tiếp rất nhạy cảm; nếu để bot tự động nhảy vào nhắn riêng giục giã sẽ rất dễ gây mất lòng và xung đột cá nhân.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
  - **Báo nhầm tệ hơn rất nhiều**. Nếu thành viên đã làm xong hoặc đã xin phép nộp muộn mà AI vẫn gửi tin nhắn giục hoặc bảo "chưa làm", thành viên sẽ rất ức chế và bực bội với nhóm trưởng.
  - Xử lý: Thiết kế đặt nhóm trưởng làm người duyệt cuối cùng (HITL). Trước khi gửi tin nhắc, nhóm trưởng sẽ liếc mắt kiểm tra xem bạn đó có nhắn riêng xin phép gì trước đó không.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Nhóm trưởng sinh viên phụ trách quản lý tiến độ bài tập lớn/đồ án nhóm (3–5 người) |
| **Quy trình** | Giao việc kèm nút xác nhận -> Rule ghi nhận trạng thái -> AI soạn nháp tin nhắc cho người chưa xác nhận -> Nhóm trưởng duyệt -> Gửi nhắc |
| **Bottleneck** | Khâu nhắn tin riêng giục từng người và giải thích lại yêu cầu |
| **Impact** | Tốn 40-50 phút/tuần của nhóm trưởng; nguy cơ trễ deadline nộp bài chung của cả nhóm |
| **Success Metric** | Thời gian theo dõi giảm từ 45 phút xuống dưới 12 phút/tuần; tỷ lệ xác nhận đạt 100% trong 24h; 0 lần trễ hạn nộp bài |
| **Boundary** | AI chỉ hỗ trợ soạn nháp tin nhắn nhắc việc; tuyệt đối không tự động nhắn tin và không được tự ý sửa đổi deadline |
| **AI intervention point** | Bước soạn thảo nội dung tin nhắn nhắc việc cá nhân hóa cho những bạn chưa bấm xác nhận sau 24h |
| **Mức chọn** | Workflow kết hợp Rule |
| **Rủi ro & người kiểm tra** | Rủi ro: câu từ nhắc nhở chưa khéo léo hoặc nhầm thông tin task. Người kiểm tra: Nhóm trưởng (duyệt trong 1–2 phút trước khi gửi) |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| **Quy trình** | Quy trình chung chung, nhóm trưởng tự đi dò hỏi thủ công | Bổ sung rõ cơ chế Rule bắt trạng thái xác nhận và điểm AI chen chân vào soạn nháp | Giúp quy trình rõ ràng từng khâu tự động hóa và chỗ con người kiểm soát |
| **AI intervention point** | Chưa chỉ rõ cụ thể ở bước nào | Xác định rõ tại bước soạn tin nhắc nhở người chưa bấm nhận việc sau 24h | Đóng khung phạm vi AI cực hẹp, tránh sa đà vào việc xây bot phức tạp |
| **Rủi ro & kiểm tra** | Chưa có trường này | Bổ sung rõ rủi ro câu từ và chỉ định nhóm trưởng là người duyệt cuối | Đảm bảo an toàn giao tiếp theo nguyên lý Human-in-the-loop |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Tính chính xác của thông tin | Nhắc đúng tên người, đúng tên task và đúng hạn nộp cụ thể | Bịa nhầm task của người khác hoặc nói sai ngày nộp |
| 2 | Giọng điệu (Tone & Mood) | Lịch sự, thân thiện, mang tính hỗ trợ và nhắc nhở khéo léo | Cộc lốc, gay gắt, mang tính ra lệnh hoặc quá suồng sã |
| 3 | Độ súc tích | Dưới 3 câu ngắn gọn, có rõ mốc giờ cần phản hồi | Dài dòng quá 5 câu, viết lan man không có lời kêu gọi hành động cụ thể |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** (An toàn) | 100% nhóm trưởng được phỏng vấn đều xác nhận tốn nhiều thời gian và ngán ngẩm việc phải đi nhắn tin giục riêng từng người. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Thấp** (An toàn) | Bản nháp tin nhắn tiếng Việt rất dễ đọc, nhóm trưởng chỉ mất 15-30 giây để đọc lướt và sửa lại nếu cần. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Thấp** (An toàn) | Không cần code phức tạp; chỉ cần kết hợp form/poll có sẵn với một câu prompt chuẩn trên ChatGPT/Claude là làm được ngay. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Thấp** (An toàn) | Chi phí 0 đồng (dùng bản miễn phí), không vi phạm bảo mật dữ liệu nhạy cảm của trường. Nhóm trưởng tự vận hành. |

### 8.2. Kết luận

**Quyết định:** **Go, phạm vi nhỏ (Pilot)**

**Lý do:**
Cả 4 rủi ro đều ở mức Thấp (rất an toàn). Vấn đề có thật, giá trị mang lại rõ ràng (tiết kiệm hơn 30 phút/tuần cho nhóm trưởng), và giải pháp cực kỳ đơn giản, không cần đầu tư công sức lập trình phức tạp.

**Nếu Go — pilot nhỏ nhất:**
Thử nghiệm ngay trong 2 tuần tiếp theo của môn học: Nhóm trưởng tạo 1 poll bình chọn 'Xác nhận deadline' trên nhóm Zalo sau mỗi buổi họp; nếu sau 24h còn bạn chưa vote thì dùng ChatGPT với prompt chuẩn để soạn tin nhắc, nhóm trưởng duyệt rồi gửi.

**Nếu Not Yet — cần kiểm chứng gì trước:** (Không áp dụng)

**Nếu No-Go — nên làm gì thay AI:** (Không áp dụng)

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):
Nếu sau 2 tuần thử nghiệm mà tỷ lệ thành viên tự giác bấm xác nhận vẫn dưới 50% hoặc nhóm trưởng thấy việc duyệt tin nhắn AI còn mất thời gian hơn tự gõ tay, nhóm sẽ dừng lại và quay về dùng bảng Google Sheets thông báo thông thường.

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế:**
  - Dữ liệu phỏng vấn kiểm chứng mới chỉ thực hiện trên phạm vi 3 người (2 nhóm trưởng, 1 thành viên) ở môn học Web và Đồ án; cần mở rộng kiểm chứng thêm ở các môn có tính chất khác (như môn nghiên cứu lý thuyết).
  - Thử nghiệm pilot mới áp dụng trên kênh chat Zalo, chưa tích hợp tự động qua Webhook hay Bot Discord/Slack chuyên nghiệp.

- **Hướng tiếp theo:**
  - Nếu pilot 2 tuần thành công (tỷ lệ bấm nhận task > 80%), nhóm sẽ tích hợp thêm tính năng: tự động bóc tách danh sách việc từ biên bản họp nhóm (nối với đề tài của bạn Hoàng ở CP2).
  - Nghiên cứu xây dựng một Mini App Zalo hoặc Discord Bot nhẹ để thành viên chỉ cần bấm 1 chạm mà không cần mở link ngoài.

## 10. Tài liệu tham khảo

- Alberto Savoia, *The Right It: Why So Many Ideas Fail and How to Make Sure Yours Succeed*, 2019 (Khái niệm Pretotyping & Pilot nhỏ nhất).
- Rob Fitzpatrick, *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*, 2013 (Phương pháp phỏng vấn kiểm chứng hành vi quá khứ).
- Teresa Torres, *Continuous Discovery Habits*, 2021 (Mô hình Opportunity Solution Tree - OST).
- Google PAIR (People + AI Research), *People + AI Guidebook* (Nguyên tắc thiết kế Augment vs. Automate và xử lý False Positive / False Negative).
- Marty Cagan, *Inspired: How to Create Tech Products Customers Love*, 2nd ed., 2017 (Khung đánh giá 4 rủi ro: Value, Usability, Feasibility, Viability).
