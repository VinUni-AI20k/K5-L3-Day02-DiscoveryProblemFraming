# Báo cáo nhóm — Day 02 Discovery & Problem Framing

## 1. Thông tin nhóm

- Tên nhóm: 3AE
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi nhận yêu cầu đặt lịch, cố vấn dịch vụ muốn có mô tả nhu cầu đủ rõ, để chuyển cho kỹ thuật viên mà không phải hỏi lại khách nhiều đợt.
- Quyết định cuối: Not Yet

---

## 2. Hội tụ nhóm (CP3)

*Người chính: Nguyễn Minh Quân · Hỗ trợ: Nguyễn Đức Minh, Phan Gia Bảo, Vũ Lê Hoàng*

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---|---|---|---|---|---|
| 1 | Nguyễn Đức Minh | Khi nhận ca, muốn biết việc dở để không sót | Nhân viên ca sau | Hỏi lại ca trước | Lần gần nhất việc bàn giao chỉ bằng hỏi lại ca trước khiến bạn bỏ sót công việc là khi nào, và hậu quả cụ thể là gì? (Nguyễn Minh Quân) |
| 2 | Nguyễn Đức Minh | Khi hết ca, muốn báo cáo nhanh, để quản lý khỏi gọi hỏi | Trưởng ca | Viết lại sự cố | Vì sao trưởng ca phải viết lại sự cố vào cuối ca, thông tin chưa được ghi nhận hay đã có nhưng nằm rải rác? (Nguyễn Minh Quân) |
| 3 | Nguyễn Đức Minh | Khi có người mới, muốn họ tự tra quy trình, để khỏi hỏi lại | Nhân viên mới | Hỏi lại người cũ | Người mới hỏi lại vì chưa có tài liệu, khó tìm tài liệu hay tài liệu có nhưng khó hiểu? (Nguyễn Minh Quân) |
| 4 | Phan Gia Bảo | Khi chuẩn bị báo cáo tuần, muốn nhận biết những triệu chứng được khách phản ánh nhiều, để trưởng xưởng ưu tiên kiểm tra và theo dõi. | Cố vấn dịch vụ | Phải đọc từng phiếu và gộp các mô tả cùng nghĩa nhưng khác câu chữ trước khi thống kê, dễ đếm trùng hoặc bỏ sót. | Tại sao không có 1 từ điển mã lỗi chung để dễ thống kê lỗi hơn, thay vì ghi các lỗi khác nhau làm loạn thống kê ? (Vũ Lê Hoàng) |
| 5 | Phan Gia Bảo | Khi tiếp nhận xe khách đã sửa chữa trước đó, muốn nắm nhanh lịch sử sự cố và cách xử lý, để tránh hỏi lại và cung cấp đủ thông tin cho kỹ thuật viên. | Cố vấn dịch vụ, khách hàng | Phải đọc nhiều phiếu sửa chữa và ghi chú rời rạc để tìm thông tin liên quan đến triệu chứng hiện tại. | Lịch sử này nằm ở đâu? Trên phần mềm quản lý xưởng, trên sổ bảo hành giấy của khách, hay lưu trong hệ thống FOTA (cập nhật phần mềm từ xa) của xe điện? (Vũ Lê Hoàng) |
| 6 | Phan Gia Bảo | Khi bàn giao xe sau sửa chữa, muốn giải thích dễ hiểu những hạng mục đã làm và lưu ý sử dụng, để khách hiểu và thực hiện đúng. | Cố vấn dịch vụ, nhân viên | Phiếu sửa chữa có thuật ngữ và ghi chú kỹ thuật; phải diễn giải lại theo tình trạng từng xe, dễ bỏ sót lưu ý. |  |
| 7 | Vũ Lê Hoàng | Khi khách hàng gọi hotline hoặc đến xưởng hỏi giá, tôi muốn có ngay bảng báo giá sơ bộ cho các mốc bảo dưỡng tiêu chuẩn, để trả lời khách ngay lập tức. | Khách hàng, Cố vấn dịch vụ | Chờ đợi người trả lời. Trường hợp hotline bận thì không thể gọi được trong khi thông tin này là cố định và có thể báo nhanh cho khách được | Nếu đã có bảng giá cố định, vì sao vẫn phải chờ người trả lời?<br>Giá sơ bộ có đủ để báo khách khi chưa kiểm tra xe không?<br>(Phan Gia Bảo) |
| 8 | Vũ Lê Hoàng | Khi khách phàn nàn về lỗi pin hoặc linh kiện, tôi muốn trích xuất ngay điều khoản trong chính sách bảo hành mới nhất, để giải thích rõ ràng việc nào miễn phí, việc nào tính phí. | Cố vấn dịch vụ, khách hàng | Phần này có trong chính sách của công ty, nhưng khách hàng thường không dành thời gian để đọc | Chỉ dựa vào điều khoản bảo hành đã xác định được việc nào miễn phí chưa? (Phan Gia Bảo) |
| 9 | Vũ Lê Hoàng | Khi nhận xe tại xưởng, tôi muốn thông tin từ hệ thống booking đồng bộ ngay thành lệnh sửa chữa chi tiết, để KTV có thể bắt đầu làm việc lập tức mà không phải chờ đợi. | Cố vấn dịch vụ, <br>Kĩ thuật viên | Cố vấn dịch vụ phải nhập tay | Thông tin đặt lịch đã đủ để kỹ thuật viên bắt đầu sửa chữa chưa? Cần kiểm tra những thông tin nào trước khi tạo lệnh sửa chữa? (Phan Gia Bảo) |
| 10 | Nguyễn Minh Quân | Làm rõ mô tả nhu cầu trước khi bàn giao | An, cố vấn dịch vụ tiếp nhận và chuẩn bị mô tả nhu cầu cho kỹ thuật viên. | Phải hỏi bổ sung nhiều đợt | Thông tin hay thiếu nhất là gì: triệu chứng, đời xe hay số km? Nếu luôn thiếu đúng mấy mục đó thì thêm ô bắt buộc vào form đặt lịch đã đủ chưa? (Nguyễn Đức Minh) |
| 11 | Nguyễn Minh Quân | Tra cứu câu trả lời dịch vụ đúng trường hợp | An, cố vấn dịch vụ phụ trách phản hồi câu hỏi của khách. | Tìm đúng đoạn tài liệu | Khách hỏi lặp lại cùng các câu hay mỗi lần một khác? Tài liệu dịch vụ dài bao nhiêu trang mà phải mất công tìm? (Nguyễn Đức Minh) |
| 12 | Nguyễn Minh Quân | Cập nhật bản chuẩn bị sau khi khách đổi lịch/nhu cầu | An, cố vấn dịch vụ cập nhật thông, kỹ thuật viên phụ trách lịch hẹn. | Đối chiếu các phiên bản để tìm phần cần cập nhật | Khách đổi lịch hoặc đổi nhu cầu mấy lần một tuần? Nếu ít thì đối chiếu bằng tay có thật sự là vấn đề không? (Nguyễn Đức Minh) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A - Chuẩn hóa và cập nhật thông tin bàn giao | Bàn giao ca bị sót việc dở; Nhập tay thông tin đặt lịch thành lệnh sửa chữa; Làm rõ mô tả nhu cầu trước khi bàn giao cho kỹ thuật viên; Cập nhật bản chuẩn bị khi khách đổi lịch hoặc đổi nhu cầu | Thông tin chuyển từ người này sang người kia (ca trước → ca sau, khách → cố vấn → kỹ thuật viên) bị thiếu, thay đổi giữa chừng hoặc phải nhập tay lại, nên người nhận phải hỏi bổ sung nhiều đợt trước khi bắt tay làm |
| B - Tra cứu và diễn giải thông tin dịch vụ đúng trường hợp | Nhân viên mới hỏi lại quy trình; Giải thích hạng mục đã sửa cho khách; Báo giá các mốc bảo dưỡng; Giải thích điều khoản bảo hành; Tra cứu câu trả lời dịch vụ đúng trường hợp | Thông tin đã có sẵn (bảng giá, chính sách bảo hành, quy trình, phiếu sửa chữa) nhưng khó tìm đúng đoạn hoặc khó hiểu, nên người hỏi phải chờ, phải hỏi người khác hoặc cố vấn phải diễn giải lại từng trường hợp |
| C - Tổng hợp lịch sử sự cố để hỗ trợ xử lý | Báo cáo sự cố cuối ca; Thống kê triệu chứng khách phản ánh nhiều; Nắm lịch sử sửa chữa của xe | Ghi chép sự cố nằm rải rác ở nhiều phiếu, mỗi người mô tả một kiểu, nên muốn báo cáo, thống kê hay xem lịch sử xe đều phải đọc lại từng phiếu và gộp bằng tay, dễ trùng hoặc sót |

