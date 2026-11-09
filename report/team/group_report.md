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
| --- | --- | --- | --- | --- | --- |
| 1 | Nguyễn Văn Minh | Muốn tóm tắt nhanh tiền sử bệnh để bác sĩ nắm ngay. | Mẹ/người thân, bác sĩ | Tìm lại thông tin từ giấy khám cũ (tốn thời gian lúc khám). | "Nhóm học IT, có đủ chuyên môn y tế để đánh giá bản tóm tắt đúng/sai không?" (Chuẩn) |
| 2 | Phạm Lê Chuẩn | Muốn biết nhanh hệ thống lỗi ở đâu để khắc phục ngay. | IT, kĩ thuật | Dò lỗi cú pháp hoặc tìm nguyên nhân gây lỗi (20-30 phút). | "Dùng AI chỉ lỗi luôn thì sinh viên có bị lười tư duy đi không?" (Cao) |
| 3 | Phạm Lê Chuẩn | Muốn tự động sắp xếp lịch trình, đặt lịch, nhắc hẹn. | Mọi người | Tự kiểm tra, đối chiếu lịch thủ công. | "Làm sao AI truy cập được tin nhắn Zalo cá nhân để lấy lịch?" (Huy) |
| 4 | Phạm Lê Chuẩn | Muốn điểm danh đầu/cuối ca học nhanh chóng. | Sinh viên, Giảng viên/trợ giảng | Xếp hàng chờ quét mã/gọi tên (15-20 phút). | "Bài này dùng mã QR tĩnh (Rule) là đủ, cần gì AI?" (Minh) |
| 5 | Vũ Quang Huy | Muốn xác định chủ đề trọng tâm từ đề cương ôn tập dài. | Sinh viên/Học sinh | Đọc dàn trải số lượng trang đề cương lớn. | "Mỗi môn cấu trúc khác nhau, đo lường độ chính xác của trọng tâm thế nào?" (Cao) |
| 6 | Vũ Quang Huy | Muốn nắm bài tập và deadline sắp tới để không bỏ sót. | Sinh viên/Học sinh | Phải lội 2-3 nguồn (LMS, nhóm lớp) mỗi tuần. | "Nếu trường đổi API của LMS thì giải pháp có sập không?" (Chuẩn) |
| 7 | Vũ Quang Huy | Muốn nắm thông tin quan trọng từ nhiều kênh thông báo của GV. | Sinh viên/Học sinh | Bỏ lỡ thông báo do trôi tin nhắn trên nhiều kênh. | "Quyền truy cập dữ liệu đa kênh cá nhân lấy ở đâu?" (Minh) |
| 8 | Phùng Văn Thanh Cao | Muốn lên kế hoạch học tập buổi tối theo deadline, độ khó. | Sinh viên | Mất 10-20 phút xếp việc nhưng vẫn miss deadline. | "Độ khó là cảm nhận chủ quan, hệ thống đo lường kiểu gì?" (Huy) |
| 9 | Phùng Văn Thanh Cao | Muốn tổng hợp deadline từ LMS, email, nhóm lớp. | Sinh viên | Lướt nhiều nguồn mỗi tối dễ bị sót thông tin. | "Có trùng lặp ý tưởng với bài toán quản lý deadline của Huy không?" (Cao) |
| 10 | Phùng Văn Thanh Cao | Muốn có hướng dẫn phân tích, từng bước tiếp cận bài khó. | Sinh viên | Tốn 1-2 tiếng kẹt lại không tìm được hướng giải. | "Làm sao ngăn chặn việc AI giải hộ luôn thay vì chỉ hướng dẫn?" (Minh) |
| 11 | Phùng Văn Thanh Cao | Muốn tổng hợp kiến thức trọng tâm cuối ngày học. | Sinh viên | Mất 45-60 phút tự đọc lại slide. | "Nếu input là file ghi âm bài giảng thì xử lý thế nào?" (Huy) |
| 12 | Phùng Văn Thanh Cao | Muốn theo dõi tiến độ task để không ảnh hưởng nhóm. | Sinh viên, thành viên nhóm | Nhắc nhở thủ công, trùng lặp công việc. | "Đây là vấn đề ý thức hay do thiếu công cụ quản lý?" (Huy) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
| --- | --- | --- |
| A | Hỗ trợ học tập / Ôn thi (5, 10, 11) | Rút gọn, tóm tắt và phân tích khối lượng tài liệu học thuật lớn. |
| B | Quản lý lịch & Deadline (3, 6, 7, 8, 9, 12) | Gom thông tin rải rác từ nhiều nguồn (LMS, Zalo, Email) để lập kế hoạch. |
| C | Tối ưu quy trình & Kỹ thuật (1, 2, 4) | Giảm thao tác lặp lại tốn thời gian ở một bước xử lý/đọc dữ liệu cụ thể. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian sinh viên IT/kỹ thuật bị kẹt lại khi hệ thống báo lỗi / lỗi code bài lab.
├── Opportunity A: Thông báo lỗi (log) của hệ thống quá dài và chứa nhiều thông tin rác.
├── Opportunity B: Việc copy mã lỗi lên Google trả về quá nhiều luồng ý kiến, phải tự chắt lọc.
└── Opportunity C: Sinh viên không xác định được chính xác dòng code nào là nguyên nhân gốc rễ.

