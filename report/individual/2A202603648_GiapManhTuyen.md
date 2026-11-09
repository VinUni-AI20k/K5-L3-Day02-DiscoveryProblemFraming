# Báo cáo cá nhân — 2A202603648_GiapManhTuyen

## 1. Thông tin học viên

- **Họ tên:** Giáp Mạnh Tuyên
- **MSSV:** 2A202603648
- **Email trường:** 26ai.gmtuyen@gmail.com
- **Tên nhóm:** TEAMLAGI
- **Link repo nhóm:** https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

### 2.1. Danh sách 8 Problems

| # | Lăng kính | Job Story | Actor chịu ảnh hưởng | Dấu hiệu và benchmark tham khảo |
|---|---|---|---|---|
| 1 | Cần tổng hợp thông tin, tốn thời gian | Khi phòng ban phát sinh nhu cầu tuyển dụng, tôi muốn truyền đạt đầy đủ vị trí, số lượng, năng lực chuyên môn và thời hạn cần nhân sự để tránh phải trao đổi, chỉnh sửa yêu cầu nhiều lần | Hiring Manager, trưởng bộ phận, HRBP, Recruitment Manager, Finance | NIJobs 2025: trung bình 3,4 giờ/vị trí dành cho trao đổi yêu cầu với các bên liên quan [N1] |
| 2 | Lặp lại, tốn thời gian | Khi cần xây dựng hoặc điều chỉnh JD cho nhiều vị trí, tôi muốn nội dung tuyển dụng phản ánh đúng yêu cầu chuyên môn và được các bên thống nhất để giảm thời gian chỉnh sửa | Hiring Manager, HR, Recruitment Marketing, trưởng bộ phận | NIJobs 2025: hoạt động viết và đăng tin tuyển dụng mất trung bình 3,2 giờ/vị trí [N1] |
| 3 | Lặp lại, tốn thời gian | Khi cần quảng bá một vị trí tuyển dụng trên nhiều nền tảng, tôi muốn giảm các thao tác đăng tải và cập nhật nội dung lặp lại để tiết kiệm thời gian và hạn chế sai lệch thông tin | Recruiter, Recruitment Marketing, Hiring Manager, IT/ATS Administrator | NIJobs 2025: 3,2 giờ/vị trí cho viết và đăng tin [N1], Employment Hero 2023: 5,4 giờ/tuần cho hoạt động đăng tin tại mẫu khảo sát Singapore và Malaysia [N6] |
| 4 | Cần đọc, tổng hợp thông tin | Khi hồ sơ ứng viên được gửi qua nhiều nguồn, tôi muốn thông tin được tập trung và chuẩn hóa để giảm việc nhập dữ liệu nhiều lần và tránh bỏ sót hồ sơ | Recruiter, Talent Acquisition Operations, Hiring Manager, ứng viên, IT/ATS Administrator | Greenhouse: 244 hồ sơ/vị trí trong dữ liệu 2025 [N2], NIJobs: 4,1 giờ/vị trí cho nhập liệu và tài liệu HR [N1] |
| 5 | Lặp lại, tốn thời gian | Khi ứng viên nộp hồ sơ qua nhiều kênh, tôi muốn phát hiện những bản ghi có thể trùng nhau để tránh liên hệ lặp lại và duy trì dữ liệu chính xác | Recruiter, HR Operations, ứng viên, IT/ATS Administrator | Greenhouse ghi nhận trung bình 4.890 lượt ứng tuyển/recruiter/năm 2025 [N2], NIJobs ghi nhận 4,1 giờ/vị trí cho nhập liệu và tài liệu [N1], chưa có tỷ lệ CV trùng được công bố cho riêng các kênh tại Việt Nam |
| 6 | Tốn thời gian, pain từ người khác | Khi cần tổ chức phỏng vấn có nhiều người tham dự, tôi muốn tìm khung giờ phù hợp giữa ứng viên và người phỏng vấn để hạn chế trao đổi và thay đổi lịch nhiều lần | Recruitment Coordinator, ứng viên, Hiring Manager, Interviewer | NIJobs 2025: 3,5 giờ/vị trí cho việc sắp lịch [N1], GoodTime 2024: thời gian từ lúc bắt đầu xếp lịch đến khi được xác nhận trung bình 38,1 giờ với quy trình xác nhận thủ công, so với 20,8 giờ khi tự động xác nhận trong mẫu khách hàng GoodTime [N4] |
| 7 | Cần tổng hợp thông tin, pain từ người khác | Khi nhiều người cùng tham gia đánh giá một ứng viên, tôi muốn nhận đầy đủ nhận xét và thống nhất bước xử lý tiếp theo để tránh các quyết định bị kéo dài do thiếu thông tin | Interviewer, Technical Lead, Hiring Manager, Recruiter, ứng viên | NIJobs 2025: trung bình 2,9 giờ/vị trí để tổng hợp và thống nhất feedback nội bộ, 3,6 giờ/vị trí cho xử lý sau phỏng vấn [N1] |
| 8 | Lặp lại, pain từ người khác | Khi theo dõi nhiều ứng viên tại các giai đoạn tuyển dụng khác nhau, tôi muốn biết hồ sơ nào chưa được xử lý và ứng viên nào đang chờ phản hồi để tránh bỏ sót hoặc chậm thông báo kết quả | Recruiter, Hiring Manager, HR Operations, ứng viên, Recruitment Manager | NIJobs: 3,6 giờ/vị trí cho phản hồi và thông báo kết quả [N1], Robert Walters Vietnam 2025: 77% người tìm việc được khảo sát cảm thấy hồ sơ của họ thường không được phản hồi [N3] |

