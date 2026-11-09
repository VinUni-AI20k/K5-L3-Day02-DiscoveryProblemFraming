# Báo cáo nhóm — Day 02 Discovery & Problem Framing

## 1. Thông tin nhóm

- Tên nhóm: 4Ward
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi vừa kết thúc cuộc họp dài 1 tiếng, tôi muốn tổng hợp lại danh sách công việc (action items) kèm người phụ trách, để gửi cho từng người trong team xác nhận ngay.
- Quyết định cuối: Go (Pilot phạm vi nhỏ)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Phùng Quang Trà | Khi có bộ hồ sơ giải ngân online mới, CRO muốn kiểm tra đủ giấy tờ và nhập lên hệ thống nhanh, để khách không phải chờ và phàn nàn vì xử lý chậm. | CRO nhập liệu; khách hàng chờ giải ngân bị ảnh hưởng gián tiếp. | Bước 3–4: đọc, trích thông tin và nhập hệ thống, ước tính ~45/80 phút mỗi bộ (~10 bộ/tháng); ~3/10 bộ bị trả về vì thiếu/sai; chưa bấm giờ thực tế. | |
| 2 | Phùng Quang Trà | Khi đến ngày đầu tháng, tôi muốn biết tháng trước đã chi bao nhiêu và phát sinh vào đâu, để điều chỉnh chi tiêu tháng sau. | Người dùng cá nhân quản lý chi tiêu từ nhiều app ngân hàng / ví. | Bước 3–4: chép và phân loại giao dịch từ nhiều app, ước tính ~10/23 phút mỗi tháng; chỉ tổng kết xong 1/3 tháng gần đây. | |
| 3 | Phùng Quang Trà | Khi kết thúc ngày làm việc, tôi muốn biết task nào đã xong, chưa xong và sắp tới, để sáng hôm sau bắt đầu ngay mà không bỏ sót việc. | Nhân viên văn phòng nhận việc qua email / chat. | Bước 1: lục lại email/chat tìm việc phát sinh, ước tính ~15/33 phút mỗi ngày; bỏ sót ~2 việc/tuần. | |
| 4 | Nguyễn Tuấn Anh |Khi cần tìm lại một thông báo hoặc quyết định cũ trong nhóm chat, tôi muốn thấy đúng tin đó ngay, để khỏi phải cuộn hàng trăm tin nhắn |Sinh viên trong nhóm 5 người |Bước 2, cuộn chat tìm thủ công: khoảng 6 phút/lần | |
| 5 | Nguyễn Tuấn Anh |Khi chuẩn bị nộp bài lúc 22h, tôi muốn biết bài còn thiếu mục nào, để không bị trừ điểm vì sai cấu trúc |Sinh viên làm bài lab |Bước 3, tự đối chiếu từng mục bằng mắt: khoảng 12 phút/lần | |
| 6 | Nguyễn Tuấn Anh |Khi làm bài nhóm, tôi muốn biết ai đang làm phần nào và hạn bao giờ, để khỏi phải nhắn hỏi lại |Nhóm trưởng và 4 thành viên |Bước 4, nhắn hỏi từng người vì không có nơi ghi chung: khoảng 8 phút/lần | |
| 7 | Vũ Nam Khánh | Khi vừa kết thúc cuộc họp dài 1 tiếng, tôi muốn tổng hợp lại danh sách công việc (action items) kèm người phụ trách, để gửi cho từng người trong team xác nhận ngay | Bản thân, Team | Trích xuất Task + Assignee | |
| 8 | Vũ Nam Khánh | Khi cần viết tài liệu cho một API/service mới, tôi muốn có cấu trúc tài liệu nhất quán từ source/config, để không phải viết thủ công từ đầu | Backend Developer | Viết mô tả param + response mẫu | |
| 9 | Vũ Nam Khánh | Khi mentor cần theo dõi tiến độ công việc, họ muốn thấy báo cáo dạng hình ảnh/bảng tổng quan ngắn gọn, để nắm tình hình mà không phải nhắn hỏi từng người | Mentor, Team | Lọc task xong & blocker | |
| 10 | Phạm Duy Thành| Gom nhanh yêu cầu và deadline từ các nguồn (LMS, chat) để làm bài không sót việc.| Sinh viên làm bài cá nhân; bạn cùng lớp có thể bị ảnh hưởng nếu thông tin được chia sẻ không thống nhất.| Bước 2–4: tìm và đối chiếu thông tin giữa các nguồn, ước tính 10–15 phút/lần; chưa bấm giờ, cần đo ở lần làm bài tiếp theo. Thời gian chờ câu trả lời chưa tính.| |
| 11 | Phạm Duy Thành| Tổng hợp tài liệu ôn tập (slide, ghi chú) để khoanh vùng phần chưa hiểu và học đúng trọng tâm.| Sinh viên đang tự ôn tập một chủ đề có nhiều tài liệu.| Bước 3–4: ghi chú rồi đối chiếu nội dung giữa các nguồn, ước tính 20–30 phút cho một chủ đề; chưa bấm giờ, số nguồn và độ dài tài liệu có thể làm thời gian thay đổi nhiều.| |
| 12 | Phạm Duy Thành| Phân loại và xếp ưu tiên các feedback để chỉnh sửa bài hiệu quả, không bị sót lỗi.| Sinh viên viết/chỉnh sửa bài; người góp ý có thể cần biết phản hồi đã được tiếp nhận.| Bước 3–5: phân loại, gắn góp ý vào phần bài và xác định thứ tự, ước tính 15–25 phút/bộ góp ý; chưa đo trên một bộ phản hồi thật.| |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A - Quản lý & Theo dõi công việc trong team/dự án | 3, 6, 7, 8, 9 | Gom thông tin, ghi chú rải rác sau cuộc họp hoặc quá trình làm việc để tạo danh sách action items, viết docs API hoặc báo cáo tiến độ cho lead/mentor/team |
| B - Thu thập & Theo dõi thông tin cá nhân (Học tập & Chi tiêu) | 2, 10, 11 | Gom và đối chiếu thông tin từ nhiều nguồn rời rác (lịch sử ngân hàng, bài tập LMS, slide/ghi chú ôn tập) để quản lý công việc và kế hoạch cá nhân |
| C - Tìm kiếm & Tra cứu thông tin rải rác | 4, 12 | Tìm kiếm, truy xuất đúng đoạn tin nhắn/quyết định cũ trong kênh chat hoặc gom/phân loại feedback để chỉnh sửa bài |
| D - Kiểm tra cấu trúc & Nhập liệu quy trình | 1, 5 | Đọc, đối chiếu và rà soát thủ công các thông tin/hồ sơ (hồ sơ giải ngân online, checklist cấu trúc bài lab) theo đúng mẫu tiêu chuẩn |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm 75% thời gian tổng hợp Action Items sau cuộc họp (từ 30 phút xuống <8 phút) mà không bị sót việc hoặc gán nhầm người phụ trách.
├── Opportunity A: Note họp dạng văn bản thô bị lan man, lẫn lộn giữa thảo luận chung và task thực sự cần làm.
├── Opportunity B: Tên người phụ trách (Assignee) và thời hạn (Deadline) không được chốt rõ ràng trong hội thoại họp.
└── Opportunity C: Việc định dạng lại danh sách việc ra dạng bảng để gửi cho team xác nhận tốn thời gian thủ công.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "Xây bot AI tự động tham gia cuộc họp để ghi chép": Đây là giải pháp công nghệ, không phải nỗi đau người dùng; bỏ để tập trung vào nhu cầu xử lý nội dung thô.
- "Tự động gửi danh sách công việc vào kênh chat ngay sau họp": Đây là tính năng/hành động giải pháp, vi phạm nguyên tắc chỉ ghi nhu cầu ở tầng Opportunity.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Candidate #7: Action items sau họp (Nam Khánh) | 5 | 5 | 5 | 5 | 5 | 5 | 5 | 35 |
| Candidate #8: Viết tài liệu API từ source (Nam Khánh) | 5 | 5 | 4 | 4 | 5 | 3 | 4 | 30 |
| Candidate #4: Tìm tin nhắn/quyết định cũ (Tuấn Anh) | 4 | 4 | 4 | 4 | 3 | 4 | 4 | 27 |

