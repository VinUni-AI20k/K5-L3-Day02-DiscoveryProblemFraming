# Báo cáo cá nhân — Tô Minh Thành

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Báo cáo cá nhân trên repo nhóm; điền bằng trải nghiệm thật của bạn, không ghi thay người khác.

## 1. Thông tin học viên

* Họ tên: Tô Minh Thành

* MSSV: 2A202603439

* Email trường (không bắt buộc, repo có thể để public): 

* Tên nhóm: Ban3

* Link repo nhóm: https://github.com/LysLama/K5-L3A-DAY02-Ban3-DiscoveryProblemFraming/tree/2A202603439-ToMinhThanh

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.


| \# | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) | 
| ----- | ----- | ----- | ----- | ----- | 
| 1 | Tốn thời gian | Khi chuẩn bị mở PR, tôi muốn giải thích rõ lý do thay đổi và cách kiểm thử, để reviewer hiểu mục đích mà không phải hỏi lại. | Junior Dev, Senior Dev | Quy trình được ước lượng khoảng 25 phút tổng cộng, trong đó khoảng 20 phút đọc lại ngữ cảnh và soạn mô tả; tần suất 4-5 PR/tuần. Chưa ghi nhật ký thời gian hoặc nguồn cho nhận xét của Senior. | 
| 2 | Lặp lại | Khi hoàn thành một API CRUD cơ bản, tôi muốn bao phủ các nhánh quan trọng bằng unit test mà không phải lặp lại nhiều thao tác viết mã, để giảm nguy cơ hồi quy. | Dev | Ước lượng 30-45 phút để viết test cho luồng cơ bản; chưa ghi loại API, số lần quan sát hoặc cách bấm giờ. | 
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi điều tra lỗi được báo trong Sentry/Kibana, tôi muốn xác định được đoạn log và bước tiếp theo cần kiểm tra, để rút ngắn thời gian chẩn đoán. | Dev, QA | Ước lượng 20-30 phút/lần và 2-3 lần/ngày trong lúc test; cần ghi khoảng thời gian và mẫu lỗi đã quan sát. | 
| 4 | Pain từ người khác | Khi QA báo một bug, tôi muốn nhận đủ bước tái hiện và dữ liệu liên quan, để có thể kiểm tra lỗi mà không phải hỏi lại nhiều lần. | Dev, QA | Con số 30% chưa có mẫu số, khoảng thời gian hay nguồn ticket đi kèm; cần bổ sung các thông tin đó hoặc bỏ tỷ lệ. | 
| 5 | Lặp lại | Khi chuẩn bị Daily Standup, tôi muốn nhớ chính xác các việc đã làm hôm trước, để cập nhật tiến độ rõ ràng. | Dev | Ước lượng 5-10 phút mỗi sáng để xem lại Git/Jira; chưa ghi nhật ký thời gian. | 
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi phải sửa một phần trong project cũ, tôi muốn hiểu các luồng liên quan trước khi thay đổi, để tránh làm hỏng hành vi hiện có. | Junior Dev | Ước lượng 3-4 giờ cho một lần tìm hiểu; cần nêu trường hợp cụ thể và phân biệt thời gian đọc với thời gian chờ/hỏi người khác. | 
| 7 | Lặp lại | Khi API thay đổi, tôi muốn frontend có thông tin endpoint, tham số và hành vi chính xác, để tích hợp mà không phải chờ hoặc sửa do tài liệu sai. | Backend Dev, Frontend Dev | Chưa có số lần thiếu tham số hoặc ví dụ ticket/comment; cần bổ sung bằng chứng cụ thể nếu giữ pain này. | 
| 8 | Tốn thời gian | Khi bắt đầu làm việc trên một dự án mới, tôi muốn hoàn tất cài đặt môi trường trong thời gian dự đoán được, để có thể bắt đầu xử lý task mà không mắc kẹt vì xung đột phiên bản. | Junior Dev mới onboarding | Ước lượng mất 1-2 ngày đầu; chưa tách thời gian thao tác thực tế khỏi thời gian chờ hoặc thời gian xử lý việc khác. | 

**Nếu có dùng AI để gợi ý thêm:** Tôi đưa bối cảnh "Tôi là Junior Software Engineer mới ra trường, làm việc theo mô hình Agile/Scrum" và nhờ AI gợi ý.

