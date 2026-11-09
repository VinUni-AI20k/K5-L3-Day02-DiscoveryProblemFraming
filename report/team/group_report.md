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
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

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

**Bài của nhóm nằm ở ô:** Chưa chốt, cần đối chiếu quy trình hiện tại và Problem Statement v0

**Phân tích sơ bộ:**

- Độ mơ hồ thấp nếu dữ liệu đầu vào có cấu trúc, quy tắc xử lý rõ ràng và kết quả có thể kiểm tra bằng điều kiện cố định
- Độ mơ hồ tăng nếu người thực hiện phải đọc tài liệu, hiểu yêu cầu tự nhiên, đối chiếu nhiều nguồn hoặc xử lý trường hợp ngoại lệ
- Độ phức tạp thấp nếu quy trình chỉ có một vài bước độc lập
- Độ phức tạp tăng nếu nhiều actor tham gia, cần bàn giao, phê duyệt và truy xuất thông tin từ nhiều hệ thống

**Nhận định:** Nên xác định chính xác bước nghẽn trong quy trình của Vinh trước khi kết luận bài toán thuộc nhóm Rule, Workflow hay Agent

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** | Chuẩn hóa quy trình, thống nhất biểu mẫu, checklist, trách nhiệm và cách bàn giao giữa các actor | Bottleneck chủ yếu do thiếu quy trình thống nhất hoặc phân công chưa rõ | Vẫn cần con người tổng hợp và kiểm tra thông tin | Phương án nền |
| **Rule** | Sử dụng các điều kiện cố định để kiểm tra dữ liệu, xác định trường hợp thiếu thông tin và cảnh báo sai lệch | Dữ liệu có cấu trúc và có thể xác định kết quả bằng quy tắc rõ ràng | Khó xử lý trường hợp ngoại lệ, thông tin không có cấu trúc | Ưu tiên nếu đủ |
| **Workflow** | Kết hợp các bước xử lý cố định với AI tại công đoạn cần đọc hiểu, trích xuất, phân loại hoặc tổng hợp thông tin | Quy trình có nhiều bước nhưng thứ tự xử lý đã xác định, một số bước cần hiểu ngữ nghĩa | AI có thể trả kết quả sai, cần kiểm tra đầu ra và có phương án dự phòng | Ứng viên chính nếu Rule không đủ |
| **Agent** | Cho phép AI lựa chọn công cụ và các bước xử lý dựa trên trạng thái công việc, trong phạm vi được cấp quyền | Nhiệm vụ có nhiều nhánh khó dự đoán trước, cần lập kế hoạch và xử lý linh hoạt | Khó kiểm soát hành động, chi phí cao, nguy cơ thực hiện sai hoặc vượt quyền | Chưa ưu tiên |

**Mức đề xuất sơ bộ:** Workflow nếu việc kiểm chứng xác nhận tồn tại bước xử lý thông tin không có cấu trúc mà Rule không giải quyết đủ tốt

**Vì sao không chọn mức đơn giản hơn:**

No AI và Rule phù hợp với việc chuẩn hóa, kiểm tra dữ liệu có cấu trúc và gửi cảnh báo, nhưng có thể không xử lý hiệu quả các nội dung cần hiểu ngữ nghĩa hoặc tổng hợp từ nhiều nguồn

**Vì sao chưa chọn Agent:**

Chưa có bằng chứng cho thấy hệ thống cần tự lập kế hoạch, tự lựa chọn chuỗi hành động hoặc thay con người thực hiện nhiều quyết định phức tạp

Với quy trình đã xác định rõ các bước, Workflow thường dễ kiểm soát, đánh giá và triển khai hơn

**Boundary:**

