# Báo cáo cá nhân — 2A202603366_NguyenHuyHoang

## 1. Thông tin học viên

- Họ tên: Nguyễn Huy Hoàng
- MSSV: 2A202603366
- Email trường (không bắt buộc, repo có thể để public): 
- Tên nhóm: SUDO
- Link repo nhóm: https://github.com/rachel157/K5-L3A-DAY02-SUDO-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | **Tốn thời gian** & **Lặp lại** | Khi làm đồ án nhóm, tôi muốn tự động đồng bộ hóa và kiểm tra trạng thái các biến môi trường (env/secrets) giữa các thành viên, để không bị lỗi xung đột hoặc lộ thông tin bảo mật khi push code lên GitHub. | Sinh viên làm đồ án nhóm, Fresher Engineer | Xảy ra mỗi khi bắt đầu sprint mới hoặc có thành viên join nhóm; mất 15-30 phút cấu hình lại file `.env` thủ công. |
| 2 | **Cần đọc, tổng hợp nhiều thông tin** | Khi tìm kiếm tài liệu nghiên cứu công nghệ mới hoặc thư viện cho đồ án, tôi muốn tổng hợp các bài viết, tài liệu API và mã nguồn mẫu từ nhiều nguồn (freeCodeCamp, GitHub, docs chính thức), để không phải mở hàng chục tab trình duyệt và đọc lặp lại thông tin cũ. | Sinh viên làm đồ án tốt nghiệp, lập trình viên | Diễn ra hằng ngày trong giai đoạn R&D; mất từ 1-2 tiếng mỗi ngày chỉ để lọc và đọc tài liệu phân tán. |
| 3 | **Pain từ người khác** | Khi ban chủ nhiệm CLB cầu lông tổ chức giải đấu nội bộ hoặc ghép cặp đấu, tôi muốn tự động hóa việc xếp lịch thi đấu và chia bảng đấu, để tránh việc bị trùng giờ của các thành viên và sai sót khi tính điểm. | Ban vận động CLB cầu lông, sinh viên tham gia giải đấu | Xảy ra trước mỗi giải đấu; thủ công trên Excel mất 3-4 tiếng, hay bị phàn nàn về lịch đấu chồng chéo. |
| 4 | **Lặp lại** & **Tốn thời gian** | Khi ứng tuyển thực tập và cập nhật CV trên các nền tảng tuyển dụng (TopCV), tôi muốn tự động điều chỉnh mô tả dự án và kỹ năng trong CV sao cho khớp với từ khóa của từng Job Description (JD), để không phải sửa thủ công từng dòng cho mỗi lần nộp hồ sơ. | Sinh viên năm cuối, ứng viên tìm việc Fresher | Diễn ra mỗi khi ứng tuyển một vị trí mới; mất khoảng 20-30 phút chỉnh sửa tỉ mỉ cho mỗi bộ hồ sơ. |
| 5 | **Cần đọc, tổng hợp nhiều thông tin** | Khi tham gia các khóa học lập trình dài hạn hoặc xem các chuỗi podcast kỹ thuật (như freeCodeCamp), tôi muốn trích xuất và tóm tắt các điểm cốt lõi, đoạn code mẫu thành tài liệu ngắn gọn, để dễ ôn tập lại mà không phải tua lại video hàng tiếng đồng hồ. | Sinh viên tự học, học viên các chương trình đào tạo công nghệ | Xảy ra hằng tuần; mỗi video dài 1-3 tiếng, tốn rất nhiều thời gian xem lại khi cần ôn kiến thức. |
| 6 | **Pain từ người khác** | Khi các thành viên trong nhóm làm đồ án phân công công việc và theo dõi tiến độ qua các công cụ quản lý, tôi muốn nhận được cảnh báo tự động khi có task bị chậm deadline, để nhóm không bị dồn việc vào phút chót trước ngày nộp. | Thành viên nhóm đồ án, nhóm trưởng (Project Manager) | Xảy ra xuyên suốt quá trình làm đồ án; tuần nào cũng có ít nhất 1-2 task bị trễ hạn do không theo dõi sát sao. |
| 7 | **Tốn thời gian** | Khi tìm sân cầu lông trống để đặt lịch đánh cùng nhóm bạn vào giờ cao điểm (tối hoặc cuối tuần), tôi muốn có một cái nhìn tổng hợp trạng thái trống/đặt của nhiều sân quanh khu vực, để không phải gọi điện hoặc nhắn tin hỏi từng sân một. | Nhóm chơi cầu lông, sinh viên thích vận động thể thao | Xảy ra 2-3 lần/trước mỗi buổi đánh; mất 20-30 phút chat/gọi điện hỏi các sân mà vẫn thường xuyên hết chỗ. |
| 8 | **Lặp lại** & **Pain từ người khác** | Khi quản lý các thông báo, lịch sinh hoạt và tài liệu học tập trong các kênh cộng đồng (như Slack hoặc Discord của nhóm lớp học), tôi muốn hệ thống tự động gom nhóm các thông báo quan trọng theo chủ đề, để không bị trôi tin nhắn và bỏ lỡ deadline nộp bài/báo cáo. | Thực tập sinh, sinh viên tham gia các chương trình đào tạo thực tế | Xảy ra hằng ngày; hàng trăm tin nhắn trôi qua khiến sinh viên dễ bỏ lỡ thông báo lịch họp hoặc deadline quan trọng. |

