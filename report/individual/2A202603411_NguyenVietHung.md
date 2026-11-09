# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Việt Hưng
- MSSV: 2A202603411
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: AEZE
- Link repo nhóm: https://github.com/hhuydaugg/K5-L3A-DAY02-AZEZ-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Tốn thời gian |Khi đang khám bệnh và phải tập trung trao đổi với bệnh nhân, tôi muốn hệ thống tự động ghi nhận và cấu trúc hóa nội dung cuộc khám, để tôi giảm thời gian nhập liệu và dành nhiều thời gian hơn cho bệnh nhân. |Bác sĩ, nhân viên quản lý bệnh án |Theo nghiên cứu công bố trên Journal of the American Medical Informatics Association năm 2025, triển khai Ambient AI Scribe tại một trung tâm y tế học thuật với 45 bác sĩ giúp giảm trung vị: 0,57 phút cho mỗi ghi chép bệnh án. 6,89 phút thời gian documentation mỗi ngày. 5,17 phút làm hồ sơ ngoài giờ mỗi ngày.|
| 2 | Pain từ người khác | Sau khi được bác sĩ khám chữa bệnh và kê đơn thuốc, tôi muốn hệ thống có thể hỗ trợ nhắc nhở tôi về việc sử dụng thuốc đúng liều lượng, đúng thời gian để việc chữa bệnh đạt hiệu quả tốt nhất. | Bệnh nhân, bác sĩ | Mẫu khảo sát từ 127 bệnh nhân tại Bệnh viện Y học gia đình Huế trong khoảng thời gian 2 tháng, cho thấy có 28,3% số bệnh nhân tham gia khảo sát tự ý điều chỉnh lịch sử dụng thuốc, khoảng 30-50% bệnh nhân tham gia khảo sát quên sử dụng thuốc theo đúng liệu trình |
| 3 | Lặp lại, tốn thời gian | Khi bệnh nhân muốn đặt hoặc thay đổi lịch khám, tôi muốn hệ thống tự động kiểm tra lịch trống và đề xuất khung giờ phù hợp, để giảm thời gian xử lý yêu cầu và hạn chế tình trạng đặt lịch không thành công. | Nhân viên CSKH, bệnh nhân | Một nghiên cứu tại bệnh viện tuyến cuối ở Ấn Độ năm 2025 ghi nhận thời gian đăng ký ngoại trú trung bình qua phương thức online là 4,15 phút, thấp hơn khoảng 60% so với phương thức đăng ký trực tiếp (10,37 phút). Tuy nhiên, việc đặt lịch online trước không đồng nghĩa với việc bệnh nhân đã hoàn tất toàn bộ thủ tục khi đến bệnh viện. Khâu check-in, xác minh danh tính và điều phối đến phòng khám vẫn cần được đánh giá riêng. |
| 4 | Cần đọc, tổng hợp thông tin | Khi bệnh nhân chuẩn bị ra viện, tôi muốn hệ thống rà soát tính đầy đủ và nhất quán của hồ sơ, để phát hiện sớm các giấy tờ hoặc thông tin còn thiếu và rút ngắn thời gian hoàn tất thủ tục. | Bác sĩ, nhân viên y tế | Nghiên cứu tổng hợp các công trình về tính kịp thời và chất lượng thông tin khi bệnh nhân ra viện. Trung vị 67% bản tóm tắt ra viện được hoàn thành trong vòng 48 giờ. Chỉ 55% được cung cấp cho bác sĩ chăm sóc ban đầu trong vòng 48 giờ. |
| 5 | | | | |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tự động hóa ghi chép hồ sơ bệnh án và nhập liệu lâm sàng|Có thể áp dụng Speech to text để giảm thiểu thời gian ghi chép hồ sơ bệnh án, dễ phân loại hồ sơ bệnh án và có thể test được với quy mô của Vinmec |Đã có các bệnh viện ứng dụng mô hình này nên có thể đã có nghiên cứu hoặc được áp dụng rồi |
| 2 |Tiếp nhận bệnh nhân, đặt lịch và điều phối lịch khám |Trải nghiệm thật của bản thân khi đặt lịch khám bệnh qua hotline của các cơ sở y tế trên địa bàn Thành phố Hà Nội |Có cần thiết phải áp dụng AI không hay chỉ cần hệ thống tiếp nhận thông tin |
| 3 |Bệnh nhân quên sử dụng thuốc và điều trị theo đúng liệu trình|Có tính thực tiễn cao, trải nghiệm thực tế từ bản thân và dễ dàng phỏng vấn|Việc đồng bộ triển khai trên các bệnh nhân sẽ gặp khó khăn trong giai đoạn đầu|Không nhất thiết phải sử dụng Agent hoặc LLM cho chức năng cốt lõi. Rule-based Workflow có thể xử lý tốt việc tạo lịch và nhắc thuốc|