- AI chỉ được xử lý dữ liệu trong phạm vi được cấp quyền
- Không tự thực hiện quyết định có tác động quan trọng khi chưa được con người xác nhận
- Không tự sửa hoặc xóa dữ liệu gốc
- Không tự gửi thông tin ra bên ngoài nếu chưa có phê duyệt
- Những kết quả không đủ căn cứ phải được đánh dấu để người phụ trách kiểm tra
- Mọi thay đổi quan trọng cần được ghi nhận để truy vết
- Khi AI không hoạt động hoặc kết quả không đáng tin cậy, hệ thống quay về quy trình Rule hoặc xử lý thủ công

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction — AI dự đoán / tạo ra gì?** | Trích xuất và phân loại thông tin từ đầu vào, xác định trường hợp có khả năng bất thường hoặc thiếu dữ liệu, tạo bản tóm tắt và đề xuất hướng xử lý kèm căn cứ |
| **Judgment — con người cân nhắc, quyết định gì?** | Xác minh thông tin, đánh giá mức độ ảnh hưởng, quyết định có chấp nhận đề xuất và thực hiện hành động hay không |
| **Action — hành động cuối cùng là gì, ai làm?** | Workflow đưa ra kết quả kiểm tra hoặc danh sách công việc cần xử lý, người được phân quyền xác nhận và thực hiện những hành động quan trọng |
| **Outcome — đo kết quả bằng gì?** | Thời gian xử lý, số thao tác thủ công, tỷ lệ kết quả chính xác, tỷ lệ sai sót và tỷ lệ trường hợp phải chuyển cho người kiểm tra |
| **Input — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không?** | Dữ liệu đầu vào của quy trình, tài liệu hoặc bản ghi liên quan, các quy định nghiệp vụ và trạng thái xử lý, quyền truy cập và mức độ sẵn có cần được kiểm chứng |
| **Feedback — lấy phản hồi ở đâu để cải thiện?** | Kết quả người dùng chấp nhận hoặc từ chối, các trường hợp xử lý sai, dữ liệu kiểm thử có đáp án đối chiếu và phản hồi từ người trực tiếp vận hành |

### 6.4. Hai câu hỏi của Google PAIR

**1. Người dùng muốn được hỗ trợ (augment) hay giao hẳn việc (automate)? Bằng chứng:**

Đề xuất ban đầu là Augment tại những bước có ảnh hưởng đến quyết định nghiệp vụ và Automate những bước lặp lại có kết quả kiểm tra rõ ràng
Những bước thu thập, định dạng, kiểm tra trường bắt buộc hoặc cập nhật trạng thái theo quy tắc có thể tự động hóa
Những bước cần đánh giá ngữ cảnh, xử lý ngoại lệ hoặc phê duyệt kết quả nên giữ sự tham gia của con người
Cần xác minh mong muốn này với actor trực tiếp sử dụng hệ thống, chưa coi đây là kết quả phỏng vấn

**2. AI sai kiểu nào tệ hơn, báo nhầm hay bỏ sót? Vì sao và thiết kế đã xử lý thế nào?**

- **Báo nhầm (False Positive):** Hệ thống cảnh báo có vấn đề trong khi dữ liệu thực tế vẫn hợp lệ, khiến người dùng mất thời gian kiểm tra lại
- **Bỏ sót (False Negative):** Hệ thống không phát hiện được trường hợp thực sự có vấn đề, khiến sai sót tiếp tục đi qua quy trình

Mức độ nghiêm trọng của từng loại lỗi phụ thuộc vào tác động thực tế của bài toán

**Phương án xử lý:**

- Đánh dấu độ tin cậy và nguồn thông tin của kết quả
- Ưu tiên Rule cho các trường dữ liệu có thể xác minh chính xác
- Có cơ chế chuyển trường hợp không chắc chắn cho người phụ trách
- Không cho phép AI tự thực hiện hành động quan trọng
- Xây dựng bộ kiểm thử có cả trường hợp đúng, sai, thiếu thông tin và ngoại lệ
- Theo dõi riêng tỷ lệ báo nhầm và bỏ sót trong quá trình thử nghiệm

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