### 2.2. Nhận xét ban đầu

Các vấn đề trên cho thấy hoạt động tuyển dụng không chỉ phụ thuộc vào HR mà còn cần sự phối hợp giữa nhiều actor ở từng giai đoạn
Một số bottleneck xuất hiện trong công việc lặp lại như đăng tin đa kênh, nhập dữ liệu ứng viên, cập nhật trạng thái và gửi phản hồi
Ngoài ra, những hoạt động cần phối hợp giữa các bên như phê duyệt JD, sắp xếp lịch và thu thập feedback cũng có thể khiến quy trình bị kéo dài
Ba vấn đề được ưu tiên phân tích sâu là Multi-channel Recruitment Posting, Candidate Application Consolidation và Candidate Pipeline Tracking
---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### 3.1. Bảng chọn Top 3

| Rank | Problem | Vì sao chọn? | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Multi-channel Recruitment Posting | Có kinh nghiệm trực tiếp phát triển công cụ hỗ trợ đăng tin tuyển dụng, quy trình lặp lại và có benchmark 3,2 giờ/vị trí cho viết và đăng tin | Các nền tảng hiện có hỗ trợ tự động hóa tới đâu, việc cập nhật JD trên nhiều kênh có phải điểm nghẽn đáng kể không |
| 2 | Candidate Application Consolidation | Số lượng hồ sơ ứng tuyển lớn, dữ liệu phân tán và cần chuẩn hóa, có benchmark 4,1 giờ/vị trí cho nhập liệu và quản lý tài liệu | ATS hiện tại đã giải quyết được bao nhiêu phần, tỷ lệ hồ sơ trùng và thiếu thông tin trong thực tế là bao nhiêu |
| 3 | Candidate Pipeline Tracking | Có nhiều actor tham gia, dễ xảy ra chậm phản hồi giữa các giai đoạn, có benchmark thời gian xử lý và dữ liệu về trải nghiệm ứng viên | Nguyên nhân chính là thiếu công cụ, thiếu dữ liệu hay việc phối hợp giữa Recruiter và Hiring Manager |

### 3.2. Problem Card #1 — Multi-channel Recruitment Posting

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi cần tuyển dụng nhiều vị trí trên các nền tảng khác nhau, tôi muốn giảm thao tác viết, đăng và cập nhật bài tuyển dụng để tiết kiệm thời gian và đảm bảo thông tin nhất quán |
| **Actor** | Recruiter, Recruitment Marketing, Hiring Manager, HRBP, IT/ATS Administrator, ứng viên |
| **Thời điểm / bối cảnh** | Doanh nghiệp mở nhiều vị trí tuyển dụng, cần đăng trên Facebook, LinkedIn, website tuyển dụng và các kênh được cấp quyền |
| **Quy trình hiện tại** | Hiring Manager xác nhận nhu cầu → HR chuẩn bị JD → Marketing điều chỉnh nội dung → Recruiter đăng trên các kênh → Kiểm tra bài đăng → Cập nhật khi có thay đổi |
| **Bottleneck** | Đăng bài qua nhiều kênh và đồng bộ nội dung khi JD thay đổi, đặc biệt khi mỗi nền tảng có cấu trúc và yêu cầu đăng tải khác nhau |
| **Impact** | Tăng thời gian thao tác, nguy cơ thông tin không đồng nhất, bài đăng cũ không được cập nhật, ảnh hưởng trải nghiệm ứng viên |
| **Benchmark** | NIJobs 2025: 3,2 giờ/vị trí cho viết và đăng tin, Employment Hero 2023: 5,4 giờ/tuần cho hoạt động đăng tin trong mẫu khảo sát Singapore và Malaysia |
| **Success metric** | Thời gian viết và đăng một vị trí, số thao tác thủ công, tỷ lệ bài đăng nhất quán với JD, thời gian cập nhật toàn bộ kênh |
| **Target đề xuất** | Giảm 30% tổng thời gian viết và đăng tin, tương đương mốc tham chiếu từ 3,2 xuống khoảng 2,2 giờ/vị trí trong điều kiện thử nghiệm tương đương |
| **Phương án không dùng AI** | Chuẩn hóa JD, template theo từng nền tảng, lịch đăng nội dung và công cụ quản lý kênh tuyển dụng |
| **Giả thuyết về AI** | AI hỗ trợ chuyển đổi JD thành nội dung phù hợp với từng nền tảng, so sánh thông tin giữa JD gốc và các phiên bản bài đăng, phát hiện nội dung cần cập nhật |
| **Cảm nhận nhanh** | Workflow kết hợp AI cho các tác vụ xử lý ngôn ngữ, không nhất thiết cần Agent |

