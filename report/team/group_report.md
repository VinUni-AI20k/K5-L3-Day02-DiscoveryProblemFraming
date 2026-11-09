# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Nhomabc404
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Người được hỏi phải giải thích lại cùng một câu hỏi cho đồng nghiệp, bạn học, khoảng 2 lần/tuần và khoảng 15–30 phút mỗi lần (survey 10 người, ước lượng từ khoảng giá trị). *(Bản nháp, chờ nhóm xác nhận.)*
- Quyết định cuối: Go, phạm vi nhỏ (pilot FAQ, mức No AI) *(bản nháp, chờ nhóm xác nhận)*

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Quang Đạo | Kiểm tra các điều khoản bất lợi trong hợp đồng dịch vụ so với quy định chuẩn của công ty | — | — | |
| 2 | Nguyễn Quang Đạo | Đọc hiểu và phân loại tin nhắn/email phàn nàn của khách hàng để chuyển đúng người | — | — | |
| 3 | Nguyễn Quang Đạo | Kiểm tra định dạng và hạn nộp bài tập của sinh viên trước khi khóa cổng nộp bài | Sinh viên | — | |
| 4 | Đỗ Cao Cường | Chọn món và đặt cơm trưa trên Grab trong giờ nghỉ ngắn: khi xong việc lúc 12h mà giờ nghỉ chỉ có ít phút, muốn có cơm đúng lúc để kịp ăn và quay lại làm việc | Nhân viên văn phòng có giờ nghỉ trưa ngắn | Đặt sau 12h vì trong giờ làm không để ý tới việc đặt, nên 30–45 phút chọn và chờ giao rơi vào giờ nghỉ (ước lượng) | |
| 5 | Đỗ Cao Cường | Giải thích lại cùng một câu hỏi cho đồng nghiệp, bạn học: muốn có sẵn chỗ để họ tự tra, không phải giải thích lại từ đầu | Tôi (người được hỏi), đồng nghiệp và bạn học | Giải thích lại từ đầu, khoảng 30 phút–1 giờ/lần, 1–2 lần/tuần (ước lượng) | |
| 6 | Đỗ Cao Cường | Sắp xếp ưu tiên công việc mỗi sáng: muốn biết ngay việc nào làm trước, không mất thời gian sắp xếp lại | Người đi làm tự sắp xếp công việc | Khoảng 15 phút mỗi sáng, 4–5 ngày/tuần (ước lượng); bước nghẽn chưa xác định | |
| 7 | Hồ Sỹ Tùng | Tìm kiếm ảnh chụp màn hình theo nội dung trong điện thoại | Người dùng điện thoại | — | |
| 8 | Hồ Sỹ Tùng | Tổng hợp công việc và deadline từ nhiều ứng dụng khác nhau | — | Công việc và deadline nằm rải ở nhiều ứng dụng | |
| 9 | Hồ Sỹ Tùng | Tổng hợp ưu và nhược điểm sản phẩm từ nhiều đánh giá online | Người mua / người đọc đánh giá | Ưu, nhược điểm nằm rải trong nhiều đánh giá | |
| 10 | Trần Quốc Đông | Khiếu nại sản phẩm không đúng mô tả được xử lý chậm | — | Xử lý khiếu nại chậm | |
| 11 | Trần Quốc Đông | Người mua khó nhận biết đánh giá giả | Người mua | — | |
| 12 | Trần Quốc Đông | Người mua mất nhiều thời gian so sánh sản phẩm | Người mua | Mất nhiều thời gian so sánh | |
| 13 | Trần Đức Mạnh | Quản lý và đối soát xe ra vào bãi xe giờ cao điểm (Lặp lại) | — | Ùn ứ giờ cao điểm, nhầm lẫn vé xe | |
| 14 | Trần Đức Mạnh | Tự động hóa tiếp nhận và điều phối lịch hẹn phòng khám (Tốn thời gian) | — | Trùng lịch, bệnh nhân quên hoặc hủy sát giờ | |
| 15 | Trần Đức Mạnh | Tóm tắt và trích xuất phương pháp/dataset từ paper PDF (Cần đọc, tổng hợp) | Sinh viên làm đồ án | Đọc lướt tài liệu kỹ thuật dài, tốn hàng chục giờ | |
| 16 | Nguyễn Văn Ngọc Sơn | Khi chỉnh sửa prompt của tính năng sinh câu trả lời tự động, muốn nhận ra những câu hỏi trước đây trả lời đúng nhưng bản mới lại trả lời sai, để tránh đưa lỗi vào phiên bản tiếp theo | Người chỉnh sửa prompt | Không nhận ra câu từng đúng nay bị sai | |
| 17 | Nguyễn Văn Ngọc Sơn | Khi job huấn luyện hoặc tinh chỉnh mô hình thất bại, muốn xác định bước lỗi và nguyên nhân cụ thể, để hạn chế các lần chạy lại không cần thiết | Người chạy huấn luyện / tinh chỉnh mô hình | Khó xác định bước lỗi và nguyên nhân | |
| 18 | Nguyễn Văn Ngọc Sơn | Khi PM/BA hỏi hệ thống đang sai ở những tình huống nào, muốn cung cấp các nhóm lỗi, ví dụ và tần suất có thể đối chiếu, để nhóm chọn đúng việc cần sửa trước | PM/BA và người cung cấp thông tin lỗi | Thiếu nhóm lỗi, ví dụ, tần suất có thể đối chiếu | |