```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

* "Tích hợp công cụ debug bằng AI vào thẳng phần mềm VS Code"
* "Chatbot tự động viết lại code cho đúng"

Dưới đây là phần nội dung được tổng hợp và hoàn thiện dựa trên bảng dữ liệu trong hình ảnh của nhóm bạn, kết hợp với bối cảnh lựa chọn "Sửa lỗi bài lab / hệ thống" của bạn ở các bước trước:

### 2. Hội tụ nhóm (CP3)

**2.1. Pitch**

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
| --- | --- | --- | --- | --- | --- |
| 1 | Nguyễn Văn Minh | Muốn tóm tắt nhanh tiền sử bệnh để bác sĩ nắm ngay. | Mẹ/người thân, bác sĩ | Tìm lại thông tin từ mớ giấy khám cũ (tốn thời gian lúc khám). | "Nhóm mình học IT, liệu có đủ chuyên môn y tế để đánh giá bản tóm tắt đúng/sai không?" (Chuẩn) |
| 2 | Phạm Lê Chuẩn | Muốn biết nhanh hệ thống lỗi ở đâu để khắc phục ngay. | IT, kỹ thuật | Đọc dò lỗi cú pháp hoặc tìm nguyên nhân (20-30 phút). | "Nếu dùng AI chỉ ra lỗi luôn thì sinh viên có bị lười tư duy đi không?" (Cao) |
| 3 | Phạm Lê Chuẩn | Muốn tự động sắp xếp lịch trình, đặt lịch, nhắc hẹn. | Mọi người | Tự kiểm tra, đối chiếu lịch thủ công. | "Làm sao AI truy cập được tin nhắn Zalo cá nhân để biết có lịch hẹn?" (Huy) |
| 4 | Phạm Lê Chuẩn | Muốn điểm danh đầu/cuối ca học nhanh chóng. | SV, Giảng viên | Xếp hàng quét mã/gọi tên (15-20 phút). | "Bài này dùng mã QR tĩnh (Rule) là xong, cần gì AI?" (Minh) |
| 5 | Vũ Quang Huy | Muốn xác định chủ đề trọng tâm từ đề cương ôn tập dài. | SV / Học sinh | Đọc dàn trải số lượng trang đề cương lớn. | "Mỗi môn một cấu trúc, làm sao đo lường độ chính xác của trọng tâm?" (Cao) |
| 6 | Vũ Quang Huy | Muốn biết bài tập/deadline sắp tới để không bỏ sót. | SV / Học sinh | Phải lội 2-3 nguồn (LMS, Zalo, Email) mỗi tuần. | "Nếu trường đổi API của LMS thì giải pháp có sập không?" (Chuẩn) |
| 7 | Vũ Quang Huy | Muốn nắm thông tin quan trọng từ nhiều kênh thông báo của GV. | SV / Học sinh | Bỏ lỡ thông báo do trôi tin nhắn nhiều kênh. | "Giống ý 6, quyền truy cập dữ liệu đa kênh lấy ở đâu?" (Minh) |
| 8 | Phùng Văn Thanh Cao | Muốn sắp xếp kế hoạch học tối ưu theo deadline, độ khó. | Sinh viên | Mất 10-20 phút mỗi tối để lên plan nhưng vẫn miss. | "Độ khó là cảm nhận chủ quan, hệ thống đo lường kiểu gì?" (Huy) |
| 9 | Phùng Văn Thanh Cao | Muốn tổng hợp deadline từ LMS, email, nhóm lớp cuối ngày. | Sinh viên | Lướt nhiều nguồn mỗi tối dễ bị sót. | (Trùng pattern với ý số 6 của Huy) |
| 10 | Phùng Văn Thanh Cao | Muốn có hướng dẫn phân tích, từng bước tiếp cận bài khó. | Sinh viên | Tốn 1-2h kẹt lại không tìm được hướng giải. | "Làm sao tránh việc AI giải hộ luôn thay vì chỉ hướng dẫn?" (Chuẩn) |
| 11 | Phùng Văn Thanh Cao | Muốn tổng hợp kiến thức trọng tâm cuối ngày học. | Sinh viên | Mất 45-60 phút tự đọc lại slide. | "Nếu bài giảng là video/audio thì input xử lý thế nào?" (Minh) |
| 12 | Phùng Văn Thanh Cao | Muốn theo dõi tiến độ nhóm để không ảnh hưởng kết quả chung. | SV, thành viên nhóm | Nhắc nhở thủ công, trùng lặp công việc. | "Đây là vấn đề ý thức hay vấn đề công cụ quản lý?" (Huy) |

**2.2. Cluster**

| Cluster | Các candidate | Pattern chung |
| --- | --- | --- |
| A — Hỗ trợ học tập / Ôn thi | Tóm tắt đề cương (5), Hướng dẫn giải bài tập (10), Tổng hợp kiến thức (11), Chuẩn bị bài trước (12). | Rút gọn, tóm tắt và phân tích khối lượng tài liệu học thuật lớn. |
| B — Quản lý lịch & Deadline | Xếp lịch (3), Tổng hợp deadline (6, 9), Xếp kế hoạch tối (8), Theo dõi task nhóm (13). | Gom thông tin rải rác từ nhiều nguồn (LMS, Zalo, Email) để lập kế hoạch. |
| C — Tối ưu quy trình & Kỹ thuật | Khắc phục lỗi hệ thống/lab (2), Tóm tắt bệnh án (1), Điểm danh (4). | Giảm thao tác lặp lại tốn thời gian ở một bước xử lý/phân tích log dữ liệu cụ thể. |

**2.3. Opportunity Solution Tree rút gọn**

Nhóm thống nhất chọn nhánh bài toán của người làm kỹ thuật/IT (Candidate 2 của Chuẩn) để đi tiếp vì phù hợp chuyên ngành nhóm.

```text
OUTCOME: Giảm thời gian sinh viên IT/kỹ thuật bị kẹt lại khi hệ thống báo lỗi / lỗi code.
├── Opportunity A: Thông báo lỗi (log) của hệ thống quá dài và chứa nhiều thông tin rác.
├── Opportunity B: Việc copy lỗi lên Google/StackOverflow trả về quá nhiều luồng ý kiến, phải tự chắt lọc.
└── Opportunity C: Sinh viên không xác định được chính xác dòng lệnh/code nào là nguyên nhân gốc rễ.
Những ý đã gạch bỏ vì là solution đội lốt opportunity:
- "Tích hợp công cụ debug bằng AI vào VS Code" (Đây là giải pháp công cụ)
- "Chatbot tự động viết lại code cho đúng" (Đây là giải pháp mức Agent)

