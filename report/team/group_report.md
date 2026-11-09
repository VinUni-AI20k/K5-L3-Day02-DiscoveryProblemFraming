# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: CodeX
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi tiếp nhận một dự án outsource/maintain cũ (hoặc onboard thành viên mới) mà tài liệu cài đặt đã lỗi thời, Developer và Techlead lãng phí 4–8 tiếng để gỡ lỗi crash do xung đột thư viện/version; nhóm hướng tới giải pháp chuẩn hóa môi trường bằng Docker (No-AI) kết hợp AI Workflow phân tích log lỗi build để giảm thời gian setup xuống dưới 30 phút.
- Quyết định cuối: *(Chưa quyết định — hoàn thiện ở CP6)*

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Tiến Cường | Khi tiếp nhận dự án outsource/maintain cũ mà docs outdate, tôi muốn có hướng dẫn cài đặt chuẩn, để đưa code lên chạy mà không tốn công người khác | Dev mới, Tester, Techlead | Crash do xung đột version thư viện/runtime; phải gọi Techlead debug (270') | Nếu dự án đã có sẵn Dockerfile thì bài toán này còn tồn tại không? (Thành viên 2 hỏi) |
| 2 | Nguyễn Tiến Cường | Khi Tester phát hiện lỗi mà máy Dev chạy bình thường, tôi muốn xác định nhanh khác biệt giữa 2 máy, để sửa bug không mất thời gian tranh cãi | Dev, Tester | So sánh thủ công cấu hình, version package và data test giữa 2 máy (60') | Tại sao Tester không test trên Staging có CI/CD mà test máy local? Nếu lệch do DB data/migration thì AI có vi phạm bảo mật không? (Thành viên 3 hỏi) |
| 3 | Nguyễn Tiến Cường | Khi API trên Swagger bị thiếu hoặc không chạy đúng spec, tôi muốn biết ngay người làm API, để xác nhận sửa mà không phải hỏi vòng qua nhiều cấp | Frontend Dev, Backend Dev, BA | Hỏi lòng vòng qua BA, Techlead, PM để tìm ra tác giả API (35') | Vấn đề này chỉ cần siết lại quy định ghi author/metadata vào Swagger là xong, tại sao cần làm phức tạp bằng AI? (Thành viên 4 hỏi) |
| 4 | Thành viên 2 | Khi vừa code xong bài tập lớn, muốn công cụ tự quét code sinh file README.md và tóm tắt hàm chính, để nộp bài đúng hạn không phải gõ lại | Sinh viên, Dev | Đọc lại code để nhớ luồng và tự gõ, căn chỉnh Markdown từ trang trắng (45–60') | Cả kỳ chỉ nộp 1-2 BTL thì tần suất có quá thấp? Thầy cô chấm điểm file Báo cáo Word/PDF và cần hướng dẫn cài đặt môi trường chứ AI đọc code sao biết nghiệp vụ thật? (Cường hỏi) |
| 5 | Thành viên 2 | Khi bạn cùng nhóm push code mới, muốn nhận tóm tắt "Ai vừa sửa gì, ảnh hưởng file nào của tôi", để lúc ghép bài không bị lỗi bất ngờ | Các thành viên làm cùng project | Tự dò hàng trăm dòng git diff không chú thích và chờ bạn trả lời tin nhắn giải thích (30–60') | Sập code trước giờ demo là do thiếu quy trình/test hay do không đọc git diff? AI tóm tắt văn bản có ngăn được runtime bug không hay chỉ cần No-AI họp sync 5 phút? (Cường hỏi) |
| 6 | Thành viên 2 | Khi đi xin thực tập/việc làm, muốn AI đọc trực tiếp đồ án trong máy để viết 3–4 gạch đầu dòng kinh nghiệm khớp với JD, để sửa CV nhanh | Người chuẩn bị CV xin việc | Lục lại code/báo cáo cũ tìm thư viện, số liệu thật và viết sang văn phong tuyển dụng khớp JD (30–45'/dự án) | Code đồ án sinh viên làm gì có số liệu impact kinh doanh thật? Đưa vào ChatGPT prompt 1 phút là xong, có cần tạo tool đọc cả folder code không? (Cường hỏi) |
| 7 | Thành viên 3 | Khi xe gặp sự cố giữa đường, muốn tìm gara/tiệm sửa xe lưu động gần nhất có thể hỗ trợ, để khắc phục nhanh không phải dắt xe đi xa | Người đi làm, tài xế công nghệ | Tìm kiếm và gọi điện liên hệ nhiều nơi để xác định thợ có sẵn sàng đến hỗ trợ lưu động không (15–30') | Đây là bài toán bản đồ/directory (No-AI), các tiệm sửa xe ven đường đa phần không dùng app, làm sao cập nhật trạng thái thợ thời gian thực? (Cường hỏi) |
| 8 | Thành viên 3 | Khi dùng máy tính/điện thoại lâu ngày, muốn hệ thống định kỳ kiểm tra, dọn rác, phát hiện mã độc và tối ưu tài nguyên để máy chạy ổn định | Nhân viên văn phòng, người dùng máy tính | Tự tra cứu Internet, mò mẫm Task Manager/ổ đĩa mà không biết chính xác nguyên nhân gây chậm (20–60') | Hệ điều hành đã có sẵn Task Manager, Storage Sense, Antivirus tự động. Can thiệp sâu vào tài nguyên hệ thống có nguy cơ crash OS và vi phạm bảo mật không? (Thành viên 2 hỏi) |
| 9 | Thành viên 3 | Khi xảy ra tai nạn giao thông xe chắn đường, muốn hệ thống hỗ trợ ghi nhận bằng chứng hiện trường, hồ sơ ban đầu và điều phối cứu hộ để giải phóng đường | CSGT, lực lượng cứu hộ, người tham gia giao thông | Ghi nhận bằng chứng, hoàn thiện hồ sơ và điều phối cứu hộ diễn ra tuần tự, rời rạc giữa các bên (30–60') | Bài toán phụ thuộc hoàn toàn vào thẩm quyền pháp lý của CSGT và bảo hiểm; làm sao nhóm sinh viên kiểm chứng và triển khai thực tế được trong lab? (Thành viên 4 hỏi) |
| 10 | Thành viên 4 | Khi làm việc nhóm, trưởng nhóm muốn theo dõi tiến độ công việc tập trung thay vì rải rác trên Zalo/Messenger/Drive để phát hiện trễ hạn kịp thời | Trưởng nhóm và thành viên | Phải hỏi từng người, chờ phản hồi và tự tổng hợp tiến độ thủ công (20–40') | Zalo/Messenger là app chat đóng, chặn API bên ngoài thì AI đọc tin nhắn thế nào? Thành viên không báo cáo là do thiếu kỷ luật chứ công cụ sao ép được? (Cường hỏi) |
| 11 | Thành viên 4 | Khi học nhiều môn trong kỳ, sinh viên muốn quản lý tập trung deadline từ LMS, email và chat nhóm để không bị quên hoặc nộp muộn bài tập | Sinh viên học nhiều môn | Phải kiểm tra nhiều nguồn rời rạc, tự nhớ và đối chiếu hạn nộp (15–30'/tuần) | Hệ thống LMS trường đóng kín không có open API; đầu kỳ nhập 10 phút vào Google Calendar (No-AI) là có chuông báo tự động, tại sao cần AI phức tạp? (Cường hỏi) |
| 12 | Thành viên 4 | Khi ôn tập hoặc làm bài, sinh viên muốn tìm kiếm nhanh tài liệu (slide, bài tập, giáo trình) nằm phân tán trên LMS, Drive, chat nhóm | Sinh viên | Phải lục tìm trên từng nền tảng, nhớ tên file hoặc phải chờ bạn bè gửi lại (15–20'/lần) | Nếu nhóm tạo 1 folder Google Drive chung (No-AI) từ đầu kỳ thì vấn đề có còn không? Đây là bài toán Search/Index truyền thống chứ AI can thiệp vào bước nào? (Thành viên 2 hỏi) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Môi trường & Triển khai phát triển phần mềm | #1, #2, #5 | Giải quyết các bất đồng, lỗi xung đột môi trường và mã nguồn giữa các máy/thành viên trong quy trình dev/test |
| B — Hỗ trợ tài liệu & Báo cáo học tập / nghề nghiệp | #3, #4, #6 | Trích xuất thông tin từ code/spec để sinh tài liệu (README, CV, API mapping) cho người khác đọc |
| C — Tiện ích đời sống, Thiết bị & Xã hội | #7, #8, #9 | Tìm kiếm, cứu hộ, tối ưu thiết bị và xử lý hiện trường sự cố vật lý ngoài đời thực |
| D — Quản lý học tập & Giao tiếp nhóm sinh viên | #10, #11, #12 | Theo dõi deadline, tiến độ và gom tài liệu học tập bị phân tán trên nhiều ứng dụng chat/LMS |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm 70% thời gian chết (downtime) và tắc nghẽn của kỹ sư/thành viên khi tiếp nhận và chuyển giao mã nguồn dự án
├── Opportunity A (Môi trường & Setup): Giảm thời gian cài đặt và gỡ lỗi xung đột dependency khi tiếp nhận dự án cũ hoặc onboard người mới
├── Opportunity B (Phối hợp Dev-Test): Rút ngắn thời gian xác định nguyên nhân sai lệch môi trường khi xảy ra lỗi "it works on my machine"
└── Opportunity C (Chuyển giao mã nguồn): Tự động nắm bắt các thay đổi cốt lõi trong code và tài liệu khi có thành viên mới hoặc push code mới
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "Chatbot AI tự động fix bug khi có exception" (Gợi ý viển vông, solution-first không khả thi)
- "Bot tự đọc tin nhắn Zalo/Messenger để nhắc việc" (Vi phạm chính sách API và rào cản nền tảng đóng)
- "App cứu hộ xe và xử lý hiện trường tai nạn" (Solution đội lốt, vượt quá phạm vi và quyền hạn kỹ thuật của lab CNTT)

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #1: Setup môi trường dự án cũ / onboard (Cường) | 5 | 5 | 5 | 5 | 4 | 5 | 5 | 34 |
| #5: Tóm tắt thay đổi code nhóm - git diff (Thành viên 2) | 4 | 4 | 4 | 4 | 4 | 3 | 4 | 27 |
| #10: Theo dõi tiến độ làm việc nhóm Zalo/Drive (Thành viên 4) | 4 | 3 | 3 | 3 | 2 | 3 | 4 | 22 |

**Candidate được chọn:**  
Candidate #1 — Setup môi trường dự án outsource/maintain cũ hoặc onboard thành viên mới (do Nguyễn Tiến Cường đề xuất).

**Vì sao chọn:**  
- Đạt điểm cao nhất trong bảng chấm điểm (34/35 điểm).
- Nỗi đau lớn nhất và đo lường được bằng số liệu thực tế (lãng phí 4–8 tiếng, bottleneck 270 phút của nhân sự mới và 1–2 tiếng của Techlead/Senior).
- Ranh giới giải pháp cực kỳ rành mạch: Nền tảng chuẩn hóa môi trường bằng **Docker (No-AI)**, AI chỉ can thiệp theo dạng **Workflow** để đọc và phân tích log lỗi xung đột thư viện/runtime khi build fail.
- Hoàn toàn nằm trong tầm kiểm soát kỹ thuật của nhóm (môi trường máy tính cục bộ/terminal), không vướng rào cản chính sách API đóng của bên thứ ba.

**Vì sao loại các candidate còn lại:**  
- Candidate #4, #6 (Sinh README, viết CV): Tần suất dùng quá thấp (1–2 lần/kỳ), giải quyết được bằng 1 câu prompt ChatGPT thông thường, thiếu tính cấp thiết kỹ thuật.
- Candidate #2, #5 (Lệch môi trường Dev-Test, Tóm tắt git diff): Phần lớn có thể giải quyết bằng quy trình No-AI (quy ước Git, commit message chuẩn, CI/CD runner), AI đọc text dễ sinh ảo giác và không ngăn được lỗi runtime.
- Candidate #7, #8, #9 (Cứu hộ xe, Bảo trì máy tính, Hiện trường tai nạn): Vượt quá thẩm quyền pháp lý (CSGT, bảo hiểm) hoặc không khả thi trong phạm vi lab CNTT.
- Candidate #10, #11, #12 (Theo dõi tiến độ Zalo, Deadline LMS, Tìm tài liệu): Vướng rào cản kỹ thuật đóng của LMS/Zalo/Messenger; bản chất là vấn đề kỷ luật cá nhân, đã có giải pháp No-AI miễn phí triệt để (Google Calendar, Drive, Notion).

**Xử lý bất đồng (nếu có):**  
Thành viên bảo vệ ý tưởng sinh viên (Candidate #4 và #10) ban đầu cho rằng đề tài sinh viên gần gũi hơn. Tuy nhiên sau khi cả nhóm phân tích các rào cản kỹ thuật (Zalo/LMS chặn API, rủi ro ảo giác của AI) và so sánh số liệu đo lường baseline, nhóm đã đồng thuận 100% chọn Candidate #1 vì đáp ứng chuẩn xác nhất các tiêu chí kỹ thuật và ranh giới AI của môn học.

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