### 2.3. Opportunity Solution Tree rút gọn

```text
OUTCOME: Cố vấn dịch vụ xử lý một lượt khách nhanh hơn và ít phải hỏi lại
         (đo bằng: số phút mỗi lượt tiếp nhận, số lần hỏi lại khách hoặc kỹ thuật viên mỗi lượt)
├── Opportunity A: Thông tin khách đưa vào thiếu hoặc đổi giữa chừng, cố vấn phải hỏi lại
│                   nhiều đợt và nhập tay lại trước khi giao cho kỹ thuật viên
├── Opportunity B: Thông tin dịch vụ có sẵn nhưng khó tìm đúng đoạn, khó hiểu, khách phải chờ
│                   hoặc cố vấn phải diễn giải lại từng trường hợp
└── Opportunity C: Ghi chép sự cố rải rác, mỗi người viết một kiểu, muốn xem lịch sử xe
                    hay thống kê phải đọc lại từng phiếu
```

**Những ý đã gạch bỏ vì là solution đội lốt opportunity:**

- "Có bảng báo giá sơ bộ cho các mốc bảo dưỡng": là cách giải cho nhánh B.
- "Đồng bộ booking thành lệnh sửa chữa": là cách giải cho nhánh A.
- "Trích xuất điều khoản bảo hành": là cách giải cho nhánh B.
- "Từ điển mã lỗi chung" (câu hỏi phản biện cho candidate thống kê triệu chứng): là cách giải cho nhánh C.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---|---|---|---|---|---|---|---|
| Cố vấn phải hỏi lại khách nhiều đợt vì mô tả nhu cầu lúc đặt lịch thiếu | 5 | 4 | 2 | 4 | 4 | 5 | 2 | 26 |
| Khách và cố vấn mất công tìm, hiểu thông tin dịch vụ (giá, bảo hành, quy trình) | 3 | 3 | 2 | 3 | 3 | 2 | 2 | 18 |
| Ghi chép sự cố rải rác, khó xem lịch sử xe và thống kê lỗi | 4 | 3 | 2 | 3 | 3 | 4 | 1 | 20 |

