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
| --- | --- | --- | --- | --- | --- |
| 1 | Nguyễn Văn Minh | Muốn tóm tắt nhanh tiền sử bệnh để bác sĩ nắm ngay. | Mẹ/người thân, bác sĩ | Tìm lại thông tin từ giấy khám cũ (tốn thời gian lúc khám). | "Nhóm học IT, có đủ chuyên môn y tế để đánh giá bản tóm tắt đúng/sai không?" (Chuẩn) |
| 2 | Phạm Lê Chuẩn | Muốn biết nhanh hệ thống lỗi ở đâu để khắc phục ngay. | IT, kĩ thuật | Dò lỗi cú pháp hoặc tìm nguyên nhân gây lỗi (20-30 phút). | "Dùng AI chỉ lỗi luôn thì sinh viên có bị lười tư duy đi không?" (Cao) |
| 3 | Phạm Lê Chuẩn | Muốn tự động sắp xếp lịch trình, đặt lịch, nhắc hẹn. | Mọi người | Tự kiểm tra, đối chiếu lịch thủ công. | "Làm sao AI truy cập được tin nhắn Zalo cá nhân để lấy lịch?" (Huy) |
| 4 | Phạm Lê Chuẩn | Muốn điểm danh đầu/cuối ca học nhanh chóng. | Sinh viên, Giảng viên/trợ giảng | Xếp hàng chờ quét mã/gọi tên (15-20 phút). | "Bài này dùng mã QR tĩnh (Rule) là đủ, cần gì AI?" (Minh) |
| 5 | Vũ Quang Huy | Muốn xác định chủ đề trọng tâm từ đề cương ôn tập dài. | Sinh viên/Học sinh | Đọc dàn trải số lượng trang đề cương lớn. | "Mỗi môn cấu trúc khác nhau, đo lường độ chính xác của trọng tâm thế nào?" (Cao) |
| 6 | Vũ Quang Huy | Muốn nắm bài tập và deadline sắp tới để không bỏ sót. | Sinh viên/Học sinh | Phải lội 2-3 nguồn (LMS, nhóm lớp) mỗi tuần. | "Nếu trường đổi API của LMS thì giải pháp có sập không?" (Chuẩn) |
| 7 | Vũ Quang Huy | Muốn nắm thông tin quan trọng từ nhiều kênh thông báo của GV. | Sinh viên/Học sinh | Bỏ lỡ thông báo do trôi tin nhắn trên nhiều kênh. | "Quyền truy cập dữ liệu đa kênh cá nhân lấy ở đâu?" (Minh) |
| 8 | Phùng Văn Thanh Cao | Muốn lên kế hoạch học tập buổi tối theo deadline, độ khó. | Sinh viên | Mất 10-20 phút xếp việc nhưng vẫn miss deadline. | "Độ khó là cảm nhận chủ quan, hệ thống đo lường kiểu gì?" (Huy) |
| 9 | Phùng Văn Thanh Cao | Muốn tổng hợp deadline từ LMS, email, nhóm lớp. | Sinh viên | Lướt nhiều nguồn mỗi tối dễ bị sót thông tin. | "Có trùng lặp ý tưởng với bài toán quản lý deadline của Huy không?" (Chuẩn) |
| 10 | Phùng Văn Thanh Cao | Muốn có hướng dẫn phân tích, từng bước tiếp cận bài khó. | Sinh viên | Tốn 1-2 tiếng kẹt lại không tìm được hướng giải. | "Làm sao ngăn chặn việc AI giải hộ luôn thay vì chỉ hướng dẫn?" (Minh) |
| 11 | Phùng Văn Thanh Cao | Muốn tổng hợp kiến thức trọng tâm cuối ngày học. | Sinh viên | Mất 45-60 phút tự đọc lại slide. | "Nếu input là file ghi âm bài giảng thì xử lý thế nào?" (Huy) |
| 12 | Phùng Văn Thanh Cao | Muốn theo dõi tiến độ task để không ảnh hưởng nhóm. | Sinh viên, thành viên nhóm | Nhắc nhở thủ công, trùng lặp công việc. | "Đây là vấn đề ý thức hay do thiếu công cụ quản lý?" (Chuẩn) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
| --- | --- | --- |
| A | Hỗ trợ học tập / Ôn thi (5, 10, 11) | Rút gọn, tóm tắt và phân tích khối lượng tài liệu học thuật lớn. |
| B | Quản lý lịch & Deadline (3, 6, 7, 8, 9, 12) | Gom thông tin rải rác từ nhiều nguồn (LMS, Zalo, Email) để lập kế hoạch. |
| C | Tối ưu quy trình & Kỹ thuật (1, 2, 4) | Giảm thao tác lặp lại tốn thời gian ở một bước xử lý/đọc dữ liệu cụ thể. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian sinh viên IT/kỹ thuật bị kẹt lại khi hệ thống báo lỗi / lỗi code bài lab.
├── Opportunity A: Thông báo lỗi (log) của hệ thống quá dài và chứa nhiều thông tin rác.
├── Opportunity B: Việc copy mã lỗi lên Google trả về quá nhiều luồng ý kiến, phải tự chắt lọc.
└── Opportunity C: Sinh viên không xác định được chính xác dòng code nào là nguyên nhân gốc rễ.

