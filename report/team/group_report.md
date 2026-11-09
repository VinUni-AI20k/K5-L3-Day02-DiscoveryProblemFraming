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
| A1 | Phụng | **Báo lỗi thiếu thông tin:** Khi nhận thông báo “máy bị lỗi”, tôi muốn có đủ thông tin về triệu chứng ngay từ đầu, để xác định cách xử lý nhanh hơn. | Nhân viên IT | Hỏi lại 2–3 lượt để lấy đủ mô tả và ảnh lỗi | "Nếu bắt điền biểu mẫu nhiều trường thì người dùng có lười rồi vẫn nhắn tin tự do không?" (Trường hỏi) |
| A2 | Phụng | **Yêu cầu hỗ trợ nằm rải rác:** Khi nhận yêu cầu hỗ trợ qua nhiều kênh, tôi muốn biết những việc nào còn chưa xử lý, để không bỏ sót yêu cầu. | Nhân viên IT | Đối chiếu trạng thái yêu cầu giữa nhiều kênh rời rạc | "Có thể quy định công ty chỉ dùng 1 kênh duy nhất không, tại sao phải gom nhiều kênh?" (Thanh hỏi) |
| A3 | Phụng | **Tìm và soạn lại hướng dẫn lỗi thường gặp:** Khi nhân viên hỏi cách xử lý một lỗi thường gặp, tôi muốn tìm nhanh hướng dẫn phù hợp, để hỗ trợ họ mà không phải soạn lại từ đầu. | Nhân viên IT | Tìm kiếm hướng dẫn cũ nằm rải rác | "Làm một trang FAQ/Wiki có giải quyết được không nếu người dùng vẫn ngại đọc bài dài?" (Trường hỏi) |
| B1 | Trường | **Khó tìm thông báo quan trọng trong Discord:** Khi kênh chat quá nhiều tin thảo luận, tôi muốn lọc nhanh các thông báo bài tập/lịch học quan trọng, để không bị trôi tin và lỡ hạn. | Học viên | Đọc lướt nhiều tin nhắn để nhận ra hạn nộp, đổi lịch | "Discord đã có tính năng ghim tin nhắn (Pinned) và kênh `#announcement`, tại sao vẫn bị trôi?" (Phụng hỏi) |
| B2 | Trường | **Chép deadline vào lịch cá nhân:** Khi có deadline mới công bố trên lớp, tôi muốn đưa nhanh vào lịch cá nhân, để nhận thông báo nhắc nhở tự động đúng hạn. | Học viên | Xác định giờ nộp và nhập lịch thủ công từng môn | "Một tuần có bao nhiêu deadline để việc nhập tay này trở thành vấn đề nghiêm trọng?" (Thanh hỏi) |
| B3 | Trường | **Conflict khi cùng sửa báo cáo:** Khi cả nhóm cùng viết báo cáo bài tập lớn, tôi muốn đồng bộ nội dung đang làm, để không bị ghi đè hoặc xung đột code/text. | Nhóm làm lab | Giải quyết xung đột nội dung khi ghép bài | "Nếu dùng Google Docs hoặc chia file Markdown riêng theo từng mục thì có còn bị conflict không?" (Phụng hỏi) |
| C1 | Thanh | **Khó chọn nội dung ưu tiên ôn từ nhiều PDF:** Khi chuẩn bị thi cuối kỳ từ hàng chục slide và tài liệu, tôi muốn biết các phần trọng tâm cần học, để ôn tập hiệu quả mà không lan man. | Sinh viên | Đọc và chọn lọc nội dung trọng tâm từ nhiều tài liệu | "Trọng tâm bài thi phụ thuộc vào đề giảng viên ra, làm sao công cụ biết được phần nào chắc chắn thi?" (Trường hỏi) |
| C2 | Thanh | **Điểm danh đầu giờ mất thời gian:** Khi bắt đầu buổi học/lab, tôi muốn ghi nhận sự có mặt nhanh chóng, để bắt đầu bài học đúng giờ mà không tốn thời gian gọi tên. | Giảng viên, sinh viên | Gọi tên và đọc lại danh sách từng người | "Trường hoặc lớp đã có mã QR quét điểm danh chưa, rào cản ở đây là công nghệ hay thói quen?" (Phụng hỏi) |
| C3 | Thanh | **Phải hướng dẫn lại thao tác điện thoại cho bố mẹ:** Khi bố mẹ gặp khó khi dùng smartphone, tôi muốn có cách hướng dẫn trực quan từ xa, để bố mẹ tự làm được mà không phải hỏi lại cùng một việc. | Bố mẹ, người hướng dẫn | Nhắc lại các thao tác nhiều lần vì người lớn tuổi chưa nhớ | "Vấn đề này quá phụ thuộc vào khả năng tiếp thu công nghệ của người lớn tuổi, liệu giải pháp số có khả thi?" (Trường hỏi) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm và chọn thông tin cần thiết | A3, B1, C1 | Phải đọc hoặc tìm kiếm qua nhiều nội dung rời rạc để lấy đúng phần thông tin phù hợp |
| B — Tiếp nhận và theo dõi yêu cầu | A1, A2 | Thiếu thông tin ban đầu hoặc thiếu trạng thái minh bạch để xử lý và bàn giao công việc |
| C — Công việc hành chính lặp lại | B2, C2 | Các thao tác thủ công, lặp đi lặp lại định kỳ có quy trình từng bước tương đối rõ ràng |
| D — Phối hợp sửa tài liệu | B3 | Nhiều người cùng thao tác và thay đổi trên một tài liệu/báo cáo dẫn đến xung đột nội dung |
| E — Hướng dẫn thao tác và ghi nhớ | C3 | Người dùng khó nhớ các bước thao tác kỹ thuật và cần người khác hướng dẫn/nhắc lại nhiều lần |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian tiếp nhận, làm rõ và phân loại yêu cầu hỗ trợ kỹ thuật từ 25 phút xuống dưới 5 phút cho nhân viên IT Helpdesk
├── Opportunity 1: Người dùng báo lỗi cụt lủn, thiếu thông tin thiết bị và ảnh chụp lỗi, buộc IT phải chat hỏi lại 2–3 lượt (A1)
├── Opportunity 2: Yêu cầu gửi rải rác qua nhiều kênh (Slack, Zalo, Email, trực tiếp), khó đối chiếu trạng thái dẫn đến nguy cơ sót việc hoặc xử lý trùng (A2)
└── Opportunity 3: Tài liệu hướng dẫn lỗi thường gặp bị phân tán ở nhiều nơi, mất 8–10 phút mỗi lần tìm lại để soạn câu trả lời (A3)
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ *"Xây dựng chatbot AI tự động hỗ trợ kỹ thuật trên Slack"* ← Solution đội lốt opportunity (nhóm cần giải quyết việc thiếu thông tin và tìm kiếm, chatbot chỉ là một công cụ khả dĩ).
- ✗ *"Triển khai hệ thống Jira Service Management hoặc Google Form bắt buộc"* ← Solution đội lốt opportunity (nhu cầu gốc là thu thập đủ thông tin triệu chứng ngay từ đầu).
- ✗ *"Tạo trang Notion Wiki tập trung tất cả tài liệu IT"* ← Solution đội lốt opportunity (nhu cầu gốc là rút ngắn thời gian tìm và gửi hướng dẫn phù hợp cho người dùng).

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