**Nếu có dùng AI để gợi ý thêm:** 
- Ý AI gợi ý được giữ lại: Các vấn đề liên quan đến đồng bộ biến môi trường khi làm đồ án, tự động hóa xếp lịch thi đấu cầu lông, và tối ưu CV theo JD.
- Ý AI gợi ý bị bỏ: Các vấn đề quá chung chung như "quản lý chi tiêu cá nhân" hoặc "lên thực đơn hằng ngày" vì không gắn liền với bối cảnh học tập, sinh hoạt kỹ thuật và thể thao thực tế của bản thân.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Quản lý và xếp lịch thi đấu giải cầu lông nội bộ CLB | Pain rõ từ người tổ chức, tần suất cao, tốn nhiều thời gian thủ công và dễ xảy ra xung đột thời gian. | Liệu ban tổ chức có sẵn sàng dùng công cụ mới thay vì thói quen dùng Excel truyền thống không? |
| 2 | Đồng bộ và quản lý biến môi trường (`.env`/secrets) khi làm đồ án nhóm | Xảy ra thường xuyên trong các dự án phần mềm, ảnh hưởng trực tiếp đến tốc độ phát triển và bảo mật. | Mức độ phức tạp của các cấu hình bảo mật có vượt quá phạm vi bài toán đơn giản không? |
| 3 | Tối ưu hóa mô tả CV theo từng Job Description (JD) khi ứng tuyển thực tập | Giúp tiết kiệm thời gian chỉnh sửa hồ sơ lặp đi lặp lại cho sinh viên năm cuối chuẩn bị đi làm. | Độ chính xác của việc parse JD và match kỹ thuật bằng AI có đủ tin cậy với người dùng không? |

### Problem Card #1 (Chọn làm trọng tâm)

