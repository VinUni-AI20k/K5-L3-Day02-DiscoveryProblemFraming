# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: hihihaha
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): #12 — Khi lập báo cáo tuần, kỹ sư sản phẩm tại nhà máy sản xuất mạch điện tử mất khoảng 70 phút mỗi tuần để tra số lượng sản xuất và đưa số liệu vào đúng mục trong biểu mẫu.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

Các câu có nhãn **Dự kiến** là bản nháp. Sau lượt phản biện, nhóm cập nhật câu thực tế và người hỏi vào đúng dòng.

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyen Tien Dat | Import Excel sổ quỹ: Khi làm task import Excel cho sổ quỹ tiền mặt, tôi muốn xác định đúng dữ liệu và cột ngay từ đầu, để không phải sửa lại file sau khi test | Thực tập sinh dev (MobifoneIT), mentor, BA | Map cột Excel (~40 phút/lần) | |
| 2 | Nguyen Tien Dat | Vẽ diagram đồ án: Khi vẽ diagram cho bài tập/đồ án, tôi muốn ra đúng cấu trúc ngay bản đầu, để không phải sửa nhiều vòng theo feedback | Sinh viên năm cuối, bạn cùng nhóm | Sửa diagram theo feedback (~20–25 phút/lần, 2 vòng) | |
| 3 | Nguyen Tien Dat | Đọc hiểu task Jira: Khi nhận task mới trên Jira, tôi muốn hiểu đúng yêu cầu và tài liệu liên quan trong một lần đọc, để không làm sai hướng rồi phải hỏi lại mentor | Thực tập sinh dev, mentor, BA | Đọc tài liệu nội bộ + đối chiếu (~35 phút/lần) | **Dự kiến – Nam:** Trong lần gần nhất, phần lớn 35 phút mất ở bước tìm tài liệu hay ở bước đối chiếu yêu cầu trên Jira? |
| 4 | Phí Hoàng Nam | Tổng hợp đầu việc lab. Khi nhận bài lab, tôi muốn xác định các đầu việc, thứ tự thực hiện và yêu cầu nộp để bắt đầu làm mà không bỏ sót phần bắt buộc. | Học viên làm bài lab | Đọc checkpoint và tổng hợp yêu cầu từ nhiều tệp Markdown (ước tính 15 phút, cần đo lại). | **Dự kiến – Huy:** Trong 30 phút chuẩn bị bài Day 1, riêng việc đọc và tổng hợp yêu cầu mất bao lâu nếu tách thời gian tìm hiểu Colab? |
| 5 | Phí Hoàng Nam | Tìm link Phoenix. Khi chuẩn bị gửi stand-up buổi sáng, tôi muốn tìm được link Phoenix để gửi bài trước 10 giờ và nhận XP. | Học viên cần gửi stand-up | Tìm lại tin nhắn chứa link Phoenix (khoảng 2 phút ở lần gần nhất). | |
| 6 | Phí Hoàng Nam | Theo dõi thông báo trên Outlook và Discord. Khi kiểm tra thông báo của chương trình, tôi muốn nhận ra những thông tin có việc cần làm để không bỏ lỡ yêu cầu hoặc thời hạn. | Học viên theo dõi thông báo của chương trình | Xác định thông báo nào có việc cần làm (ước tính 7 phút, cần kiểm tra xem có phải bước dẫn đến bỏ sót hay không). | |
| 7 | Nguyễn Bá Thành | Sau họp nhóm, tôi muốn rõ việc, người phụ trách và hạn để không phải hỏi lại. | Thành viên nhóm; nhóm trưởng | Hỏi lại thông tin sau họp: 5 lần từ 3 thành viên; chưa rõ thuộc bao nhiêu buổi. | **Dự kiến – Đạt:** Năm lượt hỏi lại xảy ra trong bao nhiêu buổi họp, và mọi người thường phải hỏi lại thông tin gì? |
| 8 | Nguyễn Bá Thành | Sau mỗi buổi LEC, tôi muốn tìm đủ link học tập để tiếp tục làm bài. | Học viên | Tìm lại link bài giảng, GitHub và nộp bài: khoảng 10 phút/buổi. |  |
| 9 | Nguyễn Bá Thành | Đầu ngày, tôi muốn nắm lịch và việc cần làm để chủ động sắp xếp. | Học viên; thành viên nhóm | Tổng hợp lịch học, việc nhóm, workshop/Office Hours: khoảng 10 phút/ngày. | |
| 10 | Nguyễn Văn Huy | Khi chuẩn bị weekly report, tôi muốn xác định 3 mã lỗi test xuất hiện nhiều nhất trong tuần, để tập trung báo cáo các lỗi chính | PE tại nhà máy sản xuất mạch điện tử | Tải file Excel từ phần mềm test và lọc, xếp hạng mã lỗi mất khoảng 60 phút mỗi tuần | |
| 11 | Nguyễn Văn Huy | Khi viết weekly report, tôi muốn xác định action phù hợp cho từng mã lỗi cũ và mới theo từng sản phẩm, để báo cáo có hướng xử lý rõ ràng | PE tại nhà máy sản xuất mạch điện tử | Viết action cho lỗi cũ mất khoảng 20 phút và lỗi mới khoảng 30 phút mỗi tuần | |
| 12 | Nguyễn Văn Huy | Khi tổng hợp weekly report, tôi muốn tra cứu số lượng sản xuất của tuần trước và đưa dữ liệu vào đúng mục, để báo cáo đầy đủ và hạn chế nhập sai | PE tại nhà máy sản xuất mạch điện tử | Tra số lượng mất khoảng 20 phút và copy-paste dữ liệu vào form báo cáo mất khoảng 50 phút mỗi tuần | **Dự kiến – Thành:** Trong lần lập báo cáo tuần gần nhất, phần nào tốn thời gian nhất trong 50 phút điền form: tìm đúng mục, chép số liệu hay kiểm tra lại? |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Xử lý dữ liệu và hoàn thiện báo cáo | #1, #10, #11, #12 | Mất thời gian đối chiếu cột dữ liệu, lọc mã lỗi, xác định hướng xử lý hoặc điền số liệu vào đúng mục báo cáo. |
| B — Làm rõ yêu cầu và đầu việc | #2, #3, #4, #7 | Phải đọc lại tài liệu, hỏi thêm hoặc sửa qua nhiều vòng để hiểu yêu cầu, việc cần làm và ai phụ trách. |
| C — Tìm và theo dõi thông tin | #5, #6, #8, #9 | Link, lịch và thông báo nằm ở nhiều nơi, khiến người dùng mất thời gian tìm lại hoặc dễ bỏ sót việc cần làm. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME — Giảm số phút tìm, hiểu và tổng hợp thông tin cho mỗi đầu việc
├── Opportunity A — Mất thời gian đối chiếu, lọc và điền số liệu vào đúng chỗ
├── Opportunity B — Phải hỏi lại hoặc sửa nhiều vòng vì yêu cầu và trách nhiệm chưa rõ
└── Opportunity C — Mất thời gian tìm lại link, lịch và thông báo nằm rải rác
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- Form Excel dùng công thức tra cứu để tự điền số liệu (#12) là một phương án giải quyết. Vấn đề ở nhánh A là thời gian Huy mất để tra và điền số liệu.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #12 — Tra số liệu và điền báo cáo tuần (Huy) | 5 | 5 | 3 | 5 | 4 | 4 | 3 | **29** |
| #7 — Làm rõ đầu việc sau họp nhóm (Thành) | 5 | 3 | 3 | 3 | 4 | 4 | 5 | **27** |
| #8 — Tìm lại link sau buổi học (Thành) | 5 | 4 | 3 | 4 | 5 | 2 | 5 | **28** |

Mức điểm phản ánh dữ kiện hiện có. #12 có thể đo riêng thời gian tra số lượng và điền biểu mẫu. Nhóm quen bối cảnh của #7 và #8 hơn, còn số liệu hiện có của cả ba đề tài cần được kiểm chứng.

**Candidate được chọn** — #12 của Nguyễn Văn Huy, đạt 29/35 điểm.

**Vì sao chọn** — Công việc lặp lại hằng tuần và có số liệu ban đầu
cho hai bước cụ thể: khoảng 20 phút tra số lượng sản xuất và 50 phút
điền form. Nhóm có thể kiểm chứng thời gian từng bước ở CP4.

**Vì sao loại #7** — Có 5 lượt hỏi lại từ 3 thành viên, nhưng chưa rõ
xảy ra trong bao nhiêu buổi họp và làm mất thêm bao nhiêu thời gian.

**Vì sao loại #8** — Ước tính 10 phút mỗi buổi đang gộp việc tìm link
bài giảng, GitHub và nơi nộp bài. Chưa rõ bước nào chiếm nhiều thời
gian nhất để khoanh phạm vi kiểm chứng.

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