* Giữ lại: Ý #4 (Ticket bug từ QA thiếu thông tin) và #6 (Đọc legacy code). Rất đúng thực tế khi mới đi làm.

* Bỏ: Ý "AI tự động fix bug giùm Dev". Vì nó quá rủi ro (Feasibility/Viability thấp), chưa phù hợp với năng lực kiểm soát của junior dev.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)


| Rank | Problem | Vì sao chọn | Điều còn chưa chắc | 
| ----- | ----- | ----- | ----- | 
| 1 | Viết mô tả Pull Request (#1) | Quy trình chuẩn bị PR có thể mô tả rõ và có đầu vào cụ thể (Git diff, Jira ticket). Tần suất và thời gian hiện mới là ước lượng, cần kiểm tra lại. | Liệu thông tin trong diff và Jira có đủ để giải thích lý do nghiệp vụ, hay chỉ tạo ra bản diễn giải thay đổi code? | 
| 2 | Sinh khung Unit Test (#2) | Có tính lặp lại cao, tiết kiệm nhiều thời gian cho Dev. | AI có sinh ra test case ảo tưởng (hallucinate) sai logic nghiệp vụ không? | 
| 3 | Tóm tắt lỗi từ Log (#3) | Giảm thời gian debug đáng kể. | Việc đẩy log (có thể chứa dữ liệu nhạy cảm của khách) lên AI có vi phạm bảo mật không? | 

### Problem Card #1: Viết mô tả Pull Request (PR Description)

| Trường | Nội dung | 
| ----- | ----- | 
| Job Story | Khi chuẩn bị gửi thay đổi để review, tôi muốn trình bày lý do, phạm vi và cách kiểm thử rõ ràng, để reviewer đánh giá được thay đổi mà không phải hỏi lại thông tin cơ bản. | 
| Actor | Junior Software Engineer | 
| Thời điểm / bối cảnh | Ngay sau khi push code lên branch và chuẩn bị tạo PR trên GitHub/GitLab. | 
| Quy trình hiện tại (5 bước) | 1\. Push branch · 2. Tạo Draft PR · 3. Đọc lại Jira và Git diff để nhớ bối cảnh · 4. Viết description theo template (Context, Changes, How to test) · 5. Kiểm tra description, chuyển PR sang trạng thái sẵn sàng review và gửi reviewer. | 
| Bottleneck | Theo ước lượng trong quy trình nháp, bước 3 (đọc lại Jira và diff) mất 8 phút, bước 4 (soạn mô tả) mất 12 phút; tổng 20 phút. Cần đo lại để xác nhận đây thực sự là phần tốn thời gian nhất. | 
| Impact | Với 4-5 PR/tuần và khoảng 20 phút đọc ngữ cảnh + soạn mô tả mỗi PR, phần việc này tương đương khoảng 80-100 phút/tuần (phép tính từ các ước lượng hiện có, chưa phải số đo độc lập). Thời gian chờ review 1-2 ngày chưa được chứng minh là do mô tả thiếu context, nên không dùng làm impact đã xác nhận. | 
| Success metric | Mục tiêu thử nghiệm: giảm thời gian đọc ngữ cảnh + soạn mô tả từ baseline ước lượng khoảng 20 phút xuống dưới 5 phút/PR. Ghi thời gian từng PR trước/sau; đồng thời đếm PR bị yêu cầu bổ sung context trên tổng PR được review. Tỷ lệ dưới 10% là target tạm thời; cần đo baseline và xác nhận target phù hợp. | 
| Phương án không dùng AI | Dùng PR template có các mục Context, Changes, How to test cùng checklist reviewer. Template có thể cải thiện độ đầy đủ nhưng người viết vẫn phải cung cấp nội dung; cần so sánh với quy trình hiện tại trước khi kết luận mức giảm thời gian. | 
| Giả thuyết về AI | Nếu được phép theo chính sách dữ liệu, AI có thể dùng diff và nội dung ticket đã được kiểm tra để soạn bản nháp. AI không được tự suy diễn business context không có trong input; Dev xác minh và chịu trách nhiệm nội dung cuối. | 
| Cảm nhận nhanh | Workflow (AI làm 1 bước tổng hợp text, người phải duyệt). | 

Quy trình nháp hiện tại:

```
HIỆN TẠI — 25 phút

[1 Push code lên nhánh: 1'] → [2 Tạo Draft PR trên GitHub: 1'] 
→ [3 Đọc lại Jira + Git diff: 8'] ← BOTTLENECK
→ [4 Soạn mô tả PR: 12'] ← BOTTLENECK
→ [5 Kiểm tra mô tả, chuyển sang sẵn sàng review: 3']

```

### Problem Card #2: Gen khung Unit Test

| Trường | Nội dung | 
| ----- | ----- | 
| Job Story | Khi hoàn thành một API CRUD cơ bản, tôi muốn kiểm tra được các nhánh quan trọng mà không phải lặp lại nhiều thao tác viết mã, để giảm nguy cơ hồi quy. | 
| Actor | Backend Developer | 
| Thời điểm / bối cảnh | Khi viết xong logic của hàm/API, chuẩn bị commit code. | 
| Quy trình hiện tại (4 bước) | 1\. Đọc lại hàm vừa viết · 2. Nghĩ ra các test cases (Happy case, Bad case, Edge case) · 3. Gõ code setup mock data và assert · 4. Chạy thử và fix lỗi test. | 
| Bottleneck | Bước 3 (Gõ boilerplate code để setup mock và assert): mất 20-30 phút/hàm. | 
| Impact | Dev lười viết test vì tốn thời gian rập khuôn, dẫn đến code coverage thấp, dễ lọt bug ra production. | 
| Success metric | Quy trình nháp hiện cộng thành 35' cho cả 4 bước, còn 20-30' là ước lượng riêng cho bước viết boilerplate. Cần đo cùng một phạm vi trước/sau; chưa chốt target thời gian cho toàn quy trình. Theo dõi coverage riêng bằng công cụ dự án, chưa đặt target coverage khi chưa có baseline. | 
| Phương án không dùng AI | Dùng test template, snippet hoặc helper của dự án để giảm phần boilerplate; vẫn cần người viết chọn case, viết assertion và xác minh test. | 
| Giả thuyết về AI | AI đọc code của hàm, tự suy luận các nhánh logic (if/else) và tự sinh ra các test case sử dụng thư viện test chuẩn của project. | 
| Cảm nhận nhanh | Workflow (AI như một trợ lý viết nháp code). | 

Quy trình nháp hiện tại:

```
HIỆN TẠI — 35 phút

[1 Đọc lại hàm: 5'] → [2 Xác định test case: 5'] 
→ [3 Viết code Unit Test + Mock: 20'] ← BOTTLENECK
→ [4 Chạy thử và sửa lỗi: 5']

```

### Problem Card #3: Phân tích Log lỗi (Error Log Analysis)

| Trường | Nội dung | 
| ----- | ----- | 
| Job Story | Khi nhận báo cáo lỗi, tôi muốn xác định được dấu vết liên quan và hướng điều tra tiếp theo, để giảm thời gian tìm nguyên nhân có thể kiểm chứng. | 
| Actor | Developer / On-call Engineer | 
| Thời điểm / bối cảnh | Khi có alert từ hệ thống hoặc QA báo bug kèm link log Kibana/Sentry. | 
| Quy trình hiện tại (4 bước) | 1\. Mở tool log · 2. Filter theo Request ID · 3. Đọc stack trace từ dưới lên trên để tìm file code bị lỗi · 4. Xác định nguyên nhân. | 
| Bottleneck | Bước 3 (Đọc stack trace hàng ngàn dòng chứa toàn thư viện không liên quan): mất 15-20 phút. | 
| Impact | Bug rò rỉ lâu, tốn thời gian debug, áp lực khi on-call. | 
| Success metric | Đo thời gian từ lúc bắt đầu điều tra đến khi xác nhận được nguyên nhân cho một tập lỗi tương đương; sau khi có baseline mới đặt target giảm 50%. Không dùng MTTR thay cho thời gian chẩn đoán nếu chưa đo thời gian khắc phục/khôi phục đầy đủ. | 
| Phương án không dùng AI | Gắn thêm nhiều log rõ ràng hơn trong code (phụ thuộc vào ý thức lúc code). | 
| Giả thuyết về AI | Chỉ khi chính sách dữ liệu cho phép, AI có thể hỗ trợ tóm tắt log đã lọc/ẩn dữ liệu nhạy cảm, nêu dấu vết liên quan và giả thuyết điều tra kèm căn cứ. Kết quả không được xem là nguyên nhân đã xác nhận nếu chưa được Dev kiểm tra. | 
| Cảm nhận nhanh | Rule (Filter log) + AI Workflow (giải thích). | 

Quy trình nháp hiện tại:

```
HIỆN TẠI — 25 phút

[1 Mở Sentry/Kibana: 2'] → [2 Lọc đúng Request ID: 3'] 
→ [3 Đọc và trace log: 15'] ← BOTTLENECK
→ [4 Xác định file lỗi: 5']

```

### Card muốn pitch nhất

* Card số: **#1 (Viết mô tả Pull Request)**

* Vì sao: Quy trình có đầu vào có thể xác định (Git diff và nội dung ticket) và đầu ra là bản mô tả để người viết kiểm tra. Tuy nhiên, đầu vào có thể chứa mã nguồn hoặc thông tin nội bộ; dạng đầu ra là văn bản không tự làm cho việc gửi dữ liệu ra dịch vụ AI trở nên an toàn. Chỉ thử với công cụ và dữ liệu được tổ chức cho phép.

* Câu hỏi muốn nhóm phản biện: Có cách nào để AI tự fetch dữ liệu từ Jira và Github mà Dev không phải copy-paste thủ công vào prompt không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì | 
| ----- | ----- | ----- | 
| Diff lớn hoặc nhiều file có thể khiến bản tóm tắt thiếu trọng tâm; chưa kiểm tra được một ngưỡng dòng cụ thể. | Đồng ý | Chưa đặt ngưỡng 500 dòng khi chưa thử nghiệm. Pilot cần ghi nhận kích thước diff và lỗi đầu ra; PR vượt phạm vi pilot sẽ được viết thủ công. | 
| AI có thể tạo mô tả nghe hợp lý nhưng sai mục đích nghiệp vụ. | Đồng ý | Người viết phải đối chiếu bản nháp với ticket và diff trước khi cập nhật mô tả PR. TODO trong nội dung không bảo đảm người dùng đã kiểm tra, nên cần checklist review và không coi đây là biện pháp kỹ thuật ngăn gửi sai. | 


## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm | 
| ----- | ----- | ----- | 
|  | 

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? | 
| ----- | ----- | ----- | ----- | ----- | 
| CP1 Scan | Nhờ gợi ý nỗi đau của lập trình viên mới. | Gợi ý đúng các pain point về docs, log, setup môi trường. | Gợi ý AI tự động fix bug. | Gạt bỏ vì hiểu rằng AI tự fix bug rất nguy hiểm và ngoài tầm kiểm soát của junior. | 
| CP2 Problem Card | Đóng vai Senior Dev chỉ trích bài toán viết PR. | Cảnh báo về việc AI có thể làm Dev phụ thuộc, mất khả năng giao tiếp kỹ thuật. | Đề xuất giải pháp là cấm dùng AI. | Tôi không cấm, mà coi AI như công cụ "dự thảo", sửa lại quy trình để con người làm chủ văn bản cuối. | 
| CP4 Research | Dùng AI để tìm các công cụ liên quan đến tạo mô tả/review PR. | AI gợi ý các dự án như `pr-agent` và `openai-pr-reviewer`. | Chưa kèm link hoặc ghi chép kiểm chứng; nhận định về tính năng mặc định của từng dự án chưa được xác minh. | Trước khi kết luận, mở tài liệu chính thức, xác nhận đúng tính năng/phạm vi và chỉ ghi các kết quả đã kiểm tra. | 
| CP5 Quy trình | Gen sơ đồ Mermaid. | Tạo sơ đồ nhanh, đúng syntax. | Gộp bước lấy Git diff và Jira thành một. | Yêu cầu AI tách ra vì việc gọi API Jira và gọi Git diff là 2 context khác nhau. | 
| CP5–6 Problem Statement | Viết lại câu văn ngắn gọn cho phần Impact. | Từ ngữ sắc sảo, thuyết phục. | Mất đi tính bối cảnh nội bộ team (sự khó chịu của Senior). | Tự thêm lại cụm "Senior review mệt mỏi, PR bị ngâm" để thấy rõ tính human trong bài toán. | 
| CP6 Mức can thiệp / quyết định | Lập bảng so sánh các mức độ AI. | Đưa ra pros/cons rõ ràng. | Có xu hướng tâng bốc Agent. | Tôi dùng phán đoán thực tế: Agent không được phép chạm vào repo công ty, chốt Workflow là tối đa. | 

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**


**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Lúc đầu tôi định lấy metric là: "100% PR được viết tự động bởi AI". Nhưng sau khi bạn Huy phản biện: "Nếu AI viết sai logic mà Junior không thèm đọc, Senior chửi ai?", tôi nhận ra rủi ro rất lớn. Tôi đổi ý, sửa lại metric là "Giảm thời gian viết PR, tỷ lệ PR bị trả lại do thiếu context <10%" và kiên quyết đưa vào Boundary quy tắc "Dev phải tự review và chịu trách nhiệm với bản nháp PR".

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Rất bất ngờ khi khảo sát 3 anh Senior Dev. Tôi tưởng họ muốn PR mô tả thật chi tiết từng hàm bị đổi (kỹ thuật). Nhưng không, cả 3 đều nói: "Code đổi gì thì anh nhìn Git diff là thấy. Cái anh cần trong description là TẠI SAO em lại làm thế này, business logic đằng sau là gì, test case em chạy là gì?". Điều này làm thay đổi hoàn toàn cách chúng tôi định viết Prompt: phải nhồi thêm bối cảnh từ Jira vào, chứ chỉ quăng Git diff cho AI thì vô dụng.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Đó là việc xác định ranh giới (Boundary) và cách đo lường chất lượng (Quality Metric). Đo thời gian viết PR giảm từ 20 phút xuống 5 phút thì dễ. Nhưng đo xem PR đó "có chất lượng hơn" hay không thì rất cảm tính. Nhóm đã rất vất vả mới chốt được metric gián tiếp là "Đếm số lượt comment (ping) yêu cầu bổ sung context của người Reviewer".

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ xem xét phương án No AI kỹ hơn. Có thể chỉ cần tạo một PR Template chuẩn trên GitHub (có các mục checklist bắt buộc check) là đã giải quyết được 80% vấn đề junior viết thiếu ý, mà không cần tốn tiền chạy API của OpenAI. Tôi sẽ phản biện mạnh hơn ở bước CP4 để nhóm thực sự chứng minh xem AI có đem lại giá trị vượt trội so với một template cứng hay không.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Bắt đầu từ **problem** là Junior Dev tốn nhiều thời gian viết mô tả PR và thường viết kém khiến Senior phàn nàn. Ta ánh xạ ra **quy trình** mở PR hiện tại, nhận ra nút thắt tốn 15-20 phút nằm ở việc tổng hợp lại logic code (Git diff) và yêu cầu (Jira) thành lời văn. Từ đó, **metric** được đặt ra là giảm thời gian viết xuống dưới 5 phút và giảm số lần bị bắt sửa PR. Để đảm bảo chất lượng, **boundary** cốt lõi là AI chỉ đóng vai trò soạn nháp, Dev bắt buộc phải kiểm duyệt và chịu trách nhiệm trước khi bấm Submit. Do đầu vào (diff, ticket) cố định và các bước rõ ràng, **mức can thiệp AI** được chọn là Workflow. Cuối cùng, nhóm đi đến **quyết định** là Go (pilot) bằng cách cho Dev tự copy/paste diff vào ChatGPT trong 2 tuần để kiểm chứng chất lượng prompt trước khi tự động hóa bằng tool.

## 7. Tài liệu tham khảo

* Ghi chú phỏng vấn cá nhân trực tiếp với 3 Senior Software Engineers tại công ty (dữ liệu đã ẩn danh thành Dev A, Dev B, Dev C). Đây là phỏng vấn sâu 1-1, không phải khảo sát. Thời điểm thực hiện: 04/10/2026 - 05/10/2026 thông qua Google Meet. Mục đích phỏng vấn: tìm hiểu kỳ vọng của reviewer khi đọc Pull Request.

Tài liệu chính thức của công cụ CodiumAI PR-Agent. URL: https://github.com/Codium-ai/pr-agent (Ngày truy cập: 08/11/2026).

Tài liệu chính thức của GitHub Copilot for Pull Requests. URL: https://docs.github.com/en/copilot/using-github-copilot/using-github-copilot-for-pull-requests (Ngày truy cập: 08/11/2026).

Hướng dẫn "How to write the perfect pull request" - GitHub Blog (Quy chuẩn viết Pull Request tốt của cộng đồng mã nguồn mở). URL: https://github.blog/2015-01-21-how-to-write-the-perfect-pull-request/ (Ngày truy cập: 07/11/2026).