**Candidate được chọn:** Candidate #7 — Khi vừa kết thúc cuộc họp dài 1 tiếng, tôi muốn tổng hợp lại danh sách công việc (action items) kèm người phụ trách, để gửi cho từng người trong team xác nhận ngay.

**Vì sao chọn:**

- Actor và quy trình cực kỳ cụ thể: Đối tượng chịu ảnh hưởng rõ ràng (note-taker, PM, thành viên dự án); quy trình 5 bước đo được chính xác bằng phút.
- Có baseline đo lường được: Mất 30 phút/buổi họp, tần suất 2–3 buổi/tuần, tác động trực tiếp đến tiến độ chung của team.
- Phân định rõ ranh giới AI (HITL): Bài toán phù hợp hoàn hảo để triển khai mức Workflow, trong đó AI xử lý bước trích xuất nháp và con người (Note-taker/PM) kiểm tra lại trước khi gửi, đảm bảo không bị rủi ro gán sai người/sai việc.

**Vì sao loại các candidate còn lại:**

- Candidate #8 (Viết Docs API): Mặc dù quy trình rất chuẩn hóa, nhưng nhóm phân tích thấy có đến 80% công việc có thể xử lý hoàn toàn bằng Rule/Script (ví dụ: các thư viện Swagger/OpenAPI spec tự sinh docs từ code annotation), không thực sự cần tới sự can thiệp của AI.
- Candidate #4 (Tìm quyết định cũ trong chat): Bài toán đòi hỏi quyền truy cập dữ liệu chat toàn công ty/nhóm, phạm vi quá rộng và chạm trần rủi ro về mặt Feasibility & Viability (quyền riêng tư và bảo mật dữ liệu).

