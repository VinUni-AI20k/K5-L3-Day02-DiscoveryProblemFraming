# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
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

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

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
