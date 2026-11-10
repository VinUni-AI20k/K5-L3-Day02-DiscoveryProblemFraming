# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Nhom5
- Thành viên: Bùi Thái Sỹ (nhóm trưởng), Phạm Lý Ngọc Đức, Nguyễn Minh Triết, Trịnh Ngọc Ninh - chi tiết vai trò và đóng góp xem [TEAM.md](../../TEAM.md)
- Candidate problem được chọn (1 câu): Khi cần chọn quán đi ăn với người yêu hoặc nhóm bạn, tôi muốn tìm được quán đáng tin mà không phải lướt nhiều app và hỏi lại bạn bè, để chốt nhanh trong một vòng mà không sợ quán dở.
- Quyết định cuối: **Go** - pilot nhỏ 2 tuần, Workflow bán thủ công (Google Sheet + prompt AI chạy tay), có ngưỡng dừng (mục 8)

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
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** | Mục 3.2: 5/5 người phỏng vấn kể được một lần gần đây mất từ 20 phút hoặc từ 2 vòng gửi link mới chốt được quán; 4/5 người tin nhận xét bạn bè hơn review công khai; 8/8 người survey gặp vấn đề, 6/8 gặp hằng tuần, mức đáng giải quyết 4/5. Research (mục 3.3) cho thấy app như Beli đã đi theo hướng dựa trên bạn bè. Mẫu còn nhỏ (5 + 8 người) |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **TB** | Đầu ra dễ hiểu và dễ kiểm tra vì có trích dẫn. Nhưng bạn bè phải gửi nhận xét và xác nhận thẻ; nếu phiền thì không ai làm (giả định #3 chưa kiểm chứng) |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **TB** | Tóm tắt và đề xuất bằng LLM là năng lực có sẵn qua API, không cần huấn luyện mô hình riêng. Rủi ro nằm ở dữ liệu: nhận xét bạn bè chưa có tập trung, vòng bạn bè nhỏ có thể không đủ quán (giả định #3, #4 chưa kiểm chứng) |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **TB** | Chi phí pilot nhỏ (5 nhóm, vài chục lượt đề xuất). Rủi ro quyền riêng tư khi dùng tin nhắn của bạn bè; chưa có mô hình vận hành và nguồn thu khi mở rộng ra ngoài pilot |

### 8.2. Kết luận

**Quyết định:** **Go** (pilot nhỏ, bán thủ công)

**Lý do:** Không rủi ro nào ở mức Cao. Value ở mức Thấp nhờ kết quả phỏng vấn và khảo sát: người dùng thật sự mất nhiều vòng để chốt quán và tin nhận xét bạn bè hơn review công khai. Usability, Feasibility và Viability ở mức TB, đều xoay quanh một câu hỏi phỏng vấn không trả lời được - bạn bè có chịu gửi nhận xét không - và câu hỏi đó chỉ trả lời được bằng hành vi thật trong pilot. Pilot được kiểm soát: có người kiểm tra ở hai điểm (người viết xác nhận thẻ quán, người rủ duyệt đề xuất), có phương án quay về Rule và No AI, và có ngưỡng dừng rõ ràng. Pilot không xây app nên chi phí nếu thất bại thấp.

**Pilot nhỏ nhất:**

- **Quy mô:** 5 nhóm bạn (gồm cả cặp đôi và nhóm 4–6 người), trong 2 tuần.
- **Chuẩn bị (tuần 0):** đo baseline bằng timestamp chat của các lần chốt quán gần nhất và hỏi mức hài lòng (có / không) về 5 bữa ăn gần nhất của mỗi nhóm; mỗi nhóm gửi lại nhận xét về quán đã ăn chung (lấy từ tin nhắn cũ, có sự đồng ý của người viết); kiểm tra giả định #4 - mỗi nhóm có từ 10 quán chưa. Dữ liệu nhập tay vào Google Sheet.
- **Chạy thử:** khi cần chốt quán, người rủ nhập yêu cầu; nhóm lọc bằng bộ lọc của Sheet (Rule), rồi chạy prompt AI thủ công để tóm tắt nhận xét và đề xuất 3 quán kèm trích dẫn. Người rủ duyệt rồi gửi vào chat nhóm, cả nhóm chốt bằng poll. Sau bữa ăn, gửi nhận xét mới.
- **Đo:** thời gian và số vòng gửi link qua timestamp chat; tỉ lệ đề xuất được chọn; đánh giá hài lòng 1 câu sau bữa ăn; tỉ lệ bữa ăn có nhận xét mới; số lỗi theo 5 tiêu chí đánh giá ở mục 7.
- **Chưa làm trong pilot:** không xây app, không tự đặt bàn, không lấy dữ liệu tự động từ Messenger/Zalo.

**Ngưỡng dừng:**

- Nếu ở bước chuẩn bị có nhóm không gom đủ 10 quán đã ăn → loại nhóm đó khỏi pilot; nếu quá nửa số nhóm không đủ → **Not Yet**, xem lại actor (cần vòng bạn bè lớn hơn).
- Nếu sau 2 tuần dưới 50% bữa ăn có nhận xét mới → quay về **No AI** (danh sách chung + poll).
- Nếu người rủ phải sửa hoặc bỏ quá 50% đề xuất của AI, hoặc có trích dẫn bịa (vi phạm tiêu chí 1, 3) → quay về **Rule** lọc.
- Nếu sau 2 tuần thời gian chốt quán không giảm xuống dưới 15 phút → dừng và xem lại problem.

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