#### Quy trình nháp hiện tại

| Bước | Hoạt động | Actor | Benchmark liên quan |
|---|---|---|---|
| 1 | Xác định nhu cầu và yêu cầu tuyển dụng | Hiring Manager, HRBP | 3,4 giờ/vị trí cho trao đổi yêu cầu với stakeholders [N1] |
| 2 | Chuẩn bị và thống nhất nội dung JD | HR, Hiring Manager | Thuộc nhóm hoạt động viết và đăng tin, 3,2 giờ/vị trí [N1] |
| 3 | Chỉnh sửa nội dung theo từng kênh | Recruitment Marketing, Recruiter | Thuộc cùng mốc 3,2 giờ/vị trí, không cộng thêm lần nữa |
| 4 | Đăng bài lên các nền tảng | Recruiter, Recruitment Marketing | Thuộc cùng mốc 3,2 giờ/vị trí, không cộng thêm lần nữa |
| 5 | Kiểm tra bài đăng và thông tin hiển thị | Recruiter, Hiring Manager | Hoạt động kiểm tra trong quy trình, nguồn chưa tách riêng thời gian |
| 6 | Cập nhật bài đăng khi JD thay đổi | Recruiter, Recruitment Marketing | Chưa có benchmark độc lập cho thời gian đồng bộ JD đa kênh |

**Luồng hiện tại:**

Hiring Manager xác nhận nhu cầu → HR chuẩn bị JD → Recruitment Marketing điều chỉnh nội dung → Recruiter đăng tuyển đa kênh → Kiểm tra bài đăng → Cập nhật khi có thay đổi

**Bottleneck:** Bước 3, bước 4 và bước 6

**Trải nghiệm liên quan:**

Đã từng phát triển công cụ hỗ trợ đăng tin tuyển dụng sử dụng dữ liệu từ Google Sheets, kết hợp Python và nhiều tài khoản Facebook
Công cụ hướng đến việc giảm thao tác lặp lại trong quá trình chuẩn bị và đăng bài tuyển dụng

**Phạm vi cải thiện đề xuất:**

Tập trung vào việc quản lý một nguồn JD thống nhất, hỗ trợ chuyển đổi nội dung theo từng kênh và phát hiện các bài đăng cần cập nhật khi thông tin tuyển dụng thay đổi

**Điểm cần xác minh trong thực tế:**

Mức độ phổ biến của việc sửa JD sau khi đăng, số lượng kênh cần cập nhật và thời gian dành cho việc đồng bộ bài đăng

### 3.3. Problem Card #2 — Candidate Application Consolidation

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi ứng viên gửi CV từ nhiều nền tảng và định dạng khác nhau, tôi muốn tập trung, chuẩn hóa và kiểm tra thông tin hồ sơ để hạn chế nhập liệu thủ công và tránh bỏ sót hoặc tạo dữ liệu trùng |
| **Actor** | Recruiter, Talent Acquisition Operations, Hiring Manager, ứng viên, IT/ATS Administrator, bộ phận quản lý dữ liệu |
| **Thời điểm / bối cảnh** | Doanh nghiệp nhận hồ sơ qua email, website tuyển dụng, biểu mẫu online, referral và các nền tảng tuyển dụng |
| **Quy trình hiện tại** | Tiếp nhận CV → Mở và đọc hồ sơ → Ghi nhận thông tin → Nhập dữ liệu vào ATS/Sheets → Kiểm tra trùng và thiếu → Chuyển hồ sơ cho Hiring Manager |
| **Bottleneck** | Thông tin đến từ nhiều nguồn, định dạng khác nhau và cần được nhập hoặc đối chiếu thủ công |
| **Impact** | Tăng khối lượng nhập liệu, dễ xảy ra dữ liệu thiếu hoặc không đồng nhất, phát sinh hồ sơ trùng và khó truy xuất lịch sử |
| **Benchmark** | Greenhouse 2026: 244 hồ sơ/vị trí trong dữ liệu 2025, NIJobs 2025: 4 giờ/vị trí cho reviewing applications và 4,1 giờ/vị trí cho data entry/documentation |
| **Success metric** | Thời gian nhập liệu và chuẩn hóa, tỷ lệ trích xuất thông tin đúng, số hồ sơ trùng được phát hiện, số hồ sơ bị bỏ sót |
| **Target đề xuất** | Giảm 40% thời gian nhập liệu và quản lý hồ sơ, lấy 4,1 giờ/vị trí làm mốc tham chiếu bên ngoài, tương đương khoảng 2,5 giờ/vị trí trong kịch bản thử nghiệm |
| **Phương án không dùng AI** | ATS, biểu mẫu ứng tuyển chung, kết nối API, chuẩn hóa trường dữ liệu, kiểm tra trùng bằng email hoặc số điện thoại |
| **Giả thuyết về AI** | AI hỗ trợ trích xuất dữ liệu từ CV có cấu trúc khác nhau, phát hiện trường thông tin thiếu và đề xuất các hồ sơ có khả năng trùng để nhân viên xác minh |
| **Cảm nhận nhanh** | Workflow kết hợp AI Document Processing, không cần Agent cho các tác vụ có quy tắc rõ ràng |

