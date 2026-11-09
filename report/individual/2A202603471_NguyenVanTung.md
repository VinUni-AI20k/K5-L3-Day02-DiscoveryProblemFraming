# Báo cáo cá nhân — 2A202603471_NguyenVanTung

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Văn Tùng
- MSSV: 2A202603471
- Email trường (không bắt buộc, repo có thể để public): tungnv.2a202603471@student.vinuni.edu.vn
- Tên nhóm: MH2T
- Link repo nhóm: https://github.com/nhtng0212/K5-L3A-Day02-MH2T-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Hệ thống giám sát liên tục đẩy cảnh báo về tiến trình mạng kết nối bất thường, tôi muốn tự động gom nhóm, kiểm tra danh tính địa chỉ IP qua các log và loại bỏ các thông báo trùng lặp, để không phải bấm thủ công hàng trăm lần cho cùng 1 sự việc | SOC Tier 1 | Nhiều cảnh báo trùng lặp trong mỗi ca trực (150–200 cảnh báo/ca, mất 60–90 phút bấm đóng thủ công trên Wazuh SIEM) |
| 2 | Tốn thời gian | Khi có nhân viên viết ticket đẩy lên, tôi muốn hệ thống tự bóc tách log, cô lập tệp vào môi trường phân tích để không làm mất thời gian xây dựng môi trường kiểm thử mà vẫn kịp thời ngăn chặn mã độc | Đội ngũ ứng phó sự cố (Incident Response / Tier 2) | Tần suất 20–50 cảnh báo mỗi tuần và mất từ 15–25 phút để kiểm tra thủ công từng tệp |
| 3 | Cần đọc, tổng hợp nhiều | Khi các sự kiện bảo mật rời rạc xuất hiện cùng lúc trên nhiều máy trạm (như thay đổi khóa đăng ký, tạo dịch vụ ẩn và chạy lệnh mã hóa), tôi muốn xâu chuỗi các hành vi theo dòng thời gian, để phát hiện sớm chiến dịch tấn công trước khi dữ liệu bị mã hóa | Chuyên gia săn tìm mối đe dọa (Threat Hunter) | Xuất hiện trong các chiến dịch kiểm tra xâm nhập hoặc sự cố phức tạp (2–3 lần/tháng), mất 4–6 tiếng đối chiếu log giữa EDR và Firewall |
| 4 | Pain từ người khác | Khi một vụ việc tấn công đã được xử lý xong và cần đóng phiếu trên hệ thống quản lý sự cố, tôi muốn tự động tổng hợp toàn bộ dấu hiệu nhận diện (IoC) và diễn biến thành bản tường trình chuẩn chỉnh, để nộp cho cấp quản lý đúng hạn | Quản lý bộ phận (SOC Manager / CISO), Kỹ sư xử lý sự cố | Các báo cáo tuần thường bị trễ hạn nộp (2/4 tuần gần nhất) do nhân sự phải dồn thời gian soạn thảo thủ công vào cuối tuần (mất 30–45 phút/phiếu sự cố) |
| 5 | Tốn thời gian | Khi có bản tin cảnh báo lỗ hổng phần mềm mới (CVE) xuất hiện với điểm mức độ nghiêm trọng cao, tôi muốn tự động quét toàn bộ danh sách tài sản hiện có trong mạng nội bộ để lọc ra ngay các máy chủ đang sử dụng phiên bản phần mềm phơi nhiễm, để không phải dò tìm thủ công qua từng hệ thống | Kỹ sư quản trị hạ tầng (Sysadmin) | 3 đến 5 đợt công bố lỗ hổng lớn mỗi tháng; mất 3–4 tiếng rà soát thủ công danh sách gói phần mềm trên hơn 50 máy chủ |
| 6 | Lặp lại | Khi tiếp nhận ca trực SOC lúc 7h sáng, tôi muốn nắm ngay tóm tắt các sự cố còn mở và tiến trình xử lý từ ca đêm, để không phải đọc lại từng ticket và chat log rời rạc | SOC Tier 1, Trưởng ca trực | 20–25 phút mỗi lần giao ca, 3 ca/ngày; thỉnh thoảng sót thông tin bàn giao giữa 2 ca trực |
| 7 | Cần đọc, tổng hợp nhiều | Khi cần cấu hình luật tường lửa (firewall rule) mới cho dự án, tôi muốn tra cứu nhanh chính sách và quy hoạch mạng hiện tại, để không làm gián đoạn các dịch vụ đang chạy hoặc tạo lỗ hổng mới | Kỹ sư mạng, DevOps | 3–4 lần/tuần, mất 40 phút/lần tra cứu tài liệu quy hoạch mạng và kiểm tra xung đột rule |
| 8 | Pain từ người khác | Khi tài khoản nhân viên bị khóa do nhập sai mật khẩu nhiều lần, họ muốn được xác minh danh tính và mở khóa an toàn ngay, để tiếp tục làm việc mà không phải chờ IT hỗ trợ quá 30 phút | Nhân viên văn phòng, IT Helpdesk | 10–15 yêu cầu/tuần, thời gian chờ trung bình 35 phút/ticket do IT bận xử lý việc khác |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Ý #6 (bàn giao ca trực SOC) và #7 (tra cứu kiểm tra firewall rule) — vì đây là các tình huống thực tế thường gặp trong quản trị hệ thống và vận hành SOC, có quy trình và thời gian đo lường rõ ràng.
- **Ý bỏ:** AI từng gợi ý *"Trợ lý AI tự động phát hiện và ngăn chặn mọi cuộc tấn công mạng"* — Nhóm quyết định bỏ vì phạm vi quá rộng, mơ hồ, không phản ánh đúng quy trình công việc cụ thể của một vai trò thực tế.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Xử lý thủ công hàng loạt cảnh báo trùng lặp| Xử lý thủ công hàng loạt cảnh báo trùng lặp| Xử lý thủ công hàng loạt cảnh báo trùng lặp , tốn quá nhiều token |
| 2 | Tổng hợp dữ liệu và viết báo cáo sự cố thủ công | Tốn 30–45 phút mỗi phiếu sau khi xử lý xong sự cố, khiến các báo cáo tuần/tháng thường xuyên bị dồn ứ và chậm trễ tiến độ nộp cho cấp quản lý | Mức độ chuẩn hóa của các trường dữ liệu đầu vào trên các công cụ khác nhau (TheHive, SIEM) có thực sự đồng nhất để tự động hóa 100% không|
| 3 | Điều tra, phân tích tệp đính kèm và email lừa đảo | Là điểm khởi đầu của hầu hết các cuộc tấn công mã độc/ransomware, đòi hỏi phải thao tác nhiều bước thủ công qua sandbox và kiểm tra headers khá mất thời gian| Tốc độ phản hồi của các nền tảng sandbox bên ngoài (Any.run hoặc các API phân tích) có đáp ứng kịp thời khi lượng email báo cáo tăng vọt vào giờ cao điểm hay không|

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi hệ thống SIEM đẩy hàng loạt cảnh báo bảo mật lặp lại liên tục, tôi muốn tự động gom nhóm, kiểm tra danh tiếng IP/domain và loại bỏ ngay các thông báo trùng lặp, để không phải bấm thủ công hàng trăm lần cho cùng một sự việc và giữ được sự tập trung|
| Actor | Tier-1 SOC Analyst |
| Thời điểm / bối cảnh | Ngay đầu ca trực hoặc vào các khung giờ cao điểm khi hệ thống ghi nhận lượng log đột biến từ các quy tắc phát hiện nhạy cảm |
| Quy trình hiện tại (3–7 bước) | 1. Mở giao diện bảng điều khiển SIEM (Wazuh) để kiểm tra danh sách cảnh báo mới xuất hiện.<br>2. Nhấp mở từng cảnh báo để đọc chi tiết các trường thông tin (IP nguồn, tài khoản, tiến trình).<br>3. Mở tab trình duyệt mới để tra cứu thủ công điểm uy tín của địa chỉ IP trên các nền tảng Threat Intelligence công khai.<br>4. Đối chiếu lịch sử xem cảnh báo này đã xuất hiện và được xử lý ở ca trước hay chưa.<br>5. Thủ công đánh dấu trạng thái (False Positive / Closed) hoặc chuyển tiếp (Escalate) nếu phát hiện bất thường. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Mất trung bình 3–5 phút cho mỗi cảnh báo lặp |
| Impact (nếu không giải thì sao) | Xảy ra hiện tượng mệt mỏi vì báo động giả (Alert Fatigue), tăng nguy cơ bỏ sót các sự cố tấn công thực sự nguy hiểm |
| Success metric (baseline → target) | Giảm 70% lượng cảnh báo rác phải thao tác thủ công, rút ngắn thời gian xử lý ban đầu từ 5 phút xuống dưới 10 giây/cảnh báo |
| Phương án không dùng AI | Viết thêm các biểu thức chính quy (Regex) cố định, tinh chỉnh ngưỡng kích hoạt (Threshold) của quy tắc trên SIEM, hoặc viết script Bash/Python tĩnh để lọc cứng các IP nằm trong danh sách trắng (Whitelist) |
| Giả thuyết về AI (nếu có) | Sử dụng Agent kết hợp cơ chế tự động tra cứu ngữ cảnh (Contextual Enrichment) và phân loại ý định cảnh báo để tự động đóng các ticket trùng lặp dựa trên hành vi lịch sử thay vì chỉ dựa vào quy tắc lọc tĩnh cứng nhắc |
| Cảm nhận nhanh | Workflow / Agent |

