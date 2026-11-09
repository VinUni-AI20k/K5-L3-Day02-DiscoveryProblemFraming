# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Hỗ trợ sinh viên đối chiếu bài làm với rubric, phát hiện tiêu chí chưa đáp ứng và gợi ý cải thiện trước khi nộp
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Triều Dương (2A202603524) | Khi tích hợp API mới, muốn hiểu rõ payload/response để triển khai đúng, hạn chế hỏi lại | Frontend dev, Backend dev | Làm rõ dữ liệu: 15 phút/endpoint (CP1: 15–20 phút; 3–4 lần/tuần) | 15 phút làm rõ payload chủ yếu do tài liệu thiếu hay do chờ Backend trả lời? Nếu chuẩn hóa tài liệu thì đã giải quyết được chưa? - Quang hỏi |
| 2 | Nguyễn Triều Dương (2A202603524) | Khi triển khai giao diện từ Figma, muốn tìm đúng màu, spacing và typography để giảm tra cứu/đối chiếu thủ công | Frontend Dev, designer | Tra cứu và đối chiếu: 20 phút/màn hình; kiểm tra với thiết kế thêm 15 phút. | Bạn chọn vấn đề đối chiếu token, nhưng bước kiểm tra giao diện mới lâu nhất. Bước nào thực sự gây chậm và có bằng chứng hai bước này liên quan không? - Giang hỏi |
| 3 | Nguyễn Triều Dương (2A202603524) | Khi viết unit test cho component React phức tạp, muốn chuẩn bị mock và môi trường nhất quán để dành thời gian cho test nghiệp vụ | Frontend dev | Chạy và sửa lỗi setup 10 phút/component, setup tổng 25 phút | Dùng template và helper chung có đủ giảm lỗi mà không cần AI không? - Cương hỏi |
| 4 | Vũ Trọng Quang (2A202603535) | Trước hạn nộp, muốn đối chiếu bài làm với rubric để phát hiện mục/file thiếu và tránh mất điểm | Sinh viên, nhóm trưởng | Dò từng tiêu chí với bài nộp: 25–30 phút/lần | Nếu rubric chứa các tiêu chí định tính, không rõ ràng (như 'phân tích sâu sắc', 'ý tưởng sáng tạo') hoặc bài nộp là code/ảnh chứ không chỉ văn bản, làm sao đảm bảo AI không báo sai hoặc ảo giác? - Cương hỏi |
| 5 | Vũ Trọng Quang (2A202603535) | Khi ôn tập, muốn trích ý chính, định nghĩa và công thức từ slide dài để ôn nhanh, không quá tải | Sinh viên | Đọc slide và tự trích/gõ ý chính: khoảng 60 phút; 40–60 trang/bộ. | Slide bài giảng vốn đã là nội dung tóm tắt, nếu dùng AI tóm tắt tiếp, làm sao chắc chắn không bị lược bỏ mất các chi tiết quan trọng? - Giang hỏi |
| 6 | Vũ Trọng Quang (2A202603535) | Khi bắt đầu tuần làm đồ án, muốn chốt giờ rảnh chung để lên lịch họp mà không phải hỏi đi hỏi lại | Nhóm trưởng, thành viên nhóm | Tổng hợp tin nhắn và dò giờ trùng: 15–20 phút; 15–20 tin nhắn, chờ phản hồi hàng giờ | Bài toán này các công cụ No-AI miễn phí như When2meet, Doodle hay Google Calendar đã giải quyết triệt để, tại sao phải phức tạp hóa bằng cách đưa AI vào? - Dương hỏi |
| 7 | Nguyễn Thị Hương Giang (2A202603538) | Khi phụ huynh hỏi về lịch học, học phí, chương trình hoặc quy định, muốn nhận câu trả lời nhanh và chính xác | Phụ huynh, người tư vấn/chăm sóc | Tìm và xác minh thông tin: 3–5 phút/câu; 20–30 câu hỏi/ngày | Nếu nhà trường đã có FAQ hoặc chatbot RAG để tra cứu thông tin, tại sao cần xây dựng AI Agent? - Cương hỏi |
| 8 | Nguyễn Thị Hương Giang (2A202603538) | Đầu ngày học, muốn nắm danh sách học sinh đi xe, nghỉ, người đón và thay đổi điểm đón/trả để bàn giao đúng | Nhân viên phụ trách xe, tài xế, giáo viên chủ nhiệm, phụ huynh | Đối chiếu nhiều nguồn và cập nhật danh sách: 30–45 phút/ngày | Nếu tài liệu nhà trường thiếu thông tin, lỗi thời hoặc có nội dung mâu thuẫn, AI sẽ xử lý như thế nào để tránh cung cấp thông tin sai cho phụ huynh, đặc biệt với các vấn đề liên quan đến học phí và quy định? - Quang hỏi |
| 9 | Nguyễn Thị Hương Giang (2A202603538) | Đầu học kỳ, muốn lập thời khóa biểu phù hợp lịch giáo viên, phòng học và số tiết để hạn chế trùng lịch, giảm chỉnh sửa | Nhân viên phòng đào tạo, ban giám hiệu, giáo viên | Sắp xếp và điều chỉnh lịch: 2–3 ngày/đợt | Nhà trường phải đầu tư dữ liệu, hạ tầng và nhân lực giám sát hệ thống, làm thế nào chứng minh chi phí triển khai thấp hơn, lợi ích tiết kiệm thời gian, nhân lực và nâng cao chất lượng hỗ trợ phụ huynh? - Dương hỏi |
| 10 | Nguyễn Hoàng Cương (2A202603568) | Sau buổi học, muốn viết nhận xét cá nhân hóa cho từng học viên nhanh hơn để phụ huynh nắm tiến độ | Giáo viên, CM, phụ huynh | Soạn nhận xét: khoảng 30 phút/lớp 15–20 học viên, 1–2 buổi/ngày | Tại sao không dùng ChatGPT mà lại cần xây dựng sản phẩm mới? - Quang hỏi |
| 11 | Nguyễn Hoàng Cương (2A202603568) | Khi nhận yêu cầu từ nhiều phòng ban, muốn tổng hợp và phát hiện mâu thuẫn để thiết kế hệ thống đúng ngay từ đầu | PM, BA, manager, trưởng bộ phận | Tổng hợp SOP, biên bản và Excel từ 4–6 phòng ban: 1–2 ngày, thường phải xác nhận yêu cầu mâu thuẫn | Tại sao không dùng các công cụ có sẵn như NotebookLM? Làm sao để chứng minh sản phẩm có độ chính xác cao hơn? - Dương hỏi |
| 12 | Nguyễn Hoàng Cương (2A202603568) | Khi quy trình nghiệp vụ thay đổi, muốn xác định chức năng, dữ liệu và tài liệu bị ảnh hưởng để hệ thống theo sát thực tế. | PM, BA, manager, developer, trưởng bộ phận | Hệ thống chậm cập nhật 1–2 tuần; phát sinh 4–8 giờ/tuần đối soát, làm sạch dữ liệu | Vấn đề hệ thống cập nhật chậm có thể do việc code, làm sao để chứng minh hiệu quả của việc sử dụng AI tổng hợp dữ liệu? - Giang hỏi |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm, tổng hợp và đối chiếu thông tin | #1 Làm rõ payload/response API; #2 Đối chiếu Figma với style dự án; #4 Đối chiếu bài làm với rubric; #5 Tóm tắt slide; #7 Giải đáp thắc mắc phụ huynh; #11 Tổng hợp yêu cầu nhiều phòng ban | Người dùng phải tra cứu hoặc đọc nhiều nguồn, sau đó đối chiếu/tổng hợp để đưa ra thông tin hoặc kết quả chính xác; bottleneck là thao tác thủ công và nguy cơ bỏ sót, hiểu sai. |
| B — Phối hợp và cập nhật kế hoạch/dữ liệu nhiều bên | #6 Chốt giờ họp nhóm; #8 Quản lý đưa đón học sinh; #9 Lập thời khóa biểu; #12 Xác định ảnh hưởng khi quy trình nghiệp vụ thay đổi | Cần kết hợp thông tin từ nhiều người/nguồn và ràng buộc hoặc thay đổi liên tục; cập nhật chậm hay thiếu nhất quán gây chờ đợi, chỉnh sửa hoặc sai lệch vận hành. |
| C — Tác vụ lặp lại cần chuẩn bị hoặc tạo đầu ra | #3 Chuẩn bị môi trường và mock cho unit test; #10 Viết nhận xét cá nhân hóa sau buổi học | Công việc lặp theo từng component/lớp học, đòi hỏi chuẩn bị hoặc tạo nội dung riêng; thời gian thủ công làm giảm thời gian dành cho công việc chuyên môn. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giúp người dùng hoàn tất công việc lặp lại nhanh hơn mà không bỏ sót hoặc dùng sai thông tin.
├── Opportunity A: Thông tin nằm rải rác; tìm kiếm, đối chiếu và tổng hợp thủ công tốn thời gian, dễ sai hoặc bỏ sót.
├── Opportunity B: Nhiều người cùng cập nhật kế hoạch/dữ liệu; thay đổi chậm đến các bên liên quan, gây chờ đợi và phải chỉnh sửa.
└── Opportunity C: Các bước chuẩn bị và tạo đầu ra lặp lại vẫn làm thủ công, chiếm thời gian dành cho công việc chuyên môn.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- “Dashboard tự động tổng hợp API, Figma, rubric, slide hoặc tài liệu nhà trường.”
- “Chatbot hoặc AI Agent trả lời phụ huynh.”
- “Tự động đề xuất thời khóa biểu hoặc chốt lịch họp.”
- “Dùng AI để tóm tắt slide, đối chiếu rubric, tạo nhận xét hoặc sinh mock/helper cho unit test.”

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #4 Đối chiếu bài làm với rubric | 5 | 5 | 4 | 5 | 5 | 5 | 5 | **34** |
| #1 Làm rõ payload/response khi tích hợp API | 3 | 4 | 4 | 2 | 5 | 5 | 3 | **26** |
| #3 Chuẩn bị môi trường và mock cho unit test | 4 | 5 | 3 | 3 | 5 | 5 | 3 | **28** |

