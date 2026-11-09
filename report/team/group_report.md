# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: BDHH
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): 
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | [Bình] | **CV theo vai trò:** Khi ứng tuyển các vai trò khác nhau (Fullstack, QA/Tester, BA), tôi muốn CV nhấn đúng dự án liên quan từng vai trò, để nhà tuyển dụng thấy mình phù hợp. | Sinh viên CS năm cuối ứng tuyển đồng thời 2–3 vai trò (Fullstack, QA/Tester, BA), có 5+ repo đồ án cũ chưa đưa lên CV. | **Bước 3:** Lục lại code/commit/test của đồ án cũ để tìm bằng chứng kỹ thuật có thật (số API, test case, cấu hình, benchmark) — mất ~30 phút/bản (trong tổng ~95 phút) vì quên chi tiết và thiếu sẵn metric. | *(Gợi ý câu hỏi dễ gặp: Nếu đã lập file "Master Project Log" ghi sẵn số liệu chỉ mất 2 phút copy thì có thực sự cần AI nữa không, hay chỉ cần 3 bản CV mẫu cố định cho 3 role?)* |
| 2 | [Bình] | **Review sơ đồ PlantUML:** Khi review bộ sơ đồ sequence PlantUML trước khi chốt báo cáo, tôi muốn biết sơ đồ nào sai mã hóa hoặc lệch luồng xử lý so với code, để không nộp sơ đồ mâu thuẫn với hệ thống thật. | Sinh viên làm đồ án cá nhân (6 sprint), viết báo cáo dùng PlantUML (`.puml`) cho ≥10 nhóm chức năng và sửa code backend nhiều đợt trước khi nộp. | **Bước 2:** Mở 3–4 file code (`Controller`/`Service`) đối chiếu thủ công luồng gọi hàm, truy vấn DB và trạng thái trả về với từng file `.puml` — mất ~25 phút/đợt (~2.5 phút × 10 sơ đồ, trên tổng ~60 phút/đợt) và dễ sót lỗi. | *(Gợi ý câu hỏi dễ gặp: Tần suất chỉ 2–3 đợt/học kỳ thì ROI của việc đưa vào AI có đáng không, hay dùng checklist cố định 4 lỗi + script bắt lỗi UTF-8 là đủ?)* |
| 3 | [Bình] | **Kiểm báo cáo lab trước khi nộp:** Khi nộp báo cáo lab (`.md`) lúc gần deadline, tôi muốn biết mình còn bỏ trống mục nào hoặc ghi lệch số liệu nào so với lần chạy notebook cuối, để không bị trừ điểm vì sai sót hình thức. | Sinh viên học môn AI/ML làm báo cáo `.md` tách rời khỏi file `.ipynb`, hay chạy lại thực nghiệm sát giờ nộp làm thay đổi tham số/kết quả. | **Bước 3:** Đối chiếu thủ công số liệu (`SEED`, tham số, kết quả) giữa báo cáo `.md` và output cell của `.ipynb` — mất ~7 phút/bài (trên tổng ~20 phút/bài, micro-pain), dễ sót khi chạy lại notebook phút chót. | *(Gợi ý câu hỏi dễ gặp: Pain chỉ mất ~7 phút và kiểm tra đúng/sai tường minh, tại sao không chốt chạy xong `.ipynb` rồi mới điền kèm regex quét ô trống thay vì dùng AI?)* |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

