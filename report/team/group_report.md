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

Candidate tổng hợp từ CP2 của bốn báo cáo cá nhân, dùng mã truy vết ở mục 2.2. Chưa có biên bản pitch hoặc câu hỏi phản biện trực tiếp.

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Khoa | K1 — Khi chuẩn bị sprint, cần tìm và ghép thông tin dự án để hiểu bối cảnh công việc | Developer mới hoặc tham gia dự án có sẵn | Tìm, đọc và đối chiếu thông tin qua nhiều nguồn (bước 2–6 trong card) | |
| 2 | Khoa | K2 — Khi làm task trên hệ thống có sẵn, cần tìm kiến thức và quyết định kỹ thuật cũ để hiểu module | Developer làm việc với module chưa quen | Đọc code, tìm lịch sử và hỏi người từng phụ trách (bước 3–6) | |
| 3 | Khoa | K3 — Khi nhận backlog mới, cần hiểu yêu cầu và acceptance criteria để bắt đầu đúng phạm vi | Developer nhận task từ PO, PM hoặc Tech Lead | Làm rõ yêu cầu qua nhiều vòng trao đổi (bước 3–6) | |
| 4 | Dương | D1 — Khi review PR lớn, cần hiểu thay đổi và rủi ro để nhận xét có căn cứ | Developer được giao review PR | Giả thuyết: lần theo mã liên quan để hiểu tác động (bước 4) | |
| 5 | Dương | D2 — Khi điền nhiều biểu mẫu, cần xác định thông tin khách hàng để hoàn tất hồ sơ không bỏ sót | Nhân viên nhập thông tin khách hàng | Giả thuyết: nhập lại các trường trùng (bước 4) | |
| 6 | Dương | D3 — Khi nhận tiền điện, nước và dịch vụ, cần đối chiếu hợp đồng để kiểm khoản phải trả | Người thuê nhà | Giả thuyết: đối chiếu từng khoản với điều khoản và dữ liệu tính tiền (bước 4) | |
| 7 | Lam | L1 — Khi dùng lại nhận định trong paper đã đọc, cần tìm đúng bằng chứng để giải thích có căn cứ | Sinh viên mới tham gia nhóm nghiên cứu, bối cảnh giả định | Dò bằng chứng trong PDF (bước 3), chưa đo thực tế | |
| 8 | Lam | L2 — Khi có nhiều paper liên quan, cần xác định bài sát câu hỏi nghiên cứu để chọn bài đọc sâu | Sinh viên chọn paper, bối cảnh giả định | Đọc tiêu đề và abstract (bước 2), chưa đo thực tế | |
| 9 | Lam | L3 — Khi so điểm số giữa paper, cần kiểm điều kiện đánh giá để tránh kết luận thiếu căn cứ | Sinh viên lập bảng so sánh, bối cảnh giả định | Đối chiếu mô hình, dữ liệu và thiết lập (bước 4), chưa đo thực tế | |
| 10 | An | A1 — Khi rà soát biến thể tín hiệu, cần nhận biết khác biệt để chọn bước thử tiếp có căn cứ | Người nghiên cứu tín hiệu định lượng | Đối chiếu nhiều thay đổi và chỉ số (bước 3), thời gian phân rã là ước lượng | |
| 11 | An | A2 — Khi tiếp tục việc sau họp, cần rõ quyết định, người phụ trách và hạn để không bỏ sót cam kết | Người tổng hợp biên bản, bối cảnh giả định | Xác nhận người phụ trách và deadline (bước 3) | |
| 12 | An | A3 — Khi tra đề nghị mua vật tư, cần biết người đang xử lý và thông tin thiếu để bổ sung đúng chỗ | Nhân viên gửi đề nghị mua, bối cảnh giả định | Xác định người giữ hồ sơ và thông tin thiếu (bước 3) | |

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

Phạm vi: tìm lại bằng chứng trong paper đã đọc, theo candidate L1 của Lam và [shortlist](shortlist.md).

~~~text
OUTCOME: Giảm thời gian tìm lại bằng chứng từ paper,
         đồng thời giữ đúng ngữ cảnh và truy xuất được nguồn.
├── Opportunity 1: Ghi chú thiếu vị trí cụ thể của bằng chứng
│                 như số trang, hình, bảng hoặc đoạn văn.
├── Opportunity 2: Mất thời gian dò lại PDF để tìm đúng
│                 đoạn, hình hoặc bảng cần dùng.
├── Opportunity 3: Khó xác nhận ngữ cảnh của bằng chứng
│                 để diễn giải nhận định đúng phạm vi.
└── Opportunity 4: Vị trí nguồn được ghi không nhất quán
                  giữa các paper, gây khó khi tìm lại.
~~~

Các opportunity trên lấy từ shortlist và [Card #1 của Lam](../individual/2A202604020_NguyenDucKhuongLam.md); cần được kiểm chứng bằng trường hợp thực tế. Hướng đo là thời gian tìm được bằng chứng, độ đúng của vị trí nguồn và ngữ cảnh. Baseline và target chưa chốt bằng số đo thực tế.

**Các ý là solution, không đặt ở tầng Opportunity:**

- AI chatbot đọc paper.
- RAG-based paper assistant.
- Tự động tóm tắt PDF.
- Ghi chú có cấu trúc, Zotero annotation và liên kết đến trang PDF.

### 2.4. Chấm điểm shortlist (1–5)

Nguồn: [shortlist.md](shortlist.md). Điểm được giữ nguyên từ bảng shortlist.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| L1 — Tìm lại bằng chứng từ paper | 5 | 5 | 4 | 5 | 5 | 5 | 4 | **33** |
| A1 — So sánh biến thể tín hiệu | 5 | 5 | 4 | 4 | 4 | 5 | 3 | **30** |
| K1 — Tổng hợp thông tin trước Sprint Planning | 5 | 4 | 2 | 3 | 3 | 4 | 4 | **25** |

Mốc 10 phút/lần, trong đó 6 phút dò PDF, là số liệu giả định trong báo cáo của Lam, chưa phải baseline đã đo. Điểm ở cột “Pain có bằng chứng” là đánh giá được ghi trong shortlist, chưa thay thế việc kiểm chứng thực tế.

**Candidate được chọn:** L1 — Tìm lại bằng chứng từ paper.

**Job Story:** Khi cần dùng lại một nhận định từ paper đã đọc, tôi muốn tìm đúng đoạn, hình hoặc bảng chứa bằng chứng, để giải thích có căn cứ mà không phải đọc lại cả bài.

**Vì sao chọn:**

- Phạm vi gọn trong một tác vụ: tìm đúng bằng chứng trong paper đã đọc.
- Có thể đo thời gian tìm và kiểm tra trực tiếp vị trí nguồn, ngữ cảnh trong PDF.
- Có phương án không dùng AI để đối chiếu: ghi số trang/hình/bảng, annotation và liên kết PDF trong Zotero.
- Không cần tích hợp nhiều nguồn dữ liệu dự án. Candidate đạt 33 điểm, cao nhất trong shortlist.

**Vì sao loại các candidate còn lại:**

- **A1 — So sánh biến thể tín hiệu:** domain quant research đặc thù; cần kiểm tra điều kiện thử nghiệm và phân biệt mô tả chênh lệch với kết luận nhân quả.
- **K1 — Tổng hợp thông tin trước Sprint Planning:** phạm vi rộng, liên quan nhiều nguồn và quyền truy cập; chưa có baseline thực nghiệm để xác định bước nghẽn chính.

**Xử lý bất đồng (nếu có):** Chưa có ghi nhận trong tài liệu nguồn.

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