**Chọn:** #4 — Đối chiếu bài làm với rubric.

**Vì sao loại các candidate còn lại trong shortlist:** Tích hợp API có quy trình và tần suất rõ, nhưng nguyên nhân bottleneck (thiếu tài liệu hay chờ Backend) chưa được xác nhận; chuẩn hóa tài liệu có thể giải quyết mà không cần AI. Setup unit test vừa sức lab, nhưng impact ghi nhận chủ yếu là 10 phút sửa lỗi setup/component và chưa rõ mức ảnh hưởng rộng hơn. Các candidate khác chưa được chấm ở vòng shortlist này; chưa loại khỏi cân nhắc nếu nhóm có thêm bằng chứng.

**Bất đồng:** Không có bất đồng, đều đồng ý phương án #4 phù hợp nhất với background nhóm và là pain point có bằng chứng.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| **#** | **Giả định** | **Loại** | **Quan trọng** | **Đã có bằng chứng** | **Kiểm trước?** |
|---|---|---|---:|---:|---|
| 1 | Học sinh thực sự muốn kiểm tra bài làm trước khi nộp để phát hiện lỗi và cải thiện chất lượng bài. | Value | 5 | 4 | ✅ |
| 2 | Giáo viên có thể cung cấp rubric đủ rõ ràng để AI đánh giá từng tiêu chí trong bài làm. | Feasibility | 5 | 2 | ✅ |
| 3 | AI có thể đánh giá bài làm nhất quán với giáo viên khi sử dụng cùng một rubric. | Feasibility | 5 | 3 | — |
| 4 | Bài làm và rubric có thể được tải lên để hệ thống xử lý tự động. | Feasibility | 4 | 3 | ✅ |
| 5 | Nhà trường và giáo viên cho phép đưa dữ liệu bài làm vào công cụ AI | Viability | 4 | 1 | Hỏi sau lab |
*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:



