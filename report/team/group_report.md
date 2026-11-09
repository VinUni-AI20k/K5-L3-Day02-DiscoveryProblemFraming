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
**Bài toán:** Kiểm tra chênh lệch khối lượng, đơn giá và các thông tin bất thường trong hồ sơ chào giá gói thầu cơ điện

**Bối cảnh:**

Một gói thầu có khoảng 4.100 dòng BOQ, 4 nhà thầu tham gia chào giá, tương đương khoảng 16.000 dòng cần đối chiếu mỗi vòng
Theo dữ liệu từ Problem Card cá nhân, quá trình kiểm tra mất khoảng 5–6 giờ/vòng và một gói thầu có thể trải qua 2 vòng chào giá

**Đánh giá các công đoạn:**

| Công đoạn | Độ mơ hồ | Độ phức tạp | Nhận định |
|---|---|---|---|
| So khối lượng chào với BOQ | Thấp | Cao về khối lượng dữ liệu | Có thể sử dụng công thức và Rule |
| Phát hiện đơn giá chênh lệch | Trung bình | Trung bình | Rule phát hiện, con người đánh giá nguyên nhân |
| Gom file đúng mẫu | Thấp | Trung bình | Power Query, Macro |
| Ghép file sai mẫu | Cao | Cao | Workflow kết hợp AI hỗ trợ đối chiếu ngữ nghĩa |
| Đánh giá hồ sơ năng lực | Cao | Cao | AI trích xuất bằng chứng, chuyên viên quyết định |

**Vị trí của bài toán chính:** Độ mơ hồ thấp, độ phức tạp xử lý dữ liệu cao

Khó khăn chính không nằm ở việc cần AI suy luận mà nằm ở số lượng dòng phải kiểm tra lớn, thao tác thủ công lặp lại và nguy cơ bỏ sót các chênh lệch

### 6.2. So sánh bốn mức can thiệp

| Mức | Phương án | Khả năng giải quyết | Hạn chế | Lựa chọn |
|---|---|---|---|---|
| No AI | Tiếp tục sử dụng Excel và kiểm tra thủ công | Không cần thay đổi quy trình | Mất 5–6 giờ/vòng, có nguy cơ bỏ sót | Không ưu tiên |
| Rule | Sử dụng Excel Formula, Conditional Formatting, Power Query để phát hiện chênh lệch | Có thể kiểm tra toàn bộ dòng đã khớp mã, tự động tính chênh khối lượng và đơn giá | Cần dữ liệu được ghép đúng, chưa tự hiểu file sai mẫu | **Ưu tiên cho bài toán chính** |
| Workflow | Kết hợp bước nhập dữ liệu, kiểm tra, tổng hợp và xuất báo cáo, bổ sung AI khi cần xử lý dữ liệu phi cấu trúc | Giảm thao tác giữa các bước, hỗ trợ xử lý nhà thầu chào sai mẫu | Phụ thuộc dữ liệu đầu vào và khả năng đối chiếu | Cân nhắc cho bài toán mở rộng |
| Agent | Hệ thống tự lựa chọn công cụ, phân tích hồ sơ và thực hiện nhiều bước | Linh hoạt với tác vụ có nhiều ngoại lệ | Chi phí cao, khó kiểm soát, nguy cơ kết luận sai | Chưa cần thiết |

**Mức lựa chọn đề xuất: Rule-based Automation**

**Lý do:**

- Chênh lệch khối lượng có thể xác định chính xác bằng phép tính
- Chênh lệch đơn giá có thể phát hiện bằng công thức và ngưỡng cảnh báo
- Không cần sử dụng LLM để xử lý dữ liệu số đã có cấu trúc
- Dễ kiểm thử, giải thích kết quả và đối chiếu với file gốc
- Giảm chi phí và rủi ro so với phương án dùng Agent

**Trường hợp có thể sử dụng AI:**

Khi nhà thầu gửi bảng chào giá không theo mẫu, mô tả hạng mục khác cách diễn đạt trong BOQ, AI có thể đề xuất ghép các dòng tương ứng theo ý nghĩa
Đây là công đoạn thuộc Problem Card #2, không phải bước so sánh số liệu của Problem Card #1

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** | Với file sai mẫu, AI đề xuất mã BOQ hoặc hạng mục tương ứng cho từng dòng chào giá dựa trên nội dung mô tả |
| **Judgment** | Chuyên viên KTKT kiểm tra mã dòng, quy cách, đơn vị tính, khối lượng và sự phù hợp của đề xuất |
| **Action** | Hệ thống tạo bảng đối chiếu và danh sách dòng bất thường, chuyên viên xác nhận trước khi sử dụng |
| **Outcome** | Giảm thời gian kiểm tra và ghép bảng, không bỏ sót dòng chênh khối lượng, tổng tiền khớp file gốc |
| **Input** | BOQ gốc, bảng chào giá của nhà thầu, mã hạng mục, mô tả, đơn vị tính, khối lượng và đơn giá |
| **Feedback** | Các dòng được chuyên viên chấp nhận, chỉnh sửa hoặc từ chối, kết quả soát lại trên gói thầu đã có đáp án |

