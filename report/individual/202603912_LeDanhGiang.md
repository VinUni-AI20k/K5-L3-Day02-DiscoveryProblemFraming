# Báo cáo cá nhân — 202603912_LeDanhGiang

## 1. Thông tin học viên

* Họ tên: Lê Danh Giang

* MSSV: 202603912

* Email trường: (bỏ trống nếu không cần thiết)

* Tên nhóm: BacHo

* Link repo nhóm: https://github.com/longhtr028/K5-L3B-DAY02-BacHo-DiscoveryProblemFraming

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| \# | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) | 
| ----- | ----- | ----- | ----- | ----- | 
| 1 | Lặp lại, Tốn thời gian | Khi sử dụng nhiều dịch vụ AI API để làm dự án, tôi muốn kiểm tra nhanh tổng lượng token và chi phí đã tiêu thụ trong ngày, để điều chỉnh ngay mà không lo vượt ngân sách | Lập trình viên, sinh viên làm dự án AI | Mất 15-20 phút/ngày để đăng nhập từng dashboard (OpenAI, Anthropic, Gemini) ghi chép lại log thủ công; lặp lại mỗi ngày | 
| 2 | Cần tổng hợp nhiều thông tin | Khi di chuyển vào HĐ qua cầu Chương Dương/Long Biên hoặc chờ buýt 09A vào giờ cao điểm, tôi muốn biết chính xác điểm ùn tắc hoặc vị trí xe thực tế, để quyết định đổi lộ trình ngay | Người đi học, đi làm tại Hà Nội | Tốn thêm 30-45 phút chôn chân vì kẹt xe; lỡ chuyến buýt phải đợi 15-20 phút/chuyến; gặp 3-4 lần/tuần | 
| 3 | Tốn thời gian | Khi xe máy (Honda Wave) đột ngột khó nổ máy vào buổi sáng, tôi muốn biết cần ưu tiên kiểm tra e gió, củ đề hay bu-gi theo đúng trình tự, để tự khắc phục nhanh mà không bị muộn giờ | Sinh viên, người đi làm đi xe số cũ | Mất 15-20 phút hì hục đạp nổ; xảy ra 1-2 lần/tuần vào mùa đông; có tin nhắn nhờ vả bạn bè/thợ xe | 
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi theo dõi các giải đấu eSports (như LMHT), tôi muốn nắm được nhanh tỷ lệ thắng và chiến thuật đằng sau các lượt cấm/chọn (ban/pick) cũng như cơ chế tướng, để hiểu sâu trận đấu mà không bị gián đoạn | Người hâm mộ eSports, người chơi game | Tốn 5-10 phút mở Wiki/OP.GG tra cứu thông số trong lúc nghỉ giữa ván; làm giảm trải nghiệm xem trực tiếp | 
| 5 | Tốn thời gian | Khi nghe một đoạn nhạc phim hoặc nhạc Trung Quốc hay trên mạng (như Cơn ác mộng biển sâu), tôi muốn tìm ngay link bài hát gốc, để lưu vào playlist nghe lại | Người nghe nhạc, sáng tạo nội dung | Mất 15-20 phút dùng các app nhận diện hoặc gõ lại phiên âm pinyin để dò tìm; 2-3 lần/tuần | 

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

* **Giữ lại — #1 Kiểm soát chi phí Token API:** Khai thác từ nỗi đau thực tế khi làm dự án thực chiến, tốn thời gian kiểm tra chéo (15-20 phút/ngày).

* **Giữ lại — #2 Quyết định lộ trình giao thông:** Dựa trên thực tế đi lại tại Hà Nội (cầu Chương Dương, xe buýt 09A), tốn 30-45 phút mỗi lần kẹt xe.

* **Bỏ — Xử lý lỗi code cơ bản:** Quá chung chung, các IDE hiện tại đã hỗ trợ rất tốt.