```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

* "Tích hợp công cụ debug bằng AI vào thẳng phần mềm VS Code"
* "Chatbot tự động viết lại code cho đúng"

Dưới đây là phần nội dung được tổng hợp và hoàn thiện dựa trên bảng dữ liệu trong hình ảnh của nhóm bạn, kết hợp với bối cảnh lựa chọn "Sửa lỗi bài lab / hệ thống" của bạn ở các bước trước:

### 2. Hội tụ nhóm (CP3)

**2.1. Pitch**

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
| --- | --- | --- | --- | --- | --- |
| 1 | Nguyễn Văn Minh | Muốn tóm tắt nhanh tiền sử bệnh để bác sĩ nắm ngay. | Mẹ/người thân, bác sĩ | Tìm lại thông tin từ mớ giấy khám cũ (tốn thời gian lúc khám). | "Nhóm mình học IT, liệu có đủ chuyên môn y tế để đánh giá bản tóm tắt đúng/sai không?" (Chuẩn) |
| 2 | Phạm Lê Chuẩn | Muốn biết nhanh hệ thống lỗi ở đâu để khắc phục ngay. | IT, kỹ thuật | Đọc dò lỗi cú pháp hoặc tìm nguyên nhân (20-30 phút). | "Nếu dùng AI chỉ ra lỗi luôn thì sinh viên có bị lười tư duy đi không?" (Cao) |
| 3 | Phạm Lê Chuẩn | Muốn tự động sắp xếp lịch trình, đặt lịch, nhắc hẹn. | Mọi người | Tự kiểm tra, đối chiếu lịch thủ công. | "Làm sao AI truy cập được tin nhắn Zalo cá nhân để biết có lịch hẹn?" (Huy) |
| 4 | Phạm Lê Chuẩn | Muốn điểm danh đầu/cuối ca học nhanh chóng. | SV, Giảng viên | Xếp hàng quét mã/gọi tên (15-20 phút). | "Bài này dùng mã QR tĩnh (Rule) là xong, cần gì AI?" (Minh) |
| 5 | Vũ Quang Huy | Muốn xác định chủ đề trọng tâm từ đề cương ôn tập dài. | SV / Học sinh | Đọc dàn trải số lượng trang đề cương lớn. | "Mỗi môn một cấu trúc, làm sao đo lường độ chính xác của trọng tâm?" (Cao) |
| 6 | Vũ Quang Huy | Muốn biết bài tập/deadline sắp tới để không bỏ sót. | SV / Học sinh | Phải lội 2-3 nguồn (LMS, Zalo, Email) mỗi tuần. | "Nếu trường đổi API của LMS thì giải pháp có sập không?" (Chuẩn) |
| 7 | Vũ Quang Huy | Muốn nắm thông tin quan trọng từ nhiều kênh thông báo của GV. | SV / Học sinh | Bỏ lỡ thông báo do trôi tin nhắn nhiều kênh. | "Giống ý 6, quyền truy cập dữ liệu đa kênh lấy ở đâu?" (Minh) |
| 8 | Phùng Văn Thanh Cao | Muốn sắp xếp kế hoạch học tối ưu theo deadline, độ khó. | Sinh viên | Mất 10-20 phút mỗi tối để lên plan nhưng vẫn miss. | "Độ khó là cảm nhận chủ quan, hệ thống đo lường kiểu gì?" (Huy) |
| 9 | Phùng Văn Thanh Cao | Muốn tổng hợp deadline từ LMS, email, nhóm lớp cuối ngày. | Sinh viên | Lướt nhiều nguồn mỗi tối dễ bị sót. | (Trùng pattern với ý số 6 của Huy) |
| 10 | Phùng Văn Thanh Cao | Muốn có hướng dẫn phân tích, từng bước tiếp cận bài khó. | Sinh viên | Tốn 1-2h kẹt lại không tìm được hướng giải. | "Làm sao tránh việc AI giải hộ luôn thay vì chỉ hướng dẫn?" (Chuẩn) |
| 11 | Phùng Văn Thanh Cao | Muốn tổng hợp kiến thức trọng tâm cuối ngày học. | Sinh viên | Mất 45-60 phút tự đọc lại slide. | "Nếu bài giảng là video/audio thì input xử lý thế nào?" (Minh) |
| 12 | Phùng Văn Thanh Cao | Muốn theo dõi tiến độ nhóm để không ảnh hưởng kết quả chung. | SV, thành viên nhóm | Nhắc nhở thủ công, trùng lặp công việc. | "Đây là vấn đề ý thức hay vấn đề công cụ quản lý?" (Huy) |

**2.2. Cluster**

| Cluster | Các candidate | Pattern chung |
| --- | --- | --- |
| A — Hỗ trợ học tập / Ôn thi | Tóm tắt đề cương (5), Hướng dẫn giải bài tập (10), Tổng hợp kiến thức (11), Chuẩn bị bài trước (12). | Rút gọn, tóm tắt và phân tích khối lượng tài liệu học thuật lớn. |
| B — Quản lý lịch & Deadline | Xếp lịch (3), Tổng hợp deadline (6, 9), Xếp kế hoạch tối (8), Theo dõi task nhóm (13). | Gom thông tin rải rác từ nhiều nguồn (LMS, Zalo, Email) để lập kế hoạch. |
| C — Tối ưu quy trình & Kỹ thuật | Khắc phục lỗi hệ thống/lab (2), Tóm tắt bệnh án (1), Điểm danh (4). | Giảm thao tác lặp lại tốn thời gian ở một bước xử lý/phân tích log dữ liệu cụ thể. |

**2.3. Opportunity Solution Tree rút gọn**

Nhóm thống nhất chọn nhánh bài toán của người làm kỹ thuật/IT (Candidate 2 của Chuẩn) để đi tiếp vì phù hợp chuyên ngành nhóm.

```text
OUTCOME: Giảm thời gian sinh viên IT/kỹ thuật bị kẹt lại khi hệ thống báo lỗi / lỗi code.
├── Opportunity A: Thông báo lỗi (log) của hệ thống quá dài và chứa nhiều thông tin rác.
├── Opportunity B: Việc copy lỗi lên Google/StackOverflow trả về quá nhiều luồng ý kiến, phải tự chắt lọc.
└── Opportunity C: Sinh viên không xác định được chính xác dòng lệnh/code nào là nguyên nhân gốc rễ.
Những ý đã gạch bỏ vì là solution đội lốt opportunity:
- "Tích hợp công cụ debug bằng AI vào VS Code" (Đây là giải pháp công cụ)
- "Chatbot tự động viết lại code cho đúng" (Đây là giải pháp mức Agent)

