# Báo cáo nhóm — Day 02 Discovery & Problem Framing

## 1. Thông tin nhóm

- Tên nhóm: NhomCold — Lớp: L3B.
- Thành viên: [TEAM.md](../../TEAM.md).
- Candidate: Khi tiếp nhận yêu cầu bồi thường kèm hình ảnh xe tai nạn, nhân viên giám định muốn xác định bộ phận hư hỏng và ước lượng chi phí sửa chữa, để có cơ sở đánh giá mức bồi thường và tư vấn khách hàng.
- Mức can thiệp: Chưa chốt; so sánh sau khi kiểm chứng và phân tích quy trình.
- Quyết định: Chưa chốt Go / Not Yet / No-Go cho candidate sửa chữa ô tô; đánh giá tại CP6.

## 2. Hội tụ nhóm (CP3)

Nhóm 4 người, 12 candidate.

### 2.1. Candidate

| # | Người có card | Candidate | Actor | Bottleneck |
|---:|---|---|---|---|
| 1 | Vũ Lương Duy | Chép đơn từ inbox | Chủ shop | Chép trường thông tin sang bảng quản lý |
| 2 | Vũ Lương Duy | Tồn kho lệch giữa các kênh | Chủ shop | Cập nhật kho thủ công |
| 3 | Vũ Lương Duy | Đăng sản phẩm nhiều kênh | Chủ shop | Viết và điều chỉnh mô tả |
| 4 | Nguyễn Thảo Quyên | Xác định hư hỏng xe | Giám định viên | Đối chiếu hư hỏng, phụ tùng và giá |
| 5 | Nguyễn Thảo Quyên | Tìm đúng phụ tùng | Nhân viên phụ tùng | Đối chiếu mã và tính tương thích |
| 6 | Nguyễn Thảo Quyên | Kiểm tra bài tập | Giảng viên | Đọc bài và đối chiếu rubric |
| 7 | Hồ Nguyễn Minh Sang | Tổng hợp ghi chú họp | Thành viên nhóm | Gom ghi chú theo chủ đề |
| 8 | Hồ Nguyễn Minh Sang | Chốt sổ thu chi nhà trọ hằng tháng | Chủ nhà trọ, người quản lý | Đối chiếu thanh toán và công nợ theo phòng/kỳ |
| 9 | Hồ Nguyễn Minh Sang | Hiểu khái niệm khó khi research | Người học, dev | Tra thuật ngữ và tìm cách giải thích phù hợp kiến thức nền |
| 10 | Mai Danh Hiếu | Tổng hợp tiến độ nhóm | Người điều phối | Đọc cập nhật và hỏi lại |
| 11 | Mai Danh Hiếu | Phân công phù hợp khả năng | Nhóm trưởng | Cân đối tải và chuyển đầu việc |
| 12 | Mai Danh Hiếu | Bàn giao việc phụ thuộc | Người nhận bàn giao | Đợi và yêu cầu bổ sung đầu vào |

### 2.2. Cluster

| Cluster | Candidate | Pattern chung |
|---|---|---|
| A — Tổng hợp và diễn giải thông tin | #1, #7, #9, #10 | Chuyển thông tin rời rạc hoặc khó hiểu thành nội dung có cấu trúc để sử dụng |
| B — Đối chiếu số liệu và giao dịch | #2, #8 | Đối chiếu lượng tồn, khoản thanh toán hoặc công nợ để xác định trạng thái đúng |
| C — Đánh giá và đối chiếu chuyên môn | #4, #5, #6 | Xác định bộ phận, mã tương thích hoặc mức độ đáp ứng tiêu chí dựa trên căn cứ chuyên môn |
| D — Phối hợp và xuất bản | #3, #11, #12 | Phụ thuộc đầu vào, tải công việc hoặc nhiều nơi nhận |

### 2.3. Opportunity Solution Tree rút gọn