**Xử lý bất đồng (nếu có):** Không

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Note-taker/PM khác cũng mất hơn 20 phút sau mỗi buổi họp 1h để lọc và tổng hợp lại action items | Value | 5 | 2 | Có |
| 2 | Bước tốn thời gian nhất là đọc lại note thô để trích xuất task và gán Assignee, không phải bước gửi tin nhắn | Value | 5 | 2 | Có |
| 3 | Thành viên trong team sẵn sàng xác nhận action items nếu nhận được dạng bảng ngắn gọn trong vòng 15 phút sau họp | Value | 4 | 3 | Có |
| 4 | Nội dung transcript/note cuộc họp cung cấp đủ ngữ cảnh để AI phân biệt được đâu là "thảo luận" và đâu là "giao việc" | Feasibility | 5 | 2 | Có |
| 5 | Người dùng dễ dàng kiểm tra, chỉnh sửa bản nháp của AI trong dưới 3 phút trước khi gửi cho team | Usability | 4 | 2 | - |
| 6 | Công ty/Nhóm cho phép đưa transcript hoặc nội dung ghi chép họp nội bộ vào công cụ AI xử lý | Viability | 5 | 1 | Có |

Giả định nhóm kiểm chứng trong buổi này: Giả định #1, #2, #4 và #6 (đây là các giả định có mức độ quan trọng cao từ 5 và bằng chứng hiện có thấp từ 1–2).

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
HIỆN TẠI — 5 bước, 30 phút, 5/5 bước thủ công