| Rủi ro | Câu hỏi | Mức độ rủi ro | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Cao | Chưa có Problem Statement được kiểm chứng trong báo cáo nhóm, chưa xác định được tần suất và tác động thực tế của bottleneck |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Có thể thiết kế giao diện kiểm tra và xác nhận kết quả, nhưng chưa có thử nghiệm trực tiếp với actor |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Trung bình đến cao | Các công nghệ Rule, Workflow và LLM có thể triển khai, nhưng chưa xác minh tính sẵn có, chất lượng và quyền truy cập dữ liệu trong quy trình thực tế |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Cao | Chưa xác định được chi phí triển khai, vận hành, cơ chế phân quyền và giá trị tiết kiệm thực tế |
Các mức rủi ro trên là đánh giá sơ bộ theo bằng chứng hiện có, không phải đánh giá đã được nhóm thống nhất

### 8.2. Kết luận

**Quyết định đề xuất:** NOT YET

**Lý do:**
Bài toán có khả năng cải thiện thông qua chuẩn hóa quy trình, Rule, Workflow và AI, tuy nhiên chưa đủ bằng chứng để xác định mức can thiệp phù hợp nhất
Việc lựa chọn Agent ngay từ đầu có thể làm tăng chi phí và rủi ro trong khi chưa chứng minh được lợi ích so với giải pháp đơn giản
Cần ưu tiên xác minh bottleneck và thử nghiệm phương án ít phức tạp nhất trước khi quyết định phát triển

**Nếu Go — pilot nhỏ nhất:**

- Chọn một quy trình cụ thể và một actor chính
- Sử dụng khoảng 20–30 trường hợp thử nghiệm có kết quả đối chiếu
- Xây dựng bản Rule-based làm phương án baseline
- Chỉ bổ sung AI ở bước Rule không giải quyết được
- Cho người phụ trách xác minh những đầu ra quan trọng
- Đo cùng bộ dữ liệu trước và sau khi bổ sung AI

**Nếu Not Yet — cần kiểm chứng gì trước:**

1. Actor chính thực sự đang gặp vấn đề gì và ở bước nào
2. Tần suất xảy ra vấn đề và thời gian bị ảnh hưởng
3. Dữ liệu cần xử lý có sẵn, đáng tin cậy và được phép truy cập hay không
4. Rule hoặc công cụ hiện tại đã giải quyết được bao nhiêu phần
5. Các tình huống AI dự kiến hỗ trợ có thực sự cần hiểu ngữ nghĩa hay không
6. Hiệu quả tiết kiệm thời gian có lớn hơn chi phí xây dựng và vận hành không

**Nếu No-Go — nên làm gì thay AI:**

- Chuẩn hóa quy trình và biểu mẫu
- Thống nhất dữ liệu đầu vào và đầu ra
- Áp dụng checklist và các quy tắc nghiệp vụ
- Tự động hóa những bước có điều kiện xử lý rõ ràng
- Cải thiện cơ chế giao việc, phản hồi và phê duyệt

**Ngưỡng dừng đề xuất:**
Sau giai đoạn thử nghiệm tối thiểu 20–30 tình huống đại diện, cần so sánh trực tiếp với phương án Rule hoặc quy trình hiện có
Dừng việc phát triển AI độc lập và quay về Rule/Workflow không dùng AI nếu xảy ra một trong các trường hợp sau:
- Không xác nhận được bottleneck có tác động đáng kể đến người dùng
- AI không tạo thêm lợi ích đo được so với phương án Rule
- Mức giảm thời gian thao tác thấp hơn 20% trong điều kiện thử nghiệm tương đương, trong khi chi phí và độ phức tạp tăng đáng kể
- Xuất hiện lỗi nghiêm trọng trong đầu ra mà không có cơ chế phát hiện và kiểm soát
- Không đảm bảo được quyền truy cập, bảo mật dữ liệu hoặc khả năng vận hành lâu dài

**Kết luận sơ bộ:**

Ưu tiên phương án có mức độ phức tạp thấp nhất nhưng giải quyết được bottleneck thực tế
Chỉ triển khai AI nếu có bằng chứng cho thấy AI tạo giá trị bổ sung so với việc chuẩn hóa quy trình và sử dụng Rule-based Automation
Quyết định cuối cùng cần được điều chỉnh theo Problem Statement, workflow và kết quả kiểm chứng thực tế của nhóm
---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