```text
OUTCOME: Giảm thời gian lập dự toán sửa chữa ban đầu cho hồ sơ bồi thường ô tô,
         đồng thời kiểm soát hạng mục bỏ sót và sai lệch chi phí
├── Opportunity: Khó xác định đầy đủ bộ phận hư hỏng từ ảnh và thông tin xe
├── Opportunity: Tốn công đối chiếu phụ tùng tương thích và phương án sửa/thay
├── Opportunity: Phải tra cứu giá phụ tùng và công sửa chữa từ nhiều nguồn
└── Opportunity: Khó đối chiếu căn cứ của từng hạng mục trong dự toán
     ✗ "Nhận diện hư hỏng bằng Computer Vision"       ← đây là SOLUTION, gạch bỏ khỏi tầng này
     ✗ "Hệ thống tự tra phụ tùng và đề xuất chi phí"  ← đây là SOLUTION, gạch bỏ khỏi tầng này
     ✗ "Agent tự xử lý hồ sơ"                        ← đây là SOLUTION, gạch bỏ khỏi tầng này
```

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được 4 mức | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Xác định hư hỏng và ước lượng chi phí sửa chữa | 5 | 5 | 2 | 5 | 3 | 5 | 3 | **28** |
| Tra cứu và xác định phụ tùng ô tô | 5 | 5 | 2 | 4 | 4 | 4 | 3 | 27 |
| Chốt sổ thu chi nhà trọ hằng tháng | 5 | 5 | 1 | 5 | 5 | 2 | 3 | 26 |

**Chọn:** Xác định hư hỏng và ước lượng chi phí sửa chữa.

**Vì sao chọn:** Quy trình rõ, đo được thời gian lập dự toán, hạng mục bỏ sót và sai lệch chi phí; có cơ sở so sánh checklist, Rule, Workflow và Agent. Phạm vi lab chỉ gồm dự toán ban đầu để người giám định kiểm tra. Điểm bằng chứng thấp vì số phút trong card là ước lượng; điểm vừa sức lab thấp hơn hai bài còn lại do cần hồ sơ và dữ liệu giá.

**Vì sao loại hai candidate kia:** Tra cứu phụ tùng hẹp hơn và đã là một bước trong bài toán được chọn, nên giữ làm phần phân tích sâu. Sổ nhà trọ dễ đo và vừa sức hơn nhưng chủ yếu là phép tính xác định; bảng tính và Rule có thể đủ, ít cơ sở so sánh các mức cao hơn. Cả ba chỉ đạt 3 điểm hiểu domain vì cần người trực tiếp làm nghiệp vụ đối chiếu.

**Bất đồng:** Không có bất đồng được ghi nhận.

## 3. Kiểm chứng + research (CP4)

> CP4–CP6 bên dưới còn là nội dung đề tài deadline cũ, chưa phải kết quả cho candidate sửa chữa ô tô vừa chốt.

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng | Bằng chứng | Cách kiểm / ngưỡng quyết định |
|---:|---|---|---:|---:|---|
| 1 | Người ngoài nhóm mất ≥10 phút/ngày kiểm hạn | Value | 5 | 1 | Hỏi 3 học viên nhóm khác về lần gần nhất; ít nhất 2 người mô tả sự việc và thời gian cụ thể |
| 2 | Có đổi hạn chỉ nằm trong chat | Value | 5 | 1 | Đối chiếu toàn bộ thông báo hạn trong 14 ngày với LMS; không có trường hợp nào thì bỏ giả thuyết này |
| 3 | Sai thông tin dẫn tới trễ hoặc suýt trễ | Value | 4 | 1 | Ghi lại sự việc, nguồn hạn và cách xử lý; không suy từ lời khen giải pháp |
| 4 | LMS thực tế xuất được lịch | Feasibility | 4 | 1 | Thử một sự kiện và một lần đổi hạn trên tài khoản được phép; docs Moodle không chứng minh nền tảng lớp |
| 5 | Coach duy trì được nguồn thông báo chuẩn | Viability | 5 | 1 | Coach xác định kênh, người cập nhật và cách đính chính; không tự tạo quy định cho lớp |
| 6 | Học viên kiểm được hai nguồn trong ≤5 phút | Usability | 3 | 1 | Đo bấm giờ trong pilot; ghi cả lần phải hỏi lại |

### 3.2. Trạng thái bằng chứng và thiết kế kiểm chứng

Trong repo có **0 snapshot phỏng vấn ngoài nhóm, 0 phản hồi survey và 0 bản đếm log** để sử dụng. Đây là số bản ghi có trong tài liệu, không khẳng định ngoài đời không ai được hỏi. Không có trích dẫn người dùng hoặc tín hiệu phản bác thực nghiệm để đưa vào kết quả.