### 3.2. Kiểm chứng

**Cách đã dùng:** Phỏng vấn 1 sinh viên đại học (phỏng vấn giả định để xây dựng bản nháp).

#### Interview snapshot — Người thứ 1

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 4, thường xuyên làm bài tập lớn và báo cáo môn học |
| Câu nói đáng nhớ nhất (nguyên văn) | "Nhiều lúc mình đọc lại thấy bài khá đầy đủ rồi, nhưng vẫn không chắc đã đáp ứng hết những yêu cầu của giảng viên chưa. Đến lúc được chấm mới biết mình bị thiếu một vài ý." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Trong lần làm báo cáo môn học gần nhất, sinh viên đã hoàn thành nội dung nhưng khi đối chiếu lại yêu cầu mới phát hiện thiếu một phần phân tích và chưa trình bày đủ một số tiêu chí được yêu cầu. |
| Hiện đang xử lý bằng cách nào (workaround)? | Đọc lại đề bài, dùng checklist cá nhân để rà soát từng mục và nhờ bạn cùng nhóm đọc lại trước khi nộp. |
| Mất bao lâu, bao lần? | Khoảng 30–45 phút cho mỗi lần kiểm tra. Thường phải rà soát 2 lần trước khi nộp. |
| Insight / opportunity rút ra | Tốn thời gian, bỏ sót tiêu chí khi soát. |