**Điểm can thiệp chính:**

- Rule phát hiện chênh lệch số liệu
- AI hỗ trợ đối chiếu mô tả hạng mục không đồng nhất
- Chuyên viên KTKT kiểm tra và xác nhận kết quả
- Lãnh đạo tiếp tục chịu trách nhiệm phê duyệt theo quy trình

**Boundary:**

- Không tự động kết luận nhà thầu đạt hoặc không đạt
- Không tự động lựa chọn nhà thầu trúng thầu
- Không thay đổi file chào giá gốc
- Không tự sửa khối lượng hoặc đơn giá do nhà thầu cung cấp
- Không tự ghép các dòng thiếu căn cứ đối chiếu
- Không sử dụng dữ liệu hồ sơ ngoài phạm vi được cấp quyền
- Các trường hợp thiếu mã, trùng mã hoặc không khớp tổng tiền phải được chuyển cho chuyên viên kiểm tra
- Khi hệ thống không thể xác định kết quả đáng tin cậy, quay về quy trình kiểm tra thủ công

### 6.4. Hai câu hỏi Google PAIR

**1. Người dùng muốn được hỗ trợ hay giao hẳn việc cho hệ thống?**

Đề xuất kết hợp cả hai cách tùy theo công đoạn
Đối với việc so sánh khối lượng, đơn giá và tổng tiền theo các công thức đã xác định, có thể tự động hóa hoàn toàn bước tính toán
Đối với việc ghép file sai mẫu, nhận diện hạng mục tương đương và đánh giá nguyên nhân chênh lệch, hệ thống chỉ đưa ra gợi ý và bằng chứng để chuyên viên xác minh
Cách tiếp cận này giúp giảm thao tác lặp lại nhưng vẫn giữ trách nhiệm chuyên môn và quyết định ở con người
Đây là đề xuất thiết kế, cần được xác nhận với người trực tiếp xử lý hồ sơ

**2. AI sai kiểu nào tệ hơn, báo nhầm hay bỏ sót?**
Đối với bài toán này, bỏ sót một chênh lệch quan trọng có thể gây hậu quả lớn hơn vì ảnh hưởng đến việc so sánh giá trị chào thầu

- False Positive: Cảnh báo dòng bất thường nhưng thực tế có lý do hợp lệ, khiến chuyên viên phải kiểm tra thêm
- False Negative: Không phát hiện dòng chênh lệch thực sự, khiến thông tin bất thường không được đưa ra xem xét

Do đó, ưu tiên phát hiện đầy đủ các chênh lệch khối lượng có thể xác định bằng công thức
Đối với đơn giá, cảnh báo bất thường không đồng nghĩa với đơn giá sai, mà chỉ là tín hiệu cần người phụ trách kiểm tra

**Phương án kiểm soát:**

- Đối chiếu theo mã dòng và đơn vị tính
- Kiểm tra toàn bộ chênh lệch khối lượng bằng Rule
- Không tự động bỏ qua những dòng chưa ghép được
- Lưu giá trị gốc, giá trị tính toán và lý do cảnh báo
- Kiểm tra tổng giá trị sau khi ghép bảng
- Chuyên viên xác nhận kết quả trước khi trình lãnh đạo

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

| Rủi ro | Mức độ sơ bộ | Lý do và bằng chứng | Phương án xử lý |
|---|---|---|---|
| **Value Risk** | Thấp đến trung bình | Đã có dấu hiệu thực tế về khối lượng khoảng 16.000 dòng/vòng và thời gian kiểm tra 5–6 giờ/vòng, nhưng chưa đo hiệu quả của phương án mới | Thử nghiệm trên gói thầu cũ và so sánh thời gian trước/sau |
| **Usability Risk** | Trung bình | Chuyên viên quen sử dụng Excel, hệ thống mới có thể gây khó khăn nếu thay đổi cấu trúc làm việc | Giữ định dạng Excel quen thuộc, hiển thị rõ dòng sai lệch và cho phép kiểm tra thủ công |
| **Feasibility Risk** | Trung bình | Công thức có thể xử lý dữ liệu đúng mã dòng, nhưng file sai mẫu và mã hạng mục không khớp có thể gây lỗi | Tách bước kiểm tra cấu trúc, bước ghép dữ liệu và bước phát hiện chênh lệch |
| **Viability Risk** | Trung bình | Giải pháp Rule có chi phí triển khai tương đối thấp, nhưng cần duy trì quy tắc và bảo mật dữ liệu chào giá | Ưu tiên công cụ sẵn có, phân quyền truy cập, đo chi phí vận hành và thời gian tiết kiệm |