#### Quy trình nháp hiện tại

| Bước | Hoạt động | Actor | Benchmark liên quan |
|---|---|---|---|
| 1 | Nộp CV qua các kênh tuyển dụng | Ứng viên | Greenhouse: 244 lượt ứng tuyển/vị trí trong dữ liệu 2025 [N2] |
| 2 | Thu thập và mở hồ sơ từ các nguồn | Recruiter, TA Operations | Thuộc quy trình xử lý hồ sơ, benchmark khối lượng 244 hồ sơ/vị trí [N2] |
| 3 | Đọc và ghi nhận thông tin ứng viên | Recruiter | 4 giờ/vị trí cho reviewing applications [N1] |
| 4 | Nhập và chuẩn hóa thông tin | TA Operations, Recruiter | 4,1 giờ/vị trí cho data entry và documentation [N1] |
| 5 | Kiểm tra hồ sơ thiếu hoặc trùng lặp | Recruiter, IT/ATS Administrator | Thuộc hoạt động kiểm tra dữ liệu, chưa có tỷ lệ trùng chuẩn chung trong nguồn |
| 6 | Chuyển hồ sơ cho người phụ trách | Recruiter, Hiring Manager | Công đoạn bàn giao, không có mốc thời gian độc lập trong nguồn được chọn |

**Luồng hiện tại:**

Ứng viên nộp CV → Recruiter thu thập hồ sơ → Đọc và ghi nhận dữ liệu → Nhập thông tin vào ATS → Kiểm tra dữ liệu → Hiring Manager tiếp nhận

**Bottleneck:** Bước 3, bước 4 và bước 5

**Điểm cần chú ý:**

Benchmark 244 hồ sơ/vị trí của Greenhouse không có nghĩa mọi doanh nghiệp đều nhận số lượng hồ sơ tương tự
Con số 4 giờ/vị trí cho rà soát hồ sơ và 4,1 giờ/vị trí cho nhập liệu là hai hoạt động khác nhau, không phải thời gian xử lý cho một CV

**Giới hạn:**

- AI không tự quyết định ứng viên có phù hợp hay không
- Không tự động loại hoặc xếp hạng ứng viên
- Những trường thông tin không chắc chắn được chuyển cho nhân viên xác minh
- Dữ liệu cá nhân chỉ được xử lý trong phạm vi có quyền truy cập và mục đích tuyển dụng hợp lệ

### 3.4. Problem Card #3 — Candidate Pipeline Tracking

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi một ứng viên trải qua nhiều giai đoạn tuyển dụng với nhiều người tham gia, tôi muốn biết chính xác trạng thái hồ sơ, công việc đang chờ và người chịu trách nhiệm tiếp theo để tránh quy trình bị gián đoạn hoặc ứng viên không nhận được phản hồi |
| **Actor** | Recruiter, Hiring Manager, Interviewer, Technical Lead, Recruitment Coordinator, ứng viên, HR Operations |
| **Thời điểm / bối cảnh** | Khi doanh nghiệp tuyển dụng nhiều vị trí cùng lúc, ứng viên trải qua các giai đoạn tiếp nhận, phỏng vấn, đánh giá và thông báo kết quả |
| **Quy trình hiện tại** | Tiếp nhận hồ sơ → Cập nhật trạng thái → Sắp lịch phỏng vấn → Thu thập feedback → Thống nhất kết quả → Phản hồi ứng viên |
| **Bottleneck** | Việc thu thập feedback, cập nhật trạng thái và chuyển thông tin giữa các bộ phận có thể bị chậm hoặc thiếu nhất quán |
| **Impact** | Ứng viên phải chờ phản hồi, Recruiter phải theo dõi và nhắc việc nhiều lần, Hiring Manager thiếu thông tin kịp thời |
| **Benchmark** | NIJobs 2025: 2,9 giờ/vị trí cho thống nhất feedback nội bộ, 3,6 giờ/vị trí cho xử lý sau phỏng vấn, 3,6 giờ/vị trí cho phản hồi ứng viên [N1] |
| **Dữ liệu về trải nghiệm ứng viên** | Robert Walters Vietnam 2025 ghi nhận 77% người tìm việc được khảo sát cảm thấy hồ sơ thường bị bỏ qua, Survale 2025 ghi nhận 31% ứng viên Bắc Mỹ trong nghiên cứu không nhận phản hồi sau 1–2 tháng hoặc lâu hơn [N3, N5] |
| **Success metric** | Thời gian cập nhật trạng thái, thời gian phản hồi ứng viên, số ứng viên quá hạn phản hồi, thời gian chờ feedback từ Hiring Manager |
| **Target đề xuất** | Giảm 30% thời gian thao tác phản hồi ứng viên, tham chiếu từ 3,6 xuống khoảng 2,5 giờ/vị trí cho hoạt động tương ứng |
| **Phương án không dùng AI** | ATS, Kanban pipeline, quy định SLA, thông báo tự động theo trạng thái và phân công trách nhiệm rõ ràng |
| **Giả thuyết về AI** | AI hỗ trợ tổng hợp nội dung feedback, phát hiện trạng thái chưa được cập nhật, soạn thông báo và tóm tắt những trường hợp cần người phụ trách xử lý |
| **Cảm nhận nhanh** | Rule / Workflow, AI hữu ích khi cần tổng hợp nội dung tự do từ email và nhận xét |