| Nguồn | Dữ liệu hiện có | Kết luận được phép |
|---|---|---|
| Bản nhóm ban đầu | Ước lượng khoảng 20 phút/ngày | Giả thuyết baseline, không phải trung bình đã đo |
| RULES/SUBMISSION | Hạn mặc định theo ca và quy định gia hạn trên LMS | Có quy tắc đối chiếu chính thức; phản bác việc mặc định mọi hạn đều chỉ ở chat |
| Phỏng vấn, survey, log | Không có bản ghi trong repo | Không tính tỉ lệ xác nhận hay nhận điểm kiểm chứng từ dữ liệu giả |

**Kế hoạch:** dùng [bộ câu hỏi CP4](../assets/cp4-interview-guide.md), hỏi 3 học viên ngoài nhóm, 5–7 phút/người. Mỗi snapshot lưu vai trò, ngày giờ GMT+7, cách hỏi, sự việc gần nhất, thời gian, workaround, câu nói nguyên văn và tín hiệu phản bác. Không công khai tên, email hoặc nội dung nội bộ.

Đối chiếu log 14 ngày: đếm thông báo hạn, thông báo thiếu trên LMS và câu hỏi trùng; lưu liên kết hoặc ảnh đã ẩn danh. Tỉ lệ thiếu trên LMS = số thông báo chỉ có trong chat / tổng thông báo hạn. Mẫu số bằng 0 thì ghi không áp dụng.

**Điều có thể bác bỏ problem:** người được hỏi chỉ dùng LMS và kiểm dưới 5 phút; hoặc mọi thay đổi đều cập nhật đầy đủ trên LMS. Đây là điều kiện tìm kiếm, không phải câu trả lời đã thu được.

**Problem được sửa:** bỏ khẳng định “học viên đều mất 20 phút và trễ hạn vì chat”; thu hẹp thành giả thuyết “khó đối chiếu hạn có hiệu lực giữa các nguồn”. Quyết định đổi từ Go sang Not Yet vì thiếu bằng chứng Value và điều kiện vận hành.

### 3.3. Research giải pháp có sẵn

Nguồn chính thức được mở và đối chiếu trong lần rà soát ngày 09/11/2026.