**Candidate được chọn:** Khi nhận yêu cầu đặt lịch, cố vấn dịch vụ muốn có mô tả nhu cầu đủ rõ, để chuyển cho kỹ thuật viên mà không phải hỏi lại khách nhiều đợt.

**Vì sao chọn:** Actor rõ (cố vấn dịch vụ tiếp nhận lịch); 3 thành viên cùng đưa ra một nỗi khó (Nguyễn Đức Minh, Vũ Lê Hoàng, Nguyễn Minh Quân); quy trình vẽ được từ đặt lịch đến bàn giao cho kỹ thuật viên; có chỗ để so sánh giữa thêm ô bắt buộc vào form (Rule) với các mức dùng AI.

**Vì sao loại các candidate còn lại:** Loại "khó tìm, khó hiểu thông tin dịch vụ": giá mốc bảo dưỡng và chính sách bảo hành là thông tin cố định, đăng sẵn hoặc làm câu hỏi thường gặp là đủ, ít chỗ để bàn về AI (đúng câu phản biện Phan Gia Bảo đặt cho candidate báo giá và bảo hành). Loại "ghi chép sự cố rải rác": cần dữ liệu phiếu sửa chữa nhiều tháng mà nhóm không có, và nhóm không ai hiểu nghiệp vụ xưởng (domain 1/5).

**Xử lý bất đồng (nếu có):** [nhóm điền nếu có]

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

*Người chính: Nguyễn Đức Minh · Hỗ trợ: Nguyễn Minh Quân, Phan Gia Bảo, Vũ Lê Hoàng*

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? | Người làm |
|---|---|---|---|---|---|---|
| 1 | Hơn một nửa số lịch đặt bảo dưỡng có mô tả nhu cầu thiếu, khiến cố vấn phải gọi lại khách hỏi thêm | Value | 5 | 1 | ✅ | Nguyễn Minh Quân |
| 2 | Thông tin hay thiếu chỉ là vài mục cố định (triệu chứng, số km, thời điểm xuất hiện lỗi) | Value | 4 | 1 | ✅ | Nguyễn Đức Minh |
| 3 | Khách sẵn lòng trả lời thêm 2–3 câu hỏi ngay lúc đặt lịch, không bỏ dở | Usability | 4 | 2 | ✅ | Vũ Lê Hoàng |
| 4 | Công ty cho phép đưa nội dung đặt lịch của khách vào công cụ xử lý bên ngoài | Viability | 4 | 1 | Sau lab (hỏi người làm ở xưởng) | Phan Gia Bảo |

