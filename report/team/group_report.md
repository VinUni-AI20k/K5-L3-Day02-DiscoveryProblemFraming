# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:D3
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi nhận được hóa đơn từ nhà cung cấp, nhân viên kế toán công nợ muốn đối chiếu thông tin với đơn đặt hàng (PO) và biên bản giao nhận, để đảm bảo tính chính xác trước khi thanh toán. Đối chiếu thông tin hóa đơn từ nhà cung cấp với đơn đặt hàng (PO) và biên bản giao nhận hàng (Kế toán công nợ - Candidate #8).
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 |Đào Ngọc Hân |Khi xe Xanh SM tiến vào bán kính đón khách nhưng bị khuất tầm nhìn (sảnh tòa nhà, phân khu đô thị, ngõ đông), tài xế và khách đặt xe muốn báo hiệu xe sắp cập điểm và nhận diện chính xác vị trí đứng thực tế của nhau mà không phải vừa lái xe vừa bấm gọi điện mô tả qua lại, để đón khớp ngay lần đầu và lái xe an toàn |Tài xế XanhSM và Khách hàng |**Bước 2 (1.0 phút)** và **Bước 3 (1.5–2.0 phút)** — tổng cộng **2.5–3.5 phút/cuốc**: tài xế vừa lái xe vừa phải bấm gọi thủ công (gây phân tâm), sau đó hai bên mất thời gian mô tả điểm mốc bằng lời do bất đồng góc nhìn trên đường| Quyến hỏi: về luật pháp, không cho phép sử dụng tai nghe khi lái xe? |
| 2 |Đào Ngọc Hân |Khi mở lại nhóm chat Zalo/Discord học tập hoặc dự án sau vài giờ bận, tôi muốn nắm ngay các quyết định đã chốt, deadline và phần việc giao cho mình giữa hàng trăm tin nhắn rời rạc, để không bỏ sót đầu việc chung hoặc phải hỏi lại cả nhóm |Học viên / thành viên nhóm dự án (tham gia đồng thời 3–4 nhóm chat hoạt động liên tục) |**Bước 3 (10 phút/lần/nhóm):** Phải đọc lướt và ghép ngữ cảnh từ luồng hội thoại phi cấu trúc vì câu chốt thường viết tắt (*"Chốt phương án 2 như bạn A nói ở trên nhé"*), buộc phải lội ngược tìm tin nhắn gốc |Rủi ro khi AI tóm tắt nhầm thông tin thời gian cuộc họp |
| 3 |Đào Ngọc Hân |Khi chi tiêu sinh hoạt hằng ngày qua nhiều tài khoản ngân hàng, quét mã QR và ví điện tử, tôi muốn gom các giao dịch lẻ về đúng danh mục chi tiêu vào cuối tuần, để biết mình đang vượt hạn mức ở nhóm nào trước khi hết tháng |Sinh viên / người đi làm trẻ thanh toán không tiền mặt qua 1–2 tài khoản ngân hàng chính và 1 ví điện tử |**Bước 2 (12 phút)** và **Bước 3 (8 phút)** — tổng **20 phút/tuần**: phải nhớ lại ngữ cảnh giao dịch chuyển khoản QR chỉ hiện tên chủ tài khoản cá nhân và nhập tay từng khoản lẻ | Vấn đề về cho phép truy cập thông tin của ngân hàng |
| 4 |Lê Thành Nguyên |Khi team đổi phiên bản prompt, tôi muốn biết bản mới tốt hơn hay tệ hơn bản cũ, để báo mentor có nên đưa lên bản chạy thật không |AI intern (người chấm); mentor dùng kết quả	 |Bước 3: đọc, đối chiếu nguồn, chấm 100 cặp câu trả lời, khoảng 90 phút/người/lần (cả quy trình khoảng 150 phút, 2 lần/tuần) | Nếu dùng LLM để kiểm tra thông tin kết quả của output của AI local của doanh nghiệp thì có thể rủi ro bảo mật |
| 5 |Lê Thành Nguyên |Khi mentor hỏi "cấu hình nào cho kết quả tốt nhất tuần trước", tôi muốn tìm lại đúng tham số và kết quả của từng lần chạy, để trả lời ngay mà không phải chạy lại |Tôi (người chạy thí nghiệm). Mentor là người hỏi và dùng kết quả |Bước 3, mở từng log để đọc tham số và metric rồi chép tay: khoảng 15 phút/lần (thêm 30–60 phút máy chạy nếu rơi vào bước 4) | Chưa rõ về hướng ứng dụng AI vào xử lý bài toán |
| 6 |Lê Thành Nguyên |Khi một intern mới vào nhóm, bạn ấy muốn tự cài được môi trường và chạy được project mẫu ngay trong ngày đầu, để không phải chờ người khác hỗ trợ  |Intern mới (người gặp khó). Tôi và mentor là người bị hỏi lại  |Bước 3–4, cài thư viện và gỡ lỗi xung đột phiên bản: 60–120 phút mỗi người, cộng 10–15 phút của người trả lời cho mỗi câu hỏi  |Có thể áp dụng chatbot vào để tăng hiệu quả làm việc được không |
| 7 |Nguyễn Thành Công |Khi nhận được nhiều CV cho một vị trí tuyển dụng, tôi muốn đánh giá mức độ phù hợp của từng ứng viên với yêu cầu công việc, để rút ngắn thời gian sàng lọc và không bỏ sót ứng viên tiềm năng. |Nhân viên tuyển dụng |Bước 2–3 – Đọc CV và đối chiếu với yêu cầu tuyển dụng, khoảng 3–5 phút/CV (ước tính).  |Trong thời đại ngày nay, ứng viên dùng AI để viết CV thì có hỗ trợ sàng lọc được hay không |
| 8 |Nguyễn Thành Công |Khi nhận được hóa đơn từ nhà cung cấp, tôi muốn đối chiếu thông tin với đơn đặt hàng và biên bản giao nhận, để đảm bảo tính chính xác trước khi thanh toán. |Nhân viên kế toán công nợ |Bước 4 – Đối chiếu thông tin giữa 3 loại chứng từ, khoảng 3–7 phút/hóa đơn (ước tính).  |Rủi ro về kinh tế khi thông tin và đối chiếu của AI sai lệch mà không được confirm lại |
| 9 |Nguyễn Thành Công |Khi tiếp nhận yêu cầu đổi trả, hoàn tiền hoặc tra cứu đơn hàng, tôi muốn xác định chính xác nội dung và mức độ ưu tiên của từng yêu cầu, để chuyển đến đúng bộ phận và xử lý kịp thời. |Nhân viên chăm sóc khách hàng |Bước 2–3 – Hiểu nội dung yêu cầu và tra cứu thông tin liên quan, ước tính 3–6 phút/ticket. | |
| 10 |Đồng Văn Quyến |Khi khách hàng gửi cùng một loại câu hỏi về đơn hàng/dịch vụ qua nhiều kênh, họ muốn được trả lời nhanh, chính xác và nhất quán, để không phải hỏi lại hoặc chờ lâu |Người phụ trách ghi biên bản, team member |Bước 3–4: viết lại và tách việc mất khoảng 20 phút/buổi, dễ ghi nhầm người phụ trách hoặc thiếu hạn chót |  |
| 11 |Đồng Văn Quyến |Khi nhận bàn giao ca trực, cần nắm đầy đủ diễn biến sức khỏe, thuốc đã dùng, chỉ định đang thực hiện, kết quả đang chờ và việc còn tồn của từng bệnh nhân, để chăm sóc tiếp chính xác và không bỏ sót việc của ca trước |điều dưỡng, bác sĩ |Bước 3: đọc và đối chiếu hồ sơ, y lệnh, kết quả đang chờ từ nhiều nguồn, khoảng 15–20 phút; hay sót kết quả đang chờ và thay đổi thuốc | Việc thao tác với thông tin của bệnh nhân và hệ thống quản lý bệnh viện có khả thi không |
| 12 |Đồng Văn Quyến |Khi vừa họp team xong, tôi muốn có bản tóm tắt các vấn đề đã bàn, cách giải quyết, việc cần làm, người phụ trách và hạn chót, để không ai bỏ sót việc |Người phụ trách ghi biên bản, team member  |Bước 3–4: viết lại và tách việc mất khoảng 20 phút/buổi, dễ ghi nhầm người phụ trách hoặc thiếu hạn chót |Khả năng cạnh tranh thị trường với các hệ sinh thái lớn rất khó?|

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
| #1 Khớp điểm đón Xanh SM | 4 | 3 | 3 | 3 | 2 | 2 | 4 | 21 |
| #2 Tóm tắt chat Zalo/Discord | 4 | 4 | 4 | 3 | 5 | 4 | 4 | 28 |
| #3 Gom sao kê ngân hàng/ví | 4 | 4 | 3 | 3 | 3 | 3 | 4 | 24 |
| #4 Đánh giá cặp câu prompt AI | 4 | 4 | 4 | 4 | 4 | 4 | 3 | 27 |
| #5 Truy vết tham số thí nghiệm | 4 | 3 | 3 | 3 | 4 | 4 | 3 | 24 |
| #6 Hỗ trợ intern cài môi trường | 4 | 3 | 3 | 3 | 4 | 3 | 4 | 24 |
| #7 Sàng lọc CV ứng viên | 5 | 4 | 4 | 4 | 4 | 4 | 3 | 28 |
| #8 Đối chiếu hóa đơn - PO - Giao nhận (Chọn) | 5 | 5 | 4 | 5 | 5 | 5 | 4 | 3 |
| #9 Phân loại ticket đổi trả CSKH | 4 | 4 | 3 | 3 | 4 | 4 | 3 | 25 |
| #10 Trả lời câu hỏi trùng CSKH | 4 | 4 | 4 | 4 | 4 | 4 | 3 | 27 |
| #11 Bàn giao ca trực bệnh viện | 4 | 4 | 5 | 4 | 2 | 4 | 2 | 25 |
| #12 Biên bản & việc sau họp team | 5 | 4 | 4 | 4 | 5 | 4 | 4 | 30 |

**Candidate được chọn:**
Candidate #8: Đối chiếu thông tin hóa đơn từ nhà cung cấp với đơn đặt hàng (PO) và biên bản giao nhận hàng (Nguyễn Thành Công).

**Vì sao chọn:**
1. **Actor và quy trình cực kỳ chuẩn xác và rõ ràng (5/5):** Kế toán công nợ thực hiện 3-way matching theo bộ 3 chứng từ cố định (Hóa đơn - PO - Phiếu giao nhận).
2. **Impact đo lường được ngay bằng thời gian và tiền bạc (5/5):** Mỗi hóa đơn mất 3–7 phút đối chiếu thủ công; rủi ro trả thừa tiền hoặc chậm thanh toán phạt vi phạm hợp đồng có tác động tài chính trực tiếp và rõ ràng.
3. **Cực kỳ vừa sức trong khuôn khổ bài lab (5/5):** Dữ liệu dạng chứng từ, file PDF/ảnh scan/bảng tính hoàn toàn giả lập hoặc thu thập mẫu thực tế được mà không vi phạm bảo mật nhạy cảm.
4. **Thể hiện trọn vẹn sự so sánh 4 mức độ can thiệp AI (5/5):**
   - *No AI:* Bảng checklist và mẫu form cứng đối chiếu bằng mắt.
   - *Rule:* Viết script/macro đối chiếu trực tiếp các trường số liệu khi dữ liệu đã ở dạng bảng Excel/CSV.
   - *Workflow:* OCR trích xuất trường dữ liệu từ PDF/ảnh hóa đơn -> Rule so khớp số lượng/đơn giá -> AI tóm tắt giải trình điểm lệch -> Kế toán kiểm tra xác nhận duyệt chi.
   - *Agent:* Tự động quét email lấy hóa đơn, tự vào kho lấy phiếu giao hàng, tự quyết định chi tiền (Rủi ro rất cao về tài chính nếu thiếu người duyệt).

**Vì sao loại các candidate còn lại:**
- **#1 (Khớp điểm đón Xanh SM):** Thuộc bài toán GPS/thời gian thực/an toàn giao thông ngoài thực địa, không thể làm và test trong bài lab, khó can thiệp bằng mô hình ngôn ngữ thông thường.
- **#3 (Gom sao kê ví/ngân hàng) & #11 (Bàn giao ca trực bệnh viện):** Vướng rào cản rất lớn về chính sách bảo mật dữ liệu nhạy cảm (tài chính cá nhân, hồ sơ bệnh án). Nhóm thiếu domain sâu về lâm sàng và không có quyền truy cập hệ thống bệnh viện thật.
- **#5, #6:** Mang tính đặc thù cá nhân trong phòng lab/nội bộ team lập trình, quy trình phụ thuộc nhiều vào từng hệ thống máy, khó chuẩn hóa và impact không đủ lớn.
- **#2, #12 (Tóm tắt chat / họp team):** Mặc dù điểm số cao (28-30) và vừa sức, nhưng thị trường đã có quá nhiều giải pháp sẵn có (Zoom AI, Teams recap, Slack AI), khó tạo ra sự khác biệt và ranh giới đo lường "thế nào là tóm tắt tốt" mang tính chủ quan.
- **#7 (Sàng lọc CV) & #9, #10 (CSKH):** Sàng lọc CV tiềm ẩn thiên kiến đạo đức (bias) và khó có ground-truth chuẩn để đánh giá "độ phù hợp", trong khi đối chiếu hóa đơn có ground-truth 100% rõ ràng (khớp số tiền, khớp mã hàng, khớp số lượng).

**Xử lý bất đồng (nếu có):**
- Ban đầu một số thành viên đề xuất chọn **#12 (Biên bản họp)** vì bản thân ai cũng gặp hằng tuần, và **#11 (Bàn giao ca trực)** vì có impact an toàn con người rất lớn.
- Sau khi thảo luận phản biện, nhóm thống nhất:
  - #11 có rủi ro quá lớn về tính khả thi và bảo mật (Feasibility & Viability).
  - #12 khó xác định tiêu chí đúng/sai tuyệt đối (chất lượng biên bản phụ thuộc cảm tính).
  - #8 (Đối chiếu hóa đơn) đạt điểm đồng thuận cao nhất vì có tính khách quan (số liệu khớp hoặc không khớp), bài toán tài chính rõ ràng và làm rõ nét vai trò của người kiểm duyệt (Human-in-the-loop). Nhóm nhất trí chọn **#8** làm bài toán chung để đi tiếp vào CP4.

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
| **AWS Textract (AnalyzeExpense) + Serverless Matching** | [AWS Textract Expense](https://aws.amazon.com/textract/) · [Sample Architecture](https://github.com/aws-samples/amazon-textract-invoice-processor) | Bước 2 (Trích xuất) & Bước 3 (Đối chiếu số liệu) | Trích xuất trường chuyên sâu (Line items, Vendor, PO, Total) theo chuẩn OCR tài chính; có kiến trúc mẫu kết nối ERP/Database | Chi phí tính theo lượt gọi API; không tự giải quyết được các bất đồng ngữ cảnh phi cấu trúc (ví dụ: tên hàng viết tắt khác nhau) | Dùng OCR/IDP chuyên dụng để lấy số liệu có cấu trúc, nhưng phần đối chiếu cần rule chặt chẽ và chấp nhận ngưỡng dung sai (tolerance). |
| **MISA meInvoice (Xử lý hóa đơn đầu vào & AI MISA AVA)** | [MISA meInvoice](https://meinvoice.vn/) | Bước 1, Bước 2 & kiểm tra tính hợp lệ cơ quan thuế | Tự động đồng bộ với Tổng cục Thuế, kiểm tra hóa đơn hủy/thay thế, tự động hạch toán vào AMIS/ERP nội địa | Chủ yếu tập trung vào đối soát thuế và hạch toán kế toán, chưa tối ưu sâu khâu 3-way matching phức tạp với biên bản giao nhận kho lẻ | Nghiệp vụ thuế và tính hợp pháp của hóa đơn có thể giải quyết bằng hệ thống sẵn có; nhóm nên tập trung vào điểm nghẽn **đối chiếu số lượng/đơn giá thực tế với PO và kho**. |
| **Rossum.ai (IDP & Accounts Payable)** | [Rossum AP Solution](https://rossum.ai/solutions/accounts-payable/) | **Bước 2** (OCR/IDP), **Bước 3** (Line-item Matching) & **Bước 4** (Exception Handling) | Công nghệ trích xuất không phụ thuộc template (Rossum Aurora); so khớp từng dòng hàng (line-item) giữa Hóa đơn và PO; giao diện làm nổi bật điểm lệch. | Cần cấu hình ngưỡng dung sai (tolerance) phức tạp; rủi ro nhận diện sai nếu nhà cung cấp gộp nhiều mã hàng thành một dòng. | Tách bạch rõ 2 bước: Dùng AI đọc hiểu bố cục phi cấu trúc thành JSON, sau đó áp dụng **Rule kiểm tra số học và mã hàng**, không để AI tự quyết toán tiền. |


**Kết luận research:**
```text
Thị trường đã có rất nhiều giải pháp từ mức Enterprise (akaBot, SAP) đến Low-code/Open-source (n8n, AWS Textract).
Vì vậy, nhóm KHÔNG TỰ XÂY dựng công cụ trích xuất hay chatbot từ con số không.
Hướng giải pháp hợp lý nhất: 
Kiến trúc Workflow: OCR trích xuất -> Rule so khớp 3 bên (Hóa đơn vs PO vs Phiếu kho) -> AI phân tích lý do lệch (nếu có) -> Kế toán viên kiểm duyệt và bấm xác nhận chi.
```

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
