# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Trustmebro
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Dev mới mất nhiều thời gian tìm hiểu hệ thống của công ty vì tài liệu có thể thiếu hoặc không tồn tại. Họ phải tự lần mò đọc mã nguồn hoặc hỏi đồng nghiệp, nhưng câu trả lời không phải lúc nào cũng đầy đủ, khiến quá trình làm việc chậm hơn
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Lê hữu Toàn | Khi nhận câu hỏi thường gặp từ khách hàng tôi muốn tôi muốn trả lời nhanh và đúng thông tin, để khách hàng sớm đc giải quyết vấn đề | Nhân viên hỗ trợ, khách hàng | Nhân viên phải tìm lại thông tin và tự soạn câu trả lời cho các câu hỏi lặp lại | 	Câu hỏi lặp lại có thật sự gây ảnh hưởng lớn không, hay chỉ làm nhân viên mất vài phút? Có bằng chứng về số lượng và tổng thời gian mỗi tuần không?  |
| 2 | Lê hữu Toàn | Khi cần thông tin trong nhiều tài liệu nội bộ, tôi muốn tìm được câu trả lời nhanh chóng để không bị mất nhiều thời gian | Nhân viên mới, nhân viên vận hành | Thông tin nằm rải rác trong nhiều tài liệu nên khó tìm đúng câu trả lời nhanh chóng |Đây là vấn đề thiếu công cụ tìm kiếm hay tài liệu nội bộ vốn thiếu, cũ và mâu thuẫn? Nếu câu trả lời không có trong tài liệu thì giải pháp có giúp được không? |
| 3 | Lê hữu Toàn | khi chuẩn bị cải thiện sản phẩm, tôi muốn hiểu khách hàng đang gặp khó khăn gì để đề xuất giải quyết đúng yêu cầu | Nhóm hỗ trợ, nhóm sản phẩm | Phải đọc và tự tổng hợp nhiều phản hồi để nhận ra vấn đề khách hàng thường gặp |	Làm sao biết vấn đề khách hàng được nhắc nhiều nhất cũng là vấn đề quan trọng nhất? Nhóm có phân biệt tần suất phản hồi với mức độ ảnh hưởng không? |
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
OUTCOME: Giảm thời gian dev mới cần để hiểu công ty và dự án trước khi bắt đầu xử lý công việc
├── Opportunity A: Dev mới mất thời gian tìm thông tin vì tài liệu nằm rải rác ở nhiều nơi
├── Opportunity B: Dev mới khó biết tài liệu nào đầy đủ, mới nhất và đáng tin cậy
└── Opportunity C: Khi thiếu thông tin, dev mới khó biết cần hỏi ai và phải tự lần theo code
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
| 1 | dev mới thường mất nhiều thời gian để tìm hiểu cấu trúc và các vận hành hệ thống | value | 5 | 2 | có |
| 2 | thông tin thường được rải trong nhiều tài liệu | value | 4 | 3 | có |
| 3 | thời gian kéo dài do khó tìm thông tin | value | 4 | 2 | có |
| 4 | sử dụng ai để tra cứu dữ liệu nội bộ |Viability| 5 | 1 |- |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:dev mới mất nhiều thời gian tìm hiểu hệ thống vì thông tin nằm rải rác; khó khăn chính là tìm đúng thông tin, và một nơi tra cứu tập trung có thể giúp họ tìm câu trả lời nhanh hơn

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
HIỆN TẠI — khoảng 4 tiếng/lần tìm hiểu feature

[1 Nhận task, xác định phần cần tìm hiểu: 15']
→ [2 Đọc kiến trúc và quy ước dự án: 45']
→ [3 Tìm tài liệu về feature: 60']
→ [4 Đọc code và lần theo feature liên quan: 90'] ← BOTTLENECK
→ [5 Hỏi đồng nghiệp, xác nhận cách hiểu: 30']


```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 |Dev mới |Task được giao|Xác định feature cần tìm hiểu |Ước tính 15 phút |Xác định phạm vi cần đọc |
| 2 | Dev mới|Tài liệu dự án |Hiểu kiến trúc và quy ước cơ bản |Ước tính 45 phút |Tài liệu có thể thiếu |
| 3 |Dev mới |Tên feature, tài liệu liên quan |Thông tin ban đầu về feature | Ước tính 60 phút|Khó biết tài liệu nào liên quan |
| 4 |Dev mới |Mã nguồn, feature liên quan |Hiểu flow và các phần liên đới |Ước tính 90 phút |Phải tự lần theo code |
| 5 |Dev mới |Câu hỏi chưa rõ |Xác nhận cách hiểu |Ước tính 30 phút |Có thể phải chờ lead |

**Bottleneck chính:**Bước 4 — dev mới phải tự đọc mã nguồn và lần theo các feature liên quan, mất ước tính 90 phút. Tài liệu có thể thiếu nên khó xác định đúng luồng xử lý

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — mục tiêu dưới 2 tiếng/lần tìm hiểu

[1 Dev nhập tên feature và câu hỏi: 5']               ← CON NGƯỜI
→ [2 Tìm tài liệu và code liên quan: 10']             ← RULE
→ [3 Tóm tắt flow, kiến trúc và liên kết nguồn: 10']  ← AI
→ [4 Dev kiểm tra nguồn, hỏi người hướng dẫn nếu thiếu: 30'] ← CON NGƯỜI
→ [5 Dev đọc sâu phần liên quan và bắt đầu task: 60'] ← CON NGƯỜI
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước |5 |5 |Một số bước tìm và tổng hợp được hỗ trợ |
| Tổng thời gian |Khoảng 4 tiếng	 |Dưới 2 tiếng	 | |
| Số bước thủ công | 5/5|3/5 |Dev vẫn kiểm chứng và đọc phần code cần thiết |
| Bottleneck chính |Tự tìm và lần theo code feature liên quan |Dev kiểm tra độ phù hợp của nguồn và tóm tắt |Cần xác nhận nguồn trước khi áp dụng |
| Rủi ro mới phát sinh | |AI bỏ sót hoặc diễn giải sai flow |dev kiểm tra và hỏi người hướng dẫn khi chưa chắc chắn|

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

-Khảo sát mới có 24 người, trong đó 7 người đã đi làm xác nhận gặp vấn đề này
-Chưa kiểm chứng mục tiêu dùng AI có giúp giảm thời gian tìm hiểu xuống dưới 2 tiếng mà vẫn đảm bảo dev hiểu đúng feature hay không
-phỏng vấn thêm dev mới, bấm giờ quy trình hiện tại và thử nghiệm trên một feature nhỏ

## 10. Tài liệu tham khảo

-