**Giả định nhóm kiểm chứng trong buổi này:** #1 (Nguyễn Minh Quân) và #2 (Nguyễn Đức Minh).

### 3.2. Kiểm chứng

**Cách đã dùng:** Log, ticket, review — tư liệu công khai trên mạng (3 nguồn, người trong nghề dịch vụ ô tô kể lại chuyện đã xảy ra) + phỏng vấn người từng đặt lịch sửa xe (nhóm điền ở snapshot 4).

*Lưu ý: snapshot 1–3 là tư liệu công khai, nhóm không trực tiếp phỏng vấn những người này.*

**Snapshot 1 — tư liệu công khai (KTAR, Mỹ) (Nguyễn Đức Minh)**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò) | Chủ một xưởng sửa hộp số, dẫn chương trình radio về xe hơi |
| Câu nói đáng nhớ nhất (nguyên văn) | "Long story short, they fixed the wrong noise." |
| Lần gần nhất gặp vấn đề: chuyện gì đã xảy ra? | Khách tả tiếng kêu mơ hồ, cố vấn không yêu cầu khách chỉ ra tiếng kêu; xưởng sửa một tiếng kêu khác, vô hại |
| Workaround hiện tại | Khuyên khách đề nghị người tiếp nhận cùng nghe, cùng thử lỗi trước khi để xe lại |
| Mất bao lâu, bao lần? | Gần 500 USD và 2 ngày không có xe |
| Insight | Mô tả thiếu ngay lúc tiếp nhận khiến cả lượt sửa đi sai hướng |

**Snapshot 2 — tư liệu công khai (diễn đàn quản lý xưởng DealersEdge) (Phan Gia Bảo)**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò) | Quản lý xưởng dịch vụ, cố vấn dịch vụ, tư vấn đại lý |
| Câu nói đáng nhớ nhất (nguyên văn) | "Customer states there is a problem with the brakes." |
| Lần gần nhất gặp vấn đề: chuyện gì đã xảy ra? | Cố vấn chép nguyên lời khách lên phiếu, không hỏi thêm; có phiếu kết thúc bằng "không tìm thấy lỗi" |
| Workaround hiện tại | Đào tạo lại cố vấn cách đặt câu hỏi bổ sung |
| Mất bao lâu, bao lần? | Không có số liệu |
| Insight | Nguyên nhân nằm cả ở thói quen hỏi của cố vấn, không chỉ ở khách |

**Snapshot 3 — tư liệu công khai (DealerELITE, bài cho bộ phận dịch vụ đại lý) (Nguyễn Minh Quân)**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò) | Đơn vị tư vấn cho bộ phận dịch vụ đại lý ô tô |
| Câu nói đáng nhớ nhất (nguyên văn) | "So now the tech has to try all 4 doors to find out which one you're talking about." |
| Lần gần nhất gặp vấn đề: chuyện gì đã xảy ra? | Phiếu ghi "cửa không mở được" nên kỹ thuật viên phải thử cả 4 cửa; mô tả mơ hồ dẫn tới sửa lại và bị từ chối bảo hành |
| Workaround hiện tại | Hướng dẫn cố vấn ghi rõ triệu chứng theo mẫu |
| Mất bao lâu, bao lần? | Không có số liệu |
| Insight | Mô tả thiếu gây hại ở 3 chỗ: thời gian kỹ thuật viên, xe quay lại sửa, tiền bảo hành |

