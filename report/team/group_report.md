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
| 1 | Kỹ sư trực ca mất trên 60 phút để khoanh vùng được tầng gây lỗi khi sự cố trải qua nhiều nguồn log | Value | 5 | 2 | Có, ưu tiên |
| 2 | Kỹ sư chấp nhận để hệ thống tự chặn IP hoặc giới hạn tốc độ khi độ tin cậy cao | Value / Usability | 5 | 1 | Có, ưu tiên |
| 3 | Sự cố ngoài giờ, nhất là ban đêm, bị phát hiện và xử lý trễ hơn nhiều so với giờ hành chính | Value | 4 | 2 | Có |
| 4 | Cảnh báo giả chiếm phần đáng kể thời gian của ca trực | Value | 4 | 2 | Có |
| 5 | Doanh nghiệp đã có log tập trung để hệ thống đọc được, không phải đăng nhập từng máy | Feasibility | 4 | 3 | Có (hỏi kèm công cụ đang dùng) |
| 6 | Độ tin cậy có thể tính từ tín hiệu kỹ thuật (thống kê, bằng chứng liên tầng, whitelist) thay vì để mô hình tự chấm | Feasibility | 5 | 2 | Sau, cần thử nghiệm kỹ thuật |

Giả định nhóm kiểm chứng trong buổi này: #1, #2, #3, #4 (quan trọng nhưng ít bằng chứng), kèm #5 qua câu hỏi về công cụ đang dùng. Giả định #6 là câu hỏi kỹ thuật, không kiểm được bằng phỏng vấn, để lại cho pilot.

### 3.2. Kiểm chứng

Cách đã dùng: **Phỏng vấn 5 người** ngoài nhóm đã từng trực sự cố hệ thống: kỹ sư DevOps/SRE đang đi làm, quản trị hệ thống, lập trình viên backend. Hình thức: gặp trực tiếp, gọi video/điện thoại và nhắn tin. Câu hỏi theo The Mom Test, chỉ hỏi về lần sự cố gần nhất đã xảy ra. Bộ câu hỏi: [cp4-cauhoi-phongvan.md](../assets/cp4-cauhoi-phongvan.md).

Interview snapshot: [Tổng hợp 5 buổi phỏng vấn](../assets/cp4-interview-tonghop.md)

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn DevOps/SRE, quản trị hệ thống, dev backend | 5 | Đa số đều gặp các pain: lần mò qua nhiều nguồn log, sự cố ban đêm không ai phản ứng kịp, và cảnh báo giả. 2/5 người thường xuyên bị gọi dậy giữa đêm để xử lý sự cố. Bên cạnh Grafana/Loki/Prometheus hoặc Datadog/New Relic, vẫn có người phải ssh vào từng máy dùng grep/tail để đọc log | Thời gian khoanh vùng tầng lỗi phổ biến chỉ **15–30 phút**, thấp hơn nhiều so với giả định 60–90 phút. Đa số **không** chấp nhận cho hệ thống tự chặn vô điều kiện, chỉ đồng ý khi có whitelist, rollback và giới hạn thời gian chặn |
| Công cụ đang dùng | 5 | Đã có log tập trung và dashboard (Grafana/Loki/Prometheus, Datadog/New Relic) nên hệ thống có nguồn dữ liệu để đọc | Một phần việc khoanh vùng đã được công cụ có sẵn hỗ trợ, nên khoảng trống thật không nằm ở việc gom log |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

1. **Đổi baseline và trọng tâm bottleneck.** Khoanh vùng tầng lỗi trong giờ hành chính chỉ mất 15–30 phút, không phải 60–90 phút. Phần tốn thời gian thật là độ trễ phát hiện và phản ứng **ngoài giờ** cùng thời gian đóng cảnh báo giả. Problem Statement chuyển trọng tâm sang "sự cố ngoài giờ bị phản ứng trễ" thay vì "đọc log chậm" nói chung.
2. **Sửa success metric.** Baseline thời gian khoanh vùng ghi 15–30 phút theo phỏng vấn. Metric chính chuyển sang thời gian từ lúc bất thường xuất hiện đến lúc cô lập xong cho các sự cố ngoài giờ, kèm số cảnh báo giả mỗi ca.
3. **Siết boundary.** Hành động tự động chỉ được phép khi có đủ ba điều kiện người dùng yêu cầu: đối tượng không nằm trong whitelist, có rollback một chạm, và thời gian chặn có giới hạn. Mọi trường hợp khác chuyển sang người duyệt (HITL).

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