### 8.2. Kết luận

**Quyết định đề xuất cá nhân: GO với Rule-based Automation cho Problem Card #1**
**Đối với AI: NOT YET**
**Lý do:**

Problem Card #1 đã có dấu hiệu thực tế rõ ràng về khối lượng dữ liệu, thời gian xử lý và những chênh lệch cần phát hiện
Các phép so sánh khối lượng và đơn giá có thể thực hiện bằng công thức khi dữ liệu đã được ghép đúng mã dòng
Vì vậy, chưa có lý do đủ mạnh để sử dụng AI hoặc Agent thay cho Rule ở công đoạn này
AI có thể được nghiên cứu thêm cho việc xử lý file sai mẫu và đối chiếu mô tả hạng mục, nhưng cần kiểm chứng riêng lợi ích so với Power Query hoặc các quy tắc ghép dữ liệu

**Pilot nhỏ nhất nếu GO:**

Sử dụng một bộ hồ sơ chào giá đã xử lý trước đây, gồm 4 nhà thầu, khoảng 4.100 dòng BOQ và hai vòng chào giá nếu dữ liệu đầy đủ

**Các bước thử nghiệm:**

1. Chuẩn bị BOQ và bảng chào giá gốc
2. Chuẩn hóa mã hạng mục và kiểm tra đơn vị tính
3. Sử dụng Rule phát hiện chênh lệch khối lượng
4. Tính toán chênh lệch đơn giá theo ngưỡng được thống nhất
5. Xuất danh sách dòng cần kiểm tra
6. Đối chiếu kết quả với bảng đã được chuyên viên rà soát
7. Đo thời gian xử lý và số trường hợp bị bỏ sót

**Success Metrics:**

| Metric | Baseline từ bài cá nhân | Target |
|---|---|---|
| Thời gian soát một vòng | 5–6 giờ/vòng | Dưới 1,5 giờ/vòng |
| Thời gian soát một gói hai vòng | 10–12 giờ/gói | Dưới 3 giờ/gói |
| Phát hiện chênh lệch khối lượng ở dòng khớp mã | Chưa đo số dòng bị bỏ sót | Không bỏ sót dòng có chênh lệch trong bộ kiểm thử |
| Tổng tiền đối chiếu | Cần kiểm tra từng file gốc | Khớp 100% với các giá trị nguồn theo cùng phương pháp tính |
| Số lần lãnh đạo hỏi lại hoặc trả lại | Khoảng 4 lần ở gói gần nhất | Không tăng so với baseline |

**Điều kiện để mở rộng sang AI Workflow:**

- Có các trường hợp file sai mẫu xảy ra lặp lại
- Phương án Rule hoặc Power Query không ghép được đầy đủ dữ liệu
- AI giúp giảm thời gian ghép bảng mà không làm sai thông tin
- Các dòng AI ghép có thể được truy xuất và kiểm tra
- Có người chịu trách nhiệm xác nhận kết quả

**Ngưỡng dừng:**

- Tổng tiền trong bảng tổng hợp không khớp với file gốc mà không giải thích được
- Hệ thống bỏ sót chênh lệch khối lượng trong dữ liệu đã khớp mã
- Không phát hiện hoặc không cảnh báo các dòng thiếu mã, trùng mã hay không ghép được
- Thời gian xử lý không cải thiện đáng kể so với Excel/Power Query hiện có
- Chi phí triển khai và vận hành vượt quá lợi ích tiết kiệm được
- Không đảm bảo quyền truy cập và bảo mật hồ sơ chào giá

**Phương án quay về:**

Tiếp tục sử dụng file Excel gốc, công thức kiểm tra và quy trình rà soát thủ công của chuyên viên KTKT
Không sử dụng kết quả ghép dữ liệu chưa xác minh để tính toán hoặc trình lãnh đạo

**Kết luận:**

Bài toán có cơ sở để tự động hóa vì khối lượng dữ liệu lớn, thao tác lặp lại và có chỉ số thời gian thực tế
Tuy nhiên, giải pháp phù hợp nhất với Problem Card #1 là Rule-based Automation thay vì AI Agent
Việc sử dụng AI chỉ nên triển khai ở các bước cần hiểu nội dung phi cấu trúc, đặc biệt khi xử lý bảng chào giá không theo mẫu hoặc tài liệu hồ sơ năng lực
Quyết định cuối cùng vẫn cần được nhóm xác nhận dựa trên kết quả kiểm chứng và đánh giá của các actor liên quan

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