#### Quy trình nháp hiện tại

| Bước | Hoạt động | Actor | Benchmark liên quan |
|---|---|---|---|
| 1 | Tiếp nhận và cập nhật thông tin ứng viên | Recruiter, TA Operations | 4,1 giờ/vị trí cho data entry/documentation [N1] |
| 2 | Xác định giai đoạn và người phụ trách tiếp theo | Recruiter, Hiring Manager | Thuộc quy trình quản lý hồ sơ và phối hợp |
| 3 | Sắp xếp lịch phỏng vấn | Recruitment Coordinator, Interviewer, ứng viên | 3,5 giờ/vị trí cho scheduling [N1] |
| 4 | Ghi nhận và xử lý thông tin sau phỏng vấn | Interviewer, Technical Lead, Recruiter | 3,6 giờ/vị trí cho post-interview processing [N1] |
| 5 | Tổng hợp feedback và thống nhất bước tiếp theo | Hiring Manager, Interviewer, Recruiter | 2,9 giờ/vị trí cho aligning internal feedback [N1] |
| 6 | Cập nhật trạng thái và thông báo kết quả | Recruiter, ứng viên | 3,6 giờ/vị trí cho candidate feedback/rejections [N1] |

**Luồng hiện tại:**

Ứng viên nộp hồ sơ → Recruiter cập nhật pipeline → Coordinator sắp xếp phỏng vấn → Interviewer đánh giá → Hiring Manager xác nhận kết quả → Recruiter phản hồi ứng viên

**Bottleneck:** Bước 4, bước 5 và bước 6

**Thông tin bổ sung:**

Theo GoodTime 2024, thời gian từ khi bắt đầu quá trình sắp xếp phỏng vấn đến khi lịch được xác nhận trung bình 38,1 giờ đối với phương thức xác nhận thủ công và 20,8 giờ khi sử dụng tính năng tự động xác nhận
Đây là thời gian chờ theo lịch, không phải số giờ nhân viên phải trực tiếp thao tác
Theo SHRM 2025, trung vị thời gian từ lúc mở yêu cầu tuyển dụng đến khi ứng viên chấp nhận offer ở Mỹ vào khoảng 45 ngày, phản ánh thời gian của toàn bộ quy trình chứ không phải riêng việc theo dõi pipeline

**Giới hạn:**

- AI không tự đưa ra quyết định tuyển dụng
- Mọi thay đổi quan trọng về kết quả ứng viên phải có người phụ trách xác nhận
- Nội dung thông báo phải được kiểm tra trước khi gửi
- Không sử dụng dữ liệu nhạy cảm ngoài phạm vi cần thiết cho công việc tuyển dụng

### 3.5. Card muốn pitch nhất

**Card số:** 1 — Multi-channel Recruitment Posting

**Vì sao chọn:**
- Có liên quan trực tiếp đến kinh nghiệm phát triển công cụ đăng tin tuyển dụng
- Có nhiều actor tham gia như Hiring Manager, HR, Recruitment Marketing và IT
- Quy trình gồm các công việc lặp lại, có khả năng tự động hóa
- Có benchmark về thời gian viết và đăng tuyển dụng
- Có thể đo thời gian thao tác trước và sau khi cải thiện
- Có thể bắt đầu bằng Rule/Workflow trước khi quyết định sử dụng AI

**Hướng thu hẹp Problem:**
Tập trung vào việc đồng bộ và cập nhật thông tin tuyển dụng trên nhiều nền tảng, đặc biệt khi JD thay đổi

**Câu hỏi muốn nhóm phản biện:**
Nếu doanh nghiệp đã sử dụng phần mềm đăng tuyển đa kênh, điểm nghẽn còn lại nằm ở thao tác đăng bài, quản lý nguồn dữ liệu JD hay việc đồng bộ các bài đăng sau khi thông tin tuyển dụng thay đổi?