### Problem 1: Tự động hóa ghi chép hồ sơ bệnh án và nhập liệu lâm sàng

| Trường | Nội dung |
|---|---|
| Job Story | Khi đang khám và trao đổi với bệnh nhân, tôi muốn ghi nhận các thông tin lâm sàng nhanh chóng và chính xác vào hồ sơ bệnh án, để giảm thời gian nhập liệu thủ công và dành nhiều thời gian hơn cho việc thăm khám. |
| Actor | Bác sĩ khám bệnh (Actor chính); điều dưỡng, nhân viên y tế và bộ phận quản lý hồ sơ bệnh án (Actor liên quan). |
| Thời điểm / bối cảnh | Trong và ngay sau mỗi lượt khám tại VINMEC, khi bác sĩ cần ghi nhận triệu chứng, tiền sử bệnh, kết quả thăm khám, chẩn đoán và kế hoạch điều trị vào hệ thống HIS/EMR. |
| Quy trình hiện tại (3–7 bước) | 1. Bác sĩ tiếp nhận và trao đổi với bệnh nhân.<br>2. Bác sĩ ghi nhận triệu chứng, tiền sử bệnh và các thông tin lâm sàng.<br>3. Bác sĩ nhập thông tin vào hệ thống HIS/EMR bằng cách nhập liệu thủ công hoặc lựa chọn biểu mẫu có sẵn.<br>4. Bác sĩ hoàn thiện chẩn đoán, chỉ định xét nghiệm và kế hoạch điều trị.<br>5. Bác sĩ kiểm tra, chỉnh sửa và xác nhận hồ sơ bệnh án. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2 và 3:** Bác sĩ phải đồng thời tập trung trao đổi, thăm khám và ghi chép thông tin. Sau đó, bác sĩ tiếp tục nhập lại, phân loại và cập nhật dữ liệu vào HIS/EMR. Điều này tạo ra công việc hành chính lặp lại sau mỗi lượt khám. Thời gian cụ thể: Chưa có dữ liệu đo lường tại VINMEC. Cần khảo sát thời gian ghi chép và hoàn thiện hồ sơ trung bình trên mỗi lượt khám (Documentation Time). |
| Impact (nếu không giải thì sao) | - Bác sĩ mất nhiều thời gian cho công việc hành chính thay vì tương tác với bệnh nhân.<br>- Có nguy cơ bỏ sót hoặc nhập thiếu thông tin lâm sàng.<br>- Tăng khối lượng công việc và áp lực cho đội ngũ y tế.<br>- Có thể làm giảm hiệu suất tiếp nhận bệnh nhân và kéo dài thời gian hoàn thiện hồ sơ. |
| Success metric (baseline → target) | - Documentation Time: Baseline cần đo → Giảm ít nhất 20%.<br>- Documentation Completeness: Baseline cần đo → Đạt ≥ 95%.<br>- AI Suggestion Acceptance Rate: Baseline chưa có → Đạt ≥ 80%.<br>- Clinical Safety: Không có lỗi nghiêm trọng do AI tự động ghi vào hồ sơ chính thức mà chưa được bác sĩ xác nhận. |
| Phương án không dùng AI | - Chuẩn hóa biểu mẫu hồ sơ bệnh án điện tử.<br>- Sử dụng template và macro để tự động điền các trường thông tin lặp lại.<br>- Tối ưu giao diện HIS/EMR nhằm giảm số thao tác nhập liệu.<br>- Phân công nhân viên hỗ trợ nhập liệu và hoàn thiện hồ sơ. |
| Giả thuyết về AI (nếu có) | Nếu sử dụng Speech-to-Text kết hợp Medical NLP/LLM, hệ thống có thể chuyển hội thoại bác sĩ – bệnh nhân thành bản nháp hồ sơ bệnh án, tự động trích xuất và phân loại thông tin lâm sàng theo các trường dữ liệu tương ứng. Bác sĩ chỉ cần rà soát, chỉnh sửa và xác nhận trước khi lưu chính thức. |
| Cảm nhận nhanh | Workflow + Agent |



### Problem 2: Tiếp nhận bệnh nhân, đặt lịch và điều phối lịch khám

