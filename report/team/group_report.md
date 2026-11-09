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
| 1 | Phạm Quỳnh Anh | Khi khách hàng nhắn tin hỏi thông tin sản phẩm (giá, kích thước, tình trạng còn hàng) ngoài giờ hành chính (22h–7h), tôi muốn cung cấp thông tin chính xác và tư vấn tức thì cho khách, để giữ chân khách mua hàng mà tôi không phải thức đêm trực page. | Chủ cửa hàng online, nhân viên trực page, khách mua ban đêm | Độ trễ phản hồi qua đêm 6–8 tiếng khiến khách chuyển sang shop khác (tỷ lệ rớt đơn ban đêm 40%). | "Nếu khách chỉ hỏi dạo lúc 2h sáng rồi không mua thì có tốn công không? Giải pháp Rule tự động gửi tin nhắn mẫu có sẵn của Facebook có giải quyết được không?" (Vũ Đức Minh hỏi) |
| 2 | Phạm Quỳnh Anh | Khi phát sinh các khoản chi tiêu nhỏ lẻ trong ngày (tiền ăn, gửi xe, tiền mua đồ), tôi muốn ghi nhận lại số tiền và phân loại vào các khoản mục, để kiểm soát chi tiêu hàng tháng mà không phải nhớ lại và cộng trừ lại vào cuối ngày. | Cá nhân, sinh viên | Bước nhớ lại và gõ tay từng dòng vào Excel/app mỗi tối (15–20 phút), dễ bỏ cuộc sau 1 tuần. | "Tại sao không dùng app như Money Lover hay kiểm tra lịch sử biến động số dư ngân hàng? Rào cản lớn nhất là do bạn lười nhập liệu hay do app hiện tại khó dùng?" (Nguyễn Văn Nhi hỏi) |
| 3 | Phạm Quỳnh Anh | Khi ôn thi cuối kỳ với hơn 200 trang slide bài giảng, tôi muốn trích xuất các công thức và kiến thức cốt lõi thành bản tóm tắt, để có thể ghi nhớ nhanh chóng mà không mất 4–5 tiếng lật giở từng trang slide. | Sinh viên đại học | Bước đọc lướt và gõ lại công thức/định nghĩa sang file Word (mất 4–5 tiếng/môn). | "Dữ liệu slide bài giảng có nhiều hình vẽ, công thức toán dạng ảnh chụp và không có cấu trúc cố định thì hệ thống có đọc được không? Đã thử xin tóm tắt của khóa trên chưa?" (Vũ Đức Minh hỏi) |
| 4 | Vũ Đức Minh | Khi một nhân viên mới bắt đầu làm việc, tôi muốn được cấp đầy đủ tài khoản và quyền truy cập vào các hệ thống cần thiết theo vị trí công việc, để có thể bắt đầu thực hiện nhiệm vụ mà không phải chờ đợi các bộ phận liên quan thiết lập tài khoản. | Nhân viên mới, HR, IT/System Admin, quản lý trực tiếp | Bước xác định hệ thống cần cấp quyền, gửi yêu cầu, chờ phê duyệt từ nhiều đầu mối và thiết lập tài khoản trên từng hệ thống (mất vài ngày). | "Việc cấp quyền truy cập hệ thống công ty có chính sách bảo mật nghiêm ngặt và cần người chịu trách nhiệm, liệu có rủi ro bảo mật nào nếu tự động hóa khâu phân quyền này không?" (Phạm Quỳnh Anh hỏi) |
| 5 | Vũ Đức Minh | Khi người dân đến hỏi về một thủ tục hành chính, tôi muốn xác định đầy đủ hoàn cảnh và điều kiện của họ để hướng dẫn chính xác các giấy tờ, bước thực hiện cần thiết, nhằm hạn chế việc người dân phải đi lại nhiều lần do thiếu hồ sơ. | Cán bộ tiếp nhận hồ sơ, cán bộ tư vấn, người dân, cơ quan hành chính | Cán bộ phải khai thác thông tin, tra cứu quy định và đối chiếu điều kiện; cán bộ ít kinh nghiệm dễ bỏ sót câu hỏi hoặc trường hợp ngoại lệ. | "Quy định pháp luật và thủ tục hành chính thay đổi thường xuyên theo thông tư mới, làm sao đảm bảo thông tin tra cứu luôn được cập nhật chính xác và có giá trị pháp lý?" (Nguyễn Văn Nhi hỏi) |
| 6 | Vũ Đức Minh | Khi nhận được đơn đặt hàng cho mặt hàng công ty không còn tồn kho, tôi muốn nhanh chóng tìm được các nhà cung cấp thay thế có hàng sẵn, giá nhập và thời gian giao phù hợp, để đáp ứng đơn hàng và hạn chế mất doanh thu. | Nhân viên kinh doanh, nhân viên mua hàng, nhà cung cấp, khách hàng | Tìm kiếm và liên hệ nhiều nhà cung cấp, chờ phản hồi rồi tổng hợp thông tin so sánh giá và thời gian giao. | "Các nhà cung cấp bên ngoài thường không công khai tồn kho real-time qua API, vậy làm sao thu thập được dữ liệu tồn kho của họ mà không phải gọi điện thoại hỏi tay?" (Phạm Quỳnh Anh hỏi) |
| 7 | Nguyễn Văn Nhi | Khi bắt đầu thực hiện một bài tập Lab, tôi muốn nhanh chóng xác định được các yêu cầu, hướng dẫn thực hiện và quy định nộp bài từ những tài liệu liên quan, để hiểu đúng nhiệm vụ và bắt đầu triển khai mà không mất quá nhiều thời gian tìm kiếm thông tin. | Học viên thực hiện bài Lab (cá nhân và nhóm), Mentor hỗ trợ | Dò tìm và đối chiếu chéo yêu cầu/rule/rubric giữa 5–6 file tài liệu rời rạc (`Slide`, `README`, `RULES`, `CHECKPOINTS`, `RUBRIC`) mất 15–20 phút/lần. | "Tại sao không chỉ cần ban tổ chức gộp các yêu cầu thành 1 bảng checklist duy nhất ngay đầu file CHECKPOINTS (No AI/Rule) thay vì phải xây dựng giải pháp công nghệ phức tạp?" (Vũ Đức Minh hỏi) |
| 8 | Nguyễn Văn Nhi | Khi viết báo cáo nghiên cứu khoa học hoặc luận văn, tôi muốn đảm bảo mỗi nội dung, số liệu và nhận định trong bài viết đều được đối chiếu chính xác với nguồn tài liệu gốc, đồng thời duy trì đúng thứ tự trích dẫn, để tránh sai lệch thông tin và đáp ứng yêu cầu học thuật. | Sinh viên làm khóa luận/NCKH, Giảng viên hướng dẫn, Người phản biện | Mở lại từng paper PDF gốc để đối chiếu thủ công độ khớp giữa nhận định/số liệu trong bài viết với nội dung bài báo gốc (mất 25 phút/lần rà soát chương). | "Đã có các phần mềm quản lý trích dẫn như Zotero hay BibTeX giải quyết việc đánh số và định dạng, việc kiểm tra độ khớp ngữ nghĩa giữa câu viết và paper gốc có thực sự làm được bằng AI với chi phí token hợp lý không?" (Phạm Quỳnh Anh hỏi) |
| 9 | Nguyễn Văn Nhi | Khi thực hiện các thí nghiệm Ablation trong quá trình nghiên cứu, tôi muốn xác định chính xác cấu hình mô hình, phiên bản dữ liệu và các thay đổi được áp dụng cho từng lần chạy, để có thể truy vết, đối chiếu và sử dụng đúng kết quả thực nghiệm khi phân tích và viết luận văn. | Sinh viên/NCS làm Machine Learning, Thành viên nhóm nghiên cứu | Dò tìm lại cấu hình từ các file log rời rạc (30 phút) và phải chạy lại thí nghiệm khi không truy vết được (mất 4–6 tiếng GPU/lần chạy). | "Vấn đề này đã có các công cụ MLOps chuyên dụng như Weights & Biases (W&B) hoặc MLflow giải quyết rất tốt bằng việc lưu log tự động, liệu có cần can thiệp AI vào đây không hay chỉ là vấn đề kỷ luật dùng công cụ?" (Vũ Đức Minh hỏi) |

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