Quy trình nháp hiện tại:

```text
[Bắt đầu ca trực] 
    ↓
[Wazuh SIEM đẩy 500+ cảnh báo] 
    ↓
[Điểm nghẽn: Tier-1 Analyst mở từng cảnh báo tra cứu thủ công (3-5 phút/cảnh báo)] 
    ↓
[Quá tải / Alert Fatigue / Dễ bỏ sót True Positive] 
    ↓
[Kết thúc ca: Báo cáo tồn đọng / Sự cố thực bị che lấp]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi một vụ việc tấn công đã được xử lý xong trên hệ thống quản lý, tôi muốn tự động tổng hợp toàn bộ mốc thời gian, dấu hiệu nhận diện (IoC) và hành động khắc phục thành một bản tường trình chuẩn chỉnh, để bàn giao cho cấp quản lý hoặc phục vụ kiểm toán mà không phải ngồi gõ lại từng mục thủ công |
| Actor | Chuyên gia ứng phó sự cố (Incident Responder / SOC Tier 2) |
| Thời điểm / bối cảnh | Ngay sau khi một phiếu sự cố (Incident ticket trên TheHive) được chuyển sang trạng thái đóng (Closed) hoặc khi cần tổng hợp báo cáo định kỳ hàng tuần |
| Quy trình hiện tại (3–7 bước) | 1. Mở trang quản lý sự cố (TheHive) để xuất dữ liệu chi tiết của vụ việc.<br>2. Mở các công cụ liên quan (SIEM Wazuh, bảng điểm Threat Intelligence, nhật ký EDR) để rà soát lại mốc thời gian (timeline).<br>3. Mở phần mềm soạn thảo văn bản (Word hoặc Notion) và sao chép thủ công các thông tin quan trọng (IP độc hại, mã băm file, tài khoản bị ảnh hưởng).<br>4. Tự viết lại phần mô tả diễn biến tấn công và các bước đội ngũ đã xử lý.<br>5. Định dạng lại bố cục, kiểm tra chính tả và xuất file gửi cho quản lý cấp cao. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Mất từ 30 đến 45 phút cho mỗi báo cáo sự cố |
| Impact (nếu không giải thì sao) | Mất từ 30 đến 45 phút cho mỗi báo cáo sự cố; tỷ lệ trễ hạn báo cáo tuần khoảng 25% |
| Success metric (baseline → target) | Rút ngắn thời gian viết báo cáo từ 30–45 phút/phiếu xuống dưới 10 phút/phiếu, tỷ lệ trễ hạn báo cáo tuần khoảng 0% |
| Phương án không dùng AI | Xây dựng các mẫu báo cáo cố định trên nền tảng quản lý sự cố, tích hợp macro/script tự động kéo trường dữ liệu thô từ API của TheHive vào form có sẵn |
| Giả thuyết về AI (nếu có) | Sử dụng Agent kết nối trực tiếp với API của các công cụ (TheHive, Wazuh) để tự động đọc ngữ cảnh vụ việc, hiểu diễn biến chuỗi tấn công và tự động sinh bản tường trình theo đúng văn phong kỹ thuật chuẩn |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[Đóng phiếu sự cố trên TheHive] 
    ↓
[Mở nhiều tab công cụ khác nhau gom log thủ công: 8 phút] 
    ↓
[Điểm nghẽn: Gõ tay báo cáo, mất 30-45 phút/phiếu] ◄── BOTTLENECK
    ↓
[Báo cáo chậm trễ / Sai sót số liệu IoC] 
    ↓
[Chuyển bàn giao cho CISO / Quản lý: 2 phút]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhân viên báo cáo nhận được email lạ chứa tệp đính kèm hoặc đường dẫn đáng ngờ, tôi muốn hệ thống tự động trích xuất headers, bóc tách tệp vào môi trường cách ly (sandbox) và phân tích hành vi độc hại, để không phải mất thời gian dựng máy ảo kiểm tra thủ công mà vẫn đưa ra kết luận chính xác |
| Actor | Chuyên viên phân tích an ninh mạng (SOC Analyst) |
| Thời điểm / bối cảnh | Khi nhân viên bấm nút báo cáo email (Phishing Report Button) trên hòm thư hoặc gửi thông báo khẩn cấp đến đội ngũ SOC qua kênh nội bộ |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận email báo cáo và yêu cầu người dùng chuyển tiếp dạng tệp gốc (.eml hoặc .msg).<br>2. Mở trình phân tích headers thủ công để kiểm tra nguồn gốc SPF, DKIM, DMARC và đường dẫn chuyển hướng (redirect URLs).<br>3. Tải xuống tệp đính kèm, tính mã băm (hash) và tra cứu trên các nền tảng kiểm tra mã độc cộng đồng.<br>4. Mở máy ảo kiểm tra độc lập (sandbox) để chạy thử nghiệm tệp đính kèm hoặc phân tích sâu URL nếu cần thiết.<br>5. Tổng hợp kết quả, đưa ra phán quyết (Clean / Phishing / Malware) và phản hồi lại cho người dùng đồng thời tạo phiếu ghi nhận sự cố. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, 3 và 4: Kiểm tra headers, bóc tách URL và chờ chạy sandbox kiểm thử tệp mất từ 15 đến 25 phút/email |
| Impact (nếu không giải thì sao) | Chậm trễ xử lý báo cáo email dẫn đến nguy cơ các nhân viên khác click nhầm tệp độc; hàng đợi phân tích email bị dồn ứ |
| Success metric (baseline → target) | Rút ngắn thời gian phản hồi từ 20 phút xuống dưới 3 phút/email, độ chính xác nhận diện đạt > 95% |
| Phương án không dùng AI | Sử dụng cổng bảo mật thư điện tử (Secure Email Gateway - SEG) và các rule lọc regex cứng trên header |
| Giả thuyết về AI (nếu có) | Sử dụng AI phân tích nội dung ngôn ngữ ngữ cảnh trong email (ngữ nghĩa lừa đảo) kết hợp kết quả sandbox để tự động phân loại |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[Nhân viên báo cáo email lạ qua nút Phishing Report] 
    ↓
[Tiếp nhận file .eml và mở công cụ phân tích thủ công: 3 phút] 
    ↓
[Điểm nghẽn: Kiểm tra headers, bóc tách URL và chạy sandbox mất 15-25 phút] ◄── BOTTLENECK
    ↓
[Chậm trễ xử lý / Nguy cơ nhân viên khác click nhầm] 
    ↓
[Đưa ra kết luận và tạo phiếu ghi nhận sự cố: 2 phút]
```

