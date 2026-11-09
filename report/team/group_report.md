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

**[CHỜ NHÓM XÁC NHẬN]** Phân nhóm sơ bộ có hỗ trợ AI, từ CP1–CP2 của bốn báo cáo trên main tại commit 71f0e47. Pitch, phản biện trực tiếp và lựa chọn cuối do các thành viên thực hiện.

**Các candidate trong top 3 của từng thành viên**

Mã dưới đây dùng để truy vết card gốc. Cột ưu tiên pitch ghi lựa chọn trong báo cáo cá nhân, chưa phải kết quả pitch của nhóm.

| Mã | Thành viên / nguồn | Candidate CP2 và mã CP1 | Ưu tiên pitch |
|---|---|---|---|
| K1 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #1: Tìm kiếm và tổng hợp thông tin dự án; CP1 #1, #5 | Có |
| K2 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #2: Truy xuất kiến thức kỹ thuật và quyết định cũ; CP1 #4, #9 | — |
| K3 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #3: Hiểu backlog và làm rõ yêu cầu; CP1 #2, #7 | — |
| D1 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #1: Đọc Pull Request lớn; CP1 #6 | Có |
| D2 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #2: Nhập lại thông tin khách hàng; CP1 #12 | — |
| D3 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #3: Đối chiếu chi phí thuê nhà; CP1 #19 | — |
| L1 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #1: Tìm lại bằng chứng trong paper đã đọc; CP1 #1 | Có |
| L2 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #2: Sàng lọc paper sát câu hỏi nghiên cứu; CP1 #3 | — |
| L3 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #3: Đối chiếu điều kiện đánh giá giữa các paper; CP1 #7 | — |
| A1 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #1: So sánh các biến thể tín hiệu định lượng; CP1 #2 | Có |
| A2 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #2: Xác định quyết định, người phụ trách và deadline sau cuộc họp; CP1 #9 | — |
| A3 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #3: Xác định trạng thái và thông tin thiếu của đề nghị mua vật tư; CP1 #8 | — |

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm và hiểu thông tin theo ngữ cảnh | K1, K2, D1, L1, L2 | Phải tìm, đọc và nối thông tin liên quan trước khi sử dụng: bối cảnh dự án, mã nguồn hoặc tài liệu nghiên cứu. Tìm lại nguồn đã biết và sàng lọc nguồn mới là các bước khác nhau, cần giữ riêng khi phân tích từng card. |
| B — Đối chiếu kết quả nghiên cứu | L3, A1 | Nhiều chỉ số và điều kiện thử nghiệm cần được đối chiếu trước khi diễn giải khác biệt; chỉ nhìn kết quả có thể dẫn đến so sánh thiếu căn cứ. |
| C — Làm rõ thông tin và trách nhiệm trong phối hợp | K3, A2, A3 | Thông tin để tiếp tục công việc còn thiếu hoặc mơ hồ; phải tìm đầu mối và xác nhận lại yêu cầu, trách nhiệm hoặc trạng thái xử lý. |
| D — Nhập lặp dữ liệu khách hàng | D2 | Cùng thông tin phải điền qua nhiều biểu mẫu, sau đó kiểm tra sự nhất quán. |
| E — Đối chiếu khoản thu với hợp đồng thuê | D3 | Người thuê phải kiểm các khoản thu bằng điều khoản và chứng từ liên quan. |

A và C gom theo pattern, chưa đồng nghĩa các card là cùng một problem. D và E tạm đứng riêng vì chưa có card khác đủ gần về pain và quy trình. Nhóm cần xác nhận ranh giới cluster, nhất là việc tìm lại thông tin so với sàng lọc thông tin mới ở A.

**Dữ liệu còn thiếu:** Dương chưa có số đo; Khoa chưa có baseline thực đo và các target còn là giả thuyết. Báo cáo của Lam dùng bối cảnh và số liệu giả định. An tự báo cáo tổng thời gian ở Card #1, còn thời gian phân rã và bối cảnh Card #2–#3 là ước lượng hoặc giả định. Chưa dùng các số này làm baseline chung hay bằng chứng đồng thuận của nhóm.

### 2.3. Opportunity Solution Tree rút gọn

**[CHỜ NHÓM XÁC NHẬN]** Cây minh họa cho phạm vi developer làm rõ một task trước khi triển khai, từ K1–K3 thuộc phần developer của cluster A và C. Các candidate còn lại vẫn giữ trong bảng cluster; phạm vi này chưa phải lựa chọn problem cuối cùng.

~~~text
OUTCOME: Giảm thời gian developer làm rõ một task trước khi triển khai,
         đồng thời hiểu đúng yêu cầu, phạm vi và căn cứ kỹ thuật.
├── Opportunity 1: Thông tin dự án liên quan đến task nằm rải rác,
│                 phải tìm và ghép lại bối cảnh. [K1]
├── Opportunity 2: Khó tìm lại kiến trúc và lý do quyết định kỹ thuật
│                 khi làm việc với module chưa quen. [K2]
└── Opportunity 3: Yêu cầu và acceptance criteria chưa rõ,
                  phải trao đổi nhiều vòng để xác nhận. [K3]
~~~

**Hướng đo đề xuất:** ghi thời gian xử lý chủ động từ lúc bắt đầu tìm hiểu task đến khi ghi được yêu cầu, phạm vi và căn cứ kỹ thuật liên quan; ghi riêng thời gian chờ phản hồi. Kiểm lại các nội dung này với nguồn và người phụ trách task, đánh dấu phần còn thiếu. Baseline, target và tiêu chí hoàn thành: [CẦN NHÓM XÁC ĐỊNH].

**Các ý là solution, không đặt ở tầng Opportunity:**

- AI assistant truy xuất và tổng hợp thông tin dự án — K1.
- RAG-based Technical Knowledge Assistant — K2.
- AI Requirements Assistant — K3.
- Shared folders, project templates và dashboard tập trung — K1.
- ADR, chuẩn hóa tài liệu và user story template/Definition of Ready — K2, K3.

Các ý trên đã xuất hiện trong phương án ở card gốc. Chúng mô tả cách xử lý pain, chưa phải giải pháp được nhóm chọn.

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