### 3.6. AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Điều chỉnh trong Problem Card |
|---|---|---|
| Việc đăng tin tuyển dụng tự động đã có công cụ hỗ trợ, đề tài có nguy cơ trùng với sản phẩm hiện tại | Có | Thu hẹp vấn đề vào đồng bộ nội dung JD và kiểm tra tính nhất quán giữa các kênh |
| Benchmark của nước ngoài không thể được xem là thời gian thực tế tại doanh nghiệp Việt Nam | Có | Phân biệt benchmark tham khảo và baseline đo từ quy trình thực tế |
| Việc đăng tin lặp lại có thể được giải quyết bằng Rule mà không cần AI | Có | Chỉ cân nhắc AI cho việc hiểu và biến đổi nội dung JD |
| Không phải mọi kênh tuyển dụng đều cho phép tích hợp hoặc tự động đăng bài | Có | Giới hạn giải pháp ở các kênh hỗ trợ tích hợp hợp lệ và có quyền truy cập |
| Quá trình tiếp nhận và xử lý CV liên quan đến dữ liệu cá nhân của ứng viên | Có | Giới hạn AI ở thao tác hỗ trợ hành chính, không tự chấm điểm hoặc loại ứng viên |

**Điều chỉnh sau phản biện:**

Vấn đề ban đầu tập trung vào việc giảm số thao tác đăng bài tuyển dụng thủ công
Sau phản biện, phạm vi được thu hẹp vào việc quản lý JD từ một nguồn thống nhất và hỗ trợ cập nhật nội dung trên nhiều kênh khi có thay đổi
Việc sử dụng AI chỉ được cân nhắc ở các bước cần xử lý ngôn ngữ tự nhiên và đối chiếu ngữ nghĩa, thay vì sử dụng AI cho toàn bộ quy trình

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Chuẩn bị 3 Problem Cards gồm Multi-channel Recruitment Posting, Candidate Application Consolidation và Candidate Pipeline Tracking, ưu tiên đề tài Multi-channel Recruitment Posting dựa trên kinh nghiệm từng phát triển công cụ đăng tin tuyển dụng bằng Python và Google Sheets | Có bản phân tích cá nhân về actor, bottleneck, impact, success metrics và quy trình hiện tại để chuẩn bị trình bày |
| Phản biện bài của bạn khác | Phản biện một số đề tài của Linh và Khương, góp ý bổ sung quy tắc và logic để hoàn thiện hơn | Cần bổ sung câu hỏi cụ thể và điều chỉnh sau trao đổi nếu có ghi chép |
| Nhận phản biện | Chưa có ghi chép xác nhận câu hỏi và câu trả lời thực tế | Cần bổ sung người hỏi, nội dung phản biện và điều chỉnh thực tế nếu đã trao đổi |
| Gom cluster / cây OST | Phân loại các vấn đề tuyển dụng thành ba nhóm gồm quản lý JD và đăng tuyển, tiếp nhận hồ sơ ứng viên, theo dõi tiến độ tuyển dụng | Có cơ sở phân nhóm các vấn đề liên quan để chuẩn bị thảo luận |
| Chọn candidate problem | Ưu tiên Multi-channel Recruitment Posting, tập trung vào việc cập nhật và đồng bộ thông tin tuyển dụng trên nhiều nền tảng | Có đề xuất vấn đề cụ thể để đưa ra thảo luận |
| Kiểm chứng / research | Tìm hiểu các benchmark từ NIJobs, Greenhouse, Robert Walters và nghiên cứu những tính năng của Workable, Zoho Recruit, Recruitee và Base E-Hiring | Có số liệu và giải pháp tham khảo để xác định phạm vi vấn đề, chưa sử dụng dữ liệu thị trường thay thế số liệu thực tế của doanh nghiệp |
| Quy trình nhóm | Chuẩn bị quy trình từ tiếp nhận yêu cầu tuyển dụng, xây dựng JD, đăng bài đa kênh đến kiểm tra và cập nhật khi có thay đổi | Xác định những công đoạn có khả năng xuất hiện bottleneck để tiếp tục kiểm chứng |
| Problem Statement | Thu hẹp vấn đề từ việc đăng tin tuyển dụng thủ công sang việc khó đảm bảo tính nhất quán của thông tin tuyển dụng khi JD thay đổi trên nhiều kênh | Có định hướng Problem Statement với actor, bottleneck, impact và metric rõ ràng hơn |
| Mức can thiệp | Phân tích các bước có thể xử lý bằng quy tắc, tự động hóa quy trình và các bước cần phân tích nội dung ngôn ngữ tự nhiên | Có cơ sở lựa chọn phương án xử lý phù hợp, tránh sử dụng công nghệ phức tạp cho các tác vụ đơn giản |
| Quyết định | Chuẩn bị các tiêu chí đánh giá tính cần thiết, khả năng sử dụng, tính khả thi và hiệu quả kinh tế | Chưa có quyết định chính thức của nhóm, cần tiếp tục kiểm chứng trước khi kết luận |

### 4.1. Phân tích và điều chỉnh vấn đề cá nhân

**Vấn đề ban đầu**

Quá trình tuyển dụng yêu cầu nhân sự đăng tải và quản lý thông tin trên nhiều nền tảng khác nhau, dẫn đến các thao tác lặp lại và mất nhiều thời gian