**Tổng hợp:**

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---|---|---|
| Tư liệu công khai (radio, diễn đàn, bài chuyên ngành) | 3 | Cả 3 xác nhận mô tả thiếu lúc tiếp nhận gây sửa sai, tốn thời gian kỹ thuật viên, tốn tiền khách | Diễn đàn cho thấy lỗi nằm ở thói quen hỏi của cố vấn, nên đào tạo hoặc danh sách câu hỏi bắt buộc (không cần AI) có thể đã đủ. Cả 3 nguồn ở Mỹ, chưa có nguồn Việt Nam hay VinFast |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Thu hẹp từ "khách mô tả thiếu" thành "cố vấn không có bộ câu hỏi bổ sung theo từng loại triệu chứng khi tiếp nhận". Thêm phương án không dùng AI (danh sách câu hỏi bắt buộc) để so sánh ở CP6. Giả định #1 vẫn chưa có số liệu Việt Nam.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| myKaarma Service Pre-Diag (công cụ cho đại lý ô tô ở Mỹ)<br>(Nguyễn Đức Minh) | https://support.mykaarma.com/hc/en-us/articles/45647747400211-Service-Pre-Diag-AI-Overview-Smarter-Service-Conversations-Before-Check-In | Sau khi khách đặt lịch, trước khi xe tới: gửi bảng hỏi theo từng xe qua tin nhắn, AI tóm tắt cho cố vấn | Đúng bước nghẽn của nhóm; cố vấn vẫn đọc lại tóm tắt và xử lý mục "Needs Review" | Khách không trả lời thì không có dữ liệu; tài liệu không nói độ chính xác hay cách xử lý khi AI hiểu sai; số liệu tiết kiệm thời gian là quảng cáo, không có nguồn | Bài toán đã có người giải bằng mức Workflow; nhóm không cần tự xây mà cần xác định bước người kiểm tra và tiêu chí "đạt" |
| ASE C1 — hướng dẫn phỏng vấn khách khi tiếp nhận (luyện thi chứng chỉ cố vấn dịch vụ)<br>(Phan Gia Bảo) | https://www.brakeandfrontend.com/ase-c1-test-prep-customer-interview-and-write-up/ | Lúc tiếp nhận: bộ câu hỏi chuẩn (lỗi là gì, khi nào xảy ra, liên tục hay thỉnh thoảng, điều kiện, lặp lại được không) | Không cần công nghệ; là chuẩn nghề, dùng làm danh sách câu hỏi bắt buộc được ngay | Phụ thuộc cố vấn có hỏi đủ hay không; không nói cách ghi phiếu theo mẫu | Là nền cho mức Rule: biến bộ câu hỏi này thành ô bắt buộc trong form đặt lịch |
| Motor Magazine — "Make your initial assessment count" (2012)<br>(Vũ Lê Hoàng) | https://www.motor.com/wp-content/uploads/MakeYourInitialAssessmentCount-Feb-2012.pdf | Chuyển thông tin từ cố vấn sang kỹ thuật viên | Chỉ rõ hậu quả: kỹ thuật viên đoán từ thông tin sai, mất thời gian, khách quay lại | Bài viết, không có số liệu thống kê | Tiêu chí "đạt" của phiếu tiếp nhận phải là đủ để kỹ thuật viên không phải đoán |

---

## 4. Quy trình trước/sau (CP5)

*Người chính: Phan Gia Bảo · Hỗ trợ: Nguyễn Minh Quân, Nguyễn Đức Minh, Vũ Lê Hoàng*

### 4.1. Quy trình hiện tại

*Thời gian là ước lượng của nhóm, chưa bấm giờ thật.*

| # | Bước | Actor | Input | Output | Thời gian / tần suất |
|---|---|---|---|---|---|
| 1 | Đọc lịch đặt mới | Cố vấn dịch vụ | Lịch đặt từ app / web / hotline | Danh sách xe sắp tới | ~2 phút / lịch, mỗi ngày |
| 2 | Gọi lại khách hỏi thêm khi mô tả thiếu | Cố vấn dịch vụ | Mô tả tự do của khách | Mô tả bổ sung | ~5 phút / lần, có thể 2 đợt ← BOTTLENECK |
| 3 | Ghi phiếu tiếp nhận | Cố vấn dịch vụ | Mô tả đã bổ sung | Phiếu tiếp nhận | ~3 phút |
| 4 | Khách tới xưởng, hỏi lại tại quầy | Cố vấn dịch vụ, khách | Phiếu tiếp nhận | Phiếu đã xác nhận | ~5 phút |
| 5 | Tạo lệnh sửa chữa, nhập tay lại | Cố vấn dịch vụ | Phiếu đã xác nhận | Lệnh sửa chữa | ~3 phút |
| 6 | Bàn giao cho kỹ thuật viên | Cố vấn → kỹ thuật viên | Lệnh sửa chữa | Kỹ thuật viên bắt tay sửa | ~2 phút; nếu thiếu thì kỹ thuật viên hỏi lại cố vấn |

**Bottleneck chính:** Bước 2, gọi lại khách hỏi thêm vì mô tả lúc đặt lịch thiếu (khoảng 5–10 phút mỗi lịch, ước lượng). Tổng khoảng 20–25 phút mỗi lượt.

### 4.2. Quy trình tương lai