---

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A (Cluster 1)** | - CV theo vai trò (Problem Card #1)<br>- Báo cáo tiến độ tuần (Ảnh #1)<br>- Meeting notes & Phân công công việc (Ảnh #3) | **Báo cáo & Tổng hợp thông tin đa nguồn (Information Synthesis & Reporting):** Dữ liệu đầu vào nằm rải rác ở nhiều nơi hoặc từ nhiều người. Con người mất nhiều thời gian đọc lướt, trích lọc, cấu trúc lại và tổng hợp thành văn bản hoàn chỉnh theo một định dạng chuẩn. |
| **B (Cluster 2)** | - Review sơ đồ PlantUML (Problem Card #2)<br>- Kiểm tra báo cáo lab trước khi nộp (Problem Card #3)<br>- Deploy code sai cấu hình (Candidate gốc) | **Đối chiếu chéo & Kiểm tra tính nhất quán (Consistency Checking & Verification):** Cần so sánh thủ công giữa hai hoặc nhiều nguồn thông tin (đặc tả và mã nguồn, cấu hình và môi trường, báo cáo và kết quả thực tế) để phát hiện sai lệch, thiếu sót hoặc những điểm không nhất quán. |
| **C (Cluster 3)** | - Debug lỗi log hệ thống (Candidate gốc)<br>- Thành viên báo lỗi thiếu log (Candidate gốc)<br>- Đọc tóm tắt bài báo nghiên cứu mới (Ảnh #2)<br>- Tìm tài liệu học tập phù hợp (Ảnh #5, #6)<br>- Tự sửa lỗi bài tập ngoài giờ (Ảnh #4) | **Thu thập, Sàng lọc & Gỡ lỗi kỹ thuật (Debugging & Information Retrieval):** Đối mặt với khối lượng dữ liệu lớn hoặc nhiễu (log dài, nhiều bài báo, tài liệu học tập hoặc thông tin lỗi). Con người cần nhanh chóng tìm kiếm, sàng lọc, khoanh vùng thông tin liên quan và xác định nguyên nhân cốt lõi để đưa ra hướng xử lý phù hợp. |

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
# 3. Kiểm chứng + research (CP4)

**Bài toán ban đầu (Problem #1):** Debug lỗi từ file log hệ thống.

- **Job Story:** Khi gặp lỗi kết nối CSDL hoặc lỗi logic lúc viết backend, tôi muốn truy ra đúng dòng gây lỗi từ file log, để không phải thử sửa mò nhiều lần.
- **Quy trình hiện tại (6 bước):** `[1. Chạy code / gặp lỗi]` → `[2. Mở file log / console]` → `[3. Đọc dò stack trace & lọc nhiễu]` *(bottleneck theo ước tính của nhóm: 20–30 phút/lần)* → `[4. Mở các file code nghi ngờ để đối chiếu]` → `[5. Sửa thử & chạy lại]` → `[6. Xác nhận hết lỗi]`.

---

## Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm trước? |
| :-: | :--- | :--- | :-: | :-: | :-: |
| 1 | Lập trình viên khác cũng mất 20 phút trở lên cho một lần debug lỗi khó, không chỉ riêng mình | Value | 5 | 1 | ✅ |
| 2 | Khi kiểm tra trạng thái lỗi, lập trình viên chủ yếu dựa vào log/console hơn là debugger (breakpoint) | Value | 4 | 2 | ✅ |
| 3 | Bước tốn thời gian nhất là lọc nhiễu trong log và mở đối chiếu nhiều file code trước khi biết sửa ở đâu | Value | 5 | 2 | ✅ |
| 4 | Có thể lọc phần nhiễu của log (timestamp, ID, log cấp thấp) bằng script/parser trước khi đưa vào AI | Feasibility | 4 | 4 | ✅ ([2], [5]) |
| 5 | AI chỉ ra được nguyên nhân từ log + code mà không báo động giả hoặc bịa (hallucination) làm mất thêm thời gian kiểm tra | Feasibility | 5 | 1 | ✅ ([2], [5]) |
| 6 | Lập trình viên / công ty chấp nhận đưa log và mã nguồn vào công cụ AI | Viability | 5 | 1 | Hỏi bạn làm backend (xem Bước 2, mục "Việc còn thiếu") |

---

## Kiểm chứng

### Cách kiểm chứng và giới hạn

Nhóm **không phỏng vấn trực tiếp** ở vòng này. Thay vào đó, nhóm dùng 5 tài liệu đã công bố làm **bằng chứng thứ cấp** để kiểm các giả định có điểm bằng chứng thấp (#1, #2, #3, #4, #5). Các giới hạn chung:

- Không tài liệu nào nghiên cứu đúng actor của nhóm (dev backend gặp lỗi CSDL) hoặc kiểm tra việc dev có chấp nhận giải pháp AI hay không. Vì vậy giả định #6 chưa có bằng chứng thực nghiệm từ người dùng (chỉ mới có thông tin chính sách bảo mật từ tài liệu sản phẩm [6]).
- Các nguồn có độ tin cậy khác nhau (quan sát hành vi > khảo sát tự khai; bài nghiên cứu > báo cáo của doanh nghiệp / dự án sinh viên). Mỗi snapshot bên dưới có dòng "Giới hạn".
- Bài [5] là nguồn duy nhất kiểm tra trực tiếp việc đưa stack trace và code vào LLM, nhưng đo trên benchmark Java mã nguồn mở và không đo thời gian tiết kiệm được khi debug [5, §3.1, §5-RQ3].

Quy ước trích dẫn: `[số, vị trí]`, ví dụ `[1, Table 5]` là tài liệu [1], bảng 5. Danh mục đầy đủ ở cuối file.

### Evidence Snapshot #1 — Quan sát hành vi thực tế [1]

| Trường | Nội dung |
| :--- | :--- |
| **Loại bằng chứng** | Quan sát thực địa (field observation) qua video lập trình live-stream của dự án mã nguồn mở `[1, §1, §3.1]` |
| **Đối tượng** | 11 lập trình viên, 15 phiên, tổng 30 giờ; các dự án như Firefox, Curl, Webpack, Alacritty… Số năm đóng góp mã nguồn mở từ 7 đến 31 (trung vị 9); một số ghi trên GitHub từng làm ở Google, Microsoft, Lyft, PayPal, Mozilla `[1, §3.2, Table 2]` |
| **Phát hiện then chốt (nguyên văn)** | *"No activity emerged as a singular bottleneck"* `[1, §4.3]` |
| **Bối cảnh ghi nhận** | 89 phiên debug (*debugging episode*), tính từ lúc xuất hiện thông báo lỗi trên console/UI, test fail, kết quả sai kỳ vọng hoặc bắt đầu tái hiện lỗi từ issue tracker đến khi hết lỗi hoặc dev dừng debug; tổng 15 giờ debug (2.137 hoạt động) và 13 giờ lập trình (1.407 hoạt động) `[1, §3.3, §4]` |
| **Hành vi / workaround thực tế** | Kiểm tra trạng thái chương trình bằng log (`log statements`) chiếm 70%, bằng debugger (`breakpoints`) 30%; mỗi lần kiểm tra trung bình 53 (±105) giây `[1, §4.2, Table 5]`. Test thủ công chiếm 84% các lần test `[1, Table 5]`. Mỗi phiên debug duyệt trung bình 3 (±5) file khác nhau, tối đa 32 file `[1, §4.2, Table 5]`. Các nghiên cứu trước ghi nhận dev dùng debugger rất ít (14% thời gian IDE; 0.87% và 3.9% tổng thời gian) `[1, §2]` |
| **Mất bao lâu, bao lần** | Debug chiếm 13%–95% thời gian phiên, trung bình 48% (±24%) `[1, §4.1]`. Cứ khoảng 8 (±10) phút lập trình lại có một lỗi mới cần debug `[1, §4.1]`. Lỗi tự gây ra lúc đang gõ code (*inserted defects*, 79 phiên) mất trung bình 6 (±8) phút (nhưng 20% trong số đó vẫn kéo dài 18 ± 9 phút); lỗi lấy từ issue tracker (*reported defects*, 10 phiên, 5 dev) mất 51 (±38) phút `[1, §4.1]`. **80% tổng thời gian debug đến từ 25 trên 89 phiên** (và 23 phiên dài ≥ 12.3 phút có thời lượng trung bình 32 ± 23 phút, chiếm 80% tổng thời gian) `[1, §4.1, §4.3, Figure 4]` |
| **Giới hạn** | Chỉ 11 dev, dự án mã nguồn mở, biết mình đang bị ghi hình `[1, §5]`. "Log" trong Table 5 là câu lệnh log/print do dev đặt để quan sát trạng thái chương trình (`log statements`), **không phải** đọc file log hệ thống hay stack trace `[1, §4.2, Table 5]`. Số liệu 51 phút chỉ từ 10 phiên (và một nửa trong số đó chưa sửa xong khi kết thúc phiên) `[1, §4.1]`. Không riêng lỗi CSDL. Bản dùng là preprint arXiv |
| **Insight** | Pain có thật nhưng **phân bố rất lệch**: ít phiên debug dài gây ra phần lớn thời gian mất đi, còn lỗi nhỏ tự gõ xong thì sửa nhanh `[1, §4.1, §4.3]`. Không có một bước đơn lẻ nào là nút thắt chính `[1, §4.3]`. Thời gian đi vào việc chuyển qua lại giữa kiểm tra trạng thái, duyệt file, sửa và chạy lại (ở phiên dài, kiểm tra trạng thái chiếm 18% và duyệt file chiếm 17% thời gian, trong khi sửa code chiếm 37% và chạy test chiếm 17% `[1, Figure 7]`) |

### Evidence Snapshot #2 — Khảo sát developer & lãnh đạo [3]

| Trường | Nội dung |
| :--- | :--- |
| **Loại bằng chứng** | Khảo sát tự khai do Stripe hợp tác với Harris Poll thực hiện và công bố (báo cáo doanh nghiệp, không bình duyệt) `[3, tr.8]` |
| **Đối tượng** | Hơn 1.000 lập trình viên và hơn 1.000 lãnh đạo C-level; trang 1 nêu tại 6 quốc gia nhưng phần phương pháp ở trang 8 chỉ liệt kê 5 quốc gia (Mỹ, Anh, Pháp, Đức, Singapore) `[3, tr.1, tr.8]` |
| **Phát hiện then chốt (nguyên văn)** | *"the average developer spends more than 17 hours a week dealing with maintenance issues, such as debugging and refactoring"* `[3, tr.3]` |
| **Bối cảnh ghi nhận** | Người trả lời tự ước lượng số giờ làm việc mỗi tuần (trung bình 41.1 giờ) và số giờ dành cho từng nhóm việc bảo trì / nợ kỹ thuật `[3, tr.3, tr.4, tr.5]` |
| **Hành vi / workaround thực tế** | Dev cho rằng thứ cản trở năng suất là bảo trì hệ thống cũ / nợ kỹ thuật (52%), việc lãnh đạo đổi ưu tiên (45%) và tự xây công nghệ riêng (40%) `[3, tr.5]` |
| **Mất bao lâu, bao lần** | Trung bình 17.3 giờ/tuần (≈42% của 41.1 giờ) cho nhóm "bad code / errors, debugging, refactoring, modifying", trong đó 13.5 giờ là nợ kỹ thuật và 3.8 giờ là bad code `[3, tr.4, tr.5]`. Gần hai phần ba dev (cụ thể là **59%** ở biểu đồ trang 4) đồng ý mức thời gian xử lý bad code này là "excessive" `[3, tr.3, tr.4]` |
| **Giới hạn** | Số tự khai. Con số 17.3 giờ **gộp** cả bad code, lỗi, debug, refactor, sửa đổi và nợ kỹ thuật nên không tách được riêng thời gian debug bằng log `[3, tr.4, tr.5]`. Không đo thời gian cho một lần debug. Báo cáo do một công ty công bố, quy đổi ra "thiệt hại GDP" ($85 tỷ - $300 tỷ/năm) bằng phép tính của chính Stripe `[3, tr.3, tr.5]` |
| **Insight** | Chỉ xác nhận ở mức chung rằng bảo trì/sửa lỗi là phần việc lớn và dev thấy nó quá nhiều. **Không xác nhận** con số 20–30 phút/lần của nhóm, nên không dùng làm bằng chứng trực tiếp cho giả định #1 |

### Evidence Snapshot #3 — Khảo sát về thời gian debug [4]

| Trường | Nội dung |
| :--- | :--- |
| **Loại bằng chứng** | Khảo sát + phỏng vấn trong một dự án sinh viên MBA (Cambridge Venture Project) của Cambridge Judge Business School `[4, trang bìa, slide 3, slide 18]` |
| **Đối tượng** | 54 phiếu khảo sát và 11 phỏng vấn (từ khoảng 10–12 tổ chức); phạm vi là lập trình viên viết mã biên dịch (compiled code) trên Linux `[4, slide 3, slide 5]` |
| **Phát hiện then chốt (nguyên văn)** | *"developers spend half their programming time debugging"* `[4, slide 2 "Abstract"]` |
| **Bối cảnh ghi nhận** | Hỏi "trong thời gian lập trình, bao nhiêu % dành cho: (1) sửa lỗi (fixing bugs), (2) làm cho code chạy (making code work), (3) thiết kế, (4) viết code". Hai mục đầu (25% + 25%) được gộp thành debugging `[4, slide 4, slide 5]` |
| **Hành vi / workaround thực tế** | Phần lớn công ty vẫn dùng debug "chạy xuôi" (forward debugging) vì thiếu công cụ chạy ngược phù hợp và thiếu nhận biết về RDB; GDB bị chậm và tốn bộ nhớ `[4, slide 2 "Introduction"]` |
| **Mất bao lâu, bao lần** | Debug chiếm 49.9% thời gian lập trình; còn 50.1% tổng thời gian làm việc dành cho việc không phải lập trình (admin, họp, sales...) `[4, slide 5]`. Báo cáo ước tính debug ≈ 1/4 tổng chi phí phát triển phần mềm ($312 tỷ / $1.25 nghìn tỷ) `[4, slide 4, slide 6]`. Với công cụ debug chạy ngược (RDB), tỷ lệ này được ước tính giảm từ 50% xuống 37% thời gian lập trình (18% fixing bugs + 19% reworking code), tức giảm 26% thời gian debug `[4, slide 7]` |
| **Giới hạn** | Phần tuyên bố miễn trừ ghi rõ đây là dự án giáo dục của sinh viên và không phải tư vấn chuyên môn `[4, slide 18 "Disclaimer"]`. Mục tiêu nêu trong tài liệu là hỗ trợ marketing cho sản phẩm RDB `[4, slide 2]`, và phụ lục A2 có dòng tính *"Potential value of Undo"* `[4, slide 15]`, cho thấy liên hệ với công cụ thương mại Undo. Dữ liệu khảo sát năm 2012, số mẫu nhỏ, đều là ước tính tự khai (mức giảm 26% là ước tính "Before/After RDBs" trong khảo sát, không phải đo thực nghiệm) `[4, slide 7]`. Chính bài [1] lưu ý các ước tính tự khai 20%–60% có thể bị phóng đại `[1, §2]` |
| **Insight** | Cùng bậc độ lớn với bài [1] (khoảng một nửa thời gian lập trình), nhưng độ tin cậy thấp hơn. Chỉ dùng như tín hiệu phụ. Con số 26% không nên dùng để hứa hẹn hiệu quả của giải pháp |

### Evidence Snapshot #4 — Thực nghiệm kỹ thuật: LLM đọc log (LogGPT) [2]

| Trường | Nội dung |
| :--- | :--- |
| **Loại bằng chứng** | Bài báo kỹ thuật và thực nghiệm đề xuất framework dùng ChatGPT (`gpt-3.5-turbo`, temperature = 0) phát hiện bất thường trong log trên 2 tập dữ liệu BGL và Spirit `[2, Abstract, §III, §IV-A, §IV-C]` |
| **Đối tượng** | Tập BGL (siêu máy tính Blue Gene/L, 4.74 triệu dòng log, 7.34% bất thường) và Spirit (cụm Linux production, 272.29 triệu dòng log, 63.47% bất thường); lấy mẫu ngẫu nhiên 2.000 dòng log liên tiếp từ tập test để đánh giá qua API `[2, §IV-A]` |
| **Phát hiện then chốt** | Tiền xử lý dùng parser Drain để tách log thành 3 dạng chuỗi theo cửa sổ thời gian (window size 10–50): *raw sequence*, *content sequence* (bỏ ID và Timestamp) và *event sequence* (bỏ thêm tham số biến thiên) `[2, §III-A, Fig. 2, Fig. 3]`. Prompt gồm *task description*, *format statement*, *human knowledge injection* (5 mẫu log trong chế độ few-shot); đầu ra ép về JSON với các khóa `is_anomaly`, `reports`, `preventive_measures` `[2, §III-B, §IV-C, Fig. 4]` |
| **Hành vi / Kết quả thực nghiệm** | 1) **Hiệu quả lọc nhiễu:** Chuỗi *content sequence* (đã lọc bỏ ID và Timestamp) đạt F1 cao nhất so với *raw sequence* và *event sequence* vì loại bỏ được thông tin nhiễu nhưng vẫn giữ được tham số ngữ nghĩa (ví dụ đạt F1 = 0.740 ở window size 30 và 0.694 ở window size 50 trên tập Spirit với Few-shot Prompt-2) `[2, §IV-D1, §IV-D2, Table I, Table II]` → **Ủng hộ trực tiếp Giả định #4**.<br>2) **Báo động giả & Hallucination:** Dù Recall rất cao (thường đạt 1.000), Precision và Specificity lại thấp (Precision trên BGL và Spirit ở Table II chỉ đạt 0.280–0.587; Specificity trên Spirit với zero-shot bằng 0.000) `[2, §IV-D3, §IV-D4, Table II]`. Tác giả chỉ rõ mô hình có **tỷ lệ báo động giả cao (high false positive rate)** do nhạy cảm với các cảnh báo cấp thấp trong log, và đôi khi sinh ra gợi ý vô ích hoặc gây nhầm lẫn do **hiện tượng bịa nội dung (hallucination)** `[2, §IV-D3, §IV-D5, §VI]` |
| **Giới hạn** | Nhiệm vụ của bài là **phát hiện bất thường trong cửa sổ log hệ thống** (siêu máy tính/Linux cluster) và giải thích cho quản trị viên hệ thống, không liên kết với mã nguồn để chỉ ra dòng code cần sửa cho lập trình viên backend `[2, §I, §IV-A, §IV-D5]`. Mô hình thử nghiệm là `gpt-3.5-turbo` với giới hạn output 100 tokens `[2, §IV-C]` |
| **Insight** | Cung cấp kiến trúc tiền xử lý (bỏ ID/Timestamp, giữ nội dung + tham số, ép đầu ra JSON) có bằng chứng thực nghiệm chứng minh hiệu quả hơn đưa log thô `[2, §IV-D1, §IV-D2]`. Đồng thời chứng minh rủi ro ở **Giả định #5 là có thật**: nếu chỉ đưa log mà không kiểm soát nhiễu cấp thấp hoặc không có ngữ cảnh code, LLM rất dễ báo động giả và bịa cách xử lý `[2, §IV-D3, §IV-D5, §VI]` |

### Evidence Snapshot #5 — Thực nghiệm LLM + stack trace + code từ repo [5]

| Trường | Nội dung |
| :--- | :--- |
| **Loại bằng chứng** | Nghiên cứu thực nghiệm (arXiv v1, 09/2025) so sánh báo cáo crash gốc với báo cáo được LLM bổ sung, kèm user study nhỏ; chưa thấy thông tin bình duyệt trong file `[5, tr.1]` |
| **Đối tượng** | 492 crash report có stack trace từ 8 hệ thống Java mã nguồn mở (ActiveMQ, Hadoop Common, HDFS, MapReduce, YARN, Hive, Storm, ZooKeeper); chỉ lấy lỗi đã sửa (Resolved/Fixed có commit), mức ưu tiên Major/Critical/Blocker, tạo từ 2010 `[5, §3.1, Table 1]`. User study: 16 người (7 sinh viên cao học, 9 lập trình viên; tất cả đều liệt kê Python là ngôn ngữ chính, trong đó 10/16 người cũng báo cáo dùng Java) `[5, §5-RQ3]` |
| **Câu nói của người tham gia (nguyên văn)** | *"The stack trace shows the location but not why it failed."* `[5, §5-RQ3]` (nhận xét về báo cáo crash gốc) |
| **Bối cảnh ghi nhận** | Hai cách bổ sung: `DIRECT-LLM` (một lượt, chỉ dùng báo cáo gốc + code của các hàm xuất hiện trong stack trace) và `AGENTIC-LLM` (tác tử duyệt thêm hàm gọi / được gọi qua call graph bằng GraphRAG) `[5, §4, §4.2]`. Cả hai dùng `gpt-4o-mini-2024-07-18`, temperature = 0; stack trace được trích bằng regex từ phần mô tả lỗi và dựng call graph tĩnh bằng thư viện `javalang` `[5, §4.1, §5]` |
| **Hành vi / workaround thực tế** | Báo cáo do dev viết thường thiếu thông tin chẩn đoán: chỉ 11.79% có bước tái hiện, 39.84% có giả thuyết nguyên nhân, 38.01% nêu thành phần/file ảnh hưởng, 20.93% có gợi ý sửa `[5, §3.2, Table 2]`. Báo cáo bổ sung dùng Meta-Reasoning Prompting (MRP) để xuất JSON gồm các trường: `Root Cause`, `Steps To Reproduce`, `Problem Location`, `Repair Suggestion`, `Possible Fix` `[5, §1, §4.2.1, Fig. 1, Fig. 4]` |
| **Kết quả chính** | Định vị đúng ít nhất một hàm được sửa (Problem Localization): **40.24%** (`DIRECT-LLM`) và **43.09%** (`AGENTIC-LLM`), so với **10.57%** (Top-1) của baseline BM25 dùng cả báo cáo gốc làm truy vấn (hai phương pháp LLM trùng nhau ở 169 ca, tức ≈85% kết quả của Direct và ≈80% của Agentic) `[5, §5-RQ1, Table 3]`. Độ tương đồng bản vá (CodeBLEU trên các ca định vị đúng): 56.51% (Direct) và 57.28% (Agentic) `[5, §5-RQ1, Table 4]`. Nguyên nhân gốc "đầy đủ" (đánh giá tay 100 ca): 30% báo cáo gốc, 46% Direct, 58% Agentic; nhưng theo LLM-as-a-Judge trên cả 492 ca chỉ đạt **34.35%** (Direct) và **35.16%** (Agentic) `[5, §5-RQ2, Table 5]`. Chi phí ≈ $0.005 (Direct) và $0.01 (Agentic) mỗi báo cáo `[5, §1, §5-RQ1]`. Trong user study (chỉ thử bản `AGENTIC-LLM`), người tham gia chấm mức hữu ích chung tăng từ 3.00 lên 4.59 (thang 5), trong đó gợi ý sửa lỗi tăng mạnh nhất từ 2.66 lên 4.53 `[5, §5-RQ3, Table 6]` |
| **Giới hạn** | Chỉ Java mã nguồn mở, lỗi đã sửa và ưu tiên cao; đầu vào là báo cáo Jira cùng mã nguồn đã checkout đúng phiên bản commit trước khi crash, không phải file log thô đang chạy `[5, §3.1, §4.1, §6]`. Tiêu chí "định vị đúng" là danh sách ứng viên có ít nhất một hàm trùng hàm được sửa; điểm CodeBLEU chỉ tính trên các ca đã định vị đúng `[5, §5-RQ1]`. Các tác giả ghi nhận tác tử đôi khi bịa (hallucinate) và bỏ sót hàm lỗi `[5, §5-RQ1]`. User study chỉ 16 người, mỗi người mất trung bình 20 phút/crash để phân tích 4 báo cáo, chỉ đo mức "hữu ích" cảm nhận theo thang Likert chứ **không đo thời gian tiết kiệm được hay tỷ lệ sửa đúng thực tế** `[5, §5-RQ3]` |
| **Insight** | Chỉ cần đưa code của các hàm trong stack trace vào LLM (`DIRECT-LLM`) đã đạt được phần lớn lợi ích định vị lỗi (40.24% so với 43.09% khi duyệt thêm call graph với chi phí gấp đôi) `[5, §5-RQ1, Table 3]`, nên hướng hybrid "script trích stack trace + code → AI" là hợp lý. Tuy nhiên, khoảng 57–60% ca vẫn chưa định vị đúng hàm cần sửa và nguyên nhân gốc đầy đủ chỉ đạt 34–58% `[5, Table 3, Table 5]`, nên kết quả AI **bắt buộc phải để dev duyệt**. Bài báo không chứng minh được việc giảm thời gian debug thực tế |

### Tổng hợp kết quả kiểm chứng

| Nguồn | Loại / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác / giới hạn | Độ tin cậy |
| :--- | :--- | :--- | :--- | :-: |
| **[1] Alaboudi & LaToza (2021)** | Quan sát hành vi, 11 dev, 15 phiên (30 giờ), 89 phiên debug | Debug ≈48% thời gian phiên `[§4.1]`; kiểm tra trạng thái bằng log statements 70% / breakpoints 30% `[§4.2, Table 5]`; 80% thời gian debug nằm ở 25/89 phiên (23 phiên dài trung bình 32 ± 23 phút); lỗi từ issue tracker mất 51 (±38) phút `[§4.1, §4.3]` | Lỗi tự gây ra lúc đang code chỉ mất trung bình 6 (±8) phút `[§4.1]`; không có một bước nào là nút thắt chính `[§4.3]`; phần lớn thời gian debug nằm ở việc sửa và chạy lại (54% ở phiên dài), không riêng đọc log `[§4.3, Fig. 7]` | Cao (quan sát hành vi), nhưng mẫu nhỏ |
| **[3] Stripe (2018)** | Khảo sát tự khai, >1.000 dev & >1.000 C-level `[tr.8]` | 17.3 giờ/tuần cho nhóm việc bảo trì/sửa lỗi; gần 2/3 dev (59%) thấy thời gian xử lý bad code là quá nhiều `[tr.3, tr.4, tr.5]` | Số liệu gộp cả nợ kỹ thuật (13.5h) và bad code/refactor (3.8h); nguyên nhân cản trở còn gồm hệ thống cũ (52%) và đổi ưu tiên (45%) `[tr.4, tr.5]` | Trung bình thấp |
| **[4] Britton et al. (Cambridge)** | Khảo sát + phỏng vấn, 54 phiếu + 11 phỏng vấn `[slide 5]` | Debug ≈ 49.9% thời gian lập trình `[slide 5]` | Dự án sinh viên MBA, mục tiêu hỗ trợ marketing RDB (Undo), dữ liệu 2012, chỉ Linux compiled code, tự khai `[slide 2, 3, 15, 18]` | Thấp |
| **[2] Qi et al. - LogGPT (2023)** | Thực nghiệm kỹ thuật trên tập log BGL & Spirit (mẫu test 2.000 dòng) `[§IV-A]` | Tiền xử lý bỏ ID/timestamp (*content sequence*) cho F1 cao nhất (đạt tới 0.740 trên Spirit) so với để log thô `[§IV-D1, §IV-D2, Table I]`; ép đầu ra JSON giúp giải thích được nguyên nhân và cách phòng tránh `[§III-B, §IV-D5]` | Bài giải bài toán phát hiện bất thường log hệ thống, không gắn với mã nguồn; **tỷ lệ báo động giả (false positive) cao** (Precision chỉ 0.28–0.58) do log cảnh báo cấp thấp và **có hiện tượng hallucination** sinh gợi ý vô ích `[§IV-D3, §IV-D5, §VI, Table II]` | Trung bình (có thực nghiệm định lượng nhưng khác bài toán code) |
| **[5] Fahim et al. (2025)** | Thực nghiệm 492 crash report Java + user study 16 người `[§3.1, §5-RQ3]` | Code của các hàm trong stack trace + LLM nâng tỷ lệ định vị đúng từ 10.57% lên 40.24–43.09% `[Table 3]`; người dùng chấm mức hữu ích tăng từ 3.00 → 4.59 `[Table 6]`; trích stack trace bằng regex và dựng call graph tĩnh được cho Java `[§4.1]` | Khoảng 57–60% ca vẫn không định vị đúng hàm sửa; nguyên nhân gốc đầy đủ chỉ 46–58% (chấm tay) / 34–35% (LLM-judge); tác tử đôi khi bịa `[§5-RQ1, Table 3, Table 5]`; chỉ Java mã nguồn mở, không đo thời gian tiết kiệm được `[§5-RQ3, §6]` | Trung bình khá (benchmark lớn, chưa bình duyệt; user study nhỏ) |

### Trạng thái từng giả định sau kiểm chứng

| # | Trạng thái | Căn cứ |
| :-: | :-: | :--- |
| 1 | Ủng hộ một phần | Debug tốn khoảng nửa thời gian lập trình và các phiên debug dài (≥12.3 phút) mất trung bình 32 (±23) phút, lỗi từ issue tracker mất 51 (±38) phút `[1, §4.1, §4.3]`; trong user study của `[5]`, người tham gia cũng mất trung bình 20 phút để phân tích 1 crash report `[5, §5-RQ3]`. Tuy nhiên lỗi tự gõ chỉ mất 6 (±8) phút `[1, §4.1]` và chưa có số liệu đo riêng cho actor dev backend gặp lỗi CSDL |
| 2 | Ủng hộ (có lưu ý) | 70% kiểm tra trạng thái bằng log statements so với 30% bằng breakpoints `[1, §4.2, Table 5]`, khớp với các nghiên cứu trước về mức dùng debugger thấp (0.87%–14%) `[1, §2]`; lưu ý "log" ở đây là lệnh log/print do dev đặt |
| 3 | Chỉ ủng hộ một phần | Không có bước nào là nút thắt đơn lẻ `[1, §4.3]`; ở phiên dài, việc kiểm tra trạng thái (18%) và duyệt file (17%) cộng lại khoảng 35% thời gian, trong khi sửa code (37%) và chạy thử (17%) chiếm 54% và dev phải chuyển qua lại liên tục giữa các hoạt động `[1, §4.3, Figure 7]` |
| 4 | Ủng hộ | `[2]` chứng minh thực nghiệm rằng dùng parser (Drain) lọc bỏ ID/timestamp (*content sequence*) giúp LLM đạt F1 cao hơn hẳn so với giữ nguyên log thô (*raw sequence*) `[2, §IV-D1, §IV-D2]`; `[5]` trích xuất thành công stack trace bằng regex và lấy thân hàm qua AST/call graph tĩnh trên 492 báo cáo Java `[5, §4.1]`. Dù vậy, vẫn cần kiểm tra thực tế với định dạng log CSDL của nhóm |
| 5 | Ủng hộ một phần, rủi ro cao | `[5]` cho thấy kết hợp stack trace + code giúp tăng gấp 4 lần độ chính xác định vị lỗi (lên 40.24–43.09%), nhưng vẫn sai ở 57–60% trường hợp, nguyên nhân gốc đầy đủ chỉ đạt 34–58% và agent đôi khi bịa `[5, §5-RQ1, Table 3, Table 5]`. `[2]` cũng chỉ ra LLM bị tỷ lệ báo động giả cao (Precision thấp) khi gặp log cảnh báo cấp thấp và có hiện tượng hallucination sinh lời khuyên vô ích `[2, §IV-D3, §IV-D5, §VI]` |
| 6 | Chưa kiểm thực tế | Chưa có nguồn khảo sát người dùng trực tiếp (chỉ mới có thông tin gián tiếp từ tài liệu Sentry Seer `[6]` rằng sản phẩm thương mại cam kết mặc định không dùng dữ liệu khách hàng để train model nhằm giải quyết rào cản này) |

### Nhóm đã sửa problem sau bước Kiểm chứng

1. **Thu hẹp phạm vi (Scope):** Dựa trên tín hiệu phản bác từ `[1]` (lỗi nhỏ vừa gõ chỉ mất khoảng 6 phút và sửa nhanh), nhóm **bỏ qua lỗi cú pháp và lỗi đơn giản**, chỉ tập trung vào **lỗi khó, phải truy qua nhiều file** (lỗi kết nối CSDL, lỗi logic liên tầng). Đây là nhóm phiên debug dài, nơi 80% thời gian debug tập trung `[1, §4.1, §4.3]`.
2. **Điều chỉnh bottleneck:** Bottleneck không chỉ là "đọc chữ trong file log" mà là **chuyển qua lại giữa kiểm tra trạng thái (log), duyệt các file code, sửa và chạy thử** `[1, §4.3, §7]`. Một người tham gia ở `[5]` nói gọn vấn đề: *"The stack trace shows the location but not why it failed"* `[5, §5-RQ3]`. Giải pháp nhắm vào việc gom log đã lọc nhiễu và code của các hàm liên quan vào một chỗ.
3. **Chọn mức độ phức tạp:** `[5]` cho thấy chỉ cần đưa code của các hàm trong stack trace (`DIRECT-LLM`) đã đạt độ chính xác định vị 40.24%, gần bằng 43.09% của cách duyệt thêm call graph (`AGENTIC-LLM`) với chi phí chỉ bằng một nửa ($0.005 so với $0.01) `[5, §5-RQ1, Table 3]`. Nhóm ưu tiên cách đơn giản trước.
4. **Kiểm soát rủi ro báo động giả & bịa nội dung:** Giả định #5 có rủi ro rõ ràng từ cả hai bài thực nghiệm: `[2]` ghi nhận tỷ lệ báo động giả cao do nhiễu log cấp thấp và hiện tượng hallucination `[2, §IV-D3, §VI]`, còn `[5]` ghi nhận 57–60% ca vẫn chưa định vị đúng hàm cần sửa và nguyên nhân gốc đầy đủ chỉ đạt 34–58% `[5, Table 3, Table 5]`. Đồng thời giả định #6 (được phép đưa code/log vào AI) **chưa được kiểm với người dùng**. Vì vậy giải pháp bắt buộc phải lọc nhiễu log trước, đính kèm đoạn code làm bằng chứng và có bước để dev duyệt, không để AI tự kết luận hay tự sửa.
5. **Định dạng đầu ra:** Dùng đầu ra có cấu trúc JSON/trường cố định gồm nguyên nhân gốc, vị trí lỗi, gợi ý sửa (kế thừa các trường của `[5, §4.2.1, Fig. 1]` và cấu trúc JSON của `[2, §III-B, Fig. 4]`), kèm đoạn code trích từ repo làm bằng chứng.

---

## Bước 3 — Research giải pháp đã có

### Sản phẩm đang dùng thật

| Công cụ / case | Link / Nguồn | Giải bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Sentry Seer (AI Debugging Agent)** | https://docs.sentry.io/product/ai-in-sentry/seer/ `[6]` | **Bước 3–5:** phân tích issue khi Sentry ghi nhận, kết hợp stack trace, thông tin lỗi, dữ liệu trace, log và mã nguồn từ repo GitHub/GitLab đã liên kết để tìm nguyên nhân gốc (Root Cause Analysis), gợi ý bản sửa và có thể tạo PR tự động hoặc chuyển tiếp cho coding agent bên ngoài `[6]` | Làm đúng chuỗi "stack trace + log + trace → code liên quan → nguyên nhân & bản vá"; tài liệu nêu rõ chính sách bảo mật (mặc định không dùng dữ liệu khách hàng để huấn luyện mô hình chung — giải quyết nỗi lo ở giả định #6) `[6]` | Là tính năng trả phí đi kèm hệ sinh thái giám sát của Sentry; yêu cầu lỗi phải được SDK đẩy lên Sentry và liên kết repo trên cloud (GitHub/GitLab); không nhắm vào việc đọc trực tiếp file log thô cục bộ trên máy dev lúc đang gõ code `[6]` | Với lỗi trên môi trường staging/production đã tích hợp Sentry thì đã có sản phẩm thương mại giải quyết trọn vẹn (cách tiếp cận tương đồng với hướng `AGENTIC-LLM` ở `[5]`). Khoảng trống của nhóm, nếu có, chỉ nằm ở lúc dev đang debug local với file log thô chưa qua Sentry, hoặc rào cản chi phí/tích hợp repo |
| **2. GitHub Copilot Chat (Prompt Engineering & Context)** | https://docs.github.com/en/copilot/concepts/prompting-and-context/prompt-engineering `[7]` | **Bước 4–5:** hỗ trợ giải thích lỗi và gợi ý sửa code ngay trong IDE khi lập trình viên cung cấp ngữ cảnh phù hợp (đoạn lỗi, các file code liên quan) và viết prompt có cấu trúc rõ ràng `[7]` | Tích hợp sẵn trong IDE phổ biến; cho phép dev chủ động đính kèm file/ngữ cảnh code và định hướng đầu ra qua kỹ thuật prompt engineering mà không cần xây hạ tầng AI mới `[7]` | Tài liệu nhấn mạnh chất lượng câu trả lời phụ thuộc lớn vào việc người dùng tự chọn lọc ngữ cảnh (context) và viết prompt cụ thể `[7]`; Copilot không tự động lọc nhiễu từ một file log hệ thống lớn hay tự trích xuất sẵn danh sách các hàm từ stack trace như pipeline của `[2]` và `[5]` — dev vẫn phải tự gom lỗi và trỏ các file liên quan | Một quy trình gồm "prompt chuẩn + stack trace đã lọc + code các hàm liên quan" đưa vào Copilot Chat có thể đã đủ giải quyết nhiều ca lỗi; cần thử nghiệm thực tế cách này trước khi quyết định viết công cụ riêng |

*Hai sản phẩm trên được đối chiếu qua tài liệu chính thức `[6, 7]`, nhóm cần chạy thử thực tế trên bài toán lỗi CSDL để đo mức độ đáp ứng.*

### Nghiên cứu / pattern

| Công cụ / case | Link / Nguồn | Giải bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **3. LogGPT** (Drain parser + ChatGPT) | https://arxiv.org/abs/2309.01189 `[2]` | **Bước 3:** dùng parser (Drain) tách log thành *raw / content / event sequence*, ghép vào prompt có cấu trúc (Task description, Format statement, Knowledge injection), ép đầu ra JSON `[2, §III-A, §III-B]` | Chứng minh thực nghiệm rằng *content sequence* (lọc bỏ ID, Timestamp) cho F1 tốt nhất `[2, §IV-D1, §IV-D2]`; đầu ra có giải thích nguyên nhân và biện pháp phòng tránh `[2, §IV-D5]` | Không gắn với mã nguồn, chỉ xét chuỗi log hệ thống rời rạc. **Tỷ lệ báo động giả cao** (Precision thấp) do nhạy cảm với cảnh báo cấp thấp và có hiện tượng **hallucination** sinh gợi ý vô ích `[2, §IV-D3, §IV-D5, §VI]` | **Mượn kiến trúc tiền xử lý:** lọc bỏ ID/Timestamp và log cấp thấp trước khi đưa vào AI, ép đầu ra JSON có cấu trúc. Bắt buộc phải bổ sung ngữ cảnh code thật để giảm đoán mò |
| **4. Reversible Debugger (RDB)** | [Reversible Debugging Software](https://www.researchgate.net/publication/345843594_Reversible_Debugging_Software_Quantify_the_time_and_cost_saved_using_reversible_debuggers) `[4]` | **Bước 3–5:** cho phép chạy ngược chương trình (backwards & forwards) để tìm nguyên nhân gốc `[4, slide 2]` | Báo cáo khảo sát ước tính giảm 26% thời gian debug (từ 50% xuống 37% thời gian lập trình) `[4, slide 7]` | Ít sản phẩm khả thi thương mại cho code phức tạp; GDB bị chậm và tốn bộ nhớ `[4, slide 2]`. Độ tin cậy của số liệu 26% thấp (khảo sát tự khai phục vụ marketing) `[4, slide 2, 7, 18]`. Dev thực tế vẫn dùng log statements 70% `[1, Table 5]` | Đừng bắt người dùng đổi sang công cụ nặng và trái thói quen; hãy bám vào thói quen đọc log và stack trace sẵn có |
| **5. Aggregator & summative debugging tools** | https://arxiv.org/abs/2105.02162 `[1, §7]` | **Bước 3–4:** tự dự đoán các file, tài nguyên và trạng thái chương trình dev cần kiểm tra rồi gom lại một chỗ để giảm chi phí chuyển đổi qua lại giữa các hoạt động `[1, §7]` | Nhắm đúng nguyên nhân khiến phiên debug kéo dài: dev phải chuyển qua lại liên tục giữa nhiều hoạt động và nhiều file `[1, §4.3, §7]` | Mới là hướng thiết kế được nhóm tác giả đề xuất ở phần thảo luận, chưa phải sản phẩm hoàn chỉnh `[1, §7]` | Định hướng thiết kế cốt lõi: tự động gom đoạn code của các hàm xuất hiện trong stack trace hiển thị cùng với log lỗi |

### Kết luận research

- Phần "stack trace → code liên quan → nguyên nhân" đã có sản phẩm thương mại (Sentry Seer cho lỗi đã đẩy lên hệ thống giám sát `[6]`; GitHub Copilot Chat ngay trong IDE nếu người dùng tự chuẩn bị ngữ cảnh và prompt tốt `[7]`) và có bằng chứng nghiên cứu rằng chỉ cần đưa code của các hàm trong stack trace vào LLM đã cải thiện gấp 4 lần khả năng định vị lỗi `[5, §5-RQ1, Table 3]`. **Không có cơ sở để huấn luyện mô hình mới hay xây dựng hệ thống multi-agent phức tạp.**
- Khoảng trống còn lại (suy luận, cần xác nhận bằng thử nghiệm và phỏng vấn): debug cục bộ (local) lúc đang viết code khi log chưa qua công cụ giám sát như Sentry, hoặc các dự án không muốn liên kết repo lên cloud / trả phí add-on `[6]`, trong khi việc tự lọc log, tìm các file trong stack trace và dán thủ công vào Copilot Chat vẫn tốn thao tác chuyển đổi ngữ cảnh `[1, §7; 7]`.
- **Hướng đề xuất (Hybrid nhẹ, tận dụng công cụ sẵn có):** Dùng script lọc nhiễu log (bỏ ID/timestamp theo kiểu *content sequence* của `[2, §III-A]`), trích xuất stack trace bằng regex và tự động lấy thân hàm của các hàm xuất hiện trong trace từ mã nguồn (kiểu `DIRECT-LLM` của `[5, §4.1, §4.2.1]`) → đóng gói thành một gói ngữ cảnh kèm prompt chuẩn (yêu cầu trả về cấu trúc gồm `Root Cause`, `Problem Location`, `Repair Suggestion`) để đưa vào trợ lý AI sẵn có trong IDE `[7]` → lập trình viên đối chiếu đoạn code bằng chứng và duyệt.
- **Điều kiện trước khi xây gì thêm:** Thử thực tế quy trình thủ công/script nhỏ này với 2–3 lỗi CSDL thật, so sánh trực tiếp với việc dán thẳng log thô vào Copilot Chat; chỉ xây dựng công cụ/extension riêng nếu khoảng trống ở trên thực sự giúp giảm thao tác rõ rệt.
- **Điểm khác biệt so với ý tưởng ban đầu:** Nhóm ban đầu định làm công cụ "đưa file log cho AI đọc để tìm dòng lỗi". Sau CP4, nhờ thấy rõ rủi ro báo động giả khi chỉ đọc log ở `[2, §VI]` và hiệu quả của việc ghép code từ stack trace ở `[5, Table 3]`, nhóm chuyển sang hướng **gom log đã lọc nhiễu và code của các hàm trong stack trace vào một chỗ** (kết hợp pattern Aggregator của `[1, §7]`, tiền xử lý *content sequence* của `[2, §III-A]`, và kiến trúc `DIRECT-LLM` của `[5, §4.2.1]`), có người duyệt, và chỉ tập trung vào các phiên debug lỗi khó liên tầng.

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

## 10. Danh mục tài liệu tham khảo

- **[1]** Abdulaziz Alaboudi and Thomas D. LaToza. 2021. *An Exploratory Study of Debugging Episodes*. https://arxiv.org/pdf/2105.02162.
- **[2]** Jiaxing Qi, Shaohan Huang, Zhongzhi Luan, Carol Fung, Hailong Yang, and Depei Qian. 2023. *LogGPT: Exploring ChatGPT for Log-Based Anomaly Detection*. https://arxiv.org/pdf/2309.01189.
- **[3]** Stripe (in partnership with Harris Poll). 2018. *The Developer Coefficient: Software engineering efficiency and its $3 trillion impact on global GDP*. Corporate Report (Sep 2018)
https://stripe.com/files/reports/the-developer-coefficient.pdf.
- **[4]** Tom Britton, Lisa Jeng, Graham Carver, Paul Cheak, and Tomer Katzenellenbogen. 2013. *Reversible Debugging Software: "Quantify the time and cost saved using reversible debuggers"*. Cambridge MBA Venture Project, University of Cambridge Judge Business School https://www.researchgate.net/publication/345843594_Reversible_Debugging_Software_Quantify_the_time_and_cost_saved_using_reversible_debuggers.
- **[5]** S M Farah Al Fahim, Md Nakhla Rafi, Zeyang Ma, Dong Jae Kim, and Tse-Hsun (Peter) Chen. 2025. *Crash Report Enhancement with Large Language Models: An Empirical Study*. https://arxiv.org/pdf/2509.13535.
- **[6]** Sentry Documentation. *Seer (AI Debugging Agent)*. https://docs.sentry.io/product/ai-in-sentry/seer/
- **[7]** GitHub Copilot Documentation. *Prompt engineering for GitHub Copilot Chat*. https://docs.github.com/en/copilot/concepts/prompting-and-context/prompt-engineering