**Các điểm nghẽn được xác định**

- Thông tin tuyển dụng phân tán trên nhiều nền tảng
- Nội dung JD có thể thay đổi trong quá trình tuyển dụng
- Người phụ trách phải đối chiếu những bài đăng hiện có với nội dung mới
- Việc chỉnh sửa nội dung trên nhiều kênh có thể gây sai lệch hoặc bỏ sót
- Thiếu khả năng theo dõi tập trung những bài đăng đã cập nhật và chưa cập nhật

**Điều chỉnh phạm vi vấn đề**

Thay vì tập trung vào việc tự động đăng tin tuyển dụng, vấn đề được thu hẹp thành quản lý và đảm bảo tính nhất quán của thông tin tuyển dụng trên nhiều kênh khi JD thay đổi

**Các chỉ số đánh giá**

- Thời gian cập nhật một JD trên các kênh
- Số thao tác thủ công cần thực hiện
- Số bài đăng có thông tin không nhất quán
- Thời gian phát hiện và xử lý nội dung sai lệch
- Tỷ lệ bài đăng được cập nhật đúng hạn

**Hướng giải quyết đề xuất**

Sử dụng một nguồn JD thống nhất, tự động phát hiện những trường thông tin thay đổi, hỗ trợ đối chiếu nội dung giữa các kênh và tạo danh sách bài đăng cần cập nhật

Những thay đổi quan trọng phải được người phụ trách kiểm tra và phê duyệt trước khi công bố

---

## 5. Dùng AI

| Checkpoint | Nội dung sử dụng | Kết quả hữu ích | Hạn chế nhận thấy | Điều chỉnh của cá nhân |
|---|---|---|---|---|
| CP1 | Hỗ trợ hệ thống hóa các vấn đề trong quy trình tuyển dụng và diễn đạt thành Job Story | Xác định thêm các actor, công đoạn và tiêu chí đánh giá | Phạm vi actor ban đầu còn hẹp, nhiều vấn đề chưa có bằng chứng thực tế | Mở rộng actor và bổ sung benchmark công khai có nguồn tham khảo |
| CP2 | Hỗ trợ xây dựng cấu trúc Problem Card, workflow và phản biện giả thuyết | Làm rõ bottleneck, impact, success metrics và phương án không sử dụng công nghệ phức tạp | Ban đầu tập trung quá nhiều vào giải pháp thay vì xác định nguyên nhân vấn đề | Điều chỉnh cách phân tích theo Problem → Bottleneck → Intervention |
| Research | Hỗ trợ tìm kiếm số liệu tuyển dụng và những phần mềm tương tự trên thị trường | Có nguồn tham khảo về thời gian tuyển dụng, khối lượng hồ sơ và các giải pháp hiện có | Benchmark chưa phản ánh trực tiếp doanh nghiệp cụ thể, một số tính năng cần kiểm tra trực tiếp | Phân biệt benchmark với baseline, giữ các khoảng trống cần kiểm chứng |
| Phân tích giải pháp | Hỗ trợ so sánh các cách xử lý thủ công, tự động hóa và xử lý nội dung | Xác định những bước có thể xử lý bằng quy tắc và các bước cần hiểu ngữ nghĩa | Một số đề xuất vượt quá phạm vi vấn đề và chưa có bằng chứng về hiệu quả | Thu hẹp phạm vi vào đồng bộ và kiểm tra tính nhất quán của JD |
| Rà soát bài nộp | Nhờ trợ lý đối chiếu báo cáo nhóm, nhật ký và báo cáo cá nhân với yêu cầu checkpoint | Xác định nội dung CP6 đã tích hợp và các việc còn cần người thực hiện hoặc nhóm xác nhận | Không thể xác nhận trải nghiệm cá nhân, kết quả thảo luận hay kiểm chứng thay thành viên | Cần tự kiểm các ghi nhận, hoàn thành reflection và cùng nhóm chốt các nội dung còn mở |

---

## 6. Reflection (CP7)

### 6.1. Tôi học được gì khi nghe Top 3 Problems của các bạn khác?

Khi góp ý cho đề tài của Linh và Khương, tôi tập trung vào việc bổ sung quy tắc xử lý và làm rõ các trường hợp ngoại lệ. Với bài ghi chú cuộc gọi vào CRM của Linh, một cách cụ thể hóa là quy định trường nào bắt buộc và xử lý ra sao khi cuộc gọi chưa có thông tin cho trường đó. Với bài làm rõ user story của Khương, có thể dùng một tình huống biên để kiểm xem tiêu chí nghiệm thu đã đủ rõ cho người triển khai chưa. Điểm tôi rút ra là mỗi quy tắc nên gắn với một tình huống mà người khác có thể kiểm lại

### 6.2. Nhóm có lúc nào bị solution-first không? Lúc đó nhóm nhận ra và xử lý thế nào?