| Trường | Nội dung |
|---|---|
| Job Story | Khi muốn đăng ký khám bệnh tại VINMEC, tôi muốn nhanh chóng tìm được chuyên khoa, bác sĩ và khung giờ phù hợp, để hoàn tất việc đặt lịch thuận tiện và giảm thời gian chờ đợi khi đến bệnh viện. |
| Actor | Bệnh nhân (Actor chính); nhân viên tổng đài (Call Center); nhân viên lễ tân/tiếp đón; bác sĩ; điều dưỡng và nhân viên điều phối lịch khám. |
| Thời điểm / bối cảnh | Khi bệnh nhân có nhu cầu đăng ký khám mới, đặt lịch tái khám, thay đổi hoặc hủy lịch. Quy trình diễn ra qua hotline, website, ứng dụng hoặc trực tiếp tại bệnh viện. |
| Quy trình hiện tại (3–7 bước) | 1. Bệnh nhân tìm kiếm thông tin về chuyên khoa, bác sĩ, dịch vụ khám và chi phí.<br>2. Bệnh nhân liên hệ VINMEC qua hotline, website, ứng dụng hoặc trực tiếp để yêu cầu đặt lịch.<br>3. Nhân viên tiếp nhận xác định nhu cầu khám, thông tin bệnh nhân và chuyên khoa phù hợp.<br>4. Nhân viên kiểm tra lịch làm việc, khung giờ trống và khả năng tiếp nhận của bác sĩ/phòng khám.<br>5. Nhân viên xác nhận lịch hẹn và hướng dẫn bệnh nhân chuẩn bị trước khi khám.<br>6. Bệnh nhân đến bệnh viện, thực hiện thủ tục tiếp đón và chờ đến lượt khám.<br>7. Khi có lịch hủy, thay đổi hoặc bệnh nhân không đến, nhân viên cập nhật và điều phối lại lịch khám. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2, 3 và 4:** Nhân viên phải tiếp nhận thông tin từ nhiều kênh, hỏi lại nhu cầu khám, xác định chuyên khoa và kiểm tra lịch trống của bác sĩ. Các thao tác này có tính lặp lại và phụ thuộc vào quá trình trao đổi giữa bệnh nhân và nhân viên. **Bước 7:** Khi có lịch hủy hoặc bệnh nhân không đến, nhân viên phải cập nhật và tìm bệnh nhân thay thế cho khung giờ trống. Thời gian cụ thể: Chưa có dữ liệu đo lường thực tế tại VINMEC. Cần đo Appointment Booking Time và thời gian xử lý một yêu cầu đổi/hủy lịch. |
| Impact (nếu không giải thì sao) | - Bệnh nhân mất thời gian tìm kiếm thông tin và hoàn tất thủ tục đặt lịch.<br>- Tăng khối lượng công việc cho nhân viên tổng đài và tiếp đón.<br>- Có thể phát sinh sai sót khi nhập thông tin hoặc đặt nhầm chuyên khoa, bác sĩ và khung giờ.<br>- Lịch hủy hoặc bệnh nhân không đến có thể khiến khung giờ khám bị bỏ trống.<br>- Giảm hiệu suất sử dụng bác sĩ và phòng khám, đồng thời có thể kéo dài thời gian chờ của bệnh nhân. |
| Success metric (baseline → target) | - Appointment Booking Time: Baseline cần đo → Giảm ít nhất 30%.<br>- Booking Automation Rate: Baseline chưa có → Đạt ≥ 50% đối với yêu cầu đặt lịch đơn giản.<br>- No-show Rate: Baseline cần đo → Giảm ít nhất 10% so với baseline hoặc nhóm đối chứng.<br>- Appointment Booking Success Rate: Baseline chưa có → Đạt ≥ 95%.<br>- Scheduling Accuracy: Không có trường hợp hệ thống tự ý đặt sai bác sĩ, chuyên khoa hoặc khung giờ do lỗi nghiệp vụ. |
| Phương án không dùng AI | - Chuẩn hóa quy trình tiếp nhận và biểu mẫu đặt lịch trên tất cả các kênh.<br>- Xây dựng hệ thống quản lý lịch hẹn tập trung, đồng bộ lịch bác sĩ và phòng khám.<br>- Sử dụng Rule-based Booking để kiểm tra khung giờ trống và điều kiện đặt lịch.<br>- Tự động gửi SMS/Push Notification xác nhận và nhắc lịch.<br>- Xây dựng danh sách chờ để lấp đầy các khung giờ bị hủy. |
| Giả thuyết về AI (nếu có) | Nếu sử dụng AI Chatbot/Voicebot kết hợp NLP/LLM, hệ thống có thể tiếp nhận yêu cầu đặt lịch qua nhiều kênh, nhận diện nhu cầu khám và trích xuất thông tin bệnh nhân. Sau đó, hệ thống kết nối Appointment Engine để kiểm tra lịch trống, đề xuất khung giờ phù hợp và hỗ trợ đặt/đổi/hủy lịch. AI cũng có thể phân tích lịch sử đặt lịch để dự báo nguy cơ No-show và hỗ trợ điều phối bệnh nhân từ danh sách chờ vào các khung giờ còn trống. Những trường hợp phức tạp hoặc có dấu hiệu cần xử lý y tế phải được chuyển cho nhân viên phụ trách. |
| Cảm nhận nhanh | Agent + Workflow |