*Dấu "—" nghĩa là thành viên chưa cung cấp, điền khi pitch. Cột "Câu hỏi phản biện" để trống cho đến khi nhóm pitch (CP3 bước 1, không dùng AI).*

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A · Gom và đọc thông tin rải ở nhiều nguồn | #7, #8, #9, #12, #15 | Người dùng phải đi qua nhiều nơi (ứng dụng, đánh giá, tài liệu dài) để rút ra một kết luận, và việc này tốn thời gian |
| B · Câu hỏi, khiếu nại, yêu cầu lặp lại xử lý bằng tay | #2, #5, #10, #14 | Cùng một loại yêu cầu quay lại nhiều lần, mỗi lần một người phải đọc, trả lời hoặc điều phối thủ công và chậm |
| C · Kiểm tra, phát hiện lỗi hoặc sai lệch | #1, #3, #11, #13, #16, #17, #18 | Lỗi, điều khoản bất lợi hoặc sai lệch bị phát hiện muộn hoặc sót vì kiểm tra thủ công, không có chỗ đối chiếu rõ ràng |
| D · Việc nhỏ hằng ngày thiếu tín hiệu nhắc đúng lúc | #4, #6 | Việc lặp lại mỗi ngày bị dồn lại hoặc làm muộn vì không có điểm nhắc cố định |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm số giờ mỗi tuần mà một người phải bỏ ra cho việc lặp lại, đọc, tìm và kiểm tra thủ công
├── Opportunity A: Mất nhiều thời gian gom và đọc thông tin rải ở nhiều nguồn mới ra được kết luận
├── Opportunity B: Cùng một câu hỏi, khiếu nại hoặc yêu cầu phải xử lý lặp lại bằng tay và chậm
├── Opportunity C: Lỗi, điều khoản bất lợi hoặc sai lệch bị phát hiện muộn hoặc bị sót
└── Opportunity D: Việc nhỏ hằng ngày bị dồn hoặc làm muộn vì không có điểm nhắc đúng lúc
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- #3 "Tự động kiểm tra định dạng và hạn nộp": "tự động kiểm tra" là cách giải. Viết lại thành pain: sinh viên nộp sai định dạng hoặc quá hạn mà chỉ biết sau khi cổng đã khóa.
- #14 "Tự động hóa tiếp nhận và điều phối lịch hẹn": "tự động hóa" là cách giải. Pain thật: trùng lịch và bệnh nhân quên hoặc hủy sát giờ.
- #7 "Tìm kiếm ảnh chụp màn hình theo nội dung": đây là tính năng. Pain thật: không tìm lại được ảnh chụp màn hình cần dùng.
- #15 "Tóm tắt và trích xuất từ paper PDF": "tóm tắt, trích xuất" là cách giải. Pain thật: đọc tài liệu kỹ thuật dài tốn hàng chục giờ.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #5 Giải thích lại cùng một câu hỏi | 5 | 4 | 3 | 4 | 5 | 5 | 4 | **30** |
| #8 Tổng hợp công việc và deadline từ nhiều ứng dụng | 2 | 2 | 2 | 3 | 3 | 4 | 3 | **19** |
| #15 Đọc paper PDF dài để lấy phương pháp và dataset | 4 | 3 | 3 | 4 | 3 | 4 | 3 | **24** |

*Điểm do nhóm chấm (thang 1–5). Tổng đã kiểm tra lại: #5 = 30, #8 = 19, #15 = 24. #5 dẫn đầu, #8 thấp nhất vì thiếu thông tin về actor, quy trình và bằng chứng.*

**Phiếu của Đỗ Cao Cường** (chọn nhất, loại nhất, câu hỏi phản biện; phiếu của các thành viên khác thêm vào đây khi có):