Trong bài đối chiếu chào giá, hướng ban đầu là dùng AI để tự động đánh giá hồ sơ. Phần kiểm chứng ghi nhận lo ngại về độ chính xác và trách nhiệm khi kết quả sai. Nhóm thu hẹp phạm vi về việc phát hiện chênh lệch để chuyên viên kiểm lại. Sau khi tách việc ghép bảng khỏi việc so số, phần soát trên dữ liệu đã ghép đúng có thể dùng công thức và quy tắc cố định

### 6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể

Ở bản CP6 ban đầu, tôi đề xuất Go với Rule vì phép so khối lượng và đơn giá khá rõ khi dữ liệu đã được ghép đúng. Khi đọc bản review, tôi thấy cần tách hai việc: chọn Rule để đánh giá và quyết định đã đủ điều kiện chạy pilot hay chưa. Chẳng hạn, hai dòng ghép sai vẫn có thể cho ra cùng tổng tiền, nên chỉ kiểm tổng là chưa đủ. Tôi giữ đề xuất dùng Rule và thấy hợp lý khi hoãn pilot cho đến khi có dữ liệu được phép dùng và đáp án do người có chuyên môn duyệt

### 6.4. Kết quả kiểm chứng có làm tôi bất ngờ không? Điều gì?

Chi tiết khiến tôi chú ý là trong ba ý kiến được tổng hợp, có một người lo kết quả đối chiếu có thể sai và không rõ ai chịu trách nhiệm. Hai ý kiến còn lại cho thấy họ quan tâm đến công cụ hỗ trợ. Điều tôi rút ra là nhóm cần kiểm được mỗi cảnh báo đến từ dòng nào, ai xác nhận và xử lý thế nào nếu cảnh báo sai. Phần phỏng vấn hiện chưa có đủ số liệu thời gian và tần suất để dùng làm baseline

### 6.5. Điều khó nhất khi viết Problem Statement là gì?

Điều khó nhất là giữ phạm vi của vấn đề và chỉ số đo cho khớp nhau. Theo số liệu Vinh ghi lại, gom và soát cộng lại mất khoảng 11–13 giờ mỗi vòng, còn riêng phần soát mất 5–6 giờ. Phương án Rule chỉ tác động đến phần soát trên bảng đã ghép đúng, nên mục tiêu dưới 90 phút phải so với thời gian của chính bước đó. Khi đo, cần tính cả thời gian chuyên viên kiểm, sửa và xử lý ngoại lệ để biết công việc thực sự giảm bao nhiêu

### 6.6. Nếu làm lại, tôi sẽ thay đổi điều gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?

Nếu làm lại, tôi sẽ làm rõ từ đầu bước nào đang gây tốn công, số liệu lấy từ đâu và phần nào đã có thể xử lý bằng cách đơn giản hơn. Với bài chào giá, tôi sẽ hỏi sớm ai kiểm việc ghép mã, ai duyệt ngưỡng cảnh báo và nhóm có quyền dùng bộ hồ sơ nào. Tôi cũng sẽ đề nghị thử cách soát có checklist trên cùng bộ dữ liệu trước, để khi so với Rule có thể thấy thời gian tiết kiệm được đến từ bước nào

### 6.7. Hiểu bài

Giải thích bằng 5–8 câu theo chuỗi:
Problem → Workflow → Metric → Boundary → Intervention → Decision

Chuyên viên kinh tế kỹ thuật mất nhiều công dò chênh lệch khối lượng và đơn giá trong bảng chào giá đã ghép. Quy trình đề xuất kiểm mã hạng mục, đơn vị và phiên bản trước, sau đó tính chênh lệch và chuyển các dòng cần xem lại cho chuyên viên. Mốc tham chiếu là 5–6 giờ công mỗi vòng theo ghi nhận của Vinh, còn mục tiêu là dưới 90 phút gồm cả kiểm, sửa và xử lý ngoại lệ, đồng thời phát hiện đủ chênh lệch đã biết trong bộ đáp án. Chuyên viên xác nhận ngoại lệ và kết quả cuối, còn số liệu gốc và quyết định chọn nhà thầu vẫn do người có trách nhiệm quản lý. Nhóm chọn Rule cho phần so số vì dữ liệu đã có cấu trúc và công thức có thể kiểm lại từng dòng. Trạng thái pilot hiện là Not Yet, chờ xác nhận quyền sử dụng hồ sơ, dữ liệu đầu vào, đáp án và ngưỡng kiểm

---

## 7. Tài liệu tham khảo
**[N1] NIJobs — What's slowing down your hiring? (2025)**
**[N2] Greenhouse — The Hire Standard, Recruiting Benchmarks (2026)**
**[N3] Robert Walters Vietnam — Job Application Overload (2025)**
**[N4] GoodTime — 2024 Year in Review**
**[N5] Survale — 2025 Candidate Experience Benchmark Research**
**[N6] Employment Hero — State of Recruitment Report Singapore & Malaysia (2023)**
**[N7] SHRM — 2025 Recruiting Executives Benchmarking**