| # | Bước | Ai / cái gì làm | Ghi chú |
|---|---|---|---|
| 1 | Khách đặt lịch, điền các ô bắt buộc (loại lỗi, khi nào xảy ra, liên tục hay thỉnh thoảng, số km) + mô tả tự do | Rule (form đặt lịch) | Ô bắt buộc lấy từ bộ câu hỏi chuẩn ASE C1 |
| 2 | Đọc mô tả tự do, gợi ý 2–3 câu hỏi còn thiếu và soạn nháp phiếu tiếp nhận theo mẫu | AI hỗ trợ | Không chẩn đoán, không báo giá |
| 3 | Duyệt câu hỏi gợi ý, sửa, rồi gửi khách hoặc hỏi khi khách tới | Cố vấn dịch vụ (người kiểm tra) | Boundary: không câu hỏi nào gửi khách nếu cố vấn chưa duyệt |
| 4 | Xác nhận phiếu với khách tại quầy | Cố vấn dịch vụ | Ngắn hơn vì phiếu đã gần đủ |
| 5 | Tạo lệnh sửa chữa từ phiếu đã duyệt, bàn giao kỹ thuật viên | Cố vấn dịch vụ |  |

**Boundary:** AI không chẩn đoán lỗi, không báo giá, không kết luận bảo hành, không tự nhắn hay gọi khách, không sửa thông tin khách đã điền.

**Phương án quay về:** Gợi ý sai hoặc nháp kém → cố vấn bỏ qua, dùng danh sách câu hỏi cố định in sẵn (mức Rule), như quy trình hiện tại.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---|---|---|
| Số bước | 6 | 5 |  |
| Tổng thời gian mỗi lượt | ~20–25 phút (ước lượng) | ~10–12 phút | Cần bấm giờ thật để có baseline |
| Bước thủ công | 6/6 | 3/5 | Cố vấn vẫn duyệt, xác nhận, bàn giao |
| Bottleneck | Gọi lại khách hỏi thêm | Cố vấn duyệt câu hỏi gợi ý | Chấp nhận được vì đây là điểm kiểm soát chất lượng |
| Rủi ro mới | — | AI gợi ý câu hỏi thừa, sai, hoặc tóm tắt sai lời khách | Xử lý bằng boundary và tiêu chí đánh giá ở mục 7 |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| Actor | Cố vấn dịch vụ tiếp nhận lịch đặt bảo dưỡng, sửa chữa tại xưởng dịch vụ |
| Quy trình | Đọc lịch đặt → gọi lại khách hỏi thêm → ghi phiếu tiếp nhận → xác nhận tại quầy → tạo lệnh sửa chữa → bàn giao kỹ thuật viên |
| Bottleneck | Gọi lại khách hỏi thêm vì mô tả lúc đặt lịch thiếu, và cố vấn không có bộ câu hỏi bổ sung theo từng loại triệu chứng (~5–10 phút mỗi lịch, ước lượng) |
| Impact | Mất thời gian cố vấn; kỹ thuật viên đoán từ thông tin thiếu, có thể sửa sai, khách quay lại (theo tư liệu công khai ở mục 3.2) |
| Success Metric | Số lần gọi lại khách mỗi lịch: [đo 1 tuần] → tối đa 1; thời gian tiếp nhận mỗi lượt: [đo 1 tuần] → giảm 50%; đo bằng cố vấn tự ghi trong 2 tuần pilot |
| Boundary | Không tự nhắn khách, không chẩn đoán lỗi, không báo giá; cố vấn duyệt mọi thứ trước khi tới khách hoặc kỹ thuật viên |

**Phản biện nhận được:** Metric chỉ đo tốc độ, chưa đo chất lượng: tiếp nhận nhanh hơn mà phiếu vẫn thiếu thì kỹ thuật viên vẫn phải hỏi lại. Nhóm đồng ý, thêm metric chất lượng ở v1.

---

## 6. Mức can thiệp AI (CP6)

*Người chính: Vũ Lê Hoàng · Hỗ trợ: Nguyễn Minh Quân, Nguyễn Đức Minh, Phan Gia Bảo*

**Ma trận:** Độ mơ hồ cao (khách mô tả bằng lời tự do: tiếng kêu, mùi, cảm giác lái; mỗi lần một kiểu). Độ phức tạp thấp–trung bình (các bước cố định, không rẽ nhánh). → Workflow có AI ở một bước.