[1] Mở file note thô: 2'
[2] Đọc lại & phân loại việc: 12'
[3] Lọc Task + Assignee: 8' ← BOTTLENECK
[4] Định dạng dạng bảng: 5'
[5] Gửi lên Slack/Email: 3'
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Note-taker | File ghi chép thô trong cuộc họp | File note thô được mở | 2 phút / 2–3 họp/tuần | Dữ liệu lan man, lộn xộn |
| 2 | Note-taker | File note thô | Các đoạn văn bản có chứa việc | 12 phút / 2–3 họp/tuần | Đọc rà soát lại toàn bộ |
| 3 | Note-taker | Các đoạn văn bản chứa việc | Danh sách Task + tên Assignee | 8 phút / 2–3 họp/tuần | Bottleneck: Dễ sót việc hoặc gán nhầm |
| 4 | Note-taker | Danh sách Task + Assignee | Bảng tổng hợp công việc | 5 phút / 2–3 họp/tuần | Định dạng thủ công |
| 5 | Note-taker | Bảng tổng hợp công việc | Tin nhắn gửi lên kênh chat | 3 phút / 2–3 họp/tuần | Copy-paste và gửi team |

**Bottleneck chính:** Bước 2 và 3 (Đọc lại note thô để trích xuất Task và gán đúng người phụ trách) mất 20/30 phút vì cuộc họp thảo luận lan man, không chốt rõ ràng từ đầu.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 4 bước, 7 phút, 2/4 bước thủ công

[1] Dán note thô vào công cụ: 1'        ← CON NGƯỜI
[2] AI trích xuất nháp bảng task: 1'    ← AI (Rule / Prompt)
[3] Note-taker kiểm tra & chỉnh sửa: 3' ← CON NGƯỜI (HITL Boundary)
[4] Gửi danh sách lên Slack: 2'         ← CON NGƯỜI

BOUNDARY: AI không tự động gửi tin nhắn, không tự nghĩ ra task không có trong note thô.
PHƯƠNG ÁN QUAY VỀ: AI sai hoặc nháp lộn xộn → Note-taker bỏ nháp, tự lọc tay theo cách cũ.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 4 | Bỏ khâu định dạng và phân loại thủ công |
| Tổng thời gian | 30 phút | khoảng 7 phút | Giảm hơn 70% thời gian sau họp |
| Số bước thủ công | 5/5 | 3/4 | AI làm nháp, con người duyệt và gửi |
| Bottleneck chính | Đọc lại note thô & gán người làm | Note-taker kiểm tra & sửa nháp | Chuyển thành bước kiểm soát chất lượng |
| Rủi ro mới phát sinh | Không có | AI đoán sai người làm hoặc lọc thiếu task | Xử lý bằng kiểm tra người duyệt (HITL) |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Note-taker / Người chủ trì cuộc họp team |
| **Quy trình** | Mở file note thô sau họp → Lọc công việc và người làm thủ công → Định dạng lại bảng → Gửi lên Slack cho team |
| **Bottleneck** | Khâu đọc lại ghi chú thô để lọc công việc và gán tên người phụ trách (Assignee), mất khoảng 20 phút |
| **Impact** | Tốn 30 phút sau mỗi buổi họp (2–3 buổi/tuần); gửi danh sách trễ khiến team dễ quên việc hoặc làm chồng chéo |
| **Success Metric** (baseline → target, cách đo) | Thời gian tổng hợp giảm từ 30 phút xuống <8 phút/buổi họp, đo bằng Note-taker tự bấm giờ 4 buổi pilot |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ được tạo bản nháp bảng task, không được tự động gửi tin nhắn và bắt buộc có con người (Note-taker) duyệt lại trước khi gửi |

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: Độ mơ hồ Cao x Độ phức tạp Trung Bình