```

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Theo dõi tiến độ task nhóm (Cao) | 5 | 4 | 5 | 5 | 4 | 5 | 5 | **33** |
| Khắc phục lỗi hệ thống/code bài lab (Chuẩn) | 5 | 5 | 4 | 4 | 3 | 4 | 3 | **28** |
| Tóm tắt tiền sử bệnh án (Minh) | 4 | 4 | 3 | 3 | 5 | 4 | 2 | **25** |

**Candidate được chọn:**
Theo dõi tiến độ task nhóm để không ảnh hưởng kết quả chung (Phùng Văn Thanh Cao).

**Vì sao chọn:**
Đây là nỗi đau (pain point) cực kỳ phổ biến mà bất kỳ sinh viên nào cũng gặp phải ("gánh team", trễ deadline do không ai nhắc, trùng lặp công việc). Bài toán có đối tượng rất rõ ràng, dễ dàng tìm người phỏng vấn để lấy bằng chứng ngay trong lớp. Impact đo lường được định lượng thông qua số lần trễ hạn hoặc số phút phải bỏ ra để họp nhóm/nhắn tin nhắc nhở mỗi tuần. Đặc biệt, bài toán này rất dễ để so sánh các mức can thiệp: từ No AI (chỉ dùng Trello/Excel), Rule (bot tự động nhắc giờ), đến Workflow (AI tự tóm tắt tiến độ từ tin nhắn chat và cập nhật trạng thái).

**Vì sao loại các candidate còn lại:**

* Bài "Khắc phục lỗi code bài lab": Dù quy trình rõ ràng, nhưng các lỗi (bug) có độ khó rất khác nhau, dẫn đến việc đo lường baseline thời gian trung bình thiếu chính xác. Hơn nữa, mức độ phức tạp của bài lab có thể vượt quá khả năng đánh giá của một số thành viên trong nhóm, dẫn đến rủi ro khó kiểm định chất lượng đầu ra của AI.
* Bài "Tóm tắt bệnh án": Bị loại do nhóm hoàn toàn không có chuyên môn y tế, rủi ro đánh giá sai tính sinh mạng (Feasibility/Viability rất cao).

**Xử lý bất đồng (nếu có):**
Chuẩn ban đầu muốn giữ bài "Khắc phục lỗi code" vì mang đậm tính kỹ thuật IT. Tuy nhiên, Cao và Huy đã phản biện và chỉ ra rằng bài "Theo dõi task nhóm" dễ thu thập dữ liệu (input) từ các đoạn chat nhóm trên Zalo/Discord hơn là việc trích xuất log lỗi hệ thống trên các môi trường máy ảo khác nhau. Nhóm đi đến thống nhất chọn bài Task Nhóm vì tệp người dùng rộng hơn, tính khả thi cao và "vừa sức lab" hơn để thiết kế một quy trình (workflow) hoàn chỉnh.
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