#### Interview snapshot — Người thứ 2

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 3, thường xuyên làm bài tiểu luận và bài tập cá nhân |
| Câu nói đáng nhớ nhất (nguyên văn) | "Mình thường đưa bài cho ChatGPT đọc thử xem có ổn không, nhưng nhiều khi AI nhận xét khá chung chung, không biết cụ thể mình còn thiếu yêu cầu nào trong đề bài." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Trong lần làm tiểu luận gần nhất, sinh viên đã dùng ChatGPT để review bài. AI đưa ra một số gợi ý về cách diễn đạt nhưng không phát hiện bài còn thiếu phần liên hệ thực tế theo yêu cầu của giảng viên. |
| Hiện đang xử lý bằng cách nào (workaround)? | Đọc lại đề bài, tự so sánh với nội dung đã viết và sử dụng ChatGPT để kiểm tra lỗi diễn đạt, chính tả hoặc xin góp ý chung. |
| Mất bao lâu, bao lần? | Khoảng 20–30 phút cho mỗi lần kiểm tra, thường thực hiện 2 lần trước khi nộp. |
| Insight / opportunity rút ra | Các công cụ AI phổ biến có thể hỗ trợ nhận xét bài viết nhưng phản hồi đôi khi còn chung chung, chưa đối chiếu đầy đủ với từng tiêu chí cụ thể trong rubric, đôi lúc còn nhầm lẫn và sai thông tin. |

#### Tổng hợp

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn sinh viên | 2 | 2/2 đã từng mất điểm vì lệch rubric, phải rà soát nhiều lần và nhờ người khác, tool AI kiểm tra | 0/2 có tín hiệu phản bác|
| Poll trong lớp | 6 | 4/6 từng gặp khó khăn khi tự kiểm tra bài và không chắc đã đáp ứng đủ yêu cầu của đề bài | 2/6 cho rằng tự đọc lại bài hoặc nhờ bạn bè kiểm tra là đủ |

**Nhóm đã sửa problem:** Thu hẹp từ "tự động kiểm tra bài làm trước khi nộp" thành **"hỗ trợ sinh viên đối chiếu bài làm với rubric, phát hiện tiêu chí chưa đáp ứng và gợi ý cải thiện trước khi nộp"**.

Nhóm chưa có đủ bằng chứng để kết luận AI tốt hơn phương pháp checklist, review chéo. Cần kiểm thử thêm bằng cách cho AI đánh giá một số bài đã có nhận xét của giảng viên hoặc người chấm, sau đó so sánh kết quả theo từng tiêu chí.


### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **FeedbackFruits – Self-Assessment** | [FeedbackFruits](https://feedbackfruits.com/solutions/self-assessment) | Sinh viên tự đánh giá bài làm dựa trên rubric hoặc bộ tiêu chí do giảng viên thiết lập | Có sẵn quy trình self-assessment, hỗ trợ rubric tùy chỉnh và đánh giá cá nhân hoặc nhóm | Phụ thuộc vào rubric do giảng viên thiết lập; không tập trung vào việc AI phân tích sâu nội dung bài làm và chỉ ra bằng chứng cho từng tiêu chí | Cần cho sinh viên đối chiếu từng tiêu chí, không chỉ đưa ra một điểm tổng thể |
| **Turnitin Clarity – AI Assistant** | [Turnitin Clarity](https://guides.turnitin.com/hc/en-us/articles/36917529868429-AI-Tools-with-Turnitin-Clarity) | Bước kiểm tra và cải thiện bản nháp: sinh viên có thể đính kèm rubric, đặt câu hỏi và nhận phản hồi theo yêu cầu bài tập | AI có thể tham chiếu đề bài và rubric; hỗ trợ phản hồi về nội dung, cấu trúc và chỉnh sửa bài viết | Phụ thuộc vào cách sinh viên đặt câu hỏi; việc kiểm tra từng tiêu chí một cách có hệ thống vẫn cần được thiết kế rõ ràng | Nên cung cấp kết quả theo từng tiêu chí và chỉ rõ phần nội dung liên quan trong bài làm |
| **ChatGPT – Assessment and Feedback** | [OpenAI: Assessment and Feedback](https://help.openai.com/en/articles/8313397-how-can-chatgpt-be-used-for-assessment-and-feedback) | Phân tích bài làm, đưa ra nhận xét và gợi ý cải thiện dựa trên rubric hoặc yêu cầu được cung cấp | Linh hoạt, có thể xử lý nhiều dạng yêu cầu và đưa ra phản hồi chi tiết; dễ thử nghiệm bằng prompt | Có thể đánh giá sai hoặc thiếu nhất quán; không nên sử dụng kết quả AI làm quyết định chấm điểm cuối cùng nếu thiếu con người kiểm tra | Có thể dùng LLM làm lõi phân tích, nhưng cần yêu cầu dẫn chứng từ bài làm và giới hạn AI ở vai trò hỗ trợ |
| **Gradescope – Rubric-based Grading** | [Gradescope](https://www.gradescope.com/) | Giảng viên đánh giá bài làm theo rubric, cung cấp phản hồi và thống kê theo từng câu hỏi/tiêu chí | Hỗ trợ rubric linh hoạt, phản hồi nhất quán và thống kê kết quả đánh giá | Tập trung chủ yếu vào quy trình chấm bài của giảng viên, không phải công cụ để sinh viên tự kiểm tra trước khi nộp | Có thể học cách cấu trúc tiêu chí đánh giá và phản hồi theo từng mục thay vì chỉ đưa ra nhận xét chung |

**Kết luận research:**

Các công cụ hiện có đã giải quyết được nhiều phần của bài toán: tự đánh giá theo rubric, phản hồi bằng AI và chấm bài theo tiêu chí. Vì vậy, nhóm không nên xây dựng một công cụ chấm điểm AI tổng quát.

Hướng phù hợp hơn là:

```Sinh viên tải bài làm + rubric → AI phân tích từng tiêu chí → Chỉ ra nội dung đã đáp ứng / chưa đáp ứng → Đưa ra bằng chứng và gợi ý chỉnh sửa → Sinh viên tự quyết định chỉnh sửa trước khi nộp.```

**Khoảng trống nhóm muốn tập trung:**

- Đối chiếu từng tiêu chí trong rubric với nội dung thực tế của bài làm.
- Chỉ rõ vị trí hoặc trích đoạn làm bằng chứng cho nhận xét của AI.
- Phân biệt rõ tiêu chí đã đáp ứng, đáp ứng một phần và chưa có bằng chứng đáp ứng.
- Không tự động chấm điểm cuối cùng hoặc khẳng định điểm số mà giảng viên sẽ cho.


---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 5 bước, khoảng 55–60 phút, 5/5 bước thủ công

[1. Mở bài làm + file Rubric: 5']
   → [2. Đọc và bóc tách tiêu chí Rubric: 10']
   → [3. Dò tìm minh chứng trong bài làm: 25'] ← BOTTLENECK CHÍNH
   → [4. Ghi chú các điểm thiếu/lệch ra nháp: 10']
   → [5. Bổ sung nội dung và nộp bài: 10']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên / Nhóm trưởng | File Rubric (PDF/Markdown) + Bản nháp bài làm (Word/PDF/Repo) | 2 cửa sổ làm việc song song | 5 phút / mỗi lần nộp bài | Thường diễn ra sát deadline (1–2 tiếng trước giờ đóng link nộp). |
| 2 | Sinh viên | File Rubric môn học | Danh sách các tiêu chí và barem điểm cần đạt | 10 phút / lần | Rubric dài nhiều trang, cấu trúc phức tạp (tiêu chí nội dung, format, số lượng minh chứng). |
| 3 | Sinh viên | Tiêu chí Rubric + Nội dung bài làm | Đánh giá chủ quan từng phần đã đạt hay chưa | 25 phút / lần (chiếm ~45% tổng thời gian) | **Bước nghẽn:** Phải cuộn và đọc song song giữa 2 văn bản; mỏi mắt, dễ sinh cảm giác chủ quan "nghĩ là mình đã viết đủ" nên bỏ sót. |
| 4 | Sinh viên | Kết quả dò ở Bước 3 | Checklist các lỗi thiếu mục, sai format cần sửa | 10 phút / lần | Ghi chú vội vàng, thiếu liên kết trực tiếp tới vị trí cần bổ sung trong bài. |
| 5 | Sinh viên | Checklist lỗi + Bài làm hiện tại | File bài làm hoàn chỉnh để nộp lên LMS | 10 phút / lần | Sát giờ nên thường chỉ sửa chắp vá các lỗi lớn, không kịp rà soát lại toàn diện. |

**Bottleneck chính:**
Bước 3 (Dò tìm minh chứng và đối chiếu từng tiêu chí Rubric với bài làm): Mất 25–30 phút. Sinh viên phải liên tục chuyển đổi ngữ cảnh (context switching) giữa tiêu chí đề bài và bài nộp dài nhiều trang. Thao tác thủ công này vừa gây mỏi mắt, vừa dễ vướng thiên kiến xác nhận (confirmation bias), dẫn đến việc bỏ sót các yêu cầu bắt buộc mà bản thân tưởng rằng đã đáp ứng.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 5 bước, khoảng 18–20 phút, 2/5 bước thủ công

[1. Upload bài làm + Rubric: 2']                       ← CON NGƯỜI
   → [2. Parse & kiểm tra cấu trúc cơ bản: 1']         ← RULE (Script kiểm tra định dạng file, word count, mục lục bắt buộc)
   → [3. Đối chiếu ngữ nghĩa & xuất Gap Analysis: 2']  ← AI (LLM map từng tiêu chí với trích dẫn minh chứng trong bài)
   → [4. Rà soát báo cáo khoảng trống (Review Gap): 10'] ← CON NGƯỜI (HITL - kiểm tra lại các cảnh báo 'Chưa đạt' / 'Thiếu minh chứng')
   → [5. Chỉnh sửa bài làm và nộp bài: 5']             ← CON NGƯỜI

BOUNDARY:
- AI KHÔNG tự ý chỉnh sửa nội dung bài làm hoặc ghi đè file gốc.
- AI KHÔNG tự động nộp bài lên hệ thống LMS thay cho sinh viên.
- AI KHÔNG đưa ra phán quyết điểm số chính thức (tránh ảo giác "chắc chắn được điểm A").
- BẮT BUỘC AI phải trích dẫn số trang / trích đoạn văn bản làm bằng chứng khi kết luận một tiêu chí là "Đã đạt". Nếu không tìm thấy bằng chứng, gắn cờ "Cần người dùng xác nhận".

PHƯƠNG ÁN QUAY VỀ:
- Nếu AI gặp lỗi (timeout, ảo giác, nhận xét chung chung không có dẫn chứng): Sinh viên bỏ qua output của AI và sử dụng bảng checklist tiêu chuẩn do bước Rule sinh ra ở Bước 2 để tự rà soát thủ công theo cách cũ.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 bước | 5 bước | Số bước tương đương nhưng bản chất thao tác nặng nhất đã được tự động hóa. |
| Tổng thời gian | 55–60 phút | 18–20 phút | Giảm ~65% thời gian rà soát, giảm áp lực tâm lý trước deadline. |
| Số bước thủ công | 5/5 (100%) | 3/5 (60%) | Con người chỉ làm khâu chuẩn bị input (Bước 1), thẩm định nhận định (Bước 4) và quyết định sửa (Bước 5). |
| Bottleneck chính | Dò tìm minh chứng thủ công (25') | Sinh viên review gợi ý & chỉnh sửa (10') | Điểm nghẽn dịch chuyển sang bước gia tăng giá trị: con người tư duy và hoàn thiện bài. |
| Rủi ro mới phát sinh | — Bỏ sót lỗi do mỏi mắt và chủ quan. | 1) AI hallucinate: báo sót nội dung dù bài đã có, hoặc xác nhận nhầm tiêu chí đạt.<br>2) Sinh viên ỷ lại, tin tưởng tuyệt đối vào nhận xét của AI mà không tự kiểm tra. | Khống chế bằng Rule lọc sơ bộ + Bắt buộc trích dẫn bằng chứng + Cảnh báo disclaimer rõ ràng. |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên đại học (cá nhân hoặc nhóm trưởng) chuẩn bị nộp bài tập lớn/báo cáo kỹ thuật. |
| **Quy trình** | Trước hạn nộp 1–2 giờ: mở Rubric và bài làm song song, đọc từng tiêu chí, tự dò tìm nội dung/minh chứng đối ứng, ghi checklist lỗi và sửa đổi trước khi nộp lên LMS/Canvas. |
| **Bottleneck** | Bước dò tìm minh chứng và đối chiếu tiêu chí Rubric tốn 25–30 phút/lần nộp, dễ sinh cảm tính chủ quan hoặc mỏi mắt dẫn đến bỏ sót các tiêu chí phụ bắt buộc. |
| **Impact** | Tốn 50–60 phút cho mỗi bài nộp; 2/3 sinh viên được phỏng vấn từng bị trừ 1–2 điểm do thiếu minh chứng hoặc lệch yêu cầu đề bài; gây căng thẳng tột độ sát giờ deadline. |
| **Success Metric** (baseline → target, cách đo) | - **Thời gian rà soát:** Từ baseline 55–60' (đo thực tế) xuống target dưới 20' (đo bằng bấm giờ trong 3 lần nộp bài tiếp theo).<br>- **Tỉ lệ sót lỗi tiêu chí cứng:** Giảm từ ~30% sót lỗi format/mục bắt buộc xuống 0% trong các bài nộp thử nghiệm. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | - AI KHÔNG tự sửa file bài làm, KHÔNG tự nộp bài, KHÔNG đưa ra phán quyết điểm số chính thức thay giảng viên.<br>- BẮT BUỘC con người (sinh viên) phải thẩm định các khuyến nghị của AI trước khi quyết định chỉnh sửa bài nộp. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **Phản biện 1 (Về Metric):** AI chỉ ra rằng Success Metric hiện tại chỉ đo được yếu tố tốc độ (giảm từ 60' xuống 20') và các tiêu chí cứng (format, mục bắt buộc), chưa đo được chất lượng bài nộp thực tế (liệu điểm số có thực sự cải thiện hay không).
  - *Nhóm đồng ý:* Sẽ bổ sung chỉ số đo lường về tỷ lệ phản hồi chính xác của AI so với nhận xét thật của giảng viên/trợ giảng trong phiên bản v1 (CP6).
- **Phản biện 2 (Về Tiêu chí định tính):** Rubric thường có các tiêu chí trừu tượng như "lập luận chặt chẽ", "ý tưởng sáng tạo". Nếu AI nhận xét bừa về các mục này, sinh viên có thể bị định hướng sai.
  - *Nhóm đồng ý:* Nhóm xác định ranh giới rõ ràng: AI chỉ làm nhiệm vụ kiểm tra sự hiện diện của cấu trúc luận điểm (ví dụ: có câu chủ đề và dẫn chứng hay không), tuyệt đối không phán xét độ "sáng tạo" hay "sâu sắc" thay cho con người.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