Vì sao:
- Độ mơ hồ Cao: Mỗi cuộc họp mọi người nói chuyện một kiểu, note thô viết mỗi lúc một khác. AI phải tự hiểu ngữ cảnh để lọc ra đâu là "việc cần làm" và ai phụ trách, chứ không có công thức đúng/sai cố định.
- Độ phức tạp Trung Bình: Luồng xử lý đi thẳng từ trên xuống dưới (Nhập note thô -> AI lọc task -> Định dạng bảng -> Người duyệt), dữ liệu hoàn toàn là chữ (text) nên không bị rẽ nhánh hay tính toán quá phức tạp.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Dùng template Notion/Docs chuẩn, bắt buộc ghi rõ Task + Người làm ngay trong lúc họp | Họp nhóm nhỏ (2–3 người), mọi người tự giác điền thẳng vào file trong lúc nói chuyện | Mọi người hay quên điền, lúc họp mải thảo luận nên note vẫn bị lộn xộn | Không chọn |
| **Rule** | Viết script tự tạo công việc khi gõ đúng cú pháp cố định (ví dụ: @tên + task) | Mọi người chịu gõ đúng định dạng quy định sẵn trong file note | Rất gượng ép, trong lúc họp nói nhanh nên không ai rảnh gõ đúng cú pháp | Không chọn |
| **Workflow** | Nhập note thô -> AI tự lọc task + người làm -> Hiện bản nháp cho Note-taker sửa -> Gửi Slack | Khi muốn giữ cách nói/ghi chép tự nhiên, nhưng vẫn cần AI lọc nháp và người duyệt lại cho chắc | AI có thể bắt thiếu task hoặc đoán sai người làm nếu note thô quá tắt | Chọn |
| **Agent** | Cho AI tự vào họp ghi âm, tự đoán việc, tự tạo task trên Jira và tự gửi tin nhắn cho từng người | Khi quy trình đã quá chuẩn hóa, không cần con người kiểm tra lại | AI tự gửi linh tinh làm trôi tin nhắn, gán sai việc gây cãi nhau trong team, chi phí cao | Không chọn |

**Mức chọn:** Workflow

**Vì sao không chọn mức đơn giản hơn:**
- No AI (Template) không giải quyết được gốc rễ vấn đề: lúc họp mọi người chỉ tập trung trao đổi chứ không ai rảnh vừa nói vừa format lại chữ cho đẹp.
- Rule (Script) thì quá cứng nhắc: bắt người dùng phải gõ đúng cú pháp @tên + làm việc X thì script mới hiểu, thực tế không ai làm theo được khi họp nhanh.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Bảng danh sách nháp gồm: Tên công việc (Action Item) + Người phụ trách (Assignee) + Hạn chót (Deadline) được lọc ra từ ghi chú thô. |
| **Judgment** — con người cân nhắc, quyết định gì? | Note-taker kiểm tra xem AI có lọc thiếu việc nào không, tên người phụ trách có bị gán nhầm không trước khi bấm gửi. |
| **Action** — hành động cuối cùng là gì, ai làm? | Note-taker bấm xác nhận gửi bảng danh sách công việc đã duyệt lên kênh chat Slack/Discord cho cả team. |
| **Outcome** — đo kết quả bằng gì? | Mất dưới 8 phút để tổng hợp (so với 30 phút cũ) và 100% việc gửi đi đều có đúng người nhận task. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Văn bản ghi chú thô (hoặc transcript) của buổi họp. Có sẵn ngay sau khi họp xong. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Xem Note-taker hay sửa lại/xóa bỏ những dòng nào trên bản nháp để chỉnh lại prompt lọc task chuẩn hơn. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**?
    - Trả lời: Người dùng muốn được hỗ trợ (augment).
    - Bằng chứng: Vì lúc họp mọi người hay nói tắt hoặc đùa vui, Note-taker rất sợ AI đoán sai người làm hoặc gán nhầm việc linh tinh. Bắt buộc phải để Note-taker nhìn qua bản nháp rồi tự tay bấm "Gửi", chứ không ai dám để AI tự động gửi thẳng vào Slack của team.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
    - Bỏ sót tệ hơn nhiều.
    - Nếu AI báo nhầm (tự bịa ra 1 việc thừa), Note-taker nhìn thấy là bấm xóa cái rẹt trong 2 giây. Nhưng nếu AI bỏ sót (bỏ quên 1 task quan trọng), team sẽ bị trễ tiến độ mà không ai hay biết. Cách thiết kế là viết prompt dặn AI "thà bắt nhầm còn hơn bỏ sót" (cứ gom hết các việc có khả năng làm), sau đó để Note-taker tự tay tích chọn và xóa bớt những ý thừa trên màn hình duyệt.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Note-taker / Người chủ trì cuộc họp team |