| Mức | Phương án | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| No AI | Đào tạo cố vấn + danh sách câu hỏi in sẵn tại quầy | Cố vấn luôn hỏi đủ, khách tới trực tiếp | Không giảm số lần gọi lại trước khi xe tới | Dùng làm phương án quay về |
| Rule | Ô bắt buộc trong form đặt lịch theo bộ câu hỏi ASE C1 | Lỗi rơi vào vài loại cố định | Không đọc được mô tả tự do; khách có thể bỏ dở form dài | Dùng cho bước 1 |
| Workflow | Form bắt buộc → AI gợi ý câu hỏi còn thiếu + soạn nháp phiếu → cố vấn duyệt | Các bước cố định, AI chỉ làm phần đọc và viết | Gợi ý sai, tóm tắt sai lời khách | Chọn |
| Agent | AI tự nhắn khách, tự hỏi tiếp, tự tạo lệnh sửa chữa | Khi bước tiếp theo không đoán trước được | Tự liên hệ khách, khó kiểm soát, nhiều quyền truy cập | Không chọn |

**Vì sao không chọn mức đơn giản hơn:** Rule (ô bắt buộc) chỉ bắt được các mục cố định; mô tả tự do kiểu "xe kêu như tiếng tất khô" (ví dụ trên diễn đàn DealersEdge) không vào được ô nào, và đây chính là phần cố vấn phải gọi lại hỏi. Tuy vậy bằng chứng còn yếu: nếu khảo sát cho thấy thông tin thiếu chỉ là vài mục cố định (giả định #2) thì Rule là đủ và nhóm sẽ dừng ở Rule.

**AI Canvas rút gọn:**

| Thành phần | Nội dung |
|---|---|
| Prediction | 2–3 câu hỏi còn thiếu cho mô tả của khách; nháp phiếu tiếp nhận theo mẫu (triệu chứng, khi nào, điều kiện, số km) |
| Judgment | Cố vấn quyết định câu hỏi nào cần hỏi, mô tả nào đủ để giao kỹ thuật viên |
| Action | Cố vấn gửi câu hỏi đã duyệt cho khách hoặc hỏi khi khách tới; tạo lệnh sửa chữa |
| Outcome | Số lần gọi lại khách mỗi lịch; số lần kỹ thuật viên hỏi lại cố vấn; tỉ lệ câu hỏi gợi ý bị cố vấn bỏ |
| Input | Nội dung khách điền khi đặt lịch (ô bắt buộc + mô tả tự do), đời xe, số km |
| Feedback | Câu hỏi cố vấn sửa hoặc bỏ mỗi ngày; câu kỹ thuật viên hỏi lại |

**Câu hỏi PAIR:**

- Augment hay automate? Augment. Cố vấn vẫn là người hỏi khách và chịu trách nhiệm phiếu; không gửi gì cho khách nếu cố vấn chưa duyệt.
- Sai kiểu nào tệ hơn? Bỏ sót tệ hơn báo nhầm: thiếu một câu hỏi quan trọng thì kỹ thuật viên sửa sai; thừa một câu hỏi chỉ tốn thêm của khách vài giây. Tiêu chí đánh giá ưu tiên "không bỏ sót thông tin cần thiết".

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| Actor | Cố vấn dịch vụ tiếp nhận lịch đặt bảo dưỡng, sửa chữa, ở xưởng có cho khách mô tả nhu cầu bằng lời tự do khi đặt lịch |
| Quy trình | Đọc lịch đặt → gọi lại khách hỏi thêm → ghi phiếu tiếp nhận → xác nhận tại quầy → tạo lệnh sửa chữa → bàn giao kỹ thuật viên |
| Bottleneck | Gọi lại khách hỏi thêm vì mô tả lúc đặt lịch thiếu, và cố vấn không có bộ câu hỏi bổ sung theo từng loại triệu chứng (~5–10 phút mỗi lịch, ước lượng) |
| Impact | Mất thời gian cố vấn; kỹ thuật viên đoán từ thông tin thiếu, có thể sửa sai, khách quay lại (theo tư liệu công khai ở mục 3.2) |
| Success Metric | (1) Số lần gọi lại khách mỗi lịch: [đo] → tối đa 1; (2) số lần kỹ thuật viên hỏi lại cố vấn: [đo] → giảm 50%; (3) cố vấn bỏ dưới 30% câu hỏi AI gợi ý; đo trong 2 tuần pilot |
| Boundary | AI không chẩn đoán, không báo giá, không kết luận bảo hành, không tự liên hệ khách, không sửa thông tin khách đã điền |
| AI intervention point | Sau khi khách gửi form đặt lịch, trước bước cố vấn gọi lại khách |
| Mức chọn | Workflow (Rule ở bước form + AI ở bước gợi ý câu hỏi, soạn nháp phiếu) |
| Rủi ro & người kiểm tra | Gợi ý sai, bỏ sót, tóm tắt sai lời khách → cố vấn đối chiếu nháp với lời khách trước khi dùng |

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | Cố vấn dịch vụ tiếp nhận lịch đặt | Thêm: ở xưởng cho khách mô tả tự do khi đặt lịch | Nếu xưởng chỉ dùng ô chọn cố định thì Rule là đủ, không cần AI |
| Success Metric | Chỉ đo tốc độ | Thêm số lần kỹ thuật viên hỏi lại và tỉ lệ câu hỏi bị bỏ | Phản biện: nhanh hơn mà phiếu vẫn thiếu thì không đạt |
| Boundary | Không tự nhắn khách, không chẩn đoán, không báo giá | Thêm: không kết luận bảo hành, không sửa thông tin khách điền | Tư liệu DealerELITE: ghi sai mô tả có thể làm mất bảo hành |

**Tiêu chí đánh giá:**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---|---|---|---|
| 1 | Không bỏ sót | Hỏi đủ các mục còn thiếu: triệu chứng, khi nào xảy ra, liên tục hay thỉnh thoảng, điều kiện | Bỏ qua mục còn thiếu mà kỹ thuật viên cần |
| 2 | Không hỏi lại điều khách đã nói | Mọi câu hỏi đều về thông tin chưa có | Hỏi lại điều khách đã ghi trong form |
| 3 | Không bịa, không chẩn đoán | Nháp phiếu chỉ chứa thông tin khách đã đưa | Có nguyên nhân lỗi, giá hoặc kết luận bảo hành |
| 4 | Ngắn, dễ trả lời | Tối đa 3 câu, mỗi câu khách trả lời được trong 1 dòng | Câu dài, dùng thuật ngữ kỹ thuật |

---

## 8. Quyết định (CP6)

| Rủi ro | Mức | Lý do |
|---|---|---|
| Value | Trung bình | Tư liệu công khai xác nhận pain, nhưng cả 3 nguồn ở Mỹ; chưa có số liệu Việt Nam hay VinFast (giả định #1, #2) |
| Usability | Thấp | Cố vấn chỉ duyệt và sửa vài câu hỏi; có phương án quay về là danh sách câu hỏi cố định |
| Feasibility | Trung bình | Đã có công cụ làm gần đúng việc này (myKaarma Service Pre-Diag), nhưng nhóm chưa biết lấy được nội dung đặt lịch từ hệ thống của xưởng không |
| Viability | Cao | Dữ liệu khách hàng; chưa biết quy định nội bộ có cho đưa vào công cụ bên ngoài (giả định #4) |

**Quyết định:** Not Yet. Viability ở mức Cao nhưng kiểm chứng nhanh được bằng cách hỏi người làm ở xưởng; Value cần số liệu Việt Nam trước khi làm.

**Ngưỡng dừng:** Nếu khảo sát 10 người từng đặt lịch cho thấy dưới 30% bị gọi lại hỏi thêm → No-Go. Nếu thông tin thiếu chỉ là vài mục cố định → dừng ở Rule (form bắt buộc). Nếu pilot 2 tuần mà cố vấn bỏ quá 50% câu hỏi AI gợi ý → quay về danh sách câu hỏi cố định.

**Bước tiếp theo:** (1) Khảo sát 10 người từng đặt lịch bảo dưỡng; (2) hỏi một cố vấn dịch vụ thật về số lần gọi lại và quy định dữ liệu; (3) thử form bắt buộc trước, chỉ thêm AI nếu form không đủ.

**Nguồn**

- [KTAR — Ever have your auto shop fix the wrong noise](https://ktar.com/uncategorized/ever-have-your-auto-shop-fix-the-wrong-noise)
- [DealersEdge forum — Terminology](https://forums.dealersedge.com/viewtopic.php?p=48481)
- [DealerELITE — The 3 C's: Customer concern](https://www.dealerelite.net/profiles/blogs/the-3c-s-customer-concern)
- [myKaarma — Service Pre-Diag AI Overview](https://support.mykaarma.com/hc/en-us/articles/45647747400211-Service-Pre-Diag-AI-Overview-Smarter-Service-Conversations-Before-Check-In)
- [Brake & Front End — ASE C1 Test Prep, Customer Interview and Write Up](https://www.brakeandfrontend.com/ase-c1-test-prep-customer-interview-and-write-up/)
- [Motor Magazine — Make Your Initial Assessment Count (2012)](https://www.motor.com/wp-content/uploads/MakeYourInitialAssessmentCount-Feb-2012.pdf)