- Chọn nhất: #5, vì có số đo (30 phút–1 giờ/lần, 1–2 lần/tuần, ước lượng), actor rõ, và dễ thử cách đơn giản (FAQ) rồi đo lại.
- Muốn loại nhất: #8, vì chưa rõ actor, nguồn việc và số phút, lại dễ trùng với việc sắp xếp ưu tiên mỗi sáng (#6).
- Câu hỏi phản biện (hỏi #8): Công việc và deadline đang nằm ở những ứng dụng nào, mỗi lần gom mất bao nhiêu phút, và vì sao đây khác với sắp xếp ưu tiên mỗi sáng?

**Candidate được chọn:** #5 · Khi đồng nghiệp hoặc bạn học hỏi lại một câu đã được trả lời, người được hỏi phải giải thích lại từ đầu, khoảng 2 lần/tuần và khoảng 15–30 phút mỗi lần (survey 10 người, ước lượng). *(Bản nháp, chờ cả nhóm xác nhận.)*

**Vì sao chọn:**

- Là candidate duy nhất đã có dữ liệu từ người ngoài nhóm: survey 10 người cho thấy 10/10 từng bị hỏi lại, 7/10 từ 3 lần trở lên trong 2 tuần, 7/10 mất từ 15 phút mỗi lần (xem mục 3.2).
- Actor rõ (người được hỏi, đồng nghiệp, bạn học) và nhóm đã khảo sát được những người bị ảnh hưởng ở CP4.
- Điểm nhóm cao nhất trong shortlist: 30, so với 24 (#15) và 19 (#8).
- Vừa sức lab, và có thể so sánh rõ các mức: một trang FAQ đã có thể đủ (No AI), nên nhóm kiểm chứng được việc có cần AI hay không.

**Vì sao loại các candidate còn lại:**

- **#8 Tổng hợp công việc và deadline từ nhiều ứng dụng:** chưa rõ actor, nguồn việc và số phút. Dễ trùng với việc sắp xếp ưu tiên mỗi sáng (#6). Có thể quay lại nếu người đưa ra bổ sung số liệu.
- **#15 Đọc paper PDF dài để lấy phương pháp và dataset:** pain thật, nhưng rủi ro trích sai số liệu từ bảng biểu cao, khó đưa ra tiêu chí đạt trong khuôn khổ lab. Chưa có số đo thời gian đọc cho từng người.
- **Các candidate ngoài shortlist (#1–#4, #6, #7, #9–#14, #16–#18):** chưa được chấm điểm đầy đủ vì thiếu actor, bottleneck hoặc số liệu. Nhóm có thể đưa lại vào shortlist nếu bổ sung được dữ kiện.

**Xử lý bất đồng (nếu có):** Chưa ghi nhận bất đồng. Sẽ bổ sung ở đây nếu có ý kiến khác về candidate được chọn.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Người khác (đồng nghiệp, bạn học) thật sự hỏi lại cùng một câu khoảng 1–2 lần/tuần | Value | 5 | 4 (survey 10 người: 10/10 từng gặp, 7/10 từ 3 lần trong 2 tuần) | Đã kiểm chứng bằng survey |
| 2 | Mỗi lần giải thích lại mất 30 phút–1 giờ, không chỉ vài phút | Value | 5 | 3 (7/10 mất từ 15 phút, chỉ 3/10 mất 30–60 phút: bị phản bác một phần) | Đã kiểm chứng, cần sửa baseline |
| 3 | Người hỏi chịu tự tra một chỗ có sẵn (FAQ, tin ghim) thay vì hỏi trực tiếp | Usability | 5 | 2 (7/10 nói sẵn sàng, 3/10 có thể: mới là ý định nói ra) | Cần pilot để xem hành vi thật |
| 4 | Các câu hỏi lặp lại đủ giống nhau để gom thành một bộ trả lời sẵn, không phải mỗi lần một khác | Feasibility | 4 | 3 (6/10 hầu hết giống, 4/10 giống một phần) | Đã kiểm chứng một phần |
| 5 | Phần tốn thời gian là giải thích lại, không phải tìm lại câu trả lời cũ | Value | 3 | 2 | Sau |
| 6 | Có người chịu cập nhật FAQ để nó không lỗi thời | Viability | 3 | 1 | Sau |

Giả định nhóm kiểm chứng trong buổi này: #1, #2, #3, #4, qua survey 10 người (xem 3.2). #3 vẫn cần pilot.

### 3.2. Kiểm chứng

Cách đã dùng: **Survey** (10 người). Không thực hiện phỏng vấn, nên không có interview snapshot.

**Thiết kế survey:** 10 người trả lời, ẩn danh theo vai trò. Thu thập 4 chỉ số: số lần bị hỏi lại trong 2 tuần gần đây, thời gian mỗi lần, mức độ giống nhau của các câu hỏi, và mức sẵn sàng dùng FAQ. Dữ liệu thô nằm ở bảng dưới (chép nguyên từ file kết quả survey của nhóm).

| Mã | Vai trò | Số lần bị hỏi lại (2 tuần) | Thời gian mỗi lần | Mức giống nhau của câu hỏi | Sẵn sàng dùng FAQ |
|---|---|---|---|---|---|
| R1 | Kỹ sư phần mềm | 3–5 | 15–30 phút | Hầu hết giống nhau | Có |
| R2 | Sinh viên | 1–2 | 5–15 phút | Giống một phần | Có thể |
| R3 | Trưởng nhóm | 6–10 | 30–60 phút | Hầu hết giống nhau | Có |
| R4 | Kỹ sư phần mềm | 3–5 | 15–30 phút | Hầu hết giống nhau | Có |
| R5 | Sinh viên | 3–5 | 15–30 phút | Giống một phần | Có |
| R6 | Nhân viên văn phòng | 1–2 | 5–15 phút | Giống một phần | Có thể |
| R7 | Kỹ sư phần mềm | 6–10 | 30–60 phút | Hầu hết giống nhau | Có |
| R8 | Sinh viên | 1–2 | Dưới 5 phút | Hầu hết giống nhau | Có |
| R9 | Trưởng nhóm | 3–5 | 30–60 phút | Hầu hết giống nhau | Có |
| R10 | Nhân viên văn phòng | 3–5 | 15–30 phút | Giống một phần | Có thể |

Tổng hợp:

| Chỉ số | Kết quả | Giả định liên quan | Tín hiệu |
|---|---:|---|---|
| Từng bị hỏi lại câu cũ | 10/10 (100%) | #1 | Xác nhận |
| Bị hỏi lại từ 3 lần trở lên trong 2 tuần | 7/10 (70%) | #1 | Xác nhận |
| Mất từ 15 phút trở lên mỗi lần | 7/10 (70%) | #2 | Xác nhận một phần |
| Mất 30–60 phút mỗi lần | 3/10 (30%) | #2 | **Phản bác một phần**: giả định ban đầu là 30 phút–1 giờ, nhưng chỉ 3/10 ở mức này |
| Câu hỏi hầu hết giống nhau | **6/10 (60%)**, 4/10 giống một phần | #4 | Xác nhận một phần |
| Sẵn sàng dùng FAQ | 7/10 (70%) Có, 3/10 (30%) Có thể, 0/10 Không | #3 | Xác nhận yếu: đây là ý định nói ra, chưa phải hành vi đã xảy ra |

Ước tính từ khoảng giá trị giữa của từng mức (ước lượng, không phải số đo): trung bình khoảng 4 lần/người trong 2 tuần (khoảng 2 lần/tuần), khoảng 25 phút/lần, tức khoảng 65 phút/tuần/người, thấp hơn mức 30 phút–1 giờ/lần ở giả định ban đầu nhưng khớp với khoảng 0,5–2 giờ/tuần của ước lượng ban đầu.

**Hạn chế của survey:**

- Mẫu nhỏ (10 người). Cả 10 người đều từng bị hỏi lại ít nhất 1–2 lần, nên có thể mẫu chưa gồm người ít bị hỏi lại (thiên lệch chọn mẫu).
- Không có câu trả lời mở ("lần gần nhất là chuyện gì"), nên chưa có một câu nói nguyên văn hay chuyện cụ thể nào.
- "Sẵn sàng dùng FAQ" là câu hỏi giả định về tương lai. Theo The Mom Test, đây là bằng chứng yếu. Cần pilot để xem hành vi thật.

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

- Giữ nguyên problem: việc bị hỏi lại câu cũ có thật và đủ thường xuyên (10/10 từng gặp, 7/10 từ 3 lần/2 tuần).
- **Sửa baseline:** từ "30 phút–1 giờ mỗi lần" xuống "khoảng 15–30 phút mỗi lần là phổ biến nhất (4/10 ở mức 15–30 phút, 3/10 ở mức 30–60 phút)". Mức 30–60 phút chỉ nên coi là trường hợp nặng (trưởng nhóm và kỹ sư có nhiều lần hỏi lại).
- **Sửa quyết định** từ Not Yet sang Go phạm vi nhỏ (pilot FAQ, No AI), vì hai giả định quan trọng nhất (#1, #4) có bằng chứng và không có ai trả lời "Không" với FAQ. Giả định #3 vẫn cần kiểm chứng bằng pilot.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Slack Workflow Builder, trả lời FAQ bằng emoji | [slack.com](https://slack.com/resources/using-slack/4-simple-ways-to-save-time-with-workflow-builder) | Bước "giải thích lại": khi ai đó hỏi câu cũ, một emoji kích hoạt tin nhắn trả lời sẵn dẫn tới tài liệu FAQ | Trang mô tả cách làm ngay: chỉ cần có sẵn một tài liệu FAQ, gắn emoji, workflow gửi trả lời trong thread | Cần người viết và duy trì tài liệu FAQ trước. Trang không nói về chi phí hay gói áp dụng. Chỉ chạy được nếu nhóm dùng Slack | Giải pháp đơn giản, không cần AI, đúng hướng No AI. Điều kiện then chốt là có FAQ tốt |
| Notion, hỏi đáp trên nội dung workspace | [notion.com](https://www.notion.com/help/guides/get-answers-about-content-faster-with-q-and-a) | Bước "tìm lại câu trả lời": người hỏi tự đặt câu hỏi cho tài liệu của nhóm thay vì nhắn cho đồng nghiệp | Trang nói thẳng vấn đề "người giữ kiến thức bị hỏi liên tục những câu thường lệ" | Chỉ trả lời được từ nội dung đã có trong workspace và người dùng có quyền truy cập. Hiệu quả phụ thuộc workspace đầy đủ và cập nhật | Dù có công cụ hỏi đáp, bước đầu vẫn là có nội dung tốt. Mức "có AI" chỉ có ích khi tài liệu nguồn đã tồn tại |
| Slack AI, tìm kiếm có trả lời | [slack.com](https://slack.com/intl/en-au/features/ai) | Bước "tìm lại câu trả lời cũ" trong các cuộc trò chuyện đã có | Tìm trong tin nhắn, tệp và ứng dụng đã tích hợp vào Slack | Trang nói tính năng AI có trên các gói trả phí và có chú thích thông tin có thể thay đổi. Con số tiết kiệm thời gian của trang dựa trên phân tích nội bộ của chính Slack, không độc lập | Cần thận trọng với số liệu của nhà cung cấp. Không phải giải pháp cho nhóm không dùng Slack hoặc không dùng gói trả phí |

*Cả 3 link đã được mở và đối chiếu nội dung trang. Trang Notion có tiêu đề hiển thị là "Get answers about work content faster with Notion Agent". Link của Slack có bản ngôn ngữ khác, nội dung có thể khác nhau chút.*

---

## 4. Quy trình trước/sau (CP5)

> **Bản nháp do AI soạn từ dữ kiện đã có (Problem Card #2 của Đỗ Cao Cường). Nhóm phải đối chiếu với thực tế và với kết quả survey ở mục 3.2 trước khi nộp.** Số phút ghi "?" là chưa đo.

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — khoảng 30 phút–1 giờ/lần, khoảng 1–2 lần/tuần (ước lượng)

[Người hỏi nhắn hoặc hỏi lại câu cũ: ?'] → [Tôi nhớ hoặc tìm lại câu trả lời: ?']
→ [Tôi giải thích lại từ đầu: 30–60'] ← BOTTLENECK
→ [Người hỏi làm thử, hỏi tiếp nếu chưa hiểu: ?']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Đồng nghiệp, bạn học | Một câu hỏi đã từng được trả lời | Tin nhắn hoặc câu hỏi trực tiếp | ? | Kênh: chưa xác định (chat nhóm, hỏi trực tiếp) |
| 2 | Người được hỏi | Câu hỏi | Nhớ lại hoặc tìm lại câu trả lời cũ | ? | Chưa rõ có phải tìm lại hay nhớ ngay |
| 3 | Người được hỏi | Câu trả lời cũ | Giải thích lại từ đầu | 30 phút–1 giờ/lần (ước lượng) | Bước tốn thời gian nhất |
| 4 | Người hỏi | Lời giải thích | Làm thử, hỏi tiếp nếu chưa hiểu | ? | Có thể kéo dài nếu chưa hiểu |

**Bottleneck chính:** Bước 3, giải thích lại từ đầu. *Cập nhật sau survey (mục 3.2):* phổ biến nhất khoảng 15–30 phút mỗi lần, 30–60 phút ở 3/10 người; khoảng 2 lần/tuần trung bình. Con số 30 phút–1 giờ ở sơ đồ là baseline ban đầu của bản nháp.

### 4.2. Quy trình tương lai

Mức chọn tạm thời: **No AI**. Bước nào cũng do con người, thêm một chỗ có sẵn câu trả lời (FAQ hoặc tin ghim). Chưa có bước nào do AI hoặc Rule xử lý.

```text
TƯƠNG LAI — No AI

[Người hỏi có câu hỏi] → [Tự tìm trong FAQ / tin ghim]  (con người)
     ├── Tìm thấy → xong
     └── Không thấy → [Hỏi người được hỏi] (con người)
                         → [Người được hỏi trả lời]
                         → [Thêm câu hỏi và câu trả lời mới vào FAQ]  (con người)

Boundary: không có AI ở quy trình này.
Phương án quay về: nếu người hỏi vẫn không tự tra được, người được hỏi giải thích trực tiếp như hiện tại.
Người kiểm tra: người duy trì FAQ rà lại nội dung hằng tuần (chưa xác định người).
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 4 | 2 khi FAQ có câu trả lời, 4 khi không | Kỳ vọng, chưa đo |
| Tổng thời gian | 30–60 phút/lần ở bản nháp; survey cho thấy phổ biến 15–30 phút (ước lượng) | ≤ 5 phút/lần khi có FAQ (mục tiêu đề xuất) | Cần đo thật trong pilot |
| Số bước thủ công | 3 | 1 khi FAQ có câu trả lời | Bước còn lại: người hỏi tự tra |
| Bottleneck chính | Giải thích lại từ đầu | Viết FAQ một lần, cập nhật khi có câu mới | |
| Rủi ro mới phát sinh | — | FAQ lỗi thời, người hỏi không đọc, không ai duy trì | Xem mục 8.1 |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Người được hỏi lại (thành viên trong nhóm học và làm việc), cùng đồng nghiệp và bạn học là người hỏi. |
| **Quy trình** | Người hỏi nhắn hoặc hỏi lại câu cũ, người được hỏi nhớ hoặc tìm lại câu trả lời rồi giải thích lại từ đầu, người hỏi làm thử và hỏi tiếp. |
| **Bottleneck** | Bước giải thích lại từ đầu, khoảng 30 phút–1 giờ mỗi lần (ước lượng). |
| **Impact** | Khoảng 0,5–2 giờ/tuần cho người được hỏi (ước lượng, từ 1–2 lần/tuần). Làm gián đoạn việc đang làm. Người hỏi phải chờ người được hỏi rảnh. |
| **Success Metric** (baseline → target, cách đo) | Thời gian người được hỏi bỏ ra cho một lần bị hỏi lại câu đã có: từ 30 phút–1 giờ xuống ≤ 5 phút (mục tiêu đề xuất). Cách đo: ghi số phút mỗi lần bị hỏi lại trong 2 tuần, trước và sau khi có FAQ. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Chưa dùng AI. Người được hỏi vẫn trả lời các câu mới chưa có trong FAQ. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- AI chỉ ra: có thể chỉ cần một trang FAQ và gửi link là đủ, chưa cần giải pháp khác. Đồng ý (ghi ở báo cáo cá nhân của Đỗ Cao Cường).
- AI chỉ ra: giả định "người hỏi chịu tự tra" chưa có bằng chứng. Đồng ý, đây là giả định #3 cần kiểm chứng bằng pilot (survey mới cho thấy ý định, chưa phải hành vi).
- Chưa ghi nhận phản biện từ các thành viên khác. Sẽ bổ sung ở đây nếu có.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **mơ hồ thấp, vận hành đơn giản** ("rule hoặc script — vùng ngọt" trong ma trận của khóa).

Vì sao: Cùng một câu hỏi lặp lại, nên câu trả lời đã biết và ổn định, không mơ hồ. Việc vận hành chỉ là tìm một câu trả lời có sẵn và gửi cho người hỏi, không cần gọi công cụ hay gây tác động ra ngoài. *(Nhận định này dựa trên giả định #4 "câu hỏi đủ giống nhau", chưa kiểm chứng.)*

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Viết một trang FAQ dùng chung hoặc ghim tin nhắn trả lời, gửi link khi bị hỏi lại | Khi câu hỏi đủ giống nhau và người hỏi chịu tự tra | FAQ lỗi thời, không ai duy trì | **Chọn** |
| **Rule** | Gắn từ khóa để tự gửi đúng mục FAQ (ví dụ phản ứng emoji kích hoạt tin nhắn trả lời sẵn, như Slack Workflow Builder) | Khi có nhiều câu hỏi và người hỏi ngại tự tìm | Cần cấu hình công cụ, chỉ chạy được trên nền tảng hỗ trợ | Chưa |
| **Workflow** | Các bước cố định: nhận câu hỏi, tìm trong FAQ, trả lời, ghi lại câu mới | Khi số câu hỏi lớn và cần ghi nhận để cập nhật FAQ | Đắt hơn, khó test hơn, cần người vận hành | Chưa |
| **Agent** | Mô hình tự chọn bước và công cụ để trả lời | Gần như không có tình huống phù hợp ở quy mô này | Khó kiểm soát, có thể trả lời sai với giọng chắc chắn | Không |

**Mức chọn:** No AI.

**Vì sao không chọn mức đơn giản hơn:** Không có mức nào đơn giản hơn No AI. Quan trọng hơn, phần tiếp theo là vì sao **không lên mức cao hơn**: chưa có bằng chứng đo được rằng FAQ viết tay không đủ. Theo quy tắc của khóa, chỉ lên mức cao hơn khi có thứ gì đó đo được tốt lên để đáng đổi lấy chi phí.

### 6.3. AI Canvas rút gọn

*Bài toán hiện chọn No AI, nên canvas dưới đây chỉ áp dụng nếu CP4 cho thấy FAQ không đủ và nhóm cân nhắc thêm một bước AI.*

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | (Giả định) Tìm mục FAQ phù hợp nhất với câu hỏi của người hỏi. Không tự viết câu trả lời mới ngoài FAQ. |
| **Judgment** — con người cân nhắc, quyết định gì? | Người được hỏi duyệt nội dung FAQ và quyết định có thêm câu mới vào FAQ hay không. |
| **Action** — hành động cuối cùng là gì, ai làm? | Người hỏi đọc mục FAQ được gợi ý. Nếu không giải quyết được thì hỏi người được hỏi. |
| **Outcome** — đo kết quả bằng gì? | Số lần bị hỏi lại câu đã có trong FAQ, và thời gian người được hỏi bỏ ra mỗi lần. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Câu hỏi của người hỏi và nội dung FAQ. FAQ chưa có, cần viết trước. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Câu hỏi nào vẫn bị hỏi lại, người hỏi có thấy câu trả lời hữu ích không. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: survey 10 người cho thấy 7/10 sẵn sàng dùng FAQ và 3/10 "có thể", không ai từ chối, nghĩa là người dùng chấp nhận được hỗ trợ (augment) hơn là giao hẳn việc. Đây vẫn là ý định nói ra, cần pilot để xem hành vi thật.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Nếu có AI, kiểu sai tệ hơn là **trả lời sai với giọng chắc chắn** (báo nhầm), vì người hỏi có thể làm theo câu trả lời sai mà không hỏi lại. Thiết kế nghiêng về tránh kiểu này: khi không chắc thì chuyển cho người, không tự trả lời ngoài FAQ. Với phương án No AI hiện tại, kiểu sai tương ứng là FAQ lỗi thời, xử lý bằng cách có người rà hằng tuần.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Người được hỏi lại (thành viên trong nhóm học và làm việc), cùng đồng nghiệp và bạn học là người hỏi. |
| **Quy trình** | Người hỏi tự tìm trong FAQ hoặc tin ghim. Nếu không thấy thì hỏi người được hỏi, người này trả lời và thêm câu mới vào FAQ. |
| **Bottleneck** | Giải thích lại từ đầu những câu đã từng trả lời, phổ biến khoảng 15–30 phút mỗi lần, nặng nhất 30–60 phút (survey 10 người). |
| **Impact** | Trung bình khoảng 65 phút/tuần/người, từ khoảng 4 lần mỗi 2 tuần × khoảng 25 phút/lần (ước lượng từ khoảng giá trị giữa của survey). Trưởng nhóm và kỹ sư phần mềm ở mức cao nhất. |
| **Success Metric** (baseline → target, cách đo) | Thời gian người được hỏi bỏ ra mỗi lần bị hỏi lại câu đã có trong FAQ: từ khoảng 15–30 phút xuống ≤ 5 phút. Số lần bị hỏi lại câu đã có: từ khoảng 1–2 lần/tuần xuống ≤ 1 lần/2 tuần (mục tiêu đề xuất). Cách đo: ghi nhận trong 2 tuần trước và 2 tuần sau khi có FAQ. |
| **Boundary** | Chưa dùng AI. Nếu sau này thêm AI, chỉ được tìm trong FAQ đã được người duyệt, không tự trả lời ngoài FAQ, câu không có trong FAQ chuyển cho người. Người duy trì FAQ rà nội dung hằng tuần. |
| **AI intervention point** | Chưa có ở phiên bản này (No AI). Điểm duy nhất có thể cân nhắc về sau: bước "tìm mục FAQ phù hợp", nếu FAQ lớn và người hỏi khó tìm. |
| **Mức chọn** | No AI |
| **Rủi ro & người kiểm tra** | FAQ lỗi thời hoặc sai: người duy trì FAQ rà hằng tuần *(chưa xác định ai)*. Người hỏi không chịu tự tra: người được hỏi theo dõi số lần bị hỏi lại. Số liệu thời gian là ước lượng: cần đo thật trong 2 tuần. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Quy trình | Mô tả quy trình hiện tại | Mô tả quy trình tương lai có FAQ | Cần chỉ ra chỗ nào thay đổi |
| Success Metric | Baseline 30 phút–1 giờ/lần, chỉ đo thời gian mỗi lần | Baseline sửa theo survey còn 15–30 phút/lần, thêm số lần bị hỏi lại câu đã có | Survey cho thấy 30–60 phút chỉ ở 3/10 người. Chỉ đo thời gian không cho biết FAQ có được dùng không |
| Bottleneck, Impact | 30 phút–1 giờ/lần, 0,5–2 giờ/tuần (ước lượng một người) | 15–30 phút/lần, khoảng 65 phút/tuần/người (survey 10 người) | Có dữ liệu từ người ngoài nhóm |
| Boundary | "Chưa dùng AI" | Thêm điều kiện nếu sau này thêm AI và người rà FAQ | Cần rõ AI được và không được làm gì, và ai kiểm tra |
| AI intervention point, Mức chọn, Rủi ro & người kiểm tra | (chưa có) | Thêm mới | Yêu cầu của v1 ở CP6 |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):** *Bài toán chọn No AI, nên các tiêu chí dưới đây áp dụng cho đầu ra của FAQ, và áp dụng nguyên cho AI nếu sau này thêm bước AI.*

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đúng nội dung | Câu trả lời trong FAQ khớp với điều người được hỏi sẽ giải thích | Câu trả lời sai hoặc lỗi thời |
| 2 | Tìm thấy nhanh | Người hỏi tìm được mục đúng trong ≤ 2 phút | Người hỏi không tìm được hoặc mất hơn 2 phút |
| 3 | Không bịa | Mọi câu trả lời đều có trong FAQ đã duyệt | Có câu trả lời không nằm trong FAQ |
| 4 | Chuyển người khi không chắc | Câu không có trong FAQ được chuyển cho người | Tự trả lời câu không có trong FAQ |
| 5 | Cập nhật | Câu hỏi bị hỏi lại ≥ 2 lần được thêm vào FAQ trong vòng 1 tuần | Câu hỏi lặp lại nhưng không được thêm vào |

*Ngưỡng 2 phút, 2 lần và 1 tuần là mục tiêu đề xuất, nhóm chỉnh sau khi có số đo thật.*

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Thấp | Survey 10 người: 10/10 từng bị hỏi lại, 7/10 từ 3 lần trong 2 tuần, 7/10 mất từ 15 phút mỗi lần. Mẫu nhỏ và có thể thiên lệch chọn mẫu. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | 7/10 sẵn sàng dùng FAQ, 3/10 "có thể", 0/10 từ chối. Nhưng đây là ý định nói ra, chưa phải hành vi, nên cần pilot (giả định #3). Với No AI thì không có đầu ra AI để sửa. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | FAQ viết tay hoặc ghim tin, không cần công nghệ đặc biệt. Cần gom các câu hỏi hay lặp lại (giả định #4 đã kiểm chứng một phần: 6/10 cho rằng câu hỏi hầu hết giống nhau). |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Trung bình | Chi phí gần như bằng 0, nhưng chưa có người duy trì FAQ (giả định #6). Không có vấn đề pháp lý hiển nhiên ở phương án No AI. |

### 8.2. Kết luận

**Quyết định:** **Go, phạm vi nhỏ** (pilot FAQ, mức No AI) *(bản nháp, chờ nhóm xác nhận)*

**Lý do:** Survey 10 người xác nhận pain có thật (10/10 từng gặp, 7/10 từ 3 lần trong 2 tuần), 7/10 mất từ 15 phút mỗi lần, 6/10 cho rằng câu hỏi hầu hết giống nhau và 0/10 từ chối dùng FAQ. Giải pháp FAQ gần như không tốn chi phí và chưa có bằng chứng cần AI. Rủi ro còn lại: mẫu nhỏ, thiên lệch chọn mẫu, và ý định dùng FAQ chưa phải hành vi. Vì vậy chỉ đi phạm vi nhỏ.

**Nếu Go — pilot nhỏ nhất:** Trong 2 tuần, viết một trang FAQ cho 5 câu hỏi hay bị hỏi lại nhất, ghim ở kênh chung và gửi link mỗi khi bị hỏi. Ghi số phút mỗi lần bị hỏi lại, trước và sau.

**Nếu Not Yet — cần kiểm chứng gì trước:** Pilot 2 tuần để xem người hỏi có thật sự tự tra FAQ không (giả định #3), và liệt kê cụ thể các câu hay bị hỏi lại để gom thành FAQ (giả định #4).

**Nếu No-Go — nên làm gì thay AI:** Nếu pilot cho thấy mỗi lần chỉ mất dưới 15 phút hoặc ít người hỏi lại, dừng việc này và quay lại shortlist (#8 hoặc #15) hoặc candidate khác.

**Ngưỡng dừng** (mục tiêu đề xuất): nếu sau 2 tuần có FAQ mà số lần bị hỏi lại câu đã có trong FAQ vẫn ≥ 1 lần/tuần, thì xem lại cách trình bày và chỗ đặt FAQ. Nếu sau 4 tuần vẫn không giảm, dừng phương án FAQ và cân nhắc mức Rule hoặc đổi problem. Nếu đo trong pilot cho thấy pain trung bình < 15 phút/lần, dừng và chọn candidate khác.

---

## 9. Hạn chế và hướng tiếp theo

- Survey chỉ có 10 người, cả 10 đều từng bị hỏi lại (có thể thiên lệch chọn mẫu), không có câu trả lời mở, và "sẵn sàng dùng FAQ" là ý định chứ chưa phải hành vi. Các số trung bình (4 lần/2 tuần, 25 phút/lần, 65 phút/tuần) là ước lượng từ khoảng giá trị giữa. Chưa có phỏng vấn.
- Điểm shortlist ở mục 2.4 là điểm nhóm đã chấm. Phiếu của từng cá nhân chưa được lưu đầy đủ trong báo cáo 
- Quy trình hiện tại và tương lai ở mục 4 là bản nháp, các bước và số phút chưa được quan sát trực tiếp.
- Ngưỡng ở mục 7 và 8 (≤ 5 phút, 2 tuần, 2 lần) là mục tiêu đề xuất, chưa có căn cứ đo.
- Phạm vi chỉ là việc bị hỏi lại, chưa phân biệt loại câu hỏi (kỹ thuật, quy trình, lịch học).
- Hướng tiếp theo: chọn người duy trì FAQ, chạy pilot 2 tuần và đo, thu thêm phiếu chấm cá nhân nếu cần.

## 10. Tài liệu tham khảo

- Slack, "4 simple ways to save time with Workflow Builder": https://slack.com/resources/using-slack/4-simple-ways-to-save-time-with-workflow-builder
- Notion, "Get answers about work content faster with Q&A" (trang hiển thị tiêu đề "…with Notion Agent"): https://www.notion.com/help/guides/get-answers-about-content-faster-with-q-and-a
- Slack, "Slack AI features & AI assistants": https://slack.com/intl/en-au/features/ai
- Rob Fitzpatrick, *The Mom Test* (3 luật phỏng vấn, theo hướng dẫn trong `docs/01-worksheet.md`).
- Google PAIR, *People + AI Guidebook* (hai câu hỏi augment/automate và báo nhầm/bỏ sót, theo hướng dẫn trong `docs/01-worksheet.md`).