| Công cụ / pattern | Nguồn | Giải bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học |
|---|---|---|---|---|---|
| Moodle Calendar export | [Moodle Docs](https://docs.moodle.org/en/Calendar_export) | Đưa hạn LMS vào lịch | Xuất ICS hoặc URL lịch | Cần xác minh nền tảng lớp; đăng ký URL khác nhập file một lần | Có thể dùng Rule có sẵn, không cần xây công cụ mới |
| Todoist Quick Add | [Todoist Help](https://www.todoist.com/help/articles/use-task-quick-add-in-todoist-va4Lhpzz) | Ghi việc và ngày giờ nhanh | Hỗ trợ nhập ngày giờ tự nhiên | Vẫn phải chọn đúng thông báo; có thể nhận nhầm chữ trong tên việc thành ngày | Nhập nhanh không giải quyết xác thực nguồn |
| Events from Gmail | [Google Calendar Help](https://support.google.com/calendar/answer/6084018) | Tạo lịch cho loại email được hỗ trợ | Có liên kết email gốc | Tài liệu liệt kê đặt chỗ, vé và xác nhận sự kiện; không bảo đảm nhận deadline lab | Không dựa vào tính năng này để thu gom hạn khóa học |

**Kết luận research:** sửa cách đối chiếu nguồn trước; chỉ thử đồng bộ nếu LMS thực tế hỗ trợ. Research công cụ không thay thế phỏng vấn người dùng.

## 4. Quy trình trước/sau (CP5)

### 4.1. Hiện tại

Thời gian dưới đây là **ước lượng thiết kế**, không phải số đo. Đơn vị là một lần kiểm tra/người/ngày có đối chiếu README; ngày không có lab thì bỏ bước đó.

| Bước | Actor | Input → output | Phút ước lượng |
|---:|---|---|---:|
| 1 | Học viên | LMS → danh sách bài và hạn | 3 |
| 2 | Học viên | Chat lớp → thông báo cần đối chiếu | 10 |
| 3 | Học viên | Email → thông báo liên quan | 2 |
| 4 | Học viên | README/SUBMISSION → quy tắc theo ca | 2 |
| 5 | Học viên | Các nguồn → ghi chú cá nhân | 2 |
| 6, nếu mâu thuẫn | Học viên + coach | Câu hỏi → xác nhận nguồn có hiệu lực | 5 phút thao tác; ghi riêng thời gian đợi |

```text
[LMS 3'] → [Chat 10' ← BOTTLENECK giả thuyết] → [Email 2']
→ [README 2'] → [Ghi chú 2'] → [Mâu thuẫn? hỏi coach +5']
Tổng: 19 phút thông thường; 24 phút nếu phải hỏi, cộng thời gian đợi.
```

### 4.2. Tương lai

Phương án chính là No AI, chỉ dùng nguồn và quyền truy cập đang có. Kênh thông báo chuẩn của coach là phương án cần thống nhất với người vận hành, không coi như đã tồn tại.

| Bước | Actor | Input → output | Phút mục tiêu |
|---:|---|---|---:|
| 1 | Học viên | LMS → hạn chính thức | 2 |
| 2 | Học viên | Kênh thông báo của coach → thay đổi có nguồn | 1 |
| 3 | Học viên | Hai nguồn + quy tắc theo ca → danh sách đối chiếu | 1 |
| 4 | Học viên | Danh sách đúng → ghi chú/lịch cập nhật | 1 |
| 5, nếu mâu thuẫn | Học viên + coach | Nguồn lệch → yêu cầu làm rõ | +5 phút thao tác; đo riêng thời gian đợi |

```text
[LMS 2'] → [Thông báo coach 1'] → [Đối chiếu 1'] → [Ghi lịch 1']
                                └─ mâu thuẫn → [Hỏi coach +5']
Rule tùy chọn: đăng ký URL lịch thay việc chép hạn; người học vẫn kiểm nguồn.
```

**Boundary:** không AI hoặc script nào được tự đặt hạn, suy diễn tin trao đổi thành gia hạn hoặc tự sửa nguồn lớp. Gia hạn chỉ có hiệu lực theo thông báo key coach trên LMS, phù hợp RULES. Khi nguồn lệch, hỏi coach và giữ cả hai nguồn để đối chiếu; không mặc định tin mới nhất trong chat thắng LMS.

**Quay về:** lịch lỗi, thiếu bài hoặc lệch giờ → ngừng dựa vào lịch cá nhân, kiểm trực tiếp LMS và thông báo chính thức. Không triển khai bot đọc chat hoặc yêu cầu coach thay quy trình trong vòng tài liệu này.

### 4.3. Before / after

| Chỉ số | Trước, ước lượng | Sau, mục tiêu | Cách kiểm |
|---|---|---|---|
| Bước thường xuyên của học viên | 5 | 4 | Không tính nhánh hỏi lại |
| Thời gian/lượt | 19 phút | ≤5 phút | Bấm giờ từ mở nguồn đầu tiên đến lưu danh sách |
| Lượt có mâu thuẫn | 24 phút + đợi | 10 phút + đợi | Tính vào số trung bình ngày, ghi riêng thời gian đợi |
| Thao tác thủ công | 5/5 bước thường xuyên | 4/4, giảm 1 bước chép nếu dùng Rule | Không gọi bước đối chiếu là tự động |
| Rủi ro | Sót hoặc nhầm hạn | Tin lịch cá nhân quá mức | Đối chiếu nguồn và ngưỡng dừng |

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| Actor | Học viên K5 học nhiều lab |
| Quy trình | Xem LMS, chat, email, README rồi ghi lịch và hỏi lại khi lệch |
| Bottleneck | Tìm và đối chiếu thông báo trong chat; giả thuyết 10 phút/lượt |
| Impact | Khoảng 20 phút/ngày theo ước lượng ban đầu; nguy cơ sót bài, chưa có số sự cố thực đo |
| Success Metric | Từ khoảng 20 xuống ≤5 phút/ngày; đo trước/sau trên 4 thành viên |
| Boundary | Không tự đặt/sửa hạn; học viên kiểm nguồn và hỏi coach khi lệch |

**Phản biện trong vòng rà soát:** khoảng 20 phút không phải baseline đo; tổng các bước thường xuyên là 19 phút; metric tốc độ thiếu chất lượng; đồng bộ LMS và sự đồng ý của coach đang bị coi là sẵn có. V1 tách số ước lượng, bổ sung tỉ lệ đầy đủ và điều kiện bật Rule.

## 6. Mức can thiệp AI (CP6)

**Ma trận:** độ mơ hồ thấp vì hạn có đáp án đúng; độ phức tạp thấp ở phương án tương lai hai nguồn, không có quyết định mở cần AI tự lập kế hoạch.

| Mức | Phương án | Đủ khi nào | Rủi ro | Kết luận |
|---|---|---|---|---|
| No AI | Checklist nguồn và ghi lịch thủ công | Hai nguồn đủ và kiểm trong 5 phút | Phụ thuộc cập nhật nguồn | Chọn thử đầu tiên |
| Rule | Đăng ký URL lịch LMS | Hỗ trợ thực tế và có bước đối chiếu | Lịch cập nhật trễ hoặc thiếu | Chỉ bật sau kiểm tra |
| Workflow | AI trích hạn từ tin tự do, người duyệt | Có bằng chứng mẫu tin cố định không đủ | Nhầm suy đoán thành hạn thật | Không chọn vòng này |
| Agent | Tự đọc nhiều kênh và quyết định sửa lịch | Không có nhu cầu được chứng minh | Quyền rộng, sai hạn khó phát hiện | Không chọn |

**Vì sao No AI đủ để thử:** bottleneck giả thuyết là chọn đúng nguồn; checklist xử lý trực tiếp mà không cần quyền tích hợp. Chỉ lên Rule nếu phần chép lịch còn tốn công và đồng bộ vượt kiểm thử. Không khẳng định Rule đã phủ một tỉ lệ thông báo khi thiếu log.

Theo worksheet CP6, No AI/Rule không cần AI Canvas và câu hỏi PAIR; tiêu chí đánh giá dưới đây áp dụng cho quy trình và dữ liệu lịch, không phải đầu ra mô hình.

## 7. Problem Statement v1 + tiêu chí đánh giá

| Trường | Nội dung |
|---|---|
| Actor | Học viên K5 có nhiều nguồn hạn cần đối chiếu, cần xác minh bằng phỏng vấn ngoài nhóm |
| Quy trình | Xem LMS → kiểm thông báo coach → đối chiếu → cập nhật danh sách; hỏi khi lệch |
| Bottleneck | Tìm nguồn hạn có hiệu lực; giả thuyết 10 phút trong 19 phút/lượt |
| Impact | Tốn thời gian kiểm tra; không gán số bài trễ cho nguyên nhân thông tin khi thiếu log |
| Success Metric | Baseline thiết kế 19 phút, cần thay bằng B = trung bình 4 người × 3 ngày; pilot 4 người × 5 ngày có trung bình ≤5 phút/ngày, giảm ≥50% so với B; 100% bài và hạn khớp nguồn, 0 bài trễ do lịch sai |
| Cách đo | Nhật ký từng lượt có ngày, phút thao tác, phút đợi, số bài, số lệch và nguồn; đối chiếu danh sách với LMS mỗi ngày; ngày thiếu ghi chép không tính bằng 0 |
| Boundary | Không tự quyết hạn; key coach xác nhận gia hạn trên LMS; mâu thuẫn phải hỏi người có thẩm quyền |
| AI intervention point | **Không có**; bài toán đối chiếu nguồn dùng checklist và quy tắc xác định |
| Mức chọn | No AI; Rule là tùy chọn có điều kiện |
| Rủi ro và người kiểm tra | Học viên kiểm thiếu/sai hạn; coach xác nhận nguồn và thay đổi chính thức |

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Baseline | Khoảng 20 phút | 19 phút thiết kế và công thức đo B | Tổng các bước và loại bằng chứng phải nhất quán |
| Metric | Chỉ tốc độ | Thêm đầy đủ, chính xác và trễ do lịch sai | Tránh nhanh nhưng sót bài |
| Mức can thiệp | No AI + Rule | No AI trước, Rule có điều kiện | Tài liệu công cụ không xác minh LMS thực tế |
| Quyền quyết định | Nguồn coach/LMS nói chung | Gia hạn theo key coach trên LMS | Phù hợp RULES, xử lý rõ mâu thuẫn |

| # | Tiêu chí | Đạt | Không đạt |
|---:|---|---|---|
| 1 | Đầy đủ | 100% bài có hạn trong phạm vi đối chiếu có trong danh sách | Thiếu ít nhất 1 bài |
| 2 | Chính xác | Tất cả hạn khớp nguồn, đúng ca và GMT+7 | Sai ngày, giờ, ca hoặc nguồn |
| 3 | Truy vết | Mỗi hạn có link nguồn; thay đổi lưu hạn cũ/mới và thời điểm | Không xác định được nguồn có hiệu lực |
| 4 | Xử lý mâu thuẫn | Đánh dấu và hỏi coach, không tự ghi đè hạn | Tự chọn một hạn mà không kiểm |
| 5 | Hiệu quả | Trung bình ≤5 phút/ngày và giảm ≥50% so với B | Vượt một trong hai ngưỡng |

## 8. Quyết định (CP6)

| Rủi ro | Mức | Căn cứ |
|---|---|---|
| Value | Cao | Không có snapshot ngoài nhóm hoặc log để chứng minh pain và nguyên nhân |
| Usability | Trung bình | Checklist đơn giản nhưng thiếu lượt thử hoàn thành có đo thời gian |
| Feasibility | Trung bình | Làm thủ công được; tính năng đồng bộ của LMS lớp không có bằng chứng thử |
| Viability | Trung bình | Phụ thuộc người cập nhật nguồn; không coi sự đồng ý của coach là sẵn có |

**Quyết định: Not Yet.** Có rủi ro Value cao nên không giữ kết luận Go của bản nháp. Đây là quyết định hoàn chỉnh theo bằng chứng hiện có, không phải yêu cầu người dùng xác nhận lựa chọn giải pháp.

**Điều kiện chuyển Go cho pilot:** có 3 snapshot ngoài nhóm, ít nhất 2 mô tả lần kiểm hạn mất ≥10 phút với hành vi cụ thể; có đối chiếu log nguồn; xác định người vận hành nguồn; đo baseline đủ 12 người-ngày. Nếu đa số kiểm dưới 5 phút và nguồn LMS đủ, No-Go cho công cụ mới, giữ checklist cá nhân.

**Pilot nhỏ nhất sau khi đủ điều kiện:** 4 học viên, 5 ngày học, No AI trước; ghi thời gian và chấm 5 tiêu chí mỗi ngày. Rule chỉ thử riêng sau khi một sự kiện và một thay đổi hạn khớp nguồn; không nhập file ICS một lần rồi gọi là đồng bộ.

**Ngưỡng dừng:** một hạn sai hoặc thiếu bài → ngừng dựa vào lịch, đối chiếu LMS ngay; một bài trễ do lịch sai → dừng pilot; sau 5 ngày trung bình >5 phút hoặc giảm <50% → không mở rộng, xem lại bottleneck. Không có quyền duy trì nguồn → giữ checklist cá nhân, không triển khai lớp.

**Bước tiếp theo:** thu 3 snapshot theo guide (20 phút), đối chiếu log 14 ngày (15 phút), đo baseline 3 ngày rồi đánh giá gate ở trên. Không gửi tin nhắn coach, truy cập tài khoản hay nộp LMS trong phạm vi chỉnh tài liệu.

## 9. Hạn chế và hướng tiếp theo

Bằng chứng hiện tại đủ thiết kế cách kiểm, không đủ xác nhận nhu cầu hay hiệu quả. Số phút từng bước là ước lượng thiết kế; không dùng để tính phần trăm cải thiện thực tế. Snapshot, nhật ký pitch trực tiếp, đóng góp theo tài khoản và reflection cá nhân phải dựa vào hoạt động thật. Nếu candidate deadline bị bác bỏ, xem lại tổng hợp tiến độ của Hiếu vì báo cáo cá nhân đã ghi thời gian và lượt hỏi lại cụ thể.

## 10. Tài liệu tham khảo

- [Moodle Calendar export](https://docs.moodle.org/en/Calendar_export).
- [Todoist Quick Add](https://www.todoist.com/help/articles/use-task-quick-add-in-todoist-va4Lhpzz).
- [Google Calendar — Events from Gmail](https://support.google.com/calendar/answer/6084018).
- [Framework và nguồn gốc phương pháp](../../docs/03-international-frameworks.md).
