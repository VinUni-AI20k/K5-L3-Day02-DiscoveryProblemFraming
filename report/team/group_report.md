# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Nhom9999
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): (#7, Nguyễn Công Quân) Học viên học song song ở trường, khóa tiếng Anh và khóa AI mất khoảng 25 phút mỗi ngày để kiểm tra nhiệm vụ trên nhiều nền tảng và xếp thứ tự ưu tiên, nên khoảng 4 lần/tháng phải làm gấp sát deadline.
- Quyết định cuối: Go, phạm vi nhỏ: pilot 6 tuần ở mức Rule, không dùng AI; hai bước AI (gợi ý thứ tự, trích nhiệm vụ từ thông báo): Not Yet (xem mục 8).

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Vũ Quang Minh | Khi luyện nghe tiếng Anh, tôi muốn tìm được bài nghe vừa trình độ, để không phí thời gian vào bài quá khó hoặc đã nghe | Sinh viên tự luyện nghe tiếng Anh ở nhà | Xem tiêu đề video rồi nghe thử, không hợp lại chọn bài khác (lặp nhiều lần): ~25 phút trong tổng ~30 phút tìm bài mỗi buổi, 7 buổi/tuần |Bạn dựa vào tiêu chí nào để xác định một bài nghe vừa trình độ? Nếu chỉ mất 25 phút tìm bài nhưng sau đó vẫn luyện nghe được thì vấn đề này có thực sự nghiêm trọng không? (Người hỏi: Hà Huy Thái)|
| 2 | Vũ Quang Minh | Khi luyện nói, tôi muốn biết mình phát âm một từ đúng hay sai, để không mang lỗi sai vào giao tiếp thật | Sinh viên tự luyện nói tiếng Anh một mình | Nghe lại bản ghi âm để so với mẫu: bình thường ~5 phút/buổi; lần gần nhất phải nghe lại 5 lần, mất ~30 phút |Làm sao bạn xác định phát âm đúng hay sai khi nghe lại bản ghi âm? Bạn có chắc việc nghe lại nhiều lần là do thiếu công cụ đánh giá chứ không phải do chưa biết cách phát âm? (Người hỏi: Nguyễn Công Quân)|
| 3 | Vũ Quang Minh | Khi viết xong một đoạn tiếng Anh, tôi muốn biết câu nào sai ngữ pháp và vì sao, để không lặp lại lỗi | Sinh viên tự luyện viết tiếng Anh | Tự soát lỗi: 10 phút/bài mà vẫn sót ~10 lỗi (người chấm chỉ ra sau khi nộp) |Bạn thường mắc những lỗi ngữ pháp nào và tại sao không tự nhận ra được? Nếu sử dụng công cụ kiểm tra ngữ pháp, liệu bạn có hiểu nguyên nhân để tránh lặp lại lỗi không? (Người hỏi: Hà Huy Thái)|
| 4 | Hà Huy Thái | Khi chuẩn bị nộp bài thực hành, tôi muốn biết còn thiếu file hay mục nào, để tránh nộp bài chưa đầy đủ | Sinh viên làm và nộp bài thực hành | So từng yêu cầu với từng file, dễ bỏ sót (chưa đo số phút) |Những yêu cầu nộp bài có được giảng viên cung cấp rõ ràng từ đầu không? Bạn thường bỏ sót file do không đọc kỹ yêu cầu hay do có quá nhiều file và định dạng khác nhau? (Người hỏi: Vũ Quang Minh)|
| 5 | Hà Huy Thái | Khi chương trình Python báo lỗi, tôi muốn hiểu lỗi và biết cần sửa chỗ nào, để tiếp tục làm bài | Sinh viên đang học Python/AI | Đọc lỗi và tìm nguyên nhân (chưa đo số phút) |Bạn gặp khó khăn ở việc hiểu thông báo lỗi hay tìm cách sửa lỗi? Nếu có công cụ giải thích lỗi nhưng bạn vẫn không hiểu kiến thức Python nền tảng thì vấn đề có được giải quyết không? (Người hỏi: Nguyễn Công Quân)|
| 6 | Hà Huy Thái | Khi train mô hình nhiều lần, tôi muốn xem lại kết quả từng lần, để chọn cấu hình phù hợp | Người học và làm bài thực hành AI | Kết quả để ở nhiều nơi nên khó so sánh (chưa đo số phút) |Bạn dựa vào những tiêu chí nào để so sánh kết quả giữa các lần train? Việc khó theo dõi kết quả có thường xuyên ảnh hưởng đến quyết định chọn mô hình hay chỉ gây bất tiện? (Người hỏi: Vũ Quang Minh)|
| 7 | Nguyễn Công Quân | Khi bắt đầu một ngày có nhiều nhiệm vụ từ trường, khóa tiếng Anh và khóa AI, tôi muốn biết việc nào cần ưu tiên và hạn của từng việc, để không phải làm gấp sát deadline | Học viên học song song ở trường, trung tâm tiếng Anh và khóa AI | Xếp thứ tự ưu tiên: ~8 phút trong tổng ~25 phút/ngày kiểm tra nhiệm vụ (hậu quả: ~4 lần/tháng phải làm gấp sát deadline) |Bạn đang quản lý deadline bằng cách nào và tại sao cách đó chưa hiệu quả? Việc làm gấp sát deadline là do không biết thứ tự ưu tiên hay do khối lượng công việc quá nhiều và thiếu thời gian? (Người hỏi: Hà Huy Thái)|
| 8 | Nguyễn Công Quân | Khi quay lại báo cáo đang làm dở, tôi muốn biết đã làm đến đâu và bước tiếp theo, để tiếp tục ngay | Học viên chuyển qua lại giữa báo cáo ở trường, bài tiếng Anh và bài lab | Đọc lại phần đã viết: ~4 phút trong tổng ~10 phút mỗi lần quay lại, 3 lần/tuần |Tại sao bạn mất thời gian khi quay lại công việc đang làm dở? Nếu có ghi chú tiến độ và việc tiếp theo, bạn có thực sự tiếp tục nhanh hơn hay vẫn cần đọc lại toàn bộ nội dung để nhớ ngữ cảnh? (Người hỏi: Vũ Quang Minh)|
| 9 | Nguyễn Công Quân | Khi tổng hợp chi tiêu trong tháng, tôi muốn phân loại giao dịch ngân hàng, để biết tiền đã đi đâu | Người tự theo dõi chi tiêu cá nhân | Nhớ lại mục đích từng giao dịch: ~15 phút trong tổng ~30 phút mỗi lần tổng hợp, 2 lần/tháng |Bạn có thường xuyên không nhớ mục đích của các giao dịch ngân hàng không? Nếu có thể tự phân loại giao dịch bằng ghi chú ngay lúc chi tiêu thì vấn đề tổng hợp cuối tháng có còn xảy ra không? (Người hỏi: Hà Huy Thái)|

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Học tập và cải thiện kỹ năng | #1 Tìm bài nghe phù hợp trình độ; #2 Kiểm tra phát âm; #3 Soát lỗi ngữ pháp | Sinh viên gặp khó khăn khi tự đánh giá năng lực, phát hiện lỗi và cải thiện kỹ năng học tập mà không có người hướng dẫn trực tiếp |
| B — Hỗ trợ thực hành và quản lý kết quả học tập | #4 Kiểm tra đủ file trước khi nộp; #5 Hiểu và sửa lỗi Python; #6 Theo dõi kết quả train mô hình | Sinh viên gặp khó khăn khi xử lý, kiểm tra và theo dõi các bước trong quá trình thực hành, dẫn đến mất thời gian và dễ mắc sai sót |
| C — Quản lý công việc và thông tin cá nhân | #7 Quản lý nhiệm vụ và deadline; #8 Tiếp tục công việc đang làm dở; #9 Phân loại giao dịch chi tiêu | Người dùng gặp khó khăn trong việc tổng hợp thông tin, ghi nhớ trạng thái và đưa ra quyết định khi có nhiều dữ liệu hoặc nhiệm vụ cần xử lý |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

Outcome gắn với candidate #7 vì vấn đề có số liệu cụ thể, tần suất xảy ra và hậu quả tương đối rõ ràng.

```text
OUTCOME: Giảm tình trạng phải làm gấp sát deadline của học viên
├── Opportunity A:
│   Khó xác định nhiệm vụ nào cần ưu tiên khi có nhiều
│   công việc từ trường, trung tâm tiếng Anh và khóa AI.
│
├── Opportunity B:
│   Khó nắm bắt deadline của các nhiệm vụ khi thông tin
│   được phân tán ở nhiều nguồn khác nhau.
│
└── Opportunity C:
    Khó duy trì tiến độ và cân đối thời gian giữa nhiều
    nhiệm vụ có mức độ quan trọng và thời hạn khác nhau.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ~~Tạo chatbot nhắc nhở deadline~~
- ~~Xây dựng ứng dụng quản lý công việc~~
- ~~Tự động sắp xếp lịch học bằng AI~~
- ~~Tạo dashboard hiển thị danh sách nhiệm vụ~~
- ~~Sử dụng AI Agent để phân tích và phân chia công việc~~

Lý do: đây đều là những cách giải quyết vấn đề (solution), chưa phải nhu cầu hoặc khó khăn thực tế của người dùng (opportunity).

### 2.4. Chấm điểm shortlist (1–5)

Shortlist gồm 3 candidate: #7, #5 và #8.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #7 Quản lý nhiệm vụ và deadline | 5 | 5 | 5 | 5 | 4 | 5 | 5 | **34** |
| #5 Hiểu và sửa lỗi Python | 5 | 4 | 3 | 3 | 4 | 5 | 5 | 29 |
| #8 Tiếp tục công việc đang làm dở | 5 | 4 | 4 | 4 | 5 | 5 | 5 | 32 |

Giải thích điểm:

- **#7 – Quản lý nhiệm vụ và deadline:** có actor cụ thể, quy trình rõ ràng, mất khoảng 8 phút mỗi ngày để sắp xếp thứ tự ưu tiên và có khoảng 4 lần/tháng phải làm gấp sát deadline. Đây là candidate có bằng chứng pain tốt nhất.
- **#5 – Hiểu và sửa lỗi Python:** vấn đề khá rõ và phù hợp với AI Lab, nhưng chưa có số liệu về thời gian tìm lỗi hoặc tần suất gặp lỗi nên impact chưa được chứng minh đầy đủ.
- **#8 – Tiếp tục công việc đang làm dở:** có số liệu cụ thể là mất khoảng 10 phút mỗi lần quay lại (riêng bước đọc lại phần đã viết ~4 phút), xảy ra 3 lần/tuần. Phạm vi tương đối rõ và có thể thử nghiệm bằng nhiều phương pháp khác nhau.

**Candidate được chọn:** #7 — Quản lý nhiệm vụ và deadline từ nhiều nền tảng (Nguyễn Công Quân)

**Vì sao chọn:**

- Pain có số liệu cụ thể về thời gian và tần suất.
- Hậu quả thực tế là phải làm gấp sát deadline.
- Có nhiều hướng tiếp cận để so sánh No AI, Rule-based, Workflow và AI Agent.
- Thành viên nhóm có thể dễ dàng hiểu và kiểm chứng vấn đề trong môi trường học tập thực tế.

**Vì sao loại các candidate còn lại:**

- **#5:** chưa có số liệu về thời gian tìm lỗi hoặc tần suất gặp lỗi, nên impact chưa được chứng minh.
- **#8:** vấn đề có số liệu về thời gian và tần suất, nhưng mức độ ảnh hưởng chưa thực sự nghiêm trọng. Việc mất khoảng 10 phút mỗi lần quay lại công việc (3 lần/tuần, khoảng 30 phút/tuần) chủ yếu gây gián đoạn và mất thời gian, chưa chứng minh được hậu quả lớn hoặc ảnh hưởng rõ rệt đến kết quả học tập.

**Xử lý bất đồng (nếu có):** Không có. Cả nhóm đồng ý chọn #7.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 |Thông tin nhiệm vụ phân tán khiến học viên mất thời gian kiểm tra và dễ bỏ sót hoặc phát hiện muộn deadline.|Value|5|2|Có|
| 2 |Khó xác định thứ tự ưu tiên góp phần khiến học viên làm gấp sát deadline, bên cạnh thiếu thời gian và trì hoãn.|Value|5|2|Có|
| 3 |Vấn đề xuất hiện ở nhiều học viên học song song các chương trình, không chỉ người đưa ra candidate #7.|Value|5|1|Có|
| 4 |Người học có thể duy trì cập nhật và điều chỉnh danh sách nhiệm vụ tập trung mà không thấy quá phiền.|Usability|4|1|Sau khi có thử nghiệm|
| 5 |Nhóm có thể lấy được tên nhiệm vụ, deadline và nguồn giao bài đủ chính xác từ dữ liệu người học cung cấp trong phạm vi lab.|Feasibility|5|1|Có|
| 6 |Thời gian tiết kiệm lớn hơn thời gian nhập liệu, kiểm tra và sửa thông tin của giải pháp.|Viability|4|1|Sau khi có thử nghiệm|

Giả định nhóm kiểm chứng trong buổi này: #1, #2 và #3.

Mục tiêu là phân biệt ba nguyên nhân: thông tin phân tán, khó xếp ưu tiên và thiếu thời gian. Nhóm chưa mặc định rằng cần xây ứng dụng mới hoặc sử dụng AI Agent.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn trực tiếp ba học viên học song song nhiều chương trình vào ngày 09/11/2026, tập trung vào lần gần nhất phải làm gấp, cách quản lý hiện tại và nguyên nhân bắt đầu muộn.

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) |Học viên A (không thuộc nhóm), học song song ở trường, trung tâm tiếng Anh và khóa AI; cùng bối cảnh với candidate #7. Phỏng vấn trực tiếp ngày 09/11/2026.|
| Câu nói đáng nhớ nhất (nguyên văn) |"Mình phải mở từng chỗ để xem có bài gì, nhưng xem xong vẫn phân vân nên làm bài nào trước."|
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? |Học viên ưu tiên báo cáo ở trường mà chưa kiểm tra lại hạn bài lab AI. Đến tối trước hạn nộp mới nhận ra bài lab còn nhiều phần chưa làm và phải hoàn thành gấp.|
| Hiện đang xử lý bằng cách nào (workaround)? |Mở từng nền tảng, xem lại thông báo, ghi một số việc vào ghi chú điện thoại và tự chọn việc cần làm trước. Danh sách chưa được cập nhật đều.|
| Mất bao lâu, bao lần? |Khoảng 25 phút/ngày, trong đó 8 phút xếp ưu tiên; khoảng 4 lần/tháng làm gấp.|
| Insight / opportunity rút ra |Cần giảm công sức kiểm tra nhiều nguồn và giúp người học nắm đồng thời hạn nộp, phần việc còn lại trước khi chọn ưu tiên.|

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) |Học viên B, đang học đại học và một khóa tiếng Anh. Phỏng vấn trực tiếp ngày 09/11/2026.|
| Câu nói đáng nhớ nhất (nguyên văn) |"Mình nhớ hạn nộp, nhưng cứ chọn bài dễ làm trước, đến lúc làm bài lớn mới biết không đủ thời gian."|
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? |Học viên hoàn thành nhiều bài tập ngắn trước rồi mới bắt đầu bài thuyết trình. Dù biết deadline, học viên đánh giá thấp thời gian chuẩn bị và phải làm gấp vào tối cuối.|
| Hiện đang xử lý bằng cách nào (workaround)? |Ghi deadline vào lịch điện thoại nhưng chưa ghi thời lượng dự kiến hoặc chia nhỏ bài lớn.|
| Mất bao lâu, bao lần? |Khoảng 15 phút/ngày kiểm tra và chọn việc, trong đó khoảng 5 phút xếp ưu tiên; khoảng 2 lần/tháng làm gấp.|
| Insight / opportunity rút ra |Nhớ deadline chưa đủ. Người học còn cần nhận biết khối lượng còn lại và thời điểm nên bắt đầu nhiệm vụ lớn.|

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) |Học viên C, đang học đại học và khóa AI, đồng thời có công việc bán thời gian. Phỏng vấn trực tiếp ngày 09/11/2026.|
| Câu nói đáng nhớ nhất (nguyên văn) |"Mình có danh sách và biết bài nào cần làm trước, nhưng hôm đi làm về thì không còn đủ thời gian."|
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? |Ca làm thêm kéo dài khiến học viên không thực hiện được kế hoạch làm bài đã đặt ra. Học viên phải dồn phần còn lại vào ngày sát hạn.|
| Hiện đang xử lý bằng cách nào (workaround)? |Dùng danh sách nhiệm vụ tập trung, ghi deadline và chọn trước công việc cho ngày hôm sau.|
| Mất bao lâu, bao lần? |Khoảng 5–10 phút/ngày kiểm tra và điều chỉnh kế hoạch; khoảng 3 lần/tháng làm gấp, chủ yếu do thời gian rảnh bị thu hẹp.|
| Insight / opportunity rút ra |Quản lý thông tin và ưu tiên không giải quyết được toàn bộ tình trạng làm gấp. Cần nhận diện trường hợp khối lượng công việc vượt thời gian có thể dành cho học tập.|

Tổng hợp: Hai trong ba tình huống (A và B) minh họa khó khăn trong việc tổng hợp nhiệm vụ, lựa chọn ưu tiên hoặc ước lượng thời gian thực hiện. Tình huống C đưa ra tín hiệu phản bác: người học vẫn có thể làm gấp dù đã biết deadline và thứ tự ưu tiên, do thời gian học bị hạn chế bởi công việc khác. Vì vậy, nhóm cần kiểm tra đồng thời yếu tố thông tin phân tán, cách lựa chọn ưu tiên và quỹ thời gian thực tế, thay vì mặc định việc làm gấp chỉ do quản lý deadline chưa hiệu quả.

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
|Mô tả candidate #7 trong CP3|1 người tự báo cáo|Có ước lượng thời gian kiểm tra, xếp ưu tiên và tần suất làm gấp.|Chưa có log hoặc tình huống cụ thể để xác định nguyên nhân.|
|Snapshot A |1 tình huống|Minh họa khả năng thông tin phân tán và khó chọn ưu tiên cùng góp phần gây làm gấp.|Việc không cập nhật ghi chú cũng có thể liên quan đến thói quen sử dụng.|
|Snapshot B |1 tình huống|Minh họa khó khăn chọn ưu tiên và ước lượng công sức dù đã biết deadline.|Không ủng hộ giả định rằng bỏ sót deadline luôn là nguyên nhân chính.|
|Snapshot C |1 tình huống|Minh họa nhu cầu cân đối nhiệm vụ với thời gian rảnh.|Cho thấy vẫn có thể làm gấp dù đã có danh sách và biết thứ tự ưu tiên.|

**Nhóm đã sửa problem thế nào sau kiểm chứng: không quy toàn bộ tình trạng làm gấp cho việc kiểm tra nhiều nền tảng: Học viên học song song ở trường, trung tâm tiếng Anh và khóa AI gặp khó khăn khi tổng hợp nhiệm vụ và lựa chọn việc cần làm trước dựa trên deadline, khối lượng còn lại và thời gian rảnh. Candidate #7 tự báo cáo dành khoảng 25 phút/ngày cho kiểm tra và xếp ưu tiên, trong đó 8 phút cho xếp ưu tiên, đồng thời khoảng 4 lần/tháng phải làm gấp sát deadline. Cần xác định mức đóng góp của khó khăn quản lý thông tin so với thiếu thời gian và trì hoãn.**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Todoist — Quick Add + Calendar integration** | [Quick Add — Todoist Help](https://www.todoist.com/help/todoist/features/use-task-quick-add-in-todoist-va4Lhpzz); [Calendar integration — Todoist Help](https://www.todoist.com/help/todoist/integrations/use-the-calendar-integration-rCqwLCt3G) | Tập trung nhiệm vụ vào một inbox; gắn deadline, priority, label, reminder; xem nhiệm vụ cùng lịch Google/Outlook. | Quick Add nhận ngày, deadline và priority từ nội dung nhập; có phím tắt để ghi nhanh khi đang ở ứng dụng khác. Đây là mức can thiệp đơn giản, dễ pilot. | Người dùng vẫn phải tự nhận biết và nhập nhiệm vụ từ Zalo, Discord, Cohort hoặc web khóa học. Calendar integration không biến sự kiện lịch bên ngoài thành task; việc kết nối lịch cũng cần cấp quyền. | Thử trước một “single source of truth” và quy tắc nhập task thủ công; đo xem riêng thay đổi quy trình có giảm thời gian và số lần làm gấp hay không trước khi thêm AI. |
| **Zapier — Discord → Todoist** | [Discord + Todoist integration — Zapier](https://zapier.com/apps/discord/integrations/todoist); [Pricing — Zapier](https://zapier.com/pricing) | Nối trigger Discord "New Message Posted to Channel" (tin nhắn mới trong một kênh cụ thể) hoặc "New Mention" với action Todoist "Create Task" để tự tạo task. | Trigger và action có sẵn, không cần tự viết code; giảm bước đọc lại và chép nhiệm vụ từ một nguồn cụ thể. | Trang tích hợp chỉ cho thấy luồng Discord–Todoist; Zalo, ứng dụng tiếng Anh, Cohort và web khóa học vẫn cần connector hoặc cách nhập khác. Trigger theo kênh bắt mọi tin nhắn mới nên có nguy cơ biến message không phải nhiệm vụ thành task. Theo trang giá, gói Free kiểm tra dữ liệu mới 15 phút/lần và không có Filter (Filter & Paths chỉ có từ gói Professional). | Chỉ pilot với một kênh Discord có cấu trúc rõ. Gói Free không lọc được theo keyword, nên bắt buộc người dùng duyệt task trước khi đưa vào danh sách ưu tiên. Không nên tự động gom mọi message. |
| **Motion — Auto-scheduling** | [Auto-scheduling — Motion Help Center](https://www.usemotion.com/help/time-management/auto-scheduling); [How auto-scheduling works — Motion Help Center](https://www.usemotion.com/help/time-management/auto-scheduling/reference-auto-scheduling/how-auto-scheduling-works-behind-the-scenes) | Sau khi nhiệm vụ đã được tập trung, hệ thống xếp lịch dựa trên duration, deadline, priority, thời gian rảnh và tự sắp lại khi lịch thay đổi. | Giải trực tiếp bottleneck xếp thứ tự/lịch làm; có cảnh báo khi task có nguy cơ trễ và tự điều chỉnh theo thay đổi lịch. | Không tự giải quyết đầy đủ bước lấy nhiệm vụ từ các nguồn của nhóm. Kết quả phụ thuộc vào deadline, duration và priority được nhập đúng; tự sắp lịch sai có thể khiến người dùng tin vào một kế hoạch không phù hợp. | Chỉ cân nhắc mức AI/optimization sau khi dữ liệu task đầu vào đã đủ và đúng; luôn cho người dùng xem, sửa, tắt auto-scheduling hoặc đổi priority. |

**Phạm vi kiểm tra nguồn:** các link trên là tài liệu chính thức, trang tích hợp hoặc trang giá của nhà cung cấp. Đã mở lại toàn bộ link ngày 09/11/2026: tất cả đều truy cập được và nội dung khớp với phần trích trong bảng. Các tính năng mới được kiểm trên tài liệu, chưa thử với tài khoản và kênh dữ liệu thực tế của nhóm; việc này để lại cho bước pilot.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 4 bước, khoảng 25 phút/ngày (dao động 15–30 phút), 4/4 bước thủ công

[1. Mở và kiểm tra 5 nền tảng: 7']
→ [2. Liệt kê nhiệm vụ: 5']
→ [3. Kiểm tra deadline và khối lượng: 5']
→ [4. Xếp thứ tự ưu tiên: 8'] ← BOTTLENECK
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Học viên | Zalo, Discord, ứng dụng tiếng Anh, Cohort và web khóa học | Các thông báo và nội dung có thể chứa nhiệm vụ | Khoảng 7 phút, mỗi ngày | Mở lần lượt 5 nguồn; hoàn toàn thủ công. |
| 2 | Học viên | Nội dung vừa đọc và ghi nhớ tạm thời | Danh sách nhiệm vụ ban đầu | Khoảng 5 phút, mỗi ngày | Tự nhận biết đâu là nhiệm vụ và chép lại; chưa có nơi tập trung được cập nhật đều. |
| 3 | Học viên | Danh sách nhiệm vụ và thông tin ở từng nguồn | Danh sách có deadline và ước lượng khối lượng còn lại | Khoảng 5 phút, mỗi ngày | Có thể phải quay lại nguồn nếu thiếu deadline hoặc yêu cầu. |
| 4 | Học viên | Deadline, khối lượng còn lại và thời gian rảnh trong ngày | Thứ tự công việc dự kiến thực hiện | Khoảng 8 phút, mỗi ngày | **Bottleneck:** phải cân nhắc nhiều yếu tố bằng trí nhớ; không có handoff, học viên tự quyết định và tự thực hiện. |

**Bottleneck chính:** Bước 4 — xác định và xếp thứ tự việc cần làm trước, khoảng 8 phút/ngày. Học viên phải so sánh đồng thời deadline, khối lượng còn lại và thời gian rảnh; CP4 cũng cho thấy chỉ biết deadline chưa đủ và thiếu thời gian vẫn có thể làm kế hoạch thất bại.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI (GIẢ THUYẾT ĐỂ ĐÁNH GIÁ Ở CP6) — 5 bước, kỳ vọng tối đa 10 phút/ngày

[1. Đồng bộ danh sách tập trung + tạo task ứng viên từ Discord: ~1'] ← RULE/WORKFLOW
→ [2. Kiểm tra 4 nguồn chưa hỗ trợ và Quick Add task còn thiếu: ~4'] ← CON NGƯỜI
→ [3. Kiểm tra trường bắt buộc, gắn cờ thiếu deadline/thời lượng: ~1'] ← RULE
→ [4. Đề xuất thứ tự/lịch làm từ deadline, thời lượng và thời gian rảnh: ~1'] ← AI/OPTIMIZATION
→ [5. Kiểm tra task, sửa dữ liệu và chốt kế hoạch: ~3'] ← CON NGƯỜI

BOUNDARY: Workflow/AI không tự thay đổi deadline chính thức, không tự xóa hoặc đánh dấu
hoàn thành nhiệm vụ, không tự chốt thứ tự cuối và không gửi/nộp bài thay học viên.
Mọi task được nhập tự động và lịch đề xuất phải được học viên kiểm tra trước khi dùng.

PHƯƠNG ÁN QUAY VỀ: nếu tích hợp hoặc AI sai/ngừng hoạt động, học viên dùng danh sách
tập trung như checklist/lịch chung, nhập task bằng Quick Add và tự sắp theo deadline,
khối lượng, thời gian rảnh. Nếu Discord tạo task rác, tắt workflow và nhập thủ công.
```

Đây là quy trình tương lai giả thuyết, chưa phải quyết định chọn AI. Các mốc thời gian sau là kỳ vọng cần đo bằng cách bấm giờ trong pilot; CP6 phải so sánh phương án này với No AI và Rule trước khi chốt mức can thiệp.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 4 | 5 | Tách bước kiểm tra dữ liệu và bước con người phê duyệt để giữ quyền kiểm soát. |
| Tổng thời gian | Khoảng 25 phút/ngày, dao động 15–30 phút | Kỳ vọng tối đa 10 phút/ngày | Target từ Problem Card #1; phải đo lại khi pilot. |
| Số bước thủ công | 4/4 | 2/5 | Con người vẫn kiểm tra các nguồn chưa hỗ trợ và chốt kế hoạch cuối. |
| Bottleneck chính | Xếp thứ tự ưu tiên, khoảng 8 phút | Kiểm tra dữ liệu và chốt kế hoạch, kỳ vọng khoảng 3 phút | Bottleneck mới là điểm kiểm soát cần giữ, không nên tự động hóa hoàn toàn. |
| Rủi ro mới phát sinh | Chưa có rủi ro tự động hóa; dễ quên hoặc phát hiện muộn task | Bỏ sót nguồn chưa hỗ trợ; Discord tạo task rác; deadline/thời lượng nhập sai; AI xếp lịch không phù hợp | Giảm rủi ro bằng cờ thiếu dữ liệu, bước duyệt của con người, quyền tắt workflow và phương án quay về. |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Học viên học song song từ hai chương trình trở lên (trường, trung tâm tiếng Anh, khóa AI). Họ nhận nhiệm vụ từ nhiều nền tảng (với candidate #7 là 5 nền tảng: Zalo, Discord, ứng dụng tiếng Anh, Cohort, web khóa AI) và mỗi ngày tự quyết nên làm việc nào trước. Bằng chứng: candidate #7 (Quân) và 3 học viên được phỏng vấn ở CP4 (A, B, C). |
| **Quy trình** | Đầu ngày hoặc trước mỗi phiên học, tổng khoảng 25 phút/ngày (dao động 15–30): (1) mở lần lượt 5 nền tảng xem thông báo mới: 7' → (2) liệt kê nhiệm vụ vào ghi chú: 5' → (3) kiểm tra deadline và khối lượng từng việc: 5' → (4) xếp thứ tự ưu tiên, chọn việc làm hôm nay: 8'. Sau đó học viên làm theo thứ tự đã chọn (không tính vào 25 phút). Các bước và số phút khớp với mục 4.1, lấy từ quy trình nháp của candidate #7 (báo cáo cá nhân của Quân, CP2). |
| **Bottleneck** | Bước 4, xếp thứ tự ưu tiên: khoảng 8 phút/ngày. Đây là bước quyết định làm việc nào trước, nhưng đầu vào thường thiếu. Danh sách ở bước 1–2 có thể sót việc ở nền tảng chưa mở lại (A ưu tiên báo cáo ở trường vì chưa kiểm lại hạn bài lab AI). Ở bước 3, khối lượng còn lại chỉ được ước lượng theo cảm tính và chưa đối chiếu với thời gian rảnh thực tế (B biết hạn nhưng đánh giá thấp thời gian chuẩn bị bài thuyết trình). Bước 1–2 tốn nhiều phút hơn (12') nhưng chỉ là chi phí thời gian; bước 4 mới là nơi chọn sai dẫn đến làm gấp. |
| **Impact** | Candidate #7 mất khoảng 25 phút/ngày (khoảng 175 phút/tuần) chỉ để kiểm tra và chọn việc, và khoảng 4 lần/tháng phải làm gấp sát deadline nên kết quả chưa đầy đủ. Cả 3 người được phỏng vấn cũng làm gấp 2–4 lần/tháng (A: 4, B: 2, C: 3). Chưa tách được bao nhiêu lần làm gấp do thông tin phân tán hoặc chọn ưu tiên sai, bao nhiêu lần do thiếu thời gian (C vẫn làm gấp dù đã có danh sách và biết thứ tự). |
| **Success Metric** (baseline → target, cách đo) | **Chính, số lần làm gấp:** baseline khoảng 4 lần/tháng (candidate #7 tự ước lượng theo trí nhớ tháng gần nhất) → target tối đa 1 lần/tháng.<br>**Phụ, thời gian kiểm tra và xếp ưu tiên:** baseline khoảng 25 phút/ngày (tự ước lượng, dao động 15–30) → target tối đa 10 phút/ngày.<br>**Cách đo:** (a) bấm giờ mỗi lần kiểm tra, từ lúc mở nền tảng đầu tiên đến lúc chốt việc làm hôm nay; (b) nhật ký deadline, mỗi nhiệm vụ một dòng: ngày giao, ngày biết đến, hạn, ngày bắt đầu, ngày xong, có làm gấp không. "Làm gấp" là khi phần lớn khối lượng phải làm trong 24 giờ cuối trước hạn, hoặc nộp chưa đủ phần yêu cầu. Ghi 2 tuần trước khi thay đổi quy trình để có baseline đo thật, rồi so với 4 tuần sau khi thay đổi. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | **AI (nếu nhóm chọn dùng ở CP6) không được:** tự quyết thứ tự ưu tiên hay việc làm hôm nay (chỉ được đề xuất kèm lý do); tự thêm, sửa hoặc xoá nhiệm vụ và deadline trong danh sách chính khi người học chưa xác nhận; tự đoán deadline khi thông báo không ghi rõ (phải đánh dấu "chưa rõ hạn"); tự gửi tin nhắn, nộp bài hay trả lời giảng viên và nhóm trên bất kỳ nền tảng nào; đọc tin nhắn cá nhân ngoài các kênh và thông báo người học chủ động đưa vào.<br>**Con người kiểm tra (HITL) khi:** (1) có nhiệm vụ mới, trước khi đưa vào danh sách ưu tiên: xác nhận tên, hạn, nguồn; (2) deadline chưa rõ hoặc hai nguồn ghi khác nhau: mở thông báo gốc để đối chiếu; (3) nhiệm vụ còn dưới 48 giờ đến hạn, hoặc khối lượng còn lại có thể vượt thời gian rảnh trước hạn: người học tự quyết chia nhỏ, cắt bớt hay xin gia hạn. Ước lượng khối lượng và thời gian rảnh luôn do người học đưa ra hoặc xác nhận, AI không tự ước lượng thay. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

Cách phản biện: nhờ Claude đóng vai "PM hoài nghi", đối chiếu bản nháp Problem Statement v0 với kết quả kiểm chứng ở mục 3 và checklist CP5. Các điểm "sửa ngay ở v0" đã có trong bảng trên; các điểm "đưa vào v1" để lại cho CP6.

| # | Điểm AI phản biện | Đồng ý? | Xử lý |
|---:|---|---|---|
| 1 | Cả hai baseline (25 phút/ngày, 4 lần/tháng) là ước lượng theo trí nhớ của 1 người, chưa có log. Nếu baseline sai thì đạt target 4 → 1 cũng không chứng minh được gì. | Đồng ý | Sửa ngay ở v0: ghi rõ nguồn và tính chất tự ước lượng của baseline; thêm 2 tuần ghi nhật ký và bấm giờ trước khi thay đổi quy trình để có baseline đo thật. |
| 2 | Số lần làm gấp/tháng phụ thuộc số deadline trong tháng: tháng ít bài thì tự giảm mà không nhờ thay đổi gì. Ngoài ra C làm gấp vì thiếu thời gian, nguyên nhân mà việc tổng hợp hay xếp ưu tiên không chạm tới. | Đồng ý | Đưa vào v1 (CP6): đổi metric chính thành tỉ lệ nhiệm vụ làm gấp trên tổng nhiệm vụ có hạn trong kỳ; nhật ký ghi thêm nguyên nhân mỗi lần làm gấp (sót thông tin / chọn ưu tiên sai / ước lượng sai khối lượng / thiếu thời gian) và báo cáo riêng từng nhóm nguyên nhân. Dùng tỉ lệ cũng giải quyết việc kỳ baseline (2 tuần) và kỳ so sánh (4 tuần) dài khác nhau. |
| 3 | Metric phụ chỉ đo tốc độ: kiểm tra nhanh hơn có thể kéo theo sót nhiệm vụ nhiều hơn mà metric vẫn "đạt". | Đồng ý | Đưa vào v1: thêm guardrail "số nhiệm vụ bị sót hoặc biết đến khi còn dưới 48 giờ đến hạn không tăng so với 2 tuần baseline", lấy từ cột "ngày biết đến" trong nhật ký. |
| 4 | Bottleneck chọn bước 4 (8') trong khi bước 1–2 cộng lại tốn 12'. Có đang đặt nghẽn sai chỗ không? | Đồng ý một phần | Giữ bước 4 vì đây là bước dẫn đến hậu quả (chọn sai việc → làm gấp), còn bước 1–2 là chi phí thời gian. Sửa ngay ở v0: ghi rõ lý do này và số phút của bước 1–2 trong ô Bottleneck. |
| 5 | Bản nháp Boundary chỉ ghi "AI không tự quyết, con người kiểm tra", chưa nói kiểm khi nào nên không kiểm được. | Đồng ý | Sửa ngay ở v0: liệt kê 3 tình huống bắt buộc con người kiểm tra (nhiệm vụ mới; deadline chưa rõ hoặc lệch nguồn; còn dưới 48 giờ hoặc quá tải). |
| 6 | Actor gộp cả người làm gấp vì thiếu thời gian (C). Với nhóm này, cải thiện việc tổng hợp và xếp ưu tiên có thể không có tác dụng. | Đồng ý một phần | Chưa thu hẹp actor ở v0 vì mới có 1/3 snapshot. Sau 2 tuần baseline, nếu phần lớn lần làm gấp do thiếu thời gian thì v1 thu hẹp actor hoặc ghi rõ phần này nằm ngoài phạm vi. |
| 7 | Target tối đa 1 lần/tháng chưa có căn cứ; dữ liệu 1 tháng của 1 người quá ít để tách thay đổi thật khỏi dao động ngẫu nhiên. | Đồng ý một phần | Giữ target của candidate #7 làm mục tiêu ban đầu vì do chính người gặp vấn đề đặt; xem lại sau khi có baseline đo thật. |
| 8 | Kiểm tra Problem Statement có lẫn giải pháp không. | — | Đạt: 6 trường không nêu tên công cụ hay tính năng; Boundary chỉ nói AI nếu được chọn ở CP6. Khi rà lại đã sửa thêm chữ "nhập" ở Boundary (ngầm giả định có công cụ nhập liệu) thành "đưa ra hoặc xác nhận". |

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **độ mơ hồ cao × độ phức tạp cao** nếu xét toàn bộ quy trình quản lý nhiệm vụ từ nhiều nền tảng, kể cả việc chọn ưu tiên. Khi tách phần người học giữ (chốt ưu tiên) khỏi phần hệ thống làm, và sửa quy trình để ghi nhiệm vụ vào một danh sách ngay khi nhận (No AI), phần cần tự động hóa nằm ở ô **độ mơ hồ thấp × độ phức tạp thấp**: "Rule hoặc Workflow đơn giản thường đủ".

Vì sao:

- **Toàn bộ quy trình mơ hồ cao, phức tạp cao:** học viên phải kiểm tra 5 nguồn và làm nhiều bước liên tiếp, từ nhận biết nhiệm vụ, xác định deadline, ước lượng khối lượng đến chọn thứ tự ưu tiên; bước sau dùng kết quả bước trước (mục 4.1). Việc chọn ưu tiên không có một đáp án đúng duy nhất vì còn phụ thuộc thời gian rảnh và tình huống cá nhân.
- **Phần mơ hồ nằm ở bước chốt ưu tiên, và Boundary ở mục 5 giao bước này cho người học.** Các đầu ra hệ thống cần tạo đều có đúng/sai rõ: nhiệm vụ có trong thông báo hay không, hạn ghi đúng hay sai, tổng giờ còn lại có vượt giờ rảnh trước hạn hay không. Những bước như kiểm tra trường dữ liệu thiếu hay nhắc hạn gần có quy tắc rõ ràng, nên không cần AI cho toàn bộ quy trình.
- **Độ phức tạp chủ yếu nằm ở việc gom từ 5 nguồn mỗi ngày.** Nếu người học ghi nhiệm vụ vào một danh sách ngay khi nhận, lúc chọn việc chỉ còn 1 nguồn, và các phép tính còn lại (sắp theo hạn, nhắc trước 48 giờ, cộng giờ còn lại so với giờ rảnh) là logic cố định. Chỗ còn mơ hồ vừa phải là đọc thông báo viết tự do để nhận ra nhiệm vụ và hạn (vd "nộp trước buổi sau"); trong quy trình tương lai, việc này vẫn do người học làm (bước 2 mục 4.2, khoảng 4 phút).

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Một danh sách tập trung duy nhất, quy tắc "ghi ngay khi nhận" với 4 trường: tên, hạn, nguồn, số giờ ước lượng. Mỗi ngày xem danh sách thay vì mở lần lượt 5 nền tảng; học viên tự chọn việc cần làm. | Nguyên nhân làm gấp chủ yếu là sót thông tin, người học giữ được thói quen ghi ngay (giả định #4) và tự xếp ưu tiên trong thời gian chấp nhận được. | Phụ thuộc hoàn toàn vào kỷ luật: dễ quên nhập hoặc không cập nhật danh sách (A có ghi chú nhưng không cập nhật đều). Người học vẫn phải tự cộng giờ còn lại và so với giờ rảnh, nên không chạm tới nguyên nhân ước lượng sai của B. Không có nhắc hạn. | Là nền của mức Rule (giữ quy tắc ghi ngay); một mình chưa đủ |
| **Rule** | No AI cộng thêm: (1) tự sắp theo hạn và nhắc khi còn 48 giờ; (2) gắn cờ nhiệm vụ thiếu hạn hoặc chưa ước lượng giờ; (3) công thức cảnh báo quá tải: tổng giờ ước lượng còn lại của nhiệm vụ đó và các nhiệm vụ có hạn sớm hơn vượt tổng giờ rảnh người học khai từ hôm nay đến hạn → gắn cờ; (4) một luồng Zapier không có AI, chuyển tin nhắn mới trên kênh thông báo Discord của lớp thành task ứng viên. Dùng công cụ có sẵn (mục 3.3) và bảng tính. | Dữ liệu đã đầy đủ và các quy tắc cố định xử lý được phần lớn tình huống: phần lớn nhiệm vụ có hạn ghi rõ trong thông báo; người học nhập tay phần còn lại trong khoảng 4 phút/ngày (mục 4.2). | Phụ thuộc dữ liệu nhập: 4/5 nguồn vẫn nhập tay, cờ quá tải chỉ đúng khi số giờ ước lượng đúng. Luồng Discord tạo task rác vì gói Free không có Filter (mục 3.3). Quy tắc cứng chưa phản ánh hết thay đổi lịch và mức độ quan trọng của từng việc. | **Chọn**: pilot 6 tuần (mục 8.2) |
| **Workflow** | Rule cộng thêm một bước AI, người học vẫn chốt. Hai phương án đã cân nhắc: (a) AI gợi ý thứ tự hoặc khung giờ làm cho các nhiệm vụ đã xác nhận, theo quy trình giả thuyết ở mục 4.2: tạo task ứng viên từ Discord → học viên đối chiếu 4 nguồn còn lại → Rule kiểm tra dữ liệu → AI gợi ý thứ tự/lịch → học viên xác nhận; (b) AI đọc thông báo viết tự do (Zalo, Cohort, web khóa AI, Discord), trích tên nhiệm vụ, hạn, nguồn thành task ứng viên. | (a) Sau pilot, danh sách đã đủ và cờ quá tải đúng mà tỉ lệ làm gấp do chọn ưu tiên sai vẫn không giảm, tức thứ tự theo hạn và cờ quá tải không đủ giúp cân nhắc khi nhiều nhiệm vụ trùng hạn hoặc quỹ thời gian thay đổi. (b) Sau pilot, bước nhập tay vẫn tốn trên 5 phút/ngày hoặc là nguyên nhân chính khiến nhiệm vụ bị sót. | (a) AI gợi ý thứ tự không phù hợp mà người học vẫn làm theo. (b) AI bỏ sót nhiệm vụ hoặc đọc sai hạn viết kiểu tương đối ("thứ 6 tuần sau"); phải đưa nội dung thông báo cho dịch vụ bên ngoài; nhóm chưa có bộ thông báo thật để chấm. Cả hai: task rác, deadline hoặc thời lượng sai từ đầu vào. | Not Yet (điều kiện ở mục 8.2) |
| **Agent** | AI tự chọn nền tảng, công cụ và bước tiếp theo: tự đọc các nền tảng, tự tạo và sửa task, tự xếp lịch và điều chỉnh. | Chỉ phù hợp nếu quy trình không thể định trước và cần AI tự quyết các bước. Bài này không như vậy: thứ tự các bước đã cố định (mục 4.2). | Khó kiểm soát; cần quyền đọc tin nhắn cá nhân trên Zalo, có thể truy cập sai phạm vi; tự thay đổi danh sách và tự chốt thứ tự, trái Boundary ở mục 5; lỗi khó phát hiện vì người học không thấy từng bước. | Không (No-Go, mục 8.2) |

**Mức chọn:** Rule (không dùng AI trong pilot).

**Vì sao không chọn mức đơn giản hơn (No AI):** No AI giải được phần sót thông tin nếu người học ghi ngay, nhưng còn 3 chỗ hở mà logic cố định bịt được ngay, không cần AI. (1) Không chạm tới nguyên nhân ước lượng sai khối lượng của B: người học vẫn phải nhẩm tổng giờ còn lại và so với thời gian rảnh, đúng là phần việc của bước 4 (8 phút, bottleneck) đang làm bằng trí nhớ; công thức quá tải làm việc này tức thì và không quên. (2) Không có nhắc khi còn 48 giờ, trong khi đây là mốc bắt buộc con người kiểm tra ở Boundary mục 5. (3) A có ghi chú nhưng không cập nhật đều; cờ "thiếu hạn / chưa ước lượng giờ" cho thấy chỗ trống trong danh sách thay vì để người học tự rà.

**Vì sao chưa cần mức cao hơn:** CP4–CP5 chưa chứng minh Rule không đủ, nên phải thử Rule trước; nếu Rule đạt các tiêu chí đánh giá ở mục 7 thì không cần nâng lên Workflow có AI. Thứ tự theo hạn và cảnh báo quá tải có đúng/sai rõ và tính được bằng công thức, không cần AI dự đoán. Workflow (a) chỉ đáng thử nếu sau pilot người học vẫn chọn sai khi nhiều việc trùng hạn dù dữ liệu đã đủ; Workflow (b) chỉ đáng thử nếu bước nhập tay thành chỗ nghẽn (mục 4.2 kỳ vọng khoảng 4 phút) và có dữ liệu thật để chấm. Quyết định thứ tự cuối thuộc về người học (Boundary mục 5), nên không có bước nào cần AI tự quyết, tức không cần Agent.

**Đối chiếu với quy trình giả thuyết ở mục 4.2:** bước 1 (đồng bộ và tạo task ứng viên từ Discord) là automation không có AI nên thuộc mức Rule. Bước 4 (đề xuất thứ tự/lịch) trong pilot làm bằng sắp theo hạn cộng cờ quá tải, tức Rule; phiên bản có AI của bước này là Workflow (a), đang Not Yet. Bước con người (2, 5), boundary và phương án quay về giữ nguyên.

### 6.3. AI Canvas rút gọn

Không bắt buộc vì nhóm chọn mức Rule (theo hướng dẫn worksheet CP6): các đầu ra hệ thống cần tạo (danh sách, thứ tự theo hạn, nhắc 48 giờ, cờ quá tải) đều có đúng/sai rõ và viết được bằng logic cố định, phần cần cân nhắc duy nhất (chốt việc làm trước) do người học giữ. Nhóm vẫn điền canvas cho bước AI gợi ý thứ tự (Workflow a) để dùng nếu sau pilot xét lại bước này. Ô **Input** cho thấy AI chỉ chạy được khi người học đã xác nhận đủ hạn, khối lượng và giờ rảnh, tức là sau khi mức Rule chạy tốt: thêm một lý do làm Rule trước. Với Workflow (b), ô Input chưa điền được vì nhóm chưa có bộ thông báo thật nào; theo AI Canvas, đây là dấu hiệu chưa sẵn sàng cho AI, và là lý do điều kiện Not Yet ở mục 8.2 yêu cầu gom ít nhất 20 thông báo thật.

| Thành phần | Nội dung (bước AI gợi ý thứ tự, Workflow a, đang Not Yet) |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Đề xuất thứ tự hoặc khung thời gian làm các nhiệm vụ đã xác nhận, kèm lý do theo deadline, khối lượng còn lại và thời gian rảnh; cảnh báo trường hợp có nguy cơ không kịp hạn. Không tự suy đoán deadline bị thiếu. |
| **Judgment** — con người cân nhắc, quyết định gì? | Học viên đối chiếu với thông báo gốc, kiểm tra hạn và khối lượng, xem xét lịch cá nhân, rồi chấp nhận hoặc sửa thứ tự đề xuất. |
| **Action** — hành động cuối cùng là gì, ai làm? | Học viên chốt kế hoạch, tự điều chỉnh và thực hiện nhiệm vụ; AI không tự sửa deadline, xóa task, gửi tin nhắn hay nộp bài. |
| **Outcome** — đo kết quả bằng gì? | Bấm giờ từ lúc mở nguồn đầu tiên đến khi chốt kế hoạch (ước lượng hiện tại khoảng 25 phút/ngày, mục tiêu tối đa 10 phút/ngày); theo dõi tỉ lệ nhiệm vụ phải làm gấp trên tổng nhiệm vụ có hạn và số nhiệm vụ bị bỏ sót/biết muộn. Baseline tỉ lệ chưa có, cần đo bằng nhật ký. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Tên nhiệm vụ, nguồn/thông báo gốc, deadline, phần việc hoặc thời lượng còn lại, thời gian rảnh và trạng thái hoàn thành. Thông tin đang phân tán ở 5 nguồn; người học phải kiểm tra 4 nguồn chưa hỗ trợ, xác nhận dữ liệu và bổ sung những trường còn thiếu trước khi AI đề xuất. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Ghi nhận gợi ý nào được học viên chấp nhận, sửa hoặc bỏ; đối chiếu với nhật ký deadline và lý do thực tế của từng lần làm gấp. Đây là nguồn đánh giá để điều chỉnh quy trình, chưa phải dữ liệu huấn luyện đã thu thập. |

### 6.4. Hai câu hỏi của Google PAIR

Không bắt buộc với mức Rule, nhưng nhóm vẫn trả lời vì hai câu này quyết định cách thiết kế Rule và mọi bước AI thêm sau này:

- **Augment hay automate:** augment. Trong CP4, A khó tổng hợp và chọn ưu tiên ("xem xong vẫn phân vân"); B biết hạn nhưng ước lượng thiếu thời gian; C vẫn làm gấp dù có danh sách và đã tự chọn việc cho hôm sau; chính card #7 ghi "tôi vẫn kiểm tra và quyết định thứ tự cuối cùng". Hệ thống có thể hỗ trợ tổng hợp, cảnh báo và gợi ý, nhưng không thay người học quyết định. Các buổi phỏng vấn chưa hỏi trực tiếp việc có muốn giao quyền cho AI hay không, nên augment là định hướng thiết kế cần kiểm chứng thêm, không phải kết quả xác nhận của cả 3 người. Vì vậy hệ thống mức Rule chỉ sắp theo hạn và gắn cờ, người học chốt thứ tự.
- **Báo nhầm hay bỏ sót tệ hơn:** bỏ sót nhiệm vụ hoặc hạn gấp tệ hơn, vì học viên có thể phát hiện quá muộn, phải làm gấp hoặc nộp thiếu (tình huống A). Báo nhầm cũng gây hại vì task rác làm mất thời gian kiểm tra, nhưng mỗi task rác chỉ tốn vài giây để loại. Thiết kế nghiêng về tránh bỏ sót: giữ trường nguồn để mở lại thông báo gốc; gắn cờ "chưa rõ hạn" thay vì bỏ qua; nhắc khi còn dưới 48 giờ; luồng Discord lấy mọi tin nhắn trên kênh thông báo nhưng chỉ tạo task ứng viên, không đưa thẳng vào danh sách chính; người học duyệt, sửa, loại task sai và có thể quay về checklist thủ công.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Học viên học song song từ hai chương trình trở lên, nhận nhiệm vụ từ nhiều nền tảng (candidate #7: 5 nền tảng) và tự chọn việc làm trước. **Phạm vi pilot:** người làm gấp vì sót thông tin, chọn ưu tiên sai hoặc ước lượng sai khối lượng (candidate #7, A, B). Người làm gấp chủ yếu vì thiếu thời gian (C) chỉ được theo dõi, nằm ngoài target; nếu sau 2 tuần baseline phần lớn lần làm gấp là do thiếu thời gian, nhóm thu hẹp actor hoặc đổi outcome (mục 8.2). |
| **Quy trình** | Giữ như v0: đầu ngày hoặc trước mỗi phiên học, khoảng 25 phút/ngày (dao động 15–30): (1) mở lần lượt 5 nền tảng: 7' → (2) liệt kê nhiệm vụ: 5' → (3) kiểm tra deadline và khối lượng: 5' → (4) xếp thứ tự ưu tiên: 8' (mục 4.1). |
| **Bottleneck** | Giữ như v0: bước 4, xếp thứ tự ưu tiên, khoảng 8 phút/ngày, vì đầu vào thường thiếu: có thể sót việc ở nền tảng chưa mở lại (A), khối lượng còn lại chỉ ước lượng theo cảm tính và chưa đối chiếu với giờ rảnh (B). |
| **Impact** | Giữ như v0: khoảng 25 phút/ngày (khoảng 175 phút/tuần) để kiểm tra và chọn việc; khoảng 4 lần/tháng làm gấp (candidate #7); A, B, C làm gấp 2–4 lần/tháng. Chưa tách được tỉ lệ từng nguyên nhân. |
| **Success Metric** (baseline → target, cách đo) | **Chính, tỉ lệ nhiệm vụ làm gấp** = số nhiệm vụ làm gấp / tổng số nhiệm vụ có hạn trong kỳ, báo cáo riêng theo 4 nguyên nhân (sót thông tin / chọn ưu tiên sai / ước lượng sai khối lượng / thiếu thời gian). Baseline: đo ở tuần 1–2 (tham chiếu tự ước lượng: khoảng 4 lần/tháng). Target: tỉ lệ làm gấp do 3 nguyên nhân đầu giảm còn tối đa 1/4 baseline (tương đương 4 → 1 lần/tháng ở v0). Làm gấp do thiếu thời gian chỉ theo dõi.<br>**Phụ, thời gian:** tổng thời gian kiểm tra, ghi và duy trì danh sách: baseline khoảng 25 phút/ngày (đo lại ở tuần 1–2) → tối đa 10 phút/ngày.<br>**Guardrail:** số nhiệm vụ bị sót hoặc biết đến khi còn dưới 48 giờ đến hạn không tăng so với 2 tuần baseline.<br>**Cách đo:** bấm giờ mỗi ngày như v0; nhật ký deadline như v0, thêm cột "nguyên nhân" cho mỗi lần làm gấp và cột "ngày vào danh sách". "Làm gấp" định nghĩa như v0. So tuần 1–2 (baseline) với tuần 3–6 (pilot) bằng tỉ lệ nên không phụ thuộc độ dài hai kỳ. |
| **Boundary** | **Hệ thống (công thức, nhắc hạn, luồng Zapier) không được:** đưa task vào danh sách chính khi người học chưa duyệt (task từ Discord chỉ là task ứng viên); tự sửa hoặc xoá nhiệm vụ, deadline; tự đoán hạn khi thông báo không ghi rõ (gắn cờ "chưa rõ hạn"); gửi tin nhắn hay nộp bài; lấy dữ liệu ngoài kênh thông báo Discord của lớp (không nối Zalo hay tin nhắn cá nhân). Hệ thống chỉ sắp theo hạn và gắn cờ, người học chốt thứ tự.<br>**Con người kiểm tra (HITL):** giữ 3 tình huống của v0: (1) nhiệm vụ mới; (2) hạn chưa rõ hoặc hai nguồn ghi khác nhau; (3) còn dưới 48 giờ hoặc quá tải. Ở mức Rule, tình huống (3) được kích hoạt bằng nhắc 48 giờ và cờ quá tải. Nếu sau này thêm AI, các điều AI không được làm ở v0 vẫn áp dụng. |
| **AI intervention point** | **Không có.** Lý do: những gì cần tự động (sắp theo hạn, nhắc 48 giờ, cờ thiếu trường, cờ quá tải, chuyển tin Discord thành task ứng viên) đều có đúng/sai rõ và viết được bằng logic cố định; phần cần cân nhắc (chốt thứ tự) thuộc về người học theo Boundary. Hai điểm có thể thêm AI sau pilot, đều đang Not Yet (mục 6.2, 8.2): (a) gợi ý thứ tự khi nhiều nhiệm vụ trùng hạn; (b) trích nhiệm vụ và hạn từ thông báo viết tự do. |
| **Mức chọn** | Rule |
| **Rủi ro & người kiểm tra** | (1) Người học không ghi nhiệm vụ ngay, danh sách thiếu (giả định #4): người học tự rà khi xem danh sách mỗi ngày; nhóm đối chiếu danh sách với nhật ký mỗi tuần (ngưỡng dừng 1).<br>(2) Luồng Discord tạo task rác hoặc trễ đến 15 phút: người học duyệt từng task ứng viên; tắt luồng nếu số nhiệm vụ bị sót tăng (ngưỡng dừng 3).<br>(3) Số giờ ước lượng sai làm cờ quá tải bật sai hoặc không bật: người học sửa ước lượng khi bắt đầu làm; nhật ký ghi nguyên nhân "ước lượng sai" để nhóm thấy.<br>(4) Duy trì danh sách tốn hơn thời gian tiết kiệm được (giả định #6): bấm giờ mỗi ngày (ngưỡng dừng 2). |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | Gộp mọi học viên học song song, kể cả người làm gấp vì thiếu thời gian | Pilot giới hạn ở người làm gấp vì sót thông tin, chọn ưu tiên sai hoặc ước lượng sai; thiếu thời gian chỉ theo dõi, xem lại sau baseline | Phản biện #6 (mục 5): với C, cải thiện việc tổng hợp và xếp ưu tiên không có tác dụng |
| Success Metric (chính) | Số lần làm gấp/tháng: 4 → tối đa 1 | Tỉ lệ nhiệm vụ làm gấp trên tổng nhiệm vụ có hạn, tách theo 4 nguyên nhân; target tối đa 1/4 baseline cho 3 nguyên nhân trong phạm vi | Phản biện #2: số lần phụ thuộc số deadline trong tháng; tỉ lệ cũng so được kỳ baseline 2 tuần với kỳ pilot 4 tuần |
| Success Metric (guardrail) | Không có | Số nhiệm vụ bị sót hoặc biết đến khi còn dưới 48 giờ không tăng | Phản biện #3: kiểm tra nhanh hơn có thể kéo theo sót nhiều hơn |
| Success Metric (phụ) | Thời gian kiểm tra và xếp ưu tiên | Tính cả thời gian ghi và duy trì danh sách | Mức Rule thêm việc nhập liệu; phải đo cả phần này mới kiểm được giả định #6 |
| Boundary | Viết cho AI "nếu nhóm chọn dùng ở CP6" | Viết cho hệ thống mức Rule và luồng Zapier; giữ nguyên 3 tình huống HITL | Mức chọn là Rule, không có bước AI |
| AI intervention point, Mức chọn, Rủi ro & người kiểm tra | Chưa có | Không có (kèm lý do); Rule; 4 rủi ro và người kiểm tra | 3 trường mới bắt buộc ở v1 |
| Quy trình, Bottleneck, Impact | — | Giữ nguyên | Chưa có số đo mới; cập nhật sau 2 tuần baseline |

**Tiêu chí đánh giá giải pháp mức Rule (không dùng AI):** kiểm mỗi tuần trong pilot bằng cách đối chiếu danh sách với nhật ký deadline và thông báo gốc.

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đủ nhiệm vụ | Mọi nhiệm vụ có hạn trong nhật ký đều vào danh sách trong ngày người học biết đến | Có nhiệm vụ trong nhật ký không có trong danh sách, hoặc vào danh sách muộn hơn ngày biết đến |
| 2 | Đúng hạn | Hạn trong danh sách khớp thông báo gốc; nhiệm vụ chưa rõ hạn mang cờ "chưa rõ hạn" | Có hạn ghi sai so với thông báo gốc, hoặc hạn bị đoán thay vì gắn cờ |
| 3 | Cảnh báo quá tải đúng | Cờ quá tải bật đúng những ngày tính tay cho thấy tổng giờ còn lại vượt giờ rảnh trước hạn | Có lần làm gấp do quá tải mà trước đó cờ không bật dù đã nhập đủ giờ, hoặc cờ bật khi tính tay không quá tải |
| 4 | Luồng Discord an toàn | Mọi thông báo nhiệm vụ trên kênh Discord của lớp đều thành task ứng viên; không task ứng viên nào vào danh sách chính khi chưa duyệt | Có thông báo nhiệm vụ trên kênh bị lọt, hoặc task vào thẳng danh sách chính |
| 5 | Nhẹ hơn cách cũ | Tổng thời gian kiểm tra, ghi và duyệt danh sách tối đa 10 phút/ngày (bấm giờ) | Trên 10 phút/ngày; nếu bằng hoặc hơn baseline 2 tuần liên tiếp thì chạm ngưỡng dừng 2 |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

Chấm cho giải pháp được chọn: mức **Rule**, không dùng AI trong pilot (lập luận chọn mức ở mục 6).

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Trung bình | Cả 4 người (candidate #7 và A, B, C) đều tự báo cáo làm gấp 2–4 lần/tháng. A và B làm gấp vì những nguyên nhân giải pháp chạm tới được: sót thông tin, ước lượng sai khối lượng. Nhưng C làm gấp vì thiếu thời gian, điều giải pháp này không giải được. Mọi baseline đều là tự báo cáo theo trí nhớ, chưa có nhật ký. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Giải pháp dựa vào việc người học tự ghi nhiệm vụ vào một danh sách ngay khi nhận (giả định #4, bằng chứng 1/5). Tín hiệu theo hai chiều: C đã duy trì được danh sách tập trung, còn A có ghi chú nhưng không cập nhật đều. Đầu ra của Rule (danh sách sắp theo hạn, cảnh báo quá tải) dễ hiểu và người học tự sửa được vì không có bước AI. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | Không cần xây gì. Danh sách tập trung, ghi nhanh và nhắc hạn có sẵn trong công cụ quản lý việc (Todoist, mục 3.3); luồng Discord → danh sách có sẵn trên Zapier, không cần code; công thức cảnh báo quá tải (giờ ước lượng còn lại so với giờ rảnh trước hạn) làm được bằng bảng tính. Khoảng trống: 4/5 nguồn (Zalo, ứng dụng tiếng Anh, Cohort, web khóa AI) chưa có connector nên vẫn nhập tay, đã tính vào bước 2 ở mục 4.2. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Trung bình | Chi phí và pháp lý thấp: pilot dùng Zapier gói Free (kiểm tra 15 phút/lần, không có Filter, mục 3.3) và công cụ sẵn có; người học tự vận hành; chỉ nối kênh thông báo của lớp, không đưa tin nhắn cá nhân trên Zalo vào dịch vụ bên ngoài. Điểm chưa chắc là thời gian duy trì danh sách có nhỏ hơn thời gian tiết kiệm được không (giả định #6, bằng chứng 1/5). |

### 8.2. Kết luận

**Quyết định:** Go, phạm vi nhỏ: pilot 6 tuần giải pháp mức Rule, không dùng AI. Hai bước AI nhóm đã cân nhắc ở mục 6.2, (a) gợi ý thứ tự và (b) trích nhiệm vụ từ thông báo: Not Yet.

**Lý do:** Không rủi ro nào ở mức Cao. Ba rủi ro Trung bình (Value, Usability, Viability) đều đo được ngay trong pilot bằng nhật ký deadline và bấm giờ đã định ở mục 5. Nhóm chưa có bằng chứng mức Rule không đủ nên chưa thêm AI, theo nguyên tắc chọn mức đơn giản nhất đủ dùng. Pilot cũng trả lời câu hỏi CP4 còn bỏ ngỏ: bao nhiêu lần làm gấp do thông tin và cách xếp ưu tiên, bao nhiêu lần do thiếu thời gian.

**Nếu Go — pilot nhỏ nhất:**

- Người tham gia: candidate #7 (Quân), mời thêm A và B vì nguyên nhân làm gấp của họ nằm trong phạm vi giải pháp.
- Tuần 1–2 (baseline): giữ cách làm cũ, chỉ ghi nhật ký deadline và bấm giờ kiểm tra như mục 5.
- Tuần 3–6 (pilot): (1) một danh sách tập trung duy nhất, ghi nhiệm vụ ngay khi nhận với tên, hạn, nguồn, số giờ ước lượng; (2) sắp theo hạn, nhắc khi còn 48 giờ, gắn cờ nhiệm vụ thiếu hạn hoặc chưa ước lượng giờ; (3) công thức cảnh báo khi tổng giờ ước lượng còn lại vượt giờ rảnh trước hạn; (4) một luồng Zapier chỉ cho kênh thông báo Discord của lớp, task tạo ra là task ứng viên, người học duyệt rồi mới đưa vào danh sách. Không xây gì, không dùng AI.
- Đo mỗi tuần: tỉ lệ nhiệm vụ làm gấp và nguyên nhân từng lần; số phút kiểm tra và duy trì danh sách mỗi ngày; số nhiệm vụ bị sót hoặc biết đến khi còn dưới 48 giờ; chấm 5 tiêu chí đánh giá ở mục 7.

**Nếu Not Yet — cần kiểm chứng gì trước:** Cả hai bước AI chỉ xét sau pilot.

- **(a) AI gợi ý thứ tự:** chỉ xét khi tiêu chí 1–3 ở mục 7 đạt (danh sách đủ, đúng hạn, cờ quá tải đúng) mà tỉ lệ làm gấp do chọn ưu tiên sai vẫn không giảm so với baseline. Khi đó dùng AI Canvas ở mục 6.3, viết tiêu chí đánh giá cho đầu ra AI và chấm trên dữ liệu nhật ký pilot trước khi dùng.
- **(b) AI trích nhiệm vụ và hạn từ thông báo viết tự do (Zalo, Cohort, web khóa AI):** chỉ xét khi có đủ 2 điều: (1) bước nhập tay từ các nguồn chưa có connector vẫn tốn trên 5 phút/ngày (mục 4.2 kỳ vọng khoảng 4 phút) hoặc là nguyên nhân chính khiến nhiệm vụ bị sót; (2) nhóm gom được ít nhất 20 thông báo thật (đã che thông tin cá nhân) để chấm đầu ra của AI trước khi dùng.

**Nếu No-Go — nên làm gì thay AI:** Không áp dụng cho quyết định chung. Riêng mức Agent (AI tự đọc các nền tảng, tự tạo task, tự xếp lịch) là No-Go vì cần quyền đọc tin nhắn cá nhân và đi ngược Boundary ở mục 5. Nếu sau pilot mức Rule đạt target và bước nhập tay không quá 5 phút/ngày, tức Rule đã đủ, thì cả hai bước AI chuyển từ Not Yet sang No-Go: giữ Rule, không thêm AI.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

- Nếu trong 2 tuần đầu pilot, người học không mở và cập nhật danh sách từ 3 ngày/tuần trở lên, thì dừng và quay về cách cũ (mở từng nền tảng, ghi chú điện thoại), xem lại quy tắc ghi nhiệm vụ, vì giả định #4 sai.
- Nếu thời gian kiểm tra và duy trì danh sách bằng hoặc hơn baseline đo ở tuần 1–2 trong 2 tuần liên tiếp, thì quay về cách cũ, vì giải pháp tốn công hơn mức tiết kiệm (giả định #6 sai).
- Nếu số nhiệm vụ bị sót hoặc biết đến khi còn dưới 48 giờ tăng so với 2 tuần baseline, thì tắt luồng Discord tự động và nhập tay toàn bộ; nếu sau 1 tuần vẫn tăng thì dừng pilot.
- Nếu sau 4 tuần pilot, tỉ lệ làm gấp do sót thông tin, chọn ưu tiên sai hoặc ước lượng sai không giảm so với baseline, thì kết luận No-Go cho hướng tổng hợp và xếp ưu tiên, không lên Workflow hay AI. Nếu phần lớn lần làm gấp do thiếu thời gian, chuyển sang hướng quản lý quỹ thời gian học.

---

## 9. Hạn chế và hướng tiếp theo

**Hạn chế:**

- Baseline (25 phút/ngày, 4 lần/tháng) là số tự ước lượng theo trí nhớ của 1 người; 3 snapshot cũng là tự báo cáo. Chưa có nhật ký hay log nào.
- Kiểm chứng chỉ có 3 buổi phỏng vấn, cùng bối cảnh học viên; chưa có survey để biết bao nhiêu người gặp vấn đề này.
- Chưa tách được tỉ lệ các nguyên nhân làm gấp (sót thông tin, chọn ưu tiên sai, ước lượng sai khối lượng, thiếu thời gian). C cho thấy có trường hợp nằm ngoài phạm vi giải pháp.
- Các công cụ ở mục 3.3 mới được kiểm trên tài liệu, chưa thử với tài khoản và kênh thật; 4/5 nguồn chưa có cách lấy nhiệm vụ tự động.

**Hướng tiếp theo:**

- Chạy pilot 6 tuần ở mục 8.2; sau pilot cập nhật baseline, target và phạm vi actor theo số đo thật.
- Nếu bước nhập tay vẫn là chỗ nghẽn, thử Workflow có AI trích nhiệm vụ từ thông báo, chấm trên bộ thông báo thật trước khi dùng.
- Nếu dữ liệu đã đủ mà người học vẫn chọn sai khi nhiều việc trùng hạn, thử Workflow có AI gợi ý thứ tự theo AI Canvas ở mục 6.3, người học vẫn chốt.
- Nếu phần lớn lần làm gấp do thiếu thời gian, đổi outcome sang quản lý quỹ thời gian học thay vì quản lý thông tin.

## 10. Tài liệu tham khảo

**Research giải pháp (mục 3.3), mở lại ngày 09/11/2026:**

- Todoist Help — [Use Task Quick Add in Todoist](https://www.todoist.com/help/todoist/features/use-task-quick-add-in-todoist-va4Lhpzz); [Use the Calendar integration](https://www.todoist.com/help/todoist/integrations/use-the-calendar-integration-rCqwLCt3G)
- Zapier — [Discord + Todoist integration](https://zapier.com/apps/discord/integrations/todoist); [Pricing](https://zapier.com/pricing)
- Motion Help Center — [Auto-scheduling](https://www.usemotion.com/help/time-management/auto-scheduling); [How auto-scheduling works behind the scenes](https://www.usemotion.com/help/time-management/auto-scheduling/reference-auto-scheduling/how-auto-scheduling-works-behind-the-scenes)

**Framework đã dùng** (theo [docs/03-international-frameworks.md](../../docs/03-international-frameworks.md)):

- Intercom, Alan Klement — [Job Stories](https://www.intercom.com/blog/accidentally-invented-job-stories/) (CP1–CP2)
- Teresa Torres — [Opportunity Solution Trees](https://www.producttalk.org/opportunity-solution-trees/) (CP3); [The Interview Snapshot](https://www.producttalk.org/interview-snapshot/) (CP4)
- David Bland — [Assumptions mapping](https://www.strategyzer.com/library/how-assumptions-mapping-can-focus-your-teams-on-running-experiments-that-matter) (CP4)
- Rob Fitzpatrick — [The Mom Test](https://www.momtestbook.com/) (CP4)
- Jeff Gothelf — [Business Problem Statement](https://jeffgothelf.com/blog/business-problem-statement-opportunity-statement/) (CP5)
- Anthropic — [Building effective agents](https://www.anthropic.com/research/building-effective-agents) (CP6, chọn mức can thiệp)
- Ajay Agrawal, Joshua Gans, Avi Goldfarb — [AI Canvas (HBR: A Simple Tool to Start Making Decisions with the Help of AI)](https://hbr.org/2018/04/a-simple-tool-to-start-making-decisions-with-the-help-of-ai) (CP6, lý do chưa sẵn sàng cho AI)
- Google PAIR — [People + AI Guidebook: User Needs](https://pair.withgoogle.com/chapter/user-needs/) (CP6, augment hay automate, báo nhầm hay bỏ sót)
- Marty Cagan, SVPG — [The Four Big Risks](https://www.svpg.com/four-big-risks/) (CP6, quyết định)