### Problem 3: Medication Reminder Assistant

| Trường | Nội dung |
|---|---|
| Job Story | Khi được bác sĩ kê đơn và phải sử dụng thuốc tại nhà, tôi muốn được nhắc nhở về thời gian, liều lượng và hướng dẫn sử dụng thuốc, để không bỏ lỡ liều và tuân thủ đúng liệu trình điều trị. |
| Actor | Bệnh nhân sau khám (Actor chính); người nhà/người chăm sóc; bác sĩ và dược sĩ theo dõi điều trị (Actor liên quan). |
| Thời điểm / bối cảnh | Sau khi bệnh nhân hoàn thành khám bệnh, nhận đơn thuốc và bắt đầu sử dụng thuốc tại nhà. Đặc biệt trong trường hợp bệnh nhân phải sử dụng nhiều loại thuốc với liều lượng, tần suất và thời điểm khác nhau. |
| Quy trình hiện tại (3–7 bước) | 1. Bệnh nhân khám bệnh và nhận đơn thuốc từ bác sĩ.<br>2. Bệnh nhân tự ghi nhớ hoặc tự thiết lập lịch uống thuốc.<br>3. Bệnh nhân mua thuốc và sử dụng tại nhà theo hướng dẫn.<br>4. Bệnh nhân tự theo dõi việc uống thuốc, có thể quên liều hoặc sử dụng sai thời điểm.<br>5. Khi có thắc mắc hoặc vấn đề phát sinh, bệnh nhân chủ động liên hệ bác sĩ/dược sĩ.<br>6. Bệnh nhân tái khám theo lịch hẹn. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2, 3 và 4:** Bệnh nhân phải tự ghi nhớ và quản lý lịch uống thuốc, đặc biệt khi có nhiều loại thuốc với thời điểm sử dụng khác nhau. Việc theo dõi thủ công khiến bệnh nhân dễ quên liều, uống sai thời điểm hoặc không duy trì đủ liệu trình. Thời gian cụ thể: Chưa có dữ liệu về số phút bệnh nhân dành cho việc quản lý thuốc. Bottleneck chính ở đây không chỉ là thời gian mà còn là nguy cơ không tuân thủ điều trị. |
| Impact (nếu không giải thì sao) | - Bệnh nhân có thể bỏ lỡ liều hoặc sử dụng thuốc không đúng hướng dẫn.<br>- Giảm mức độ tuân thủ điều trị, ảnh hưởng đến hiệu quả điều trị.<br>- Có thể phát sinh các vấn đề sức khỏe do sử dụng thuốc không đúng chỉ định.<br>- Bác sĩ và dược sĩ phải dành thêm thời gian giải đáp những câu hỏi lặp lại về cách sử dụng thuốc. |
| Success metric (baseline → target) | - Medication Adherence Rate: Baseline cần đo → Tăng ít nhất 10 điểm phần trăm so với baseline hoặc nhóm đối chứng.<br>- Patient Activation Rate: Baseline chưa có → Đạt ≥ 60%.<br>- Notification Delivery Rate: Baseline chưa có → Đạt ≥ 99%.<br>- Medication Safety: 0 lỗi nghiêm trọng do hệ thống tự ý thay đổi liều lượng hoặc chỉ định thuốc. |
| Phương án không dùng AI | - Xây dựng tính năng nhắc uống thuốc theo lịch cố định trên ứng dụng VINMEC.<br>- Sử dụng SMS hoặc thông báo Push Notification theo thời gian được thiết lập.<br>- Cung cấp bảng hướng dẫn sử dụng thuốc rõ ràng sau khi kê đơn.<br>- Khuyến khích người nhà/người chăm sóc hỗ trợ theo dõi lịch uống thuốc. |
| Giả thuyết về AI (nếu có) | Nếu kết hợp OCR/Medical NLP để trích xuất thông tin từ đơn thuốc và LLM + RAG để giải thích hướng dẫn sử dụng thuốc, hệ thống có thể hỗ trợ bệnh nhân hiểu đơn thuốc và thiết lập lịch sử dụng phù hợp. Rule-based Schedule Engine chịu trách nhiệm tạo lịch nhắc chính xác theo đơn đã được bác sĩ xác nhận. AI có thể nhận diện tình trạng bỏ lỡ nhiều liều từ dữ liệu bệnh nhân tự khai báo và chuyển thông tin cho nhân viên y tế khi cần thiết. |
| Cảm nhận nhanh | Rule + Workflow |


### Card muốn pitch nhất

- Card số: 3
- Vì sao: vấn đề xảy ra phổ biến và dễ phỏng vấn.
- Câu hỏi muốn nhóm phản biện: 

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
