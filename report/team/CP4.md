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

Thang điểm: 1 = thấp, 5 = cao; ưu tiên giả định quan trọng cao nhưng ít bằng chứng.

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Việc tìm lại bằng chứng xảy ra khoảng 3 lần/tuần, ảnh hưởng đến viết bảng so sánh và trả lời mentor. | Value | 5 | 2 | Có — đối chiếu các lần tìm trong tuần gần nhất. |
| 2 | Thiếu vị trí nguồn trong ghi chú là nguyên nhân chính khiến bước dò PDF mất khoảng 6 phút. | Value | 5 | 2 | Có — xem ghi chú và thao tác tìm thực tế. |
| 3 | Ghi chú kèm trang/hình/bảng và liên kết nguồn giúp hoàn tất một lượt trong tối đa 3 phút, vẫn đúng ngữ cảnh. | Usability | 5 | 1 | Có — đo thử cả thời gian và độ đúng. |
| 4 | Zotero hỗ trợ nối annotation trong ghi chú về trang PDF. | Feasibility | 4 | 4 | Đã đối chiếu tài liệu [Zotero PDF Reader](https://www.zotero.org/support/pdf_reader); cần thử với PDF đang dùng. |
| 5 | Công sức ghi nguồn ngay khi đọc thấp hơn thời gian tiết kiệm khi tìm lại. | Viability | 4 | 1 | Có — ghi thêm thời gian tạo ghi chú. |

**Ưu tiên kiểm chứng:** #2 và #3; nếu nghẽn ở hiểu ngữ cảnh thay vì định vị nguồn, liên kết trang chưa đủ giải quyết problem.

### 3.2. Kiểm chứng

| Nội dung rà soát | Ghi nhận từ Problem Card #1 |
|---|---|
| Actor / bối cảnh | Rachal, sinh viên mới tham gia nhóm nghiên cứu; cần dùng lại nhận định khi viết bảng so sánh hoặc trả lời nhóm/mentor. |
| Quy trình / workaround | Mở ghi chú → xác định paper → dò PDF → kiểm tra ngữ cảnh → ghi vị trí nguồn; đang dò lại vì ghi chú thiếu vị trí. |
| Thời gian / tần suất | Khoảng 10 phút/lần × 3 lần/tuần = 30 phút/tuần; riêng dò PDF khoảng 6 phút/lần = 18 phút/tuần. |
| Opportunity | Giúp đi từ nhận định đã ghi đến đúng bằng chứng trong paper, giữ được ngữ cảnh để giải thích. |

**Câu hỏi kiểm chứng hành vi:**

1. Lần gần nhất cần tìm lại bằng chứng để viết bảng so sánh hoặc trả lời mentor là khi nào? Hãy mở ghi chú và PDF đã dùng, kể lại từng bước.
2. Khi đó ghi chú có trang, số hình/bảng hoặc liên kết không? Bước nào mất lâu nhất, có lịch sử thao tác hay ghi nhận thời gian không?
3. Trong tuần gần nhất đã tìm lại bao nhiêu lần? Lần nào tìm nhanh hoặc không tìm được, khác nhau ở điểm gì?
4. Đã dùng annotation hoặc liên kết PDF lần nào? Hãy chỉ một ghi chú cụ thể và cách kiểm tra bằng chứng có thực sự hỗ trợ nhận định.

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác / cần kiểm tra |
|---|---|---|---|
| Problem Card #1 | 1 card; chưa có mẫu phỏng vấn | Mô tả bước dò PDF chiếm 6/10 phút và thiếu vị trí nguồn. | Chưa đủ để kết luận thiếu vị trí là nguyên nhân chính hoặc mức 10 phút đại diện cho người khác. |
| Tài liệu Zotero tại mục 3.3 | 2 trang tài liệu; không phải mẫu người dùng | Có sẵn cách gắn ghi chú với paper và quay lại trang PDF. | Phản bác nhu cầu phải xây công cụ AI mới; chưa chứng minh người dùng đạt mục tiêu 3 phút. |

### 3.3. Research giải pháp đã có

Các nguồn chính thức đã mở kiểm tra ngày 09/11/2026. Khoảng trống và bài học là nhận định của nhóm cho quy trình đang xét.

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Zotero — annotation → note → trang PDF | [PDF Reader and Note Editor](https://www.zotero.org/support/pdf_reader) | Bước 3, 5: annotation đưa vào note có liên kết về trang PDF và trích dẫn. | Giữ đường dẫn từ ghi chú về bằng chứng, không cần AI. | Ghi chú cũ thiếu annotation cần bổ sung; mở đúng trang chưa đảm bảo hiểu đúng điều kiện của kết quả. | Thử mẫu: nhận định + annotation + trang/hình/bảng + ngữ cảnh; vẫn giữ bước 4 do người đọc thực hiện. |
| Zotero — ghi chú gắn với paper | [Notes](https://www.zotero.org/support/notes) | Bước 1, 2: child note thuộc một tài liệu; nội dung note tìm được qua tìm kiếm Zotero. | Giữ ghi chú cùng paper, hỗ trợ xác định nguồn. | Chỉ gắn note với paper chưa chỉ ra đoạn bằng chứng. | Kết hợp child note với annotation; tên paper hoặc citation đơn lẻ chưa đủ. |
| Adobe Acrobat — tìm kiếm PDF | [Searching PDFs](https://helpx.adobe.com/acrobat/using/searching-pdfs.html) | Bước 3: tìm từ/cụm từ trong PDF để định vị nội dung. | Tận dụng công cụ tìm kiếm sẵn có khi nhớ từ khóa. | Nhận định diễn đạt lại có thể không khớp từ khóa; vẫn phải đọc kết quả và ngữ cảnh. | Dùng tìm kiếm khi ghi chú chưa có liên kết; tìm thấy thì lưu ngay vị trí để dùng lần sau. |

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