```

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Theo dõi tiến độ task nhóm (Cao) | 5 | 4 | 5 | 5 | 4 | 5 | 5 | **33** |
| Khắc phục lỗi hệ thống/code bài lab (Chuẩn) | 5 | 5 | 4 | 4 | 3 | 4 | 3 | **28** |
| Tóm tắt tiền sử bệnh án (Minh) | 4 | 4 | 3 | 3 | 5 | 4 | 2 | **25** |

**Candidate được chọn:**
Theo dõi tiến độ task nhóm để không ảnh hưởng kết quả chung (Phùng Văn Thanh Cao).

**Vì sao chọn:**
Đây là nỗi đau (pain point) cực kỳ phổ biến mà bất kỳ sinh viên nào cũng gặp phải ("gánh team", trễ deadline do không ai nhắc, trùng lặp công việc). Bài toán có đối tượng rất rõ ràng, dễ dàng tìm người phỏng vấn để lấy bằng chứng ngay trong lớp. Impact đo lường được định lượng thông qua số lần trễ hạn hoặc số phút phải bỏ ra để họp nhóm/nhắn tin nhắc nhở mỗi tuần. Đặc biệt, bài toán này rất dễ để so sánh các mức can thiệp: từ No AI (chỉ dùng Trello/Excel), Rule (bot tự động nhắc giờ), đến Workflow (AI tự tóm tắt tiến độ từ tin nhắn chat và cập nhật trạng thái).

**Vì sao loại các candidate còn lại:**

* Bài "Khắc phục lỗi code bài lab": Dù quy trình rõ ràng, nhưng các lỗi (bug) có độ khó rất khác nhau, dẫn đến việc đo lường baseline thời gian trung bình thiếu chính xác. Hơn nữa, mức độ phức tạp của bài lab có thể vượt quá khả năng đánh giá của một số thành viên trong nhóm, dẫn đến rủi ro khó kiểm định chất lượng đầu ra của AI.
* Bài "Tóm tắt bệnh án": Bị loại do nhóm hoàn toàn không có chuyên môn y tế, rủi ro đánh giá sai tính sinh mạng (Feasibility/Viability rất cao).

**Xử lý bất đồng (nếu có):**
Chuẩn ban đầu muốn giữ bài "Khắc phục lỗi code" vì mang đậm tính kỹ thuật IT. Tuy nhiên, Cao và Huy đã phản biện và chỉ ra rằng bài "Theo dõi task nhóm" dễ thu thập dữ liệu (input) từ các đoạn chat nhóm trên Zalo/Discord hơn là việc trích xuất log lỗi hệ thống trên các môi trường máy ảo khác nhau. Nhóm đi đến thống nhất chọn bài Task Nhóm vì tệp người dùng rộng hơn, tính khả thi cao và "vừa sức lab" hơn để thiết kế một quy trình (workflow) hoàn chỉnh.
---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên học từ 4–5 môn/kỳ đều mất từ 20–30 phút mỗi tối để lướt kiểm tra bài tập và deadline từ nhiều nguồn rời rạc (LMS, Zalo, Teams, Email). | Value | 5 | 2 | ✅ |
| 2 | Đa số các lần bị trễ hạn hoặc bỏ sót deadline xuất phát từ các thông báo không có cấu trúc (dặn dò trong nhóm chat Zalo/Teams, slide bài giảng) chứ không phải bài tập chính thức đã tạo trên LMS. | Value | 5 | 2 | ✅ |
| 3 | Sinh viên sẵn sàng dành 2–3 phút mỗi tối để xem lại và bấm duyệt danh sách deadline do hệ thống tổng hợp thay vì tự đi tìm thủ công. | Usability | 4 | 3 | — |
| 4 | Có thể lấy dữ liệu bài tập từ LMS tự động qua chuẩn lịch iCal, và trích xuất ngày giờ hạn nộp từ tin nhắn ngôn ngữ tự nhiên bằng Rule/LLM. | Feasibility | 4 | 4 | — |
| 5 | Sinh viên lo ngại rủi ro bảo mật thông tin cá nhân và không sẵn sàng cấp quyền truy cập toàn bộ tài khoản chat Zalo cá nhân cho một ứng dụng bên thứ ba. | Viability | 5 | 1 | ✅ |

Giả định nhóm kiểm chứng trong buổi này: **Giả định #1, #2 và #5** (nhóm giả định có độ quan trọng cao nhưng bằng chứng thực tế còn thấp).

### 3.2. Kiểm chứng

**Cách đã dùng:** Phỏng vấn sâu 3 sinh viên kỹ thuật trong nhóm theo trải nghiệm thực tế đã xảy ra (theo đúng 3 luật The Mom Test: Nguyễn Văn Minh, Vũ Quang Huy, Phạm Lê Chuẩn) + Khảo sát nhanh (micro-survey) 8 sinh viên trong lớp L3B.

#### Interview Snapshot #1 — Trải nghiệm từ Nguyễn Văn Minh

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 2 ngành AI / Kỹ thuật (Nguyễn Văn Minh), đang theo học các môn lab thực hành và đồ án dự án |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Sợ nhất là hạn nộp bài trên LMS ghi là Chủ nhật, nhưng tối thứ Sáu trợ giảng ghim tin nhắn trong nhóm Zalo bảo nộp sớm vào sáng thứ Bảy để chấm bù; mình mà không lướt Zalo lúc 23h đêm là coi như sáng hôm sau mất trắng 20% điểm."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước ở môn Lập trình/AI, suýt bị trễ hạn nộp bài lab vì thông báo cập nhật rubric và hạn nộp của trợ giảng bị trôi sau hàng chục tin nhắn thảo luận bài của các bạn trong nhóm chat Zalo. |
| Hiện đang xử lý bằng cách nào (workaround)? | Chụp ảnh màn hình các đoạn tin nhắn quan trọng gửi vào mục "Cloud của tôi" trên Zalo hoặc tự copy paste vào ứng dụng Google Keep/Notion cá nhân. |
| Mất bao lâu, bao lần? | Mỗi tối mất 20–25 phút trước giờ ngủ (khoảng 22h–23h) mở lần lượt Canvas LMS, nhóm Zalo lớp và Teams để rà soát; lặp lại đều đặn 4–5 buổi/tuần. |
| Insight / opportunity rút ra | Nỗi đau lớn nhất không nằm ở việc thiếu lịch của LMS (LMS đã có lịch rõ ràng), mà nằm ở việc thông tin bài tập bị phân mảnh ở **các kênh chat phi chính thức (Zalo/Teams)** với định dạng văn bản tự do, rất dễ trôi mất nếu không đọc kịp. |

#### Interview Snapshot #2 — Trải nghiệm từ Vũ Quang Huy

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 2 ngành Công nghệ Thông tin (Vũ Quang Huy), theo dõi nhiều kênh học tập và thông báo môn học cùng lúc |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Thông báo thì giảng viên gửi qua Email trường, bài tập thì nộp trên LMS, còn lịch dời ca học hay dặn dò bài tập lớn thì trợ giảng lại nhắn vào nhóm Zalo; mỗi tối mở đủ 3 cái ứng dụng để check bài là hết cả buổi tối."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Đợt vừa rồi giảng viên gửi email thông báo thay đổi đề cương và dời hạn nộp bài tập lớn, nhưng vì hòm thư sinh viên nhận quá nhiều email thông báo tự động từ trường nên email quan trọng bị trôi mất, dẫn đến bị nộp trễ 1 ngày. |
| Hiện đang xử lý bằng cách nào (workaround)? | Dùng một cuốn sổ tay nhỏ đặt trên bàn học để tự ghi lại danh sách deadline đầu tuần; tuy nhiên giữa tuần giảng viên đổi lịch đột xuất là sổ tay bị sai lệch ngay. |
| Mất bao lâu, bao lần? | Đầu mỗi tuần mất khoảng 30–40 phút ngồi gom bài; mỗi buổi tối mất thêm 15–20 phút kiểm tra lại các kênh; kỳ trước từng bị trễ 1 bài tập quan trọng. |
| Insight / opportunity rút ra | Thông tin quan trọng thường bị "chôn vùi" trong biển thông báo; giải pháp cần có tính năng **bóc tách chính xác nội dung chứa bài tập/hạn chót** thay vì bắt sinh viên phải tự đọc và lọc thủ công hàng chục thông báo mỗi ngày. |

#### Interview Snapshot #3 — Trải nghiệm từ Phạm Lê Chuẩn

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 2 ngành Kỹ thuật Hệ thống / IT (Phạm Lê Chuẩn), thường xuyên làm bài tập kỹ thuật và đồ án nhóm |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Mình muốn có một công cụ nhìn vào là biết tối nay và ngày mai phải nộp bài gì ngay lập tức, chứ không muốn mất thời gian tự tay ngồi gõ từng đầu việc vào ứng dụng nhắc việc."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Thứ Sáu tuần trước, ngồi sửa lỗi code cho bài lab đến tận 1h sáng nên quên bẵng mất có một bài kiểm tra trắc nghiệm lý thuyết ngắn phải hoàn thành trước 23h59 trên LMS. |
| Hiện đang xử lý bằng cách nào (workaround)? | Dùng ứng dụng nhắc việc trên điện thoại (Apple Reminders / Google Tasks) nhưng vì phải tự gõ tay từng bài nên nhiều hôm mệt mỏi quên không nhập, dẫn đến app không nhắc được. |
| Mất bao lâu, bao lần? | Mất 15–20 phút tự đối chiếu và kiểm tra lịch mỗi ngày; tháng trước bị trễ 2 bài quiz trắc nghiệm do không ai nhắc. |
| Insight / opportunity rút ra | Sinh viên có tâm lý ngại nhập liệu thủ công; việc tổng hợp bài tập phải diễn ra **tự động hoặc bán tự động (tối thiểu thao tác nhập tay)**, và phải làm nổi bật những việc sắp hết hạn trong vòng 24 giờ tới. |

#### Tổng hợp kết quả kiểm chứng:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn sâu (The Mom Test) | 3 (Minh, Huy, Chuẩn) | Cả 3/3 sinh viên xác nhận mất 15–25 phút mỗi tối để rà soát bài tập; việc bỏ sót deadline đều do thông báo bị phân mảnh ở nhiều kênh (LMS, Zalo, Teams, Email). | Chuẩn phản bác: Nếu giải pháp yêu cầu cấp mật khẩu hoặc quyền đọc toàn bộ tin nhắn Zalo cá nhân thì sẽ không dùng vì lo ngại an toàn dữ liệu riêng tư.<br>Minh & Huy phản bác: Nếu bot tự động gom quá nhiều thông báo rác (lời cảm ơn, chat chit trong nhóm lớp) thì sẽ làm ngập lụt thông báo và bị tắt chuông. |
| Micro survey trong lớp | 8 sinh viên lớp L3B | 7/8 sinh viên xác nhận phải theo dõi bài tập từ 3 nguồn trở lên; 6/8 người từng bị sót hoặc suýt trễ deadline ít nhất 1 lần trong tháng trước. | 1/8 sinh viên cho biết lớp họ giảng viên cam kết 100% chỉ dùng Canvas LMS nên chỉ cần xem LMS là đủ; 2/8 người đề nghị phải có chế độ tóm tắt ngắn gọn dưới 5 dòng mỗi tối thay vì gửi danh sách quá dài. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
1. **Thu hẹp ranh giới (Boundary) và cách lấy dữ liệu:** Nhóm hủy bỏ ý tưởng "tự động đọc mọi tin nhắn từ Zalo cá nhân" (vướng rào cản bảo mật và quyền riêng tư theo phản bác của Chuẩn ở Giả định #5). Thay vào đó, nhóm chuyển sang mô hình lai: **Tự động đồng bộ bài tập chính thức từ LMS qua chuẩn iCal/RSS + Cho phép sinh viên chủ động forward/dán tin nhắn dặn dò vào bot để AI bóc tách ngày giờ hạn nộp.**
2. **Cơ chế xác nhận con người (Human-in-the-loop):** Để tránh việc AI trích xuất nhầm hoặc làm phiền sinh viên (theo phản bác của Minh và Huy về ngập lụt thông báo), nhóm bổ sung bước: Hệ thống chỉ gửi **1 bản tin Daily Digest ngắn gọn vào lúc 22h00** tóm tắt các task sắp tới, sinh viên kiểm tra và bấm xác nhận trước khi lưu vào lịch cá nhân.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Canvas LMS Calendar Feed (iCal)** | https://community.canvaslms.com/t5/Student-Guide/How-do-I-subscribe-to-the-Calendar-feed-using-Google-Calendar/ta-p/522 | Bước 1: Lấy bài tập chính thức từ LMS Canvas đồng bộ về Google/Apple Calendar. | Chuẩn iCal toàn cầu, hoàn toàn tự động, độ trễ thấp, ổn định 100%, không tốn chi phí và không cần AI. | Hoàn toàn không lấy được bài tập dặn dò qua Zalo, Teams, slide hay email của giảng viên. | **Không dùng AI cho phần LMS**. Bước này chỉ cần dùng Rule (iCal feed) có sẵn, vừa chính xác tuyệt đối vừa tiết kiệm tài nguyên. |
| **Motion (usemotion.com)** | https://www.usemotion.com/ | Bước tự động tính toán và xếp lịch làm bài tập vào các khoảng thời gian trống trong ngày. | Thuật toán xếp lịch và phân bổ thời gian theo mức độ ưu tiên và deadline rất thông minh. | Chi phí quá đắt ($19/tháng), không phù hợp sinh viên; người dùng vẫn phải tự gõ task thủ công; không có khả năng đọc hiểu tin nhắn chat tiếng Việt. | Sinh viên không cần một hệ thống xếp lịch đắt tiền, nhu cầu cốt lõi nằm ở bước **thu thập và trích xuất thông tin rải rác từ các kênh chat/email tiếng Việt**. |
| **Template n8n: AI Message Summarizer & Task Extractor** | https://n8n.io/workflows/1888-summarize-messages-using-openai/ | Bước 2–3: Đọc tin nhắn từ kênh chat (webhook), dùng LLM trích xuất deadline thành cấu trúc JSON. | Kiến trúc Workflow định sẵn rõ ràng, dùng AI bóc tách ngôn ngữ tự nhiên thành dữ liệu có cấu trúc rất hiệu quả. | Zalo hạn chế API bot cá nhân; nếu AI trích xuất sai ngày giờ deadline mà tự động tạo lịch sẽ gây hậu quả bỏ sót bài. | Áp dụng mô hình Workflow của n8n nhưng **bắt buộc phải có bước sinh viên duyệt lại (Human-in-the-loop)** trước khi đưa task vào lịch chính thức. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 6 bước, khoảng 45–50 phút thao tác cho một chu kỳ họp + theo dõi,
6/6 bước thủ công (không tính thời gian họp và thời gian thực hiện task)

[1 Đọc lại ghi chú/tin nhắn sau họp: 10']
→ [2 Tách task, owner và deadline: 15'] ← BOTTLENECK
→ [3 Gửi danh sách phân công vào nhóm chat: 5']
→ [4 Thành viên báo trạng thái rải rác trong chat: không cố định]
→ [5 Trưởng nhóm tìm và đối chiếu các cập nhật: 15']
→ [6 Trưởng nhóm nhắn nhắc hoặc hỏi lại: 5']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Handoff / ghi chú |
|---:|---|---|---|---|---|
| 1 | Trưởng nhóm / người ghi chép | Ghi chú họp và lịch sử chat Zalo/Discord | Các đoạn chứa quyết định, task hoặc deadline | Khoảng 10 phút sau mỗi buổi họp | Chuyển các đoạn liên quan sang bước 2; có thể phải lướt lại nhiều tin nhắn |
| 2 | Trưởng nhóm / người ghi chép | Các đoạn thông tin từ bước 1 | Danh sách task gồm nội dung, owner và deadline | Khoảng 15 phút sau mỗi buổi họp | **Bottleneck:** chuyển danh sách cho cả nhóm; dễ thiếu owner/deadline hoặc hiểu nhầm người thực hiện |
| 3 | Trưởng nhóm | Danh sách task đã tổng hợp | Tin nhắn phân công trong nhóm chat | Khoảng 5 phút sau mỗi buổi họp | Handoff sang từng thành viên; danh sách có thể bị trôi khi xuất hiện tin nhắn mới |
| 4 | Thành viên | Task được giao và kết quả đang thực hiện | Tin nhắn “đang làm/đã xong/bị chặn” | Không cố định trong tuần | Handoff ngược lại cho trưởng nhóm; cách báo trạng thái chưa thống nhất |
| 5 | Trưởng nhóm | Lịch sử chat và các cập nhật từ thành viên | Bảng trạng thái tạm thời trong đầu/ghi chú riêng | Khoảng 15 phút cho mỗi lần kiểm tra tiến độ | Phải tìm và đối chiếu thủ công; dễ bỏ sót hoặc ghi nhận trùng |
| 6 | Trưởng nhóm | Trạng thái đã đối chiếu và deadline | Tin nhắn nhắc việc hoặc câu hỏi xác nhận | Khoảng 5 phút cho mỗi lần kiểm tra | Handoff cho thành viên cần cập nhật; phụ thuộc vào trưởng nhóm chủ động nhắc |

**Bottleneck chính:** Bước 2 — chuyển nội dung họp/chat không có cấu trúc thành danh sách task có đủ nội dung, owner và deadline. Bằng chứng hiện có trong báo cáo cá nhân ghi nhận mất 25–30 phút sau một buổi họp để đọc lại và tổng hợp action item; đã có một task bị trễ vì hai thành viên hiểu nhầm người thực hiện. Khi cần tìm lại quyết định/tài liệu cũ, một thành viên còn mất 15–20 phút/lần, khoảng 3–4 lần/tuần. CP4 cần xác nhận các tín hiệu này với người dùng ngoài nhóm.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 5 bước, mục tiêu dưới 10 phút thao tác sau mỗi buổi họp,
3/5 bước có thao tác thủ công

[1 Người ghi chép chọn ghi chú/đoạn chat được phép dùng: 2'] ← CON NGƯỜI
→ [2 Kiểm tra đủ trường task–owner–deadline: <1']           ← RULE
→ [3 Trích xuất action item thành bản nháp: 1']              ← AI
→ [4 Trưởng nhóm đối chiếu nguồn, sửa và xác nhận: 5']       ← CON NGƯỜI
→ [5 Xác nhận cập nhật bảng task; gửi/nhắc theo hạn: 1']      ← CON NGƯỜI + RULE

BOUNDARY:
- AI chỉ xử lý ghi chú hoặc đoạn chat được thành viên chủ động cung cấp; không tự đọc chat riêng.
- Nếu nguồn không nêu owner hoặc deadline, AI phải đánh dấu “thiếu thông tin”, không tự suy đoán.
- AI không tự giao việc, đổi deadline, đánh dấu hoàn thành hoặc gửi thông báo cho cả nhóm.
- Trưởng nhóm phải đối chiếu từng task, owner và deadline với nội dung nguồn trước khi xác nhận.

PHƯƠNG ÁN QUAY VỀ:
- Nếu AI trích xuất thiếu/sai hoặc không hoạt động, trưởng nhóm bỏ bản nháp AI và điền thủ công
  template task–owner–deadline–status. Rule nhắc hạn vẫn chạy trên dữ liệu đã được xác nhận.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 | 5 | Gộp việc tìm/chép lại thành một bản nháp có cấu trúc |
| Tổng thời gian thao tác | Khoảng 45–50 phút cho một chu kỳ họp + kiểm tra tiến độ | Dưới 10 phút sau họp; việc nhắc hạn chạy từ dữ liệu đã xác nhận | Baseline 45–50 phút là tổng ước lượng từ các bước; CP4 cần kiểm chứng |
| Số bước thủ công | 6/6 | 3/5 | Trưởng nhóm vẫn chọn nguồn, duyệt và xác nhận cập nhật |
| Bottleneck chính | Tách task/owner/deadline và tìm lại cập nhật trong chat | Trưởng nhóm kiểm tra và sửa bản nháp | Điểm kiểm tra của con người được giữ để bảo đảm chất lượng |
| Rủi ro mới phát sinh | — | AI bỏ sót task, gán nhầm owner/deadline; lộ nội dung chat | Xử lý bằng boundary, HITL và phương án quay về |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên làm bài tập/dự án theo nhóm, đặc biệt là trưởng nhóm hoặc người chịu trách nhiệm theo dõi tiến độ |
| **Quy trình** | Sau buổi họp hoặc khi có task mới, nhóm phải đọc lại ghi chú/tin nhắn, tách action item, xác định người phụ trách và deadline, gửi lại phân công, nhận cập nhật trạng thái rồi nhắc các task sắp hoặc đã trễ hạn |
| **Bottleneck** | Chuyển nội dung thảo luận rải rác thành danh sách task có đủ nội dung, owner và deadline; riêng bước đọc lại và tổng hợp hiện mất khoảng 25–30 phút sau mỗi buổi họp và vẫn có nguy cơ hiểu nhầm hoặc bỏ sót |
| **Impact** | Trưởng nhóm mất thời gian tổng hợp và nhắc thủ công; thông tin bị trôi trong chat có thể làm hai người hiểu nhầm phân công, trùng việc hoặc để task trễ, ảnh hưởng tiến độ và kết quả chung |
| **Success Metric** (baseline → target, cách đo) | Thời gian tổng hợp action item sau họp từ 25–30 phút xuống dưới 10 phút, đồng thời 100% task trong nội dung nguồn có đủ task/owner/deadline hoặc được đánh dấu “thiếu thông tin”. Đo bằng cách trưởng nhóm bấm giờ từ lúc bắt đầu đọc lại nội dung đến lúc gửi danh sách đã xác nhận trong 4 buổi họp liên tiếp, rồi đối chiếu danh sách với ghi chú/chat nguồn. Baseline/target phải được cập nhật nếu CP4 cho bằng chứng khác. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không tự truy cập chat riêng, tự giao việc, đổi owner/deadline, đánh dấu task hoàn thành hoặc tự gửi thông báo. Trưởng nhóm phải đối chiếu mọi task, owner và deadline với nội dung nguồn và xác nhận trước khi cập nhật bảng chung hoặc gửi cho thành viên. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **Phản biện từ AI:** Metric ban đầu trộn hai pain khác nhau — “tổng hợp action item sau họp” và “theo dõi tiến độ trong tuần” — nên khó biết cải thiện đến từ bước nào. Baseline cũng mới dựa trên trải nghiệm của một thành viên.
- **Trạng thái nhóm cần xác nhận:** Đồng ý hay không với việc thu hẹp metric chính vào thời gian tổng hợp action item sau họp; sau CP4, thay dòng này bằng quyết định thật của nhóm và số liệu đã được kiểm chứng.

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
