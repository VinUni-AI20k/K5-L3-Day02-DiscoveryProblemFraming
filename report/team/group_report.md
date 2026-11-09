# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: C204T1
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): CEO khó theo dõi quyết định, cam kết và việc còn treo trong hơn 10 nhóm Zalo, mất thời gian đọc lại và dễ sót việc.
- Quyết định cuối: Not Yet — đề xuất chờ nhóm xác nhận.

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

|   # | Người đưa ra    | Candidate (Job Story ngắn)                                                                                                                                                                                                      | Actor                                                           | Bottleneck                                                                                                                                                                                                                | Câu hỏi phản biện nhận được (ai hỏi)                                                                                                                                                                                                                                               |
| --: | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|   1 | Đặng Việt Anh   | **Khi** đọc lại các nhóm Zalo sau một tuần (khách, NCC, nội bộ), **tôi muốn** có bản tóm tắt các quyết định, cam kết và việc còn treo, **để** không bỏ sót việc quan trọng bị chìm trong hàng trăm tin nhắn.                    | CEO và nhân viên                                                | Phải đọc tin nhắn thường xuyên, đọc lướt và lọc thông tin quan trọng                                                                                                                                                      | Chuẩn đầu vào và đầu ra nhiều, và bị loạn \|                                                                                                                                                                                                                                       |
|   2 | Đặng Việt Anh   | Khi** lên kế hoạch tuần tới, **tôi muốn** thấy lịch hàng về và các khoản phải thu/phải trả đến hạn, **để** chuẩn bị tiền đúng lúc để lấy hàng hoặc xuất hàng ra khỏi kho.                                                       | CEO và kế toán                                                  | Tra và ghép dữ liệu từ 3 nguồn, khoảng 60 phút/lần                                                                                                                                                                        | Chưa có                                                                                                                                                                                                                                                                            |
|   3 | Đặng Việt Anh   | **Khi** sáng thứ Hai bắt đầu tuần mới, **tôi muốn** có sẵn một báo cáo kinh doanh tuần trước (doanh thu, số đơn, khách mới, đơn đang treo) gom từ các sheet, **để** khỏi copy-paste thủ công và họp đầu tuần đúng giờ.          | CEO và nhân viên                                                | Lọc, copy-paste và tính toán, khoảng 60 phút/tuần                                                                                                                                                                         | Chưa có                                                                                                                                                                                                                                                                            |
|   4 | Trần Minh Nhật  | Khi nhắn tin mua bán, mỗi khách hàng sẽ có yêu cầu khác nhau và nội dung nhắn tin khác nhau, tôi cần tổng hợp các yêu cầu đặt hàng/chăm sóc khách hàng,... theo mức độ ưu tiên cần xử lý.                                       | Chủ shop hoặc nhân viên nhận đơn hoa/quà tặng làm theo yêu cầu. | 1. Nhân viên thay ca không nắm được các công việc, tin nhắn cần xử lý của ca trước.<br>2. Một ngày có thể có hàng trăm tin nhắn của khách hàng nhân viên không có thời gian để sắp xếp các tin nhắn cần xử lý theo thứ tự | Chưa có                                                                                                                                                                                                                                                                            |
|   5 | Trần Minh Nhật  | Khi cân nhắc một vị trí tuyển dụng, tôi muốn biết đối với công việc đó hồ sơ ứng tuyển đã đáp ứng và còn thiếu gì, để quyết định ứng tuyển và chuẩn bị phù hợp. Các công việc phù hợp lại được đăng ở nhiều nền tảng khác nhau. | Sinh viên đang tìm vị trí thực tập                              | 1. Tự đối chiều hồ sơ thủ công<br>2. Phải rà soát nhiều nền tảng ứng dụng khác nhau để ứng tuyển cho vị trí mong muốn                                                                                                     | Chưa có                                                                                                                                                                                                                                                                            |
|   6 | Trần Minh Nhật  | Khi nhận lịch hẹn, tôi phải quản lý nhiều lịch cùng một lúc và nhiều khi sắp trùng lịch của khách hàng                                                                                                                          | Chủ hoặc lễ tân salon/spa/studio có nhiều nhân viên             | 1. Ghi nhận lịch hẹn của khách hàng trên sheet<br>2. Mỗi lần khách đặt lịch tôi mở sheet ra để xem khung giờ đó đã có khách đặt hay chưa                                                                                  | Chưa có                                                                                                                                                                                                                                                                            |
|   7 | Hoàng Hải Nam   | Khi đã tái hiện được bug, tôi muốn khoanh vùng nhanh dòng lỗi trong file log hệ thống và đối chiếu với dữ liệu đầu vào của Tester, để tìm ra nguyên nhân gốc thay vì mò từng dòng log                                           | Developer                                                       | Đọc dò hàng trăm dòng log hệ thống (15') và đối chiếu thủ công với dữ liệu của Tester + code (10')                                                                                                                        | Hiện tại đã có 1 số nền tảng như firebase, ... đã có các service tracing log, chỉ hướng sửa, tái hiện lại được quy trình người dùng thực hiện thao tác trên production như thế nào với chi phí rất rẻ. Vậy thì ý tưởng này có khả thi để tiếp tục thực hiện không? (Đặng Việt Anh) |
|   8 | Hoàng Hải Nam   | Khi vừa hoàn thành logic của một task, tôi muốn chuẩn bị nhanh mock data và các kịch bản kiểm thử biên, để viết xong unit test trước khi đẩy PR cho Tech Lead                                                                   | Developer                                                       | Tự gõ thủ công bộ mock data khớp cấu trúc model (15') và viết code unit test cho các kịch bản biên (10')                                                                                                                  | Chưa có                                                                                                                                                                                                                                                                            |
|   9 | Hoàng Hải Nam   | Khi đến cuối ngày làm việc, tôi muốn nắm được danh sách các commit, PR và tiến độ phần việc đã làm trong ngày, để gửi báo cáo cuối ngày cho Tech Lead                                                                           | Developer, Tech Lead                                            | Mở 3 nơi (Git, PR, Jira) và tự nhớ lại tiến độ hôm nay + việc ngày mai để viết báo cáo (7–9')                                                                                                                             | Chưa có                                                                                                                                                                                                                                                                            |
|  10 | Phạm Thanh Tùng | Khi Phải kiểm tra deadline từ LMS, nhóm chat và file đề bài, tôi muốn có hệ thông tạo checklist các công việc , để không bỏ sót việc quan trọng                                                                                 | sinh viên , nhân viên                                           | Phải vào rất nhiều website để kiểm tra các công việc                                                                                                                                                                      | Xác định cách công việc chính xác của người đó                                                                                                                                                                                                                                     |
|  11 | Phạm Thanh Tùng | Khi làm bài nhóm nhưng cập nhật tiến độ nằm rải rác trong chat, tôi muốn Tổng hợp ai đã làm gì, phần nào còn thiếu trước deadline , để không bỏ sót việc quan trọng .                                                           | Thành viên                                                      | Phải rà xoát lại nhiều tin nhắn                                                                                                                                                                                           | Không có                                                                                                                                                                                                                                                                           |
|  12 | Phạm Thanh Tùng | Khi chia đầu việc khi nhóm mới nhận đề bài, tôi biến yêu cầu dài thành các đầu việc cụ thể và phân công cân bằng, để phân công 1 cách công bằng các công việc.                                                                  | Nhóm                                                            | Phải cần sự cân bằng giữa các công việc thời lượng , khả năng                                                                                                                                                             | Không có                                                                                                                                                                                                                                                                           |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung                                                   |
| ------- | ------------- | --------------------------------------------------------------- |
| A       | 1 và 4        | tổng hợp tin nhắn, các công việc cần xử lý để đưa ra quyết định |
| B       |               |                                                                 |
| C       |               |                                                                 |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian CEO đọc lại Zalo và số cam kết bị bỏ sót.
├── Opportunity A: Quyết định quan trọng bị chìm trong nhiều nhóm.
├── Opportunity B: Khó theo dõi ai làm gì và hạn hoàn thành.
└── Opportunity C: Câu hỏi, việc còn chờ chưa được theo dõi đến khi xong.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- Ý 5, 7

### 2.4. Chấm điểm shortlist (1–5)

| Candidate                      | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| ------------------------------ | -------: | -----------: | -----------------: | -------------: | ----------: | -------------------------------------: | ---------------: | ---: |
| #1 — Tổng hợp nhóm Zalo        |        5 |            5 |                  1 |              5 |           5 |                                      4 |                2 |   27 |
| #2 — Lịch hàng về và dòng tiền |        5 |            4 |                  1 |              4 |           3 |                                      4 |                2 |   23 |
| #3 — Báo cáo kinh doanh tuần   |        5 |            4 |                  1 |              4 |           2 |                                      5 |                2 |   23 |

Điểm đề xuất, chưa phải điểm nhóm thống nhất. Pain chấm 1 vì chưa có bằng chứng cụ thể; hiểu domain chấm 2 vì chưa được xác nhận. #3 dễ làm và đo nên tổng cao hơn. Nhóm vẫn chọn #1 để kiểm chứng cơ hội giảm công đọc và sót cam kết; khả năng lấy tin Zalo còn chưa rõ.

**Candidate được chọn:** #1

**Vì sao chọn:** đây là vấn đề tốn thời gian nhất

**Vì sao loại các candidate còn lại:** các giải pháp còn lại đã có giải pháp hoặc mức độ chấp nhận sử dụng chưa cao

**Xử lý bất đồng (nếu có):** Không có

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Lấy được tin nhắn nhóm hiện tại một cách hợp lệ. | Feasibility | 5 | 1 | Đầu tiên: thử 1 nhóm thật. |
| 2 | CEO mất nhiều thời gian đọc lại và từng sót cam kết. | Value | 5 | 1 | Bấm giờ và xem sự cố cụ thể. |
| 3 | AI bắt được ≥85% việc quan trọng, ý sai/bịa ≤5%. | Feasibility | 5 | 1 | So với chat được đánh dấu tay. |
| 4 | CEO dùng bản tóm tắt thay vì đọc lại mọi nhóm. | Usability | 4 | 1 | Quan sát khi thử bản mẫu. |
| 5 | Doanh nghiệp đồng ý phạm vi dữ liệu và dịch vụ AI. | Viability | 5 | 1 | Trước khi xử lý chat thật. |
| 6 | AI tiết kiệm tổng công hơn tóm tắt theo mẫu. | Viability | 4 | 1 | So sánh cả công rà soát và chi phí. |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này: ưu tiên #1, #5, sau đó #2, #3; chưa có kết quả được cung cấp.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường                                            | Nội dung                                                                                                                                            |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| Người được hỏi (vai trò, không ghi tên thật)      | Người đã đi làm                                                                                                                                     |
| Câu nói đáng nhớ nhất (nguyên văn)                | Sếp tôi cũng kêu làm như thế                                                                                                                        |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Cách đây vài tháng                                                                                                                                  |
| Hiện đang xử lý bằng cách nào (workaround)?       | Không có cách xử lý                                                                                                                                 |
| Mất bao lâu, bao lần?                             | Mỗi lần                                                                                                                                             |
| Insight / opportunity rút ra                      | Insigh rút ra những công cụ giúp tổng hợp báo cáo vô cùng tiện lợi, có thể giảm thời gian cho báo cáo và tập trung cho các công việc quan trọng hơn |

Tổng hợp:

| Nguồn   | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
| ------- | ----------------: | ----------------- | ----------------- |
| Tại lớp |                 2 | Tích cực          | Không có          |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Không sửa

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Slack AI | [Slack Help](https://slack.com/help/articles/25076892548883-Guide-to-AI-features-in-Slack) | Tóm tắt và recap hằng ngày. | Xem được nguồn. | Chỉ dùng trên Slack. | Bản ngắn, kiểm tra được nguồn. |
| Zalo OA / GMF | [Zalo OA](https://oa.zalo.me/home/documents/vie/guides/quan-ly-nhom-gmf_1954166378348758227) | Quản lý nhóm do OA tạo. | Có hướng tích hợp chính thức. | Chưa rõ lấy được lịch sử nhóm hiện tại. | Thử đầu vào trước khi xây. |
| n8n Information Extractor | [n8n Docs](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.information-extractor/) | Trích thông tin từ text. | Định sẵn trường cần lấy. | Không bảo đảm nội dung đúng. | Thử Workflow nhỏ, có người kiểm tra. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
[Mở nhóm] → [Tìm tin chưa đọc]
→ [Đọc, lọc quyết định / cam kết / việc treo] ← BƯỚC NGHẼN
→ [Ghi chú hoặc ghi nhớ] → [Hỏi lại, giao việc / trả lời]
Đọc và lọc: khoảng 120 phút/ngày (ước lượng, chưa đo).
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | CEO | Danh sách nhóm | Nhóm cần đọc | Hằng ngày, chưa đo riêng | Khách, NCC, forwarder, nội bộ. |
| 2 | CEO | Tin chưa đọc | Ngữ cảnh cần xem | Hằng ngày, chưa đo riêng | Tìm lại tin cũ. |
| 3 | CEO | Hội thoại | Quyết định, cam kết, việc treo | Bước 2–3 khoảng 120 phút/ngày, chưa đo | Bước nghẽn dự kiến. |
| 4 | CEO | Ý quan trọng | Ghi chú hoặc ghi nhớ | Hằng ngày, chưa đo | Chưa có danh sách chung. |
| 5 | CEO, nhân viên | Ghi chú và chỗ chưa rõ | Xác nhận, giao việc hoặc trả lời | Khi phát sinh, chưa đo | Chuyển người phụ trách. |

**Bottleneck chính:** tìm và lọc tin quan trọng giữa nhiều nhóm; 120 phút/ngày là ước lượng cần đo lại.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
[RULE: Gom text từ 3 nhóm được phép, giữ nguồn, kiểm tra thiếu tin]
→ [AI: Trích quyết định, cam kết (ai–việc–hạn), câu hỏi còn chờ]
→ [CON NGƯỜI: Kiểm tra bản nháp trước khi gửi trong tuần đầu]
→ [RULE: Gửi một bản nội bộ lúc 7h, nếu kênh cho phép]
→ [CEO: Đọc, xem nguồn, tự quyết định giao việc / trả lời]
→ [CON NGƯỜI + RULE: Xác nhận cam kết, cập nhật và nhắc hạn]

Boundary: Không tự nhắn khách/NCC, giao việc, duyệt chi hay đoán hạn.
Báo rõ nguồn thiếu, ảnh/voice chưa xử lý để người xem lại.
Quay về: kết nối hoặc AI lỗi → nhân viên tóm tắt theo mẫu.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 6 | Theo hai sơ đồ nháp. |
| Tổng thời gian | CEO đọc/lọc khoảng 120 phút/ngày, chưa đo | CEO đọc/kiểm tra ≤20 phút/ngày | So cùng nhóm; đo thêm công nhân viên và rà soát. |
| Số bước thủ công | 5 | 3 bước có người tham gia | Bước 3, 5, 6; chưa tính nhập dữ liệu nếu cần. |
| Bottleneck chính | Đọc và lọc tin | Kiểm tra bản nháp | Cần đo công kiểm tra. |
| Rủi ro mới phát sinh | Sót tin khi đọc tay | AI bịa/sót, thiếu đầu vào, lộ dữ liệu | Có nguồn và phương án thủ công. |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | CEO công ty XNK máy móc khoảng 5 người. |
| **Quy trình** | Đọc các nhóm, ghi chú, hỏi lại rồi giao việc hoặc trả lời. |
| **Bottleneck** | Tìm, lọc quyết định và cam kết trong hơn 10 nhóm; khoảng 120 phút/ngày, chưa đo. |
| **Impact** | Mất thời gian quản lý, dễ quên cam kết và phản hồi chậm. |
| **Success Metric** (baseline → target, cách đo) | 120 phút/ngày (ước lượng) → ≤20 phút/ngày; sự cố sót việc giảm ≥80%. Đo baseline 2 tuần và pilot 2 tuần trên cùng nhóm; chưa có số sự cố gốc. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | CEO giữ quyền quyết định; người phụ trách kiểm tra thông tin thiếu/mâu thuẫn. Không tự liên hệ khách/NCC hay duyệt chi. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- Theo candidate: đầu vào, bảo mật và số việc sót chưa rõ; mẫu tóm tắt thủ công có thể đã đủ. Candidate ghi nhận, nhóm chưa xác nhận riêng.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: độ mơ hồ cao × độ phức tạp cao.

Vì sao: cần hiểu chat tự do và ghép ngữ cảnh nhiều nhóm qua nhiều bước; các bước vẫn định sẵn.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Nhân viên tóm tắt theo mẫu. | Đủ đúng, nhanh và ít công. | Phụ thuộc cập nhật đều. | Đối chứng và quay về. |
| **Rule** | Gom dữ liệu, biểu mẫu, nhắc hạn. | Đầu vào có cấu trúc. | Khó hiểu chat tự do. | Cho bước cố định. |
| **Workflow** | Gom tin → AI trích xuất → người kiểm tra → gửi. | Đầu vào hợp lệ, tốt hơn No AI. | Bịa/sót, công rà soát. | Thử có điều kiện. |
| **Agent** | AI tự chọn bước và hành động. | Chưa có nhu cầu được xác nhận. | Vượt quyền, hành động sai. | Không chọn. |

**Mức chọn:** Workflow có LLM, nếu qua kiểm chứng.

**Vì sao không chọn mức đơn giản hơn:** Rule khó hiểu chat tự do, nhưng chưa loại No AI. Chỉ dùng AI nếu tổng công thấp hơn mà chất lượng không giảm.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Quyết định, cam kết và câu hỏi còn chờ, kèm nguồn. |
| **Judgment** — con người cân nhắc, quyết định gì? | Kiểm tra ngữ cảnh, chọn ưu tiên và cách phản hồi. |
| **Action** — hành động cuối cùng là gì, ai làm? | Rule gửi bản đã duyệt; CEO giao việc/trả lời; nhân viên xác nhận cam kết. |
| **Outcome** — đo kết quả bằng gì? | Thời gian đọc, việc bị sót, độ phủ và tổng công cả team. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Text, nhóm, người gửi, thời điểm và nguồn; chưa xác nhận lấy được. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Lỗi được sửa, việc CEO báo sót và sổ sự cố. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: đề xuất là augment, CEO vẫn quyết định; cần hỏi trực tiếp để xác nhận.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: bỏ sót làm trễ việc, bịa cam kết có thể dẫn đến quyết định sai. Kiểm tra nguồn, không chấp nhận cam kết quan trọng bị bịa; chưa đủ dữ liệu so mức thiệt hại.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | CEO công ty XNK máy móc; người phụ trách nhóm hỗ trợ kiểm tra. |
| **Quy trình** | Thử 3 nhóm: gom tin → trích xuất → kiểm tra → gửi 7h → CEO xử lý → theo dõi hạn. |
| **Bottleneck** | Đọc và lọc thông tin; 120 phút/ngày là ước lượng toàn bộ nhóm, cần đo lại theo phạm vi thử. |
| **Impact** | Giảm công đọc lại và nguy cơ sót cam kết; chưa có kết quả thực tế. |
| **Success Metric** (baseline → target, cách đo) | 120 phút/ngày (ước lượng) → ≤20 phút/ngày; sự cố sót việc giảm ≥80%. Đo baseline 2 tuần và pilot 2 tuần trên cùng nhóm; chưa có số sự cố gốc. Độ phủ ≥85%, ý bịa/sai ≤5%. |
| **Boundary** | Chỉ dùng dữ liệu được phép, mỗi ý có nguồn. Không tự nhắn khách/NCC, giao việc hay duyệt chi; tuần đầu duyệt trước khi gửi. |
| **AI intervention point** | Trích quyết định, cam kết và việc còn chờ từ text; bước cố định dùng Rule. |
| **Mức chọn** | Workflow có điều kiện. |
| **Rủi ro & người kiểm tra** | Kỹ thuật kiểm tra đầu vào; người phụ trách nhóm kiểm tra nội dung; CEO xác nhận quyết định. Chưa chốt người cụ thể. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Phạm vi và cách can thiệp | Chưa chốt giải pháp | Thử 3 nhóm bằng Workflow, có nguồn và người kiểm tra | Giảm phạm vi và kiểm chứng trước khi mở rộng. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đủ việc quan trọng | Bắt được ≥85% việc đánh dấu tay. | Dưới 85% hoặc sót việc gây thiệt hại thật. |
| 2 | Đúng nội dung | Ý sai/bịa ≤5%; không bịa/sai người, hạn ở cam kết quan trọng; thiếu thì ghi chưa rõ. | Vượt ngưỡng hoặc tự đoán thông tin quan trọng. |
| 3 | Có nguồn, rõ phạm vi | Mỗi ý có nguồn đối chiếu; báo dữ liệu, ảnh/voice chưa xử lý. | Nguồn sai/thiếu hoặc giấu phần chưa xử lý. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Cao | Chưa đo thời gian và sự cố thật của CEO. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | TB | Chưa thử bản mẫu và cách xem nguồn. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Cao | Chưa thử lấy tin nhóm và chất lượng AI. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Cao | Chưa chốt phạm vi dữ liệu, chi phí và người vận hành. |

### 8.2. Kết luận

**Quyết định:** Not Yet

**Lý do:** chưa xác nhận đầu vào, bảo mật và lợi ích so với tóm tắt thủ công.

**Nếu Go — pilot nhỏ nhất:** Tuần 0 kiểm tra kết nối/bảo mật; tuần 1–2 đo baseline; tuần 3–4 thử bản tóm tắt 7h, có người duyệt tuần đầu.

**Nếu Not Yet — cần kiểm chứng gì trước:** lấy tin hợp lệ, sự đồng ý về dữ liệu, pain thật và hiệu quả so với nhân viên tóm tắt.

**Nếu No-Go — nên làm gì thay AI:** tóm tắt theo mẫu, danh sách cam kết chung và Rule nhắc hạn.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …): không có đầu vào hợp lệ/đồng ý dữ liệu thì dừng tuần 0. Sau 2 vòng chỉnh, độ phủ <70% hoặc ý sai/bịa >10% thì quay về thủ công; không đạt ngưỡng đánh giá thì chưa mở rộng.

---

## 9. Hạn chế và hướng tiếp theo

- Số liệu là giả định; nguồn còn lệch mốc ngày/tuần nên cần đo lại. So cùng nhóm khi thử; baseline không có sự cố thì chưa tính % giảm. Nhóm bổ sung điểm CP3, bằng chứng phỏng vấn và phân công từ hoạt động thật.

## 10. Tài liệu tham khảo

- [Candidate CEO XNK](../assets/candidate-ceo-xnk.md); [Slack AI](https://slack.com/help/articles/25076892548883-Guide-to-AI-features-in-Slack); [Zalo OA/GMF](https://oa.zalo.me/home/documents/vie/guides/quan-ly-nhom-gmf_1954166378348758227); [n8n](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.information-extractor/).