### Card muốn pitch nhất

- Card số: 2
- Vì sao: nó giảm thiểu thời gian viết ticket đẩy lên cho tier2 kiểm tra và xử lý cảnh báo
- Câu hỏi muốn nhóm phản biện: *"Làm thế nào để đảm bảo mô hình AI khi sinh văn bản báo cáo không bị ảo giác (hallucination) làm sai lệch các thông số kỹ thuật nhạy cảm như địa chỉ IP, mã băm mã độc hay mốc thời gian vi phạm?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Rủi ro "Ảo giác" (Hallucination) dữ liệu kỹ thuật | Hoàn toàn đồng ý | Ràng buộc cấu trúc (Structured JSON Output): Bắt buộc Agent phải lấy dữ liệu thô trực tiếp từ các trường API đã định nghĩa sẵn trên TheHive/Wazuh |
| Thiếu sự chuẩn hóa dữ liệu đầu vào | Đồng ý một phần | Chuẩn hóa template log (Data Normalization): Thiết lập trước một khung schema cố định cho các trường đầu vào |
| Vấn đề bảo mật thông tin nhạy cảm (Data Privacy) | Hoàn toàn đồng ý | Triển khai mô hình nội bộ (On-premise LLM): Sử dụng các mô hình mã nguồn mở chạy trực tiếp trên hạ tầng nội bộ của SOC |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày Problem Card #2 (Tự động tổng hợp và viết báo cáo sự cố an ninh mạng) với baseline 30–45 phút/phiếu | Thuyết phục cả nhóm chọn đây làm candidate chính vì giải quyết trực tiếp nỗi đau tốn thời gian hành chính của kỹ sư |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: <br>1. Hỏi bạn Hoàng Tùng (bài lọc cảnh báo SIEM #10): *"Nếu dùng Agent tự động đóng ticket mà bỏ sót một cảnh báo tấn công thật thì ai chịu trách nhiệm?"*<br>2. Hỏi bạn Hoàng Minh (bài mở khóa tài khoản #3): *"Bài này dùng form OTP nội bộ là đủ, có cần giải pháp AI phức tạp không?"* | Đóng góp phản biện then chốt giúp nhóm nhận ra rủi ro pháp lý của việc tự động hóa hoàn toàn; định hướng chọn giải pháp Workflow hỗ trợ (Augment) |
| Nhận phản biện | Câu hỏi tôi nhận được: <br>Bạn Hoàng Tùng hỏi: *"Nếu AI bịa ra một mốc thời gian hoặc ghi sai 1 địa chỉ IP trong báo cáo gửi CISO thì ai chịu trách nhiệm?"* | Tôi đã sửa gì: <br>Bổ sung cơ chế **Locked Schema**: tách riêng bảng IoC/Timeline (trích xuất 100% nguyên bản từ API) và chỉ dùng AI cho đoạn văn tóm tắt diễn biến, có con người ký duyệt |
| Gom cluster / cây OST | Cùng nhóm gom 12 candidate thành 3 cụm; cùng Nhóm trưởng Hoàng Tùng dựng cây OST rút gọn | Tách bạch rõ ràng giữa Outcome và Opportunity, loại bỏ 2 giải pháp trá hình ("Chatbot viết báo cáo", "Multi-Agent tự trị") |
| Chọn candidate problem | Cùng nhóm chấm điểm 7 tiêu chí cho shortlist 3 bài toán | Thống nhất chọn Candidate #2 với số điểm cao nhất (34/35 điểm) |
| Kiểm chứng / research | Soạn câu hỏi phỏng vấn theo phương pháp The Mom Test và phối hợp cùng Quang Huy trực tiếp phỏng vấn 1 Kỹ sư Incident Response | Thu được bằng chứng thực tế: kỹ sư mất 40 phút/báo cáo và cực kỳ mong muốn có công cụ tự gom log vào khung mẫu sẵn |
| Quy trình nhóm | Phối hợp cùng bạn Hoàng Tùng vẽ sơ đồ Before/After bằng ASCII | Xác định chính xác bottleneck nằm ở khâu gom log thủ công và gõ tay văn bản |
| Problem Statement | Soạn thảo bản Problem Statement v0 và cùng hoàn thiện bản v1 | Định nghĩa đầy đủ 6 trường thông tin, đặc biệt là boundary cấm AI tự ý phát hành báo cáo và bắt buộc dùng On-premise LLM |
| Mức can thiệp AI | Phân tích ma trận độ mơ hồ × độ phức tạp; so sánh 4 mức No AI / Rule / Workflow / Agent | Thuyết phục nhóm chọn mức **Workflow** thay vì Agent tự trị để triệt tiêu rủi ro ảo giác và rò rỉ dữ liệu |
| Quyết định | Tham gia đánh giá 4 rủi ro và xác lập phạm vi pilot kèm ngưỡng dừng (Stopping Threshold) | Đưa ra quyết định **Go** cho pilot nhỏ 2 tuần trên các sự cố mức độ Low/Medium |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm các tình huống thường gặp trong quản trị hệ thống và vận hành SOC | Gợi ý các góc nhìn thực tế về bàn giao ca trực và kiểm tra rule firewall | AI đưa ra ý quá rộng kiểu "AI tự động ngăn chặn mọi cuộc tấn công" | Bỏ các ý viển vông, tự viết lại thành các Job Story cụ thể có đo lường thời gian thực tế |
| CP2 Problem Card | Đóng vai "PM hoài nghi" để phản biện điểm yếu của Problem Card #2 | Chỉ ra rủi ro nghiêm trọng về ảo giác dữ liệu (hallucination) và lộ lọt dữ liệu nội bộ | AI khuyên nên dùng Agent tự động đăng bài báo cáo lên hệ thống mà không cần người duyệt | Nhận định bài toán an ninh cần tính pháp lý cao; bổ sung cơ chế khóa dữ liệu thô (Locked Schema) và giữ con người phê duyệt |
| CP4 Research | Tìm kiếm các tài liệu và giải pháp công nghệ hiện có về tự động hóa báo cáo sự cố an ninh | Giúp tìm nhanh tính năng War Room của Cortex XSOAR và SIRP TheHive | AI trích dẫn thiếu link nguồn trực tiếp hoặc đưa link chung chung | Tự tra cứu link tài liệu chính thức từ Palo Alto Networks và TheHive Project để đưa vào bài |
| CP5 Quy trình | Chuyển đổi mô tả các bước thành sơ đồ dạng text/ASCII trực quan | Định dạng sơ đồ luồng dữ liệu nhanh, căn lề thẳng hàng | AI vẽ thiếu bước Fallback (phương án quay về khi AI sinh văn bản không đạt) | Tự bổ sung nhánh rẽ [Phương án quay về: Trả về template trống để kỹ sư gõ tay như cũ] vào sơ đồ |
| CP5–6 Problem Statement | Gợi ý các tiêu chí đánh giá (Eval criteria) cho bài toán sinh báo cáo tự động | Gợi ý tiêu chí về độ bao phủ thông tin và thời gian phản hồi | AI không tính đến khía cạnh bảo mật an toàn (bảo toàn 100% tính chính xác của IoC) | Bổ sung tiêu chí bắt buộc: Data Integrity (100% IoC và Timestamp phải khớp tuyệt đối với log thô) |
| CP6 Mức can thiệp / quyết định | So sánh ưu nhược điểm giữa Workflow và Multi-Agent | Liệt kê các góc nhìn về chi phí vận hành và rủi ro lỗi kỹ thuật | AI thiên vị việc dùng Agent phức tạp cho hợp xu hướng | Nhận định bài toán pháp lý an ninh mạng đòi hỏi tính kiểm soát tuyệt đối nên kiên quyết chốt mức Workflow |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi lắng nghe phần trình bày của bạn Hoàng Tùng, Hoàng Minh và Quang Huy trong nhóm MH2T, tôi nhận ra mọi người đều có xu hướng chọn những bài toán mang tính chất phòng thủ diện rộng hoặc mong muốn hệ thống tự động ngăn chặn tấn công ngay lập tức. Tuy nhiên, qua quá trình mổ xẻ từng bước, tôi thấy rằng những bài toán đó chứa đựng quá nhiều rủi ro vận hành (như chặn nhầm IP khách hàng hoặc phụ thuộc quyền hạn switch mạng). Ngược lại, việc nghe các bạn phản biện về bài toán viết báo cáo sự cố của tôi giúp tôi hiểu rằng một bài toán có quy trình khép kín, dữ liệu đầu vào đã nằm sẵn trong hệ thống (TheHive/Wazuh) và đo lường được thời gian lãng phí rõ ràng lại là ứng viên hoàn hảo nhất để tối ưu hóa.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm tôi bị "solution-first" rất rõ ở giai đoạn đầu của CP3. Khi bắt đầu thảo luận, bạn Hoàng Minh đã hào hứng đề xuất: *"Chúng ta hãy xây dựng một con Multi-Agent tự động: Agent 1 đọc log, Agent 2 tự viết báo cáo, Agent 3 tự gửi email cho CISO và tự đóng ticket"*. Cả nhóm lúc đó thấy ý tưởng này rất 'ngầu' và định bắt tay vào làm ngay. Rất may, khi đưa lên cây Opportunity Solution Tree (OST), tôi và bạn Hoàng Tùng nhận ra đây hoàn toàn là giải pháp kỹ thuật đang đội lốt nhu cầu người dùng. Nỗi đau thực sự của kỹ sư là *"mất 30–45 phút mỗi phiếu chỉ để sao chép dữ liệu rời rạc và gõ văn bản lặp đi lặp lại"*, chứ người dùng không hề có nhu cầu giao phó toàn bộ quyền quyết định cho máy. Nhóm đã kịp thời gạch bỏ cụm từ "Multi-Agent tự trị" ra khỏi cây OST và quay về đào sâu vào các bước nghẽn thực tế.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đã thay đổi hoàn toàn thiết kế sau khi nhận câu hỏi phản biện từ bạn Hoàng Tùng: *"Nếu AI bịa ra một mốc thời gian hoặc ghi sai 1 địa chỉ IP trong báo cáo gửi CISO thì ai chịu trách nhiệm?"*. Lúc đầu, tôi dự định đưa toàn bộ log thô vào một mô hình ngôn ngữ lớn (LLM) và để nó tự do viết ra toàn bộ bản báo cáo. Nhưng phản biện của Tùng khiến tôi giật mình nhận ra hiện tượng ảo giác (hallucination) trong an ninh mạng có thể hủy hoại uy tín kỹ thuật và vi phạm các tiêu chuẩn kiểm toán quốc tế. Tôi lập tức đổi ý: chuyển sang kiến trúc lai (Hybrid). Trong đó, bảng IoC và mốc thời gian bắt buộc phải do code trích xuất trực tiếp từ API nguyên bản và khóa cứng lại; AI chỉ được phép hỗ trợ diễn đạt phần narrative tóm tắt diễn biến. Đồng thời, kỹ sư con người bắt buộc phải là người đọc duyệt và bấm nút xác nhận cuối cùng.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều làm tôi bất ngờ nhất khi tiến hành phỏng vấn thực tế một Chuyên viên Incident Response theo phương pháp The Mom Test là họ hoàn toàn không hào hứng với ý tưởng để AI tự động gửi báo cáo cho cấp trên. Họ chia sẻ rất thật lòng rằng báo cáo sự cố là tài liệu mang tính pháp lý cao; nếu có một lỗi sai nhỏ gửi lên CISO, người trực tiếp xử lý sự cố sẽ bị kỷ luật. Điều họ thực sự khao khát chỉ là một công cụ giúp họ không phải chuyển qua lại giữa 5 tab trình duyệt để copy từng dòng IP, hash và mốc thời gian. Họ muốn hệ thống gom sẵn dữ liệu vào một bản nháp sạch sẽ để họ chỉ cần đọc lướt, chỉnh sửa 2–3 câu rồi ký tên gửi đi.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất đối với tôi là việc thiết lập ranh giới (Boundary) và các tiêu chí đánh giá (Eval Criteria) định lượng cho sản phẩm AI. Khi viết về giải pháp truyền thống, ta chỉ cần nói tính năng hoạt động hay không. Nhưng với AI, ta phải trả lời được: khi nào thì đầu ra của AI được coi là đạt chuẩn, và quan trọng hơn cả là AI tuyệt đối không được phép làm những gì. Việc đặt ra boundary bắt buộc sử dụng mô hình nội bộ (On-premise LLM) để bảo vệ quyền riêng tư dữ liệu và cấm AI tự ý phát hành tài liệu đòi hỏi nhóm phải cân nhắc rất kỹ lưỡng giữa tính tiện dụng và sự an toàn của toàn hệ thống.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu được làm lại từ đầu, tôi sẽ thúc đẩy nhóm thực hiện bước kiểm chứng phỏng vấn sớm hơn ngay từ CP1 thay vì đợi đến CP4. Việc có dữ liệu thực tế từ người làm nghề sớm sẽ giúp nhóm không mất thời gian tranh cãi về những ý tưởng viển vông ở CP2 và CP3. Ngoài ra, tôi sẽ phản biện mạnh hơn đối với xu hướng muốn áp dụng các công nghệ phức tạp: trong buổi làm việc, nhóm đã mất hơn 30 phút để bàn về việc triển khai Agent tự trị, trong khi một quy trình Workflow rõ ràng với sự tham gia của con người (Human-in-the-loop) đã đủ giải quyết 90% nỗi đau của người dùng với chi phí và rủi ro thấp nhất.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán của nhóm xuất phát từ **nỗi đau tốn thời gian hành chính** của chuyên gia ứng cứu sự cố khi phải mất 30–45 phút gõ tay báo cáo sau mỗi vụ việc tấn công, khiến 25% báo cáo tuần bị nộp trễ hạn. **Quy trình giải quyết** gồm: tự động trích xuất IoC và log qua API TheHive/Wazuh, dùng LLM tổng hợp diễn biến thành bản nháp narrative, và chuyên gia con người rà soát lần cuối trước khi xuất file gửi quản lý. **Success metric** đặt ra là rút ngắn thời gian soạn thảo xuống dưới 10 phút/phiếu, xóa bỏ 100% tình trạng trễ hạn báo cáo và đảm bảo độ chính xác trích xuất dữ liệu kỹ thuật đạt 100%. **Boundary an toàn** quy định dữ liệu IoC phải được khóa cứng không cho AI tự ý biến tấu, bắt buộc dùng mô hình On-premise để chống rò rỉ dữ liệu nội bộ và AI tuyệt đối không được tự ý phát hành báo cáo. Nhóm chọn **mức can thiệp Workflow** vì mức Rule không thể diễn đạt văn phong linh hoạt, còn mức Agent tự trị tiềm ẩn rủi ro ảo giác pháp lý không thể kiểm soát. Cuối cùng, nhóm đưa ra **quyết định Go** để triển khai thử nghiệm pilot 2 tuần trên các sự cố mức độ Low/Medium, đi kèm **ngưỡng dừng** rõ ràng: nếu tỷ lệ chuyên gia phải viết lại bản nháp vượt quá 30% hoặc phát hiện dù chỉ 01 lỗi sai lệch IoC thì lập tức dừng dự án để điều chỉnh lại quy trình.

---

## 7. Tài liệu tham khảo

1. TheHive Project Documentation. *Security Incident Response Platform Administrator Guide*. https://thehive-project.org/
2. Wazuh Documentation. *Open Source Security Platform & SIEM Capabilities*. https://documentation.wazuh.com/
3. Palo Alto Networks. *Incident War Room and Post-Incident Reporting in Cortex XSOAR*. https://docs-cortex.paloaltonetworks.com/
4. Rob Fitzpatrick. *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*.
5. Google People + AI Research (PAIR). *People + AI Guidebook: Designing human-centered AI products*. https://pair.withgoogle.com/
6. Marty Cagan. *Inspired: How to Create Tech Products Customers Love* (4 Product Risks Framework).