| **Quy trình** | Mở note thô sau họp -> Dán vào công cụ AI lọc task -> Kiểm tra & sửa bản nháp -> Gửi danh sách lên Slack |
| **Bottleneck** | Khâu đọc lại ghi chú thô để lọc công việc và gán tên người phụ trách (Assignee) |
| **Impact** | Tốn 30 phút sau mỗi buổi họp (2–3 buổi/tuần); trễ gửi danh sách khiến team quên việc hoặc làm chồng chéo |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian tổng hợp giảm từ 30 phút xuống <8 phút; (2) 100% action items gửi đi có đúng tên người làm |
| **Boundary** | AI chỉ được tạo bản nháp, không tự động gửi tin nhắn và không tự nghĩ ra task không có trong note thô |
| **AI intervention point** | Ngay sau khi họp xong (sau khi Note-taker dán ghi chú thô vào) |
| **Mức chọn** | Workflow |
| **Rủi ro & người kiểm tra** | AI đoán sai người làm hoặc lọc thiếu việc -> Note-taker phải tự nhìn qua và sửa trước khi bấm gửi |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Success Metric | Chỉ đo thời gian tổng hợp (<8 phút) | Thêm chỉ số: 100% việc gửi đi có đúng người làm | Nhanh hơn mà gửi sai tên người làm thì cũng công cốc, nên cần đo thêm độ chuẩn xác |
| Boundary | AI trợ giúp tóm tắt nội dung cuộc họp | Thêm cấm AI tự động gửi tin nhắn và cấm tự bịa task | Đặt ranh giới rõ ràng để Note-taker không sợ AI làm bậy |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Không bịa task | Mọi công việc liệt kê ra đều có thông tin trong note thô | AI tự sáng tác thêm công việc không ai nói trong họp |
| 2 | Đúng người phụ trách | Tên Assignee khớp chính xác với người được giao trong note | Gán nhầm việc của người này sang cho người khác |
| 3 | Đúng định dạng bảng | Ra đúng dạng bảng 3 cột: Task, Assignee,  Deadline | Ra chữ lan man thành đoạn văn dài khó nhìn |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Thấp | Note-taker nào họp xong cũng ngán khâu đọc lại note thô để gom việc. Nhu cầu rút ngắn thời gian sau họp là có thật. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Thấp | Giao diện hiện ra dạng bảng 3 cột (Task, Assignee, Deadline), Note-taker chỉ cần nhìn qua, bấm sửa chữ hoặc xóa dòng rất dễ dàng. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | Input chỉ là văn bản note thô dán vào, dùng API của các model phổ biến (như ChatGPT/Claude) viết prompt lọc task là chạy được ngay. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Trung bình | Một số cuộc họp nội bộ có thông tin nhạy cảm nên công ty ngại dán vào AI bên ngoài; chi phí dùng API thì rất rẻ không đáng lo. |

### 8.2. Kết luận

**Quyết định:** Go (Pilot phạm vi nhỏ)

**Lý do:** Không có rủi ro nào ở mức Cao. Rủi ro duy nhất là Viability (bảo mật thông tin họp) có thể giải quyết bằng cách dặn người dùng xóa bớt các thông tin quá nhạy cảm trước khi dán vào AI.

**Nếu Go — pilot nhỏ nhất:** Nhóm chưa cần viết code/app gì phức tạp. Tạo sẵn 1 khung Prompt chuẩn. Mỗi lần họp nhóm xong, Note-taker dán note thô + Prompt đó vào AI (ChatGPT/Claude) để lấy bản nháp bảng task, dùng thử trong 2 tuần (khoảng 4–6 buổi họp).

**Ngưỡng dừng**: Nếu sau 2 tuần dùng thử mà Note-taker vẫn phải ngồi gõ lại tay hơn 50% nội dung bảng nháp -> Dừng lại, quay về dùng template Google Docs thủ công như cũ.

---

## 9. Hạn chế và hướng tiếp theo

## 10. Tài liệu tham khảo