* **Bỏ — Tóm tắt video bài giảng dài:** Sinh viên thường chọn cách xem tua nhanh (x1.5, x2) thay vì đọc tóm tắt văn bản.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc | 
| ----- | ----- | ----- | ----- | 
| 1 | Quản lý hạn mức tiêu thụ token AI API (#1) | Ảnh hưởng trực tiếp đến tài chính khi học/làm AI; lặp lại hằng ngày | Các nền tảng có cho phép kéo dữ liệu usage tự động dễ dàng qua API hay không? | 
| 2 | Quyết định lộ trình qua điểm kẹt xe HN (#2) | Giá trị tiết kiệm thời gian lớn (30-45 phút/lần); tác động ngay lập tức | Camera giao thông công cộng có đủ cập nhật real-time để đưa ra dự báo chuẩn xác? | 
| 3 | Tự sửa lỗi xe máy khó nổ đột xuất (#3) | Khắc phục được sự cố 15-20 phút rất ức chế vào buổi sáng | Người dùng có đủ chuyên môn thao tác cơ học dù đã biết nguyên nhân? | 

### Problem Card #1

| Trường | Nội dung | 
| ----- | ----- | 
| Job Story | Khi sử dụng nhiều dịch vụ AI API để làm dự án, tôi muốn kiểm tra nhanh tổng lượng token và chi phí đã tiêu thụ trong ngày, để điều chỉnh ngay mà không lo vượt ngân sách | 
| Actor | Lập trình viên, sinh viên các khóa AI thực chiến | 
| Thời điểm / bối cảnh | Cuối ngày hoặc sau khi chạy test một batch data lớn | 
| Quy trình hiện tại (3–7 bước) | Tổng khoảng 15-20 phút/ngày:  1\. Mở trình duyệt, vào tab dashboard từng nhà cung cấp (OpenAI, Gemini...): 2 phút  2\. Đăng nhập và điều hướng đến mục Usage/Billing: 3 phút  3\. Chọn đúng ngày và đọc thông số token prompt/completion: 5 phút  4\. Nhập vào file Excel/Notion để tính tổng chi phí: 5 phút | 
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & 4 (mất 10 phút tổng hợp thủ công từ nhiều nguồn) | 
| Impact (nếu không giải thì sao) | Mất 1,5 - 2 giờ/tuần chỉ cho việc copy-paste số liệu. Nguy hiểm hơn là rủi ro rò rỉ token hoặc lỡ chạy loop làm trừ cạn tiền trong thẻ tín dụng mà không biết sớm | 
| Success metric (baseline → target) | Baseline: 15-20 phút/lần kiểm tra → Target: Dưới 2 phút/lần, tự động có báo cáo chi phí tổng hợp | 
| Phương án không dùng AI | Viết một script Python gọi API billing của từng hãng (nếu có hỗ trợ) rồi xuất ra console hoặc Slack | 
| Giả thuyết về AI (nếu có) | AI (dưới dạng agent) có thể chủ động theo dõi script, khi phát hiện lượng token tiêu thụ tăng bất thường sẽ tự động phân tích log và báo động bằng ngôn ngữ tự nhiên | 
| Cảm nhận nhanh | Dashboard/Automation | 

Quy trình nháp hiện tại:

```
HIỆN TẠI — 15-20 phút/ngày

[1 Mở các tab: 2'] → [2 Đăng nhập & tìm mục Usage: 3'] 
→ [3 Tra cứu thông số từng nền tảng: 5'] ← BOTTLENECK 
→ [4 Nhập Excel tính tổng tiền: 5'] ← BOTTLENECK

```

### Problem Card #2

| Trường | Nội dung | 
| ----- | ----- | 
| Job Story | Khi di chuyển vào HĐ qua cầu Chương Dương/Long Biên hoặc chờ buýt 09A vào giờ cao điểm, tôi muốn biết chính xác điểm ùn tắc hoặc vị trí xe thực tế, để quyết định đổi lộ trình ngay | 
| Actor | Sinh viên, người đi làm bằng xe máy hoặc phương tiện công cộng tại Hà Nội | 
| Thời điểm / bối cảnh | 7h00 - 8h00 sáng và 17h00 - 18h30 chiều hằng ngày | 
| Quy trình hiện tại (3–7 bước) | Khoảng 5-10 phút ra quyết định, nhưng rủi ro tốn 30-45 phút kẹt:  1\. Mở Google Maps xem màu đường (đỏ/cam): 2 phút  2\. Mở app Tìm Buýt tra tuyến 09A xem xe cách bao xa: 3 phút  3\. Đoán xem cầu Chương Dương có đang kẹt cứng không qua các hội nhóm Facebook: 5 phút  4\. Quyết định đi tiếp hoặc vòng đường khác | 
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (tìm kiếm thông tin kẹt xe trên các hội nhóm rất mất thời gian và nhiễu loạn) | 
| Impact (nếu không giải thì sao) | Chôn chân giữa cầu 30-45 phút, muộn giờ học/làm, hao xăng và hít khói bụi | 
| Success metric (baseline → target) | Baseline: Tra cứu mất 10 phút, rủi ro trễ giờ cao → Target: Chỉ tốn 1-2 phút tra cứu, độ chính xác cập nhật tình hình giao thông lên 90% | 
| Phương án không dùng AI | Nghe VOV Giao thông hoặc xem bản đồ vệ tinh thuần túy | 
| Giả thuyết về AI (nếu có) | AI cào dữ liệu (crawl) liên tục từ các bài đăng hội nhóm giao thông mới nhất kết hợp dữ liệu Google Maps để tóm tắt 1 câu: "Cầu Chương Dương đang kẹt cứng hướng đi sang quận Hoàn Kiếm do va chạm, nên đi cầu Vĩnh Tuy" | 
| Cảm nhận nhanh | Data Aggregator/Alert | 

Quy trình nháp hiện tại:

```
HIỆN TẠI — Rủi ro kẹt xe 30-45 phút, thao tác tra cứu 10 phút

[1 Check Google Maps: 2'] → [2 Check app Tìm Buýt 09A: 3'] 
→ [3 Đọc tin hội nhóm giao thông FB: 5'] ← BOTTLENECK 
→ [4 Ra quyết định lộ trình]

```

### Problem Card #3

| Trường | Nội dung | 
| ----- | ----- | 
| Job Story | Khi xe máy (Honda Wave) đột ngột khó nổ máy vào buổi sáng, tôi muốn biết cần ưu tiên kiểm tra e gió, củ đề hay bu-gi theo đúng trình tự, để tự khắc phục nhanh mà không bị muộn giờ | 
| Actor | Người dùng xe máy số (đặc biệt xe cũ) | 
| Thời điểm / bối cảnh | Buổi sáng mùa đông hoặc sau những ngày mưa ngập | 
| Quy trình hiện tại (3–7 bước) | Tổng khoảng 15-20 phút:  1\. Đạp nổ liên tục 10-20 cái: 3 phút  2\. Tìm và kéo e gió thử lại: 2 phút  3\. Mở điện thoại tra Google "xe Wave không nổ máy": 5 phút  4\. Mở cốp kiểm tra/lau bu-gi (nếu biết cách): 5-10 phút | 
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & 4 (Tra cứu thông tin chung chung, không biết bắt bệnh từ đâu) | 
| Impact (nếu không giải thì sao) | Chậm giờ làm/học, phải dắt bộ tìm quán sửa xe tốn kém tiền bạc và thời gian | 
| Success metric (baseline → target) | Baseline: Loay hoay 15-20 phút → Target: Biết ngay thao tác xử lý trong 1-2 phút | 
| Phương án không dùng AI | Lưu một bảng checklist "Các bước xử lý khi xe không nổ máy" vào ghi chú điện thoại từ trước | 
| Giả thuyết về AI (nếu có) | Chụp ảnh tình trạng xe, mô tả tiếng kêu đề (hoặc ghi âm), AI chuẩn đoán ngay lập tức là do acquy hay bu-gi và hướng dẫn thao tác từng bước | 
| Cảm nhận nhanh | Troubleshooting Assistant | 

Quy trình nháp hiện tại:

```
HIỆN TẠI — 15-20 phút loay hoay

[1 Cố đạp nổ/đề liên tục: 3'] → [2 Kéo e gió: 2'] 
→ [3 Lên Google tra nguyên nhân: 5'] ← BOTTLENECK 
→ [4 Mở tháo kiểm tra bu-gi: 5-10']

```

### Card muốn pitch nhất

* Card số: 1 (Quản lý hạn mức tiêu thụ token AI API)

* Vì sao: Là vấn đề "sát sườn" nhất với sinh viên đang tham gia khóa đào tạo AI Thực chiến, cần dùng nhiều API và dễ gặp rủi ro chi phí.

* Câu hỏi muốn nhóm phản biện: Có thực sự cần AI giải quyết không, hay chỉ cần một cronjob chạy script kéo API lấy dữ liệu là đủ?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì | 
| ----- | ----- | ----- | 
| Card 1: Việc tổng hợp chi phí có thể giải quyết thuần túy bằng lập trình (Code), AI chưa mang lại "trí tuệ" rõ nét | Đồng ý | Thêm phần giả thuyết: AI phân tích xu hướng dùng token và cảnh báo các vòng lặp ẩn tiêu tốn chi phí bất thường | 
| Card 2: Dữ liệu giao thông mạng xã hội rất nhiễu, AI có thể bị hallucinate | Đồng ý | Giới hạn success metric vào tính tóm tắt nhanh thay vì chỉ đường tự động hoàn toàn | 
| Card 3: Xử lý xe máy đòi hỏi tay chân thao tác vật lý, AI không thể vặn ốc thay | Đồng ý | Đổi trọng tâm sang "chuẩn đoán đúng bệnh" (Troubleshooting) thay vì sửa xe | 

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch cả 3 card của mình (#4 gom tổng token và chi phí từ nhiều dashboard API AI, #5 tìm điểm kẹt xe khi qua cầu giờ cao điểm ở HN, #6 kiểm tra khi xe máy số cũ khó nổ buổi sáng) | Đóng góp 3 bài toán vào danh sách 12 candidate ở mục 2.1; sau khi so bằng chứng và khả năng kiểm chứng, nhóm thống nhất chọn #11 (ghép report nhóm nhiều người) của Tuấn Anh |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Đặt câu hỏi kiểm tra khả năng tiếp cận người dùng thật ở CP4 cho các bài ngoài lớp (#7 giáo viên, #9 chủ hộ kinh doanh, #10 dữ liệu nội bộ công ty) và hỏi về bài #11: "Nếu mọi người nộp đúng hạn, đúng format thì bước đọc có còn là bottleneck không?" | Giúp nhóm loại sớm các candidate không phỏng vấn được người thật trong buổi lab và đưa giả định #2, #3 (template + deadline nội bộ đã đủ chưa) vào Assumption Map để kiểm chứng ở CP4 |
| Nhận phản biện | Câu hỏi tôi nhận được: #4: "Lần gần nhất bạn thật sự vượt ngân sách là khi nào?" (Hải); #5: "Dữ liệu realtime lấy ở đâu, nhóm có tiếp cận được không?"; #6: "Đây là thiếu thông tin hay thiếu kỹ năng sửa xe?" | Kết quả: nhóm loại #4 vì mới có 1 người gặp và các hãng đã có usage dashboard; loại #5, #6 vì ngoài tầm dữ liệu giao thông realtime và ngoài domain của nhóm. Tôi đã sửa gì: Nhận ra #4 tần suất vượt ngân sách thấp, còn #6 nghiêng về kỹ năng thao tác thực hành hơn là bài toán xử lý thông tin cho AI |
| Gom cluster / cây OST | Cùng nhóm gom 12 candidate thành 4 cluster (card #4 của tôi vào Cluster B — tự tìm và đối chiếu thông tin rời rạc; #5, #6 vào nhóm Ngoài cluster) và rà soát cây OST của bài #11 | Giúp nhóm phân biệt rõ đâu là opportunity (nỗi đau nộp trễ, sai format, lệch nội dung) và gạch bỏ được 3 giải pháp đội lốt opportunity (Template Docs chung, Bot nhắc deadline, AI tóm tắt từng phần) ở mục 2.3 |
| Chọn candidate problem | Cùng nhóm chấm điểm shortlist 3 bài toán theo 7 tiêu chí và thảo luận khi chuyển từ đề xuất ban đầu (#1 đọc đề lab) sang #11 (ghép report nhóm, 33/35 điểm) | Thống nhất chọn #11 vì có số liệu hành vi thật từ nhiều người, cả 4 thành viên đều hiểu domain và so sánh rõ được cả 4 mức No AI / Rule / Workflow / Agent |
| Kiểm chứng / research | Cùng nhóm đối chiếu kết quả phỏng vấn DA (mục 3.2) với 3 giả định đầu và tìm hiểu các công cụ có sẵn (Google Docs tabs, Gemini trong Docs, Gemini Notebook ở mục 3.3) | Phát hiện giả định #2 sai một phần (bottleneck thật là đồng bộ số liệu, biểu đồ và viết lại insight nối logic từ EDA sang Model mất 3–4 tiếng); kết luận đã có công cụ sẵn nên không tự xây agent |
| Quy trình nhóm | Review quy trình hiện tại (5 bước thủ công) và quy trình tương lai (6 bước, kỳ vọng 90 phút), tách bước 0–2 cho No AI + Rule (template, hàm vẽ chung, bảng "Số liệu chính") | Chuẩn hóa bảng Before/After ở mục 4.3; chốt rõ boundary là AI chỉ chạy ở bước 3 để liệt kê chỗ mâu thuẫn kèm trích dẫn, không tự sửa file hay viết thay insight |
| Problem Statement | Review Problem Statement v0, đọc các điểm phản biện ở mục 5 và cập nhật lên bản v1 kèm 5 tiêu chí đánh giá đầu ra của AI (mục 7) | Bỏ giới hạn "nhóm 4–7 người" chưa đủ nguồn ở Actor, bổ sung metric chất lượng (số chênh lệch số liệu còn sót = 0, số đoạn insight phải viết lại giảm ít nhất một nửa) |
| Mức can thiệp AI | Review ma trận độ mơ hồ × độ phức tạp, bảng so sánh 4 mức, AI Canvas và 2 câu hỏi Google PAIR (Augment vs Automate; Báo nhầm vs Bỏ sót) ở mục 6 | Thống nhất chọn mức Workflow (No AI + Rule ở bước 0–2, AI ở bước 3); xác định "bỏ sót tệ hơn báo nhầm" để thiết kế Rule kiểm số liệu chạy trước AI |
| Quyết định | Review phần đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability) và chốt kế hoạch pilot kèm ngưỡng dừng (mục 8) | Chốt quyết định "Go, phạm vi nhỏ": ưu tiên chạy bước 0–2 (No AI + Rule) và bấm giờ trước; nếu đã giảm xuống dưới 90 phút hoặc AI bỏ sót lỗi trong 2 lần liên tiếp thì dừng AI, quay về No AI + Rule |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý mở rộng các vấn đề cá nhân thường gặp xoay quanh việc học, làm dự án AI và sinh hoạt hằng ngày theo 4 lăng kính để lập bảng scan | Giúp diễn đạt đúng cấu trúc Job Story ("Khi... tôi muốn... để...") và gợi nhớ nhanh các tình huống tốn thời gian bản thân từng gặp (theo dõi token API AI, kẹt xe qua cầu, xe máy khó nổ) | AI hay gợi ý các vấn đề chung chung và ước lượng thời gian/tần suất cảm tính, không chỉ ra được đâu là vấn đề ngoài tầm dữ liệu của nhóm | Chỉ giữ lại 3 vấn đề sát trải nghiệm thật của bản thân (#4, #5, #6), tự điền dấu hiệu thời gian thực tế (như khoảng 10 phút gom số từ các dashboard) thay vì lấy con số suy diễn của AI |
| CP2 Problem Card | Hỗ trợ chia nhỏ các bước trong quy trình hiện tại cho 3 card (#4 theo dõi chi phí API AI, #5 tìm điểm kẹt xe qua cầu, #6 kiểm tra xe số cũ khó nổ) và gợi ý phương án không dùng AI | Giúp tách quy trình thành từng bước rõ ràng, xác định nhanh bước bottleneck và gợi ý các cách xử lý thủ công/quy tắc (như đặt hạn mức cảnh báo billing sẵn có hoặc lập checklist kiểm tra xe) | AI có xu hướng đề xuất xây công cụ/app AI tự động hóa cho cả 3 card mà bỏ qua rào cản thiếu dữ liệu giao thông realtime (#5) hoặc đặc thù kỹ năng thực hành (#6) | Giữ phần mô tả quy trình thực tế nhưng hạ kỳ vọng về AI, ghi rõ phương án No AI / Rule đã giải quyết được phần lớn cho card #4 và nhận diện hạn chế dữ liệu ở card #5, #6 |
| CP4 Research | Hỗ trợ tóm tắt tính năng và giới hạn của các công cụ có sẵn (Google Docs document tabs, Gemini trong Docs, Gemini Notebook) để đối chiếu với quy trình ghép report | Giúp liệt kê nhanh công cụ nào giải được bước nào (thu bài, tóm tắt, hỏi chéo có trích dẫn inline) và điều kiện sử dụng gói tài khoản | AI thường đánh giá quá lạc quan khả năng tự động phát hiện mâu thuẫn của công cụ mà ít nhấn mạnh việc người ghép phải nạp lại nguồn khi thành viên sửa bài | Kiểm tra lại trên trang tài liệu chính thức của Google Support, bổ sung rõ cột "Khoảng trống / rủi ro" và rút ra bài học: tận dụng công cụ sẵn có theo hướng Workflow, không tự xây agent |
| CP5 Quy trình | Không dùng | | | |
| CP5–6 Problem Statement | Không dùng | | | |
| CP6 Mức can thiệp / quyết định | Không dùng | | | |

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi nhận ra mỗi người có một góc nhìn khác nhau về nỗi đau. Học được cách dùng những con số thực tế (bao nhiêu giờ, bao nhiêu lần) để đo lường vấn đề thay vì chỉ nói chung chung là "việc này rất mất thời gian".

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có, ban đầu nhóm định "code luôn một con bot Telegram báo cáo". Sau đó nhóm xem lại checklist, nhận ra mình đi sai hướng nên đã bỏ ý định làm bot và quay lại vẽ quy trình hiện tại để tìm chính xác bước nào tốn thời gian nhất.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Ban đầu tôi chọn vấn đề sửa xe, nhưng bạn khác chỉ ra: "Dù biết xe hỏng bugi mà không có đồ nghề thì vẫn phải dắt bộ". Tôi thấy hợp lý vì AI không thể sửa thay mình được, nên đã đồng ý bỏ vấn đề này.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Rất bất ngờ. Khi tìm hiểu, nhóm thấy đã có nhiều công cụ tóm tắt bài báo rất tốt (như ChatPDF). Hóa ra nỗi đau thực sự không phải là thiếu công cụ, mà là người dùng sợ AI bịa thông tin (hallucination) nên không dám dùng.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là viết ngắn gọn mà vẫn đủ ý bối cảnh, nỗi đau và tác động. Đặc biệt là phải "kìm nén", không được đưa các từ khóa giải pháp (như "cần một app AI", "cần xây bot") vào câu phát biểu.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Tôi sẽ tìm số liệu thực tế kỹ hơn thay vì chỉ tự ước lượng. Ngoài ra, tôi sẽ phản biện mạnh hơn ở bước "Phương án không dùng AI", vì nhiều vấn đề hiện nay chỉ cần dùng một file Excel là xong, không nhất thiết phải nhét AI vào bằng được.

**6.7. Hiểu bài:** (Giải thích bằng 5–8 câu)
Đầu tiên, nhóm đi tìm các **problem** thực tế và ưu tiên vấn đề quan trọng nhất. Sau đó, nhóm vẽ **quy trình** làm việc hiện tại để tìm ra "nút thắt cổ chai" (bước tốn thời gian nhất). Dựa trên nút thắt này, nhóm đặt ra **metric** để đo lường mức độ cải thiện và **boundary** (phạm vi giải quyết giới hạn ở đâu). Do lo ngại rủi ro AI tạo thông tin sai, nhóm chọn **mức can thiệp AI** là Copilot (có người duyệt). Cuối cùng, nhóm đi đến **quyết định** "Go, phạm vi nhỏ", tận dụng các công cụ có sẵn thay vì tự xây dựng một hệ thống đắt đỏ.

---
## 7. Tài liệu tham khảo

* S. Keshav (2007), How to Read a Paper, ACM SIGCOMM Computer Communication Review 37(3).

* Báo cáo và thông số API Usage tham khảo từ tài liệu OpenAI Billing & Limits.