| Trường | Nội dung |
|---|---|
| Job Story | Khi ban vận động CLB cầu lông tổ chức giải đấu nội bộ, tôi muốn tự động hóa quy trình xếp lịch thi đấu và chia bảng đấu, để tránh việc bị trùng giờ của các thành viên và giảm sai sót khi tính điểm. |
| Actor | Ban chủ nhiệm / Ban tổ chức giải đấu CLB cầu lông |
| Thời điểm / bối cảnh | 1-2 tuần trước khi diễn ra giải đấu nội bộ của trường hoặc câu lạc bộ |
| Quy trình hiện tại (3–7 bước) | 1. Thu thập danh sách thành viên đăng ký qua Google Form.<br>2. Xuất danh sách ra file Excel và lọc điều kiện trình độ.<br>3. Thủ công chia bảng đấu và bốc thăm cặp đấu.<br>4. Xếp lịch giờ đánh dựa trên khung giờ trống của các sân.<br>5. Thông báo lịch đấu lên nhóm chat và nhận phản hồi đổi giờ.<br>6. Cập nhật lại lịch thủ công khi có người xin đổi lịch. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 và Bước 5 (Xếp lịch giờ đánh và xử lý phản hồi đổi lịch); mất trung bình 3-4 tiếng và thường xuyên bị xung đột thời gian sân/vận động viên. |
| Impact (nếu không giải thì sao) | Giải đấu bị chậm tiến độ, ban tổ chức áp lực, nhiều vận động viên bỏ giải vì trùng lịch thi đấu cá nhân. |
| Success metric (baseline → target) | Thời gian hoàn thành xếp lịch giảm từ 3-4 tiếng xuống dưới 15 phút; tỷ lệ xung đột lịch thi đấu giảm từ 25% xuống 0%. |
| Phương án không dùng AI | Dùng template Excel chuẩn hóa có sẵn hàm macro/VBA tự động chia cặp đấu ngẫu nhiên và kiểm tra trùng lịch cơ bản bằng conditional formatting. |
| Giả thuyết về AI (nếu có) | Dùng AI/Workflow để tự động phân tích khung giờ rảnh của các thành viên từ form đăng ký và gợi ý lịch thi đấu tối ưu không bị chồng chéo. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại (Card #1):
```text
[Thu thập form đăng ký] ──▶ [Xuất Excel lọc thủ công] ──▶ [Chia bảng & bốc thăm] ──▶ [Xếp lịch sân/giờ (Bottleneck)] ──▶ [Thông báo & Xử lý đổi lịch] ──▶ [Chốt lịch thi đấu]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhóm sinh viên phát triển đồ án phần mềm, tôi muốn tự động đồng bộ hóa các biến môi trường (`.env`) giữa các thành viên, để không bị lỗi kết nối cơ sở dữ liệu hoặc lộ thông tin bảo mật khi làm việc nhóm. |
| Actor | Thành viên nhóm phát triển đồ án phần mềm (Developer) |
| Thời điểm / bối cảnh | Giai đoạn khởi tạo dự án và mỗi khi có thay đổi cấu hình kết nối trong quá trình code. |
| Quy trình hiện tại (3–7 bước) | 1. Trưởng nhóm tạo file `.env.example` đẩy lên GitHub.<br>2. Thành viên clone repo về máy.<br>3. Tự điền các giá trị secret thủ công qua chat riêng hoặc hướng dẫn miệng.<br>4. Khi có thay đổi cấu hình, thông báo lại qua Slack/Zalo.<br>5. Thành viên tự cập nhật lại file `.env` cá nhân. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 và Bước 5 (Cập nhật thủ công và đồng bộ thông tin qua chat); mất 15-30 phút mỗi lần đổi cấu hình và dễ gây lỗi `Connection Refused` do lệch biến. |
| Impact (nếu không giải thì sao) | Mất thời gian debug lỗi cấu hình môi trường của các thành viên mới, rủi ro lộ API Key/Secret lên public repo. |
| Success metric (baseline → target) | Thời gian cấu hình môi trường cho thành viên mới giảm từ 20 phút xuống dưới 2 phút; số lần lỗi lệch biến env giảm về 0. |
| Phương án không dùng AI | Sử dụng các dịch vụ quản lý secret chuyên dụng như Doppler hoặc tính năng Environment Variables của GitHub/Railway. |
| Giả thuyết về AI (nếu có) | Không cần AI, chỉ cần Rule/Script tự động kiểm tra tính hợp lệ của file env so với schema mẫu. |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại (Card #2):
```text
[Tạo file .env.example] ──▶ [Clone repo về máy] ──▶ [Điền secret thủ công (Bottleneck)] ──▶ [Đồng bộ qua chat khi đổi] ──▶ [Cập nhật file .env cá nhân]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi sinh viên năm cuối chuẩn bị nộp hồ sơ thực tập, tôi muốn tự động điều chỉnh từ khóa trong CV sao cho khớp với mô tả công việc (JD) của nhà tuyển dụng, để tăng tỷ lệ qua vòng lọc hồ sơ tự động (ATS). |
| Actor | Sinh viên tìm việc Fresher / Thực tập sinh |
| Thời điểm / bối cảnh | Trước mỗi đợt nộp hồ sơ ứng tuyển vị trí thực tập phần mềm. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc kỹ yêu cầu trong JD của công ty.<br>2. Mở file CV gốc trên TopCV/Word.<br>3. Đọc dò từng dòng để chỉnh sửa lại phần mô tả kỹ năng và dự án cho khớp với JD.<br>4. Xuất file PDF và kiểm tra lại bố cục.<br>5. Nộp hồ sơ. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (Chỉnh sửa thủ công phần mô tả dự án và từ khóa); mất 20-30 phút cho mỗi bản CV ứng tuyển khác nhau. |
| Impact (nếu không giải thì sao) | CV không khớp từ khóa ATS, dễ bị loại từ vòng gửi xe, tốn nhiều thời gian sửa hồ sơ thủ công nếu nộp nhiều công ty. |
| Success metric (baseline → target) | Thời gian tùy chỉnh CV cho mỗi JD giảm từ 30 phút xuống dưới 5 phút; tỷ lệ vượt qua vòng lọc ATS tăng lên. |
| Phương án không dùng AI | Tạo sẵn các phiên bản CV theo từng nhóm vị trí (Backend, Frontend, AI Engineer) để chọn nhanh bản phù hợp nhất. |
| Giả thuyết về AI (nếu có) | Dùng Workflow kết hợp LLM để phân tích JD, đối chiếu với ngân hàng dự án của cá nhân và tự động sinh ra phần mô tả phù hợp nhất. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại (Card #3):
```text
[Đọc yêu cầu JD] ──▶ [Mở file CV gốc] ──▶ [Chỉnh sửa thủ công từ khóa (Bottleneck)] ──▶ [Xuất file PDF & Kiểm tra bố cục] ──▶ [Nộp hồ sơ]
```

### Card muốn pitch nhất

- Card số: **Card #1 (Quản lý và xếp lịch thi đấu giải cầu lông nội bộ CLB)**
- Vì sao: Đây là bài toán thực tế có pain rất rõ ràng từ người tổ chức (Ban vận động CLB cầu lông HUST), số liệu đo lường thời gian thủ công lớn và có thể giải quyết dứt điểm bằng quy trình hệ thống hóa.
- Câu hỏi muốn nhóm phản biện: *"Liệu việc tự động hóa xếp lịch có giải quyết được hoàn toàn các ngoại lệ khi thành viên đột xuất xin đổi giờ vào phút chót không?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI chỉ ra rằng các thành viên thường có lịch học/lịch cá nhân thay đổi liên tục, việc chỉ dùng thuật toán tĩnh từ form đăng ký sẽ dễ gãy khi bước vào thời điểm diễn ra giải. | Đồng ý | Bổ sung thêm cơ chế workflow linh hoạt cho phép cập nhật lịch trống động và sinh thông báo tự động khi có yêu cầu đổi lịch giữa các cặp đấu. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày Card Quản lý giải đấu cầu lông của nhóm SUDO. | Giúp nhóm hình dung rõ pain thực tế từ việc tổ chức hoạt động thể thao sinh viên. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: *"Giải pháp của nhóm bạn có phụ thuộc vào việc người dùng phải nhập liệu hoàn toàn thủ công không?"* | Giúp nhóm bạn tối ưu hóa bước đầu vào dữ liệu (data input). |
| Nhận phản biện | Câu hỏi tôi nhận được: *"Làm sao xử lý trường hợp sân cầu lông bị quá tải khung giờ tối?"* | Tôi đã bổ sung thêm tính năng gợi ý khung giờ thay thế (buổi sáng hoặc trưa) vào quy trình To-Be. |
| Gom cluster / cây OST | Đóng góp ý kiến gom các vấn đề về quản lý sinh hoạt cộng đồng và tổ chức sự kiện vào một nhánh chung. | Giúp nhóm định hình rõ phạm vi bài toán tập trung vào khâu tổ chức sự kiện thể thao. |
| Chọn candidate problem | Cùng nhóm thảo luận và vote chọn bài toán **Tự động hóa xếp lịch và quản lý giải đấu cầu lông**. | Thống nhất được đề tài chính thức cho toàn nhóm SUDO. |
| Kiểm chứng / research | Tham gia phỏng vấn nhanh 2 thành viên ban tổ chức CLB cầu lông (theo phương pháp The Mom Test). | Xác nhận đúng bottleneck mất 3-4 tiếng xếp lịch thủ công là có thật. |
| Quy trình nhóm | Vẽ sơ đồ quy trình As-Is và To-Be của bài toán xếp lịch giải đấu. | Làm rõ các bước nghẽn trong việc xếp lịch thủ công hiện tại. |
| Problem Statement | Viết và tinh chỉnh câu Problem Statement v0 của nhóm. | Xác định rõ boundary và success metric đo được. |
| Mức can thiệp AI | Phân tích 4 rủi ro (Value, Usability, Feasibility, Viability) để chốt mức can thiệp **Workflow**. | Đảm bảo AI hỗ trợ xử lý logic xếp lịch nhưng vẫn giữ quyền quyết định cuối cùng cho con người. |
| Quyết định | Tham gia biểu quyết đưa ra quyết định **Go** cho đề tài. | Hoàn thiện biên bản quyết định chung của nhóm SUDO. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI gợi ý các lăng kính vấn đề trong đời sống sinh viên. | Mở rộng góc nhìn sang các mảng quản lý sự kiện và học tập. | Đưa ra các ý tưởng quá vĩ mô, không gắn với thực tế cá nhân. | Lọc lại các ý thực tế liên quan đến cầu lông, đồ án và tuyển dụng. |
| CP2 Problem Card | Hỗ trợ cấu trúc hóa các trường thông tin trong Problem Card. | Giúp chuẩn hóa văn phong Job Story và Success Metric. | Đặt sai thời gian ước lượng cho bottleneck (quá nhanh so với thực tế). | Tự điều chỉnh lại thời gian thực tế dựa trên kinh nghiệm tổ chức giải. |
| CP4 Research | Tóm tắt các phương pháp giải quyết bài toán xếp lịch thi đấu (sports scheduling). | Cung cấp góc nhìn về thuật toán chia bảng đấu phổ biến. | Đề xuất các giải pháp công nghệ quá phức tạp so với quy mô CLB trường học. | Thu gọn lại phạm vi giải pháp ở mức workflow thực tế, dễ triển khai. |
| CP5 Quy trình | Gợi ý các bước trong sơ đồ quy trình As-Is và To-Be. | Tạo khung Mermaid cơ bản cho sơ đồ quy trình. | Bỏ sót các bước xử lý ngoại lệ khi đổi lịch thi đấu giữa chừng. | Bổ sung thêm các bước kiểm tra xung đột thời gian và xử lý đổi lịch thủ công. |
| CP5–6 Problem Statement | Viết câu Problem Statement chuẩn theo mô hình Lean UX. | Tổng hợp nhanh các ý chính của nhóm thành một đoạn văn hoàn chỉnh. | Định nghĩa boundary quá lỏng lẻo, cho phép AI tự quyết định thay con người. | Siết chặt boundary: AI chỉ gợi ý lịch, ban tổ chức là người chốt quyết định cuối cùng. |
| CP6 Mức can thiệp / quyết định | Phân tích ưu nhược điểm giữa các mức Rule, Workflow và Agent. | Làm rõ rủi ro Feasibility và Usability khi ứng dụng Agent. | Khuyên dùng Agent cho toàn bộ hệ thống quản lý. | Chọn mức **Workflow** vì an toàn hơn, dễ kiểm soát và phù hợp với nguồn lực nhóm. |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Việc lắng nghe các vấn đề từ bạn bè trong lớp giúp tôi nhận ra rằng những "nỗi đau" nhỏ nhặt trong đời sống hằng ngày (như việc quản lý thông báo nhóm, tìm tài liệu học tập, hay sắp xếp lịch sinh hoạt) nếu được nhìn nhận qua lăng kính sản phẩm đều có thể trở thành những bài toán giá trị. Nhiều bạn có góc nhìn rất thực tế về việc tự động hóa các tác vụ lặp đi lặp lại mà trước đó tôi xem là chuyện hiển nhiên phải chịu đựng.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có, ngay trong phần thảo luận đầu tiên, một số thành viên trong nhóm đã nghĩ ngay đến việc xây dựng một "ứng dụng AI thông minh tự động hoàn toàn mọi khâu tổ chức giải đấu". Nhóm đã nhận ra sự lệch hướng này khi đối chiếu lại với phương pháp luận của bài học: chưa làm rõ bottleneck và quy trình hiện tại của người dùng. Chúng tôi đã dừng lại, quay về phân tích kỹ actor và quy trình As-Is trước khi bàn tiếp về việc có cần dùng AI hay không.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi đã đổi ý sau khi nhận được câu hỏi phản biện về việc AI có thể tự ý thay đổi lịch thi đấu của các vận động viên mà không cần sự đồng ý của ban tổ chức hay không. Ban đầu tôi nghĩ nên cho AI tự động xếp lịch toàn quyền (mức Agent). Tuy nhiên, sau khi thảo luận và nhận thấy rủi ro sai sót ngữ cảnh (như VĐV bận thi đấu môn học đột xuất), tôi đã đồng ý hạ mức can thiệp xuống **Workflow**, trong đó AI chỉ đóng vai trò gợi ý phương án tối ưu, còn quyết định cuối cùng vẫn thuộc về con người.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Kết quả kiểm chứng thực tế qua phỏng vấn ngắn với ban tổ chức CLB cầu lông làm tôi khá bất ngờ ở chỗ thời gian tốn kém nhất không phải là khâu bốc thăm chia bảng ban đầu, mà là khâu **xử lý các yêu cầu đổi lịch phát sinh** từ các cặp đấu do trùng lịch học đột xuất. Điều này khiến nhóm phải điều chỉnh trọng tâm giải pháp tập trung nhiều hơn vào cơ chế xử lý ngoại lệ thay vì chỉ làm đẹp thuật toán chia bảng.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó nhất là việc giới hạn phạm vi bài toán (boundary) sao cho đủ hẹp để có thể giải quyết trong thời gian ngắn nhưng vẫn đủ giá trị để mang lại tác động thực tế. Việc viết success metric sao cho có số liệu đo lường cụ thể (baseline → target) thay vì dùng các từ ngữ chung chung cũng đòi hỏi nhiều thời gian suy ngẫm và căn cứ vào dữ liệu thực tế.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ chủ động thực hiện việc phỏng vấn kiểm chứng thực tế (The Mom Test) sớm hơn ngay từ đầu giờ thay vì đợi đến phần CP4 mới tiến hành. Tôi cũng sẽ phản biện nhóm mạnh mẽ hơn ở khâu xác định giả thuyết AI, yêu cầu nhóm làm rõ xem việc đưa AI vào có thực sự giải quyết được bài toán tốt hơn các phương pháp quy tắc (Rule/Workflow) đơn giản hay không, tránh việc lạm dụng AI không cần thiết.

**6.7. Hiểu bài:** 
Chuỗi bài toán của nhóm tôi đi từ việc nhận diện **problem** thực tế là ban tổ chức CLB cầu lông mất 3-4 tiếng để xếp lịch giải đấu thủ công và hay bị trùng giờ. Tiếp theo, nhóm vẽ rõ **quy trình** hiện tại (As-Is) để tìm ra đúng **bottleneck** ở khâu xếp giờ sân và xử lý đổi lịch. Từ đó, chúng tôi đặt ra **metric** thành công là giảm thời gian xếp lịch xuống dưới 15 phút và triệt tiêu xung đột giờ đấu. Về mặt **boundary**, hệ thống chỉ được phép gợi ý lịch tối ưu chứ không được tự ý chốt lịch thay con người. Xét về **mức can thiệp AI**, nhóm chọn mức **Workflow** kết hợp thuật toán và AI gợi ý có kiểm soát. Cuối cùng, với lập luận chặt chẽ và đánh giá kỹ 4 rủi ro, nhóm đưa ra quyết định **Go** để triển khai xây dựng giải pháp trong các buổi học tiếp theo.

---

## 7. Tài liệu tham khảo

- Tài liệu hướng dẫn Day 02: Discovery & Problem Framing (K5 Level 3).
- Các nguyên lý thiết kế sản phẩm từ Marty Cagan và Google PAIR.
- Ghi chú phỏng vấn thực tế từ Ban vận động CLB Cầu lông HUST.