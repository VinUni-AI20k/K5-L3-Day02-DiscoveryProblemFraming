# Phần cá nhân (của Quang)


## 1. Thông tin học viên

- Họ tên: Nguyễn Minh Quang
- MSSV: 2A202603791
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: I3
- Link repo nhóm: https://github.com/QuangNEU/K5-L3B-Day02-I3-DiscoveryProblemFraming

---
## 2. Scan problem (CP1)

Quang scan 5 problem, đạt mức tối thiểu 5.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận được tài liệu môn học hoặc requirement đồ án dài nhiều trang, tôi muốn có ngay một bản tóm tắt các ý chính và phần việc cần làm, để nắm bắt yêu cầu nhanh chóng mà không phải cày từng chữ | Bản thân tôi, Nhóm làm bài tập | Mất trung bình 45–60 phút để đọc hiểu một tài liệu môn học/công nghệ mới, tần suất 2–3 lần/tuần |
| 2 | Pain từ người khác | Khi các bạn trong nhóm cần tập trung cao độ để code hoặc làm đồ án, họ muốn hạn chế và chặn xao nhãng từ điện thoại, để không bị đứt mạch suy nghĩ và tránh kéo chậm tiến độ chung | Bạn học, Thành viên nhóm đồ án, Cả nhóm | 3/4 bạn trong nhóm liên tục than phiền trên nhóm chat vì mất 1.5–2 tiếng lướt mạng xã hội lúc học; 2 tuần gần nhất có 2 bạn trễ deadline task nhóm do mất tập trung |
| 3 | Lặp lại | Khi cần ôn tập lại thuật toán trước kỳ phỏng vấn, tôi muốn thống kê nhanh các dạng bài (DP, Graph, v.v.) hay làm sai hoặc tốn nhiều thời gian, để tối ưu việc luyện tập thay vì dò lại lịch sử giải bài từ đầu | Bản thân tôi | Tốn 30–45 phút mỗi cuối tuần lướt lại lịch sử submit trên LeetCode/HackerRank để tự note lại các bài cần làm lại |
| 4 | Tốn thời gian | Khi hệ thống báo lỗi liên quan đến luồng dữ liệu realtime, tôi muốn gom toàn bộ log từ backend (framework, database, cache) về một màn hình theo thứ tự thời gian, để tra cứu nguyên nhân chéo nhanh chóng thay vì mở từng tab terminal lẻ tẻ | Bản thân tôi, Team Backend | Mất trung bình 45–60 phút mò mẫm log mỗi khi fix bug liên quan đến đồng bộ dữ liệu; xảy ra 1–2 lần/tuần |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi kết thúc chuyến đi dài và nghe xong các podcast, tôi muốn có ngay các gạch đầu dòng từ khóa và kiến trúc cốt lõi vừa được nhắc tới, để lưu vào não và note cá nhân mà không phải tua lại audio để chép | Bản thân tôi | Dành 2–3 tiếng/ngày trên xe buýt nghe kỹ thuật nhưng thường quên khoảng 40% chi tiết nếu không mở máy tính ghi chép lại ngay lúc đó |

**AI gợi ý thêm:** Sau khi tự scan các ý đầu, Quang hỏi AI gợi ý qua 4 lăng kính và giữ lại ý #4 và #5. Bỏ qua các ý tưởng giải pháp AI quá rộng như "trợ lý học tập toàn năng" vì thiếu quy trình thật.

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tóm tắt tài liệu môn học / requirement (#1) | Quy trình rõ, tốn thời gian cày cuốc, impact trực tiếp tới việc học và tiến độ làm đồ án của nhóm | Chất lượng tóm tắt có đủ sâu không, sợ sót edge case |
| 2 | Gom log realtime tra cứu bug (#4) | Pain thật, tốn thời gian dò thủ công chéo các tab, lặp lại mỗi khi code backend | Có dễ truy cập và gom luồng log liên tục tự động không? Hay chỉ cần code Rule là đủ? |
| 3 | Tóm tắt kiến thức từ Podcast (#5) | Lặp lại hằng ngày (đi xe buýt 2-3 tiếng), dễ đo lường kết quả | AI có nhận diện và hiểu đúng các thuật ngữ chuyên ngành (System Design) không? |

---

### Problem Card #1 — Tóm tắt tài liệu môn học / requirement đồ án

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận được tài liệu môn học hoặc requirement đồ án dài nhiều trang, tôi muốn có ngay một bản tóm tắt các ý chính và phần việc cần làm, để nắm bắt yêu cầu nhanh chóng mà không phải cày từng chữ. |
| Actor | Sinh viên IT (Tôi) / Trưởng nhóm đồ án |
| Thời điểm / bối cảnh | Lúc bắt đầu sprint mới hoặc nhận đề bài môn học/đồ án mới (tài liệu dài 10-20 trang). |
| Quy trình hiện tại | 1. Tải tài liệu (PDF/Doc) · 2. Đọc lướt mục lục · 3. Đọc chi tiết từng phần · 4. Highlight & trích xuất yêu cầu · 5. Chia task cho nhóm |
| Bottleneck | Bước 3 và 4 (Đọc chi tiết và trích xuất yêu cầu): khoảng 45 phút, dễ mất tập trung và sót ý. |
| Impact | 60 phút/tài liệu; tuần có 2-3 tài liệu tốn khoảng 3 tiếng; các thành viên trong nhóm phải chờ đợi để hiểu đề bài. |
| Success metric | Tổng thời gian đọc và lọc task từ 60 phút xuống dưới 15 phút, số lượng task bị hiểu sai yêu cầu = 0. |
| Phương án không dùng AI | Dùng highlight PDF truyền thống hoặc xin giảng viên/người giao đề cung cấp checklist (rất khó vì giảng viên thường đưa tài liệu dài). Chưa giảm được thời gian tự đọc. |
| Giả thuyết về AI | Đưa tài liệu vào AI rút trích ý chính, action items. Tôi review, đối chiếu với bản gốc trước khi chia task. |
| Cảm nhận nhanh | Workflow |

**Quy trình nháp hiện tại — 60 phút:**
> [1 Tải tài liệu: 2'] → [2 Đọc lướt mục lục: 3'] → [3 Đọc chi tiết: 30'] ← BOTTLENECK 
> → [4 Highlight & lọc yêu cầu: 15'] ← BOTTLENECK 
> → [5 Chia task: 10']

**AI phản biện card #1:**
| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 45-60 phút áp dụng cho tài liệu dài bao nhiêu? | Đồng ý | Bổ sung định mức: "tài liệu dài 10-20 trang". |
| AI tóm tắt có thể bỏ sót yêu cầu kỹ thuật (edge cases). | Đồng ý | Thêm boundary: AI quét ý chính, tôi VẪN PHẢI kiểm tra lại trước khi chia task. |
| Nên làm Agent tự tạo ticket trên Jira luôn? | Không | Giữ bước "Tôi chia task" làm boundary để kiểm soát tiến độ, không giao AI. |

---

### Problem Card #2 — Gom log realtime tra cứu bug

| Trường | Nội dung |
|---|---|
| Job Story | Khi hệ thống báo lỗi liên quan đến luồng dữ liệu realtime, tôi muốn gom toàn bộ log từ backend (framework, database, cache) về một màn hình theo thứ tự thời gian, để tra cứu nguyên nhân chéo nhanh chóng thay vì mở từng tab terminal lẻ tẻ. |
| Actor | Dev Backend (Tôi) |
| Thời điểm / bối cảnh | Khi hệ thống báo lỗi trong quá trình dev/test các luồng dữ liệu đồng bộ (vd: gọi API có kết hợp DB và Redis). |
| Quy trình hiện tại | 1. Mở terminal API · 2. Mở log DB · 3. Mở log Cache/Redis · 4. Dò timestamp và so khớp sự kiện thủ công · 5. Xác định lỗi |
| Bottleneck | Bước 4 (Dò timestamp & so khớp sự kiện thủ công): khoảng 25 phút. |
| Impact | 45-60 phút mò mẫm log mỗi lần fix bug; xảy ra 1-2 lần/tuần, làm đứt mạch suy nghĩ khi code. |
| Success metric | Thời gian tra cứu và gom log từ 45 phút xuống dưới 10 phút/lần fix bug. |
| Phương án không dùng AI | Tự viết script bash gom log thủ công hoặc chia nhỏ màn hình terminal. Vẫn tốn sức nhìn bằng mắt thường. |
| Giả thuyết về AI | AI (hoặc script có AI) parse các file log, chuẩn hóa timestamp và highlight các điểm bất thường/lỗi chéo. Tôi tự xác định bug từ dữ liệu đã gom. |
| Cảm nhận nhanh | Rule / Workflow |

**Quy trình nháp hiện tại — 45 phút:**
> [1 Mở terminal API: 5'] → [2 Mở log DB: 5'] → [3 Mở log Redis: 5'] 
> → [4 Dò timestamp & so khớp: 25'] ← BOTTLENECK 
> → [5 Xác định dòng code lỗi: 5']

**AI phản biện card #2:**
| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chỉ cần dùng ELK stack hoặc Rule script là đủ gom log, nhảy sang AI quá sớm? | Đồng ý 1 phần | Rule làm tốt việc gom, nhưng AI sẽ mạnh ở bước "nhận diện điểm bất thường/lỗi logic" giữa các luồng. Sẽ xác định rõ ở CP6. |

---

### Problem Card #3 — Tóm tắt kiến thức từ Podcast

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc chuyến đi dài và nghe xong các podcast về System Design, tôi muốn có ngay các gạch đầu dòng từ khóa và kiến trúc cốt lõi vừa được nhắc tới, để lưu vào não và note cá nhân mà không phải tua lại audio để chép. |
| Actor | Sinh viên IT tự học (Tôi) |
| Thời điểm / bối cảnh | Về đến nhà sau chuyến đi xe buýt dài (2-3 tiếng) nghe podcast hoặc audiobook kỹ thuật. |
| Quy trình hiện tại | 1. Nghe podcast trên xe · 2. Về nhà mở máy tính/Notion · 3. Cố nhớ lại các ý chính · 4. Tua lại đoạn audio bị quên · 5. Gõ lại note |
| Bottleneck | Bước 3 và 4 (Nhớ lại và tua lại audio): tốn 25 phút, dễ quên 40% chi tiết quan trọng. |
| Impact | Lãng phí thời gian học trên xe do rơi rụng kiến thức; tốn thêm 30 phút mỗi ngày để chép lại note. |
| Success metric | Lưu lại được >90% keyword quan trọng; thời gian làm note giảm từ 30 phút xuống dưới 5 phút. |
| Phương án không dùng AI | Vừa nghe vừa gõ note trên điện thoại (gây say xe, mất an toàn). |
| Giả thuyết về AI | Cung cấp link/transcript podcast cho AI tóm tắt, hoặc tôi ghi âm bằng giọng nói các keyword nhớ được rồi AI tự đắp thịt thành bản note hoàn chỉnh. |
| Cảm nhận nhanh | Workflow |

**Quy trình nháp hiện tại — 32 phút (không tính thời gian nghe):**
> [1 Mở Notion: 2'] → [2 Cố nhớ lại ý: 10'] ← BOTTLENECK 
> → [3 Tua lại đoạn quên: 15'] ← BOTTLENECK 
> → [4 Gõ note: 5']

**AI phản biện card #3:**
| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI có thể hiểu sai hoặc dịch sai các thuật ngữ System Design chuyên sâu không? | Đồng ý | Thêm boundary: Phải sử dụng prompt ép AI giữ nguyên thuật ngữ tiếng Anh gốc, không tự ý dịch sang tiếng Việt. | 
# 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| **Pitch Problem Card** | Trình bày 3 ý tưởng cá nhân (Tóm tắt tài liệu đồ án, Gom log realtime, Tóm tắt podcast). | Mang đến các bài toán thực tế từ góc nhìn của sinh viên IT/Dev để nhóm có nhiều lựa chọn kỹ thuật. |
| **Phản biện bài của bạn khác** | Đặt câu hỏi cho bài xe buýt E03 của Minh: *"Lấy API đếm người real-time ở đâu ra để làm?"* | Giúp nhóm nhận diện ngay rủi ro cốt lõi về Tính khả thi (Feasibility) của dữ liệu. |
| **Nhận phản biện** | Minh hỏi bài Tóm tắt tài liệu của tôi: *"AI có bỏ sót các yêu cầu ẩn/edge case của đồ án không?"* | Tôi sửa lại Problem Card: Bổ sung boundary là AI chỉ quét ý chính, người dùng vẫn phải tự đọc đối chiếu để tránh sót requirement. |
| **Gom cluster / cây OST** | Tham gia phân loại 9 candidate thành 3 nhóm (Rút trích thông tin, So sánh/Quyết định, Phân loại dữ liệu). | Giúp nhóm nhìn ra bức tranh tổng thể để xây dựng Opportunity Solution Tree rõ ràng hơn. |
| **Chọn candidate problem** | Trực tiếp đánh giá điểm Feasibility và Impact cho các candidate, chốt chọn bài E03 của Minh. | Thống nhất hướng đi chung, gác lại bài toán cá nhân để làm một bài toán mang tính cộng đồng lớn hơn. |
| **Kiểm chứng / research** | Phân tích giải pháp kỹ thuật, đề xuất dùng dữ liệu thẻ từ (Tap-in) kết hợp ML thay vì đòi hỏi camera đếm người. | Giải quyết được rào cản lớn nhất của dự án, chứng minh tính khả thi của bài toán xe buýt. |
| **Quy trình nhóm** | Vẽ quy trình tương lai (Before/After), chỉ rõ điểm AI can thiệp vào hành trình người dùng. | Làm rõ được nút thắt (bottleneck) cũ đã được xóa bỏ như thế nào nhờ hệ thống cảnh báo màu. |
| **Problem Statement** | Cập nhật v1, đổi Success Metric sang độ chính xác của AI và định hình rõ Boundary. | Định hình rõ ranh giới: AI chỉ gợi ý mức độ đông, không ép người dùng đổi lộ trình. |
| **Mức can thiệp AI** | Xây dựng AI Canvas, lập bảng so sánh 4 mức độ AI và trả lời 2 câu hỏi PAIR. | Chốt được mức Workflow vì lý giải được tại sao Rule cứng không xử lý được việc khách xuống xe không quẹt thẻ. |
| **Quyết định** | Đánh giá 4 rủi ro, đề xuất dùng Mock Data để chạy Pilot. | Chốt quyết định "Go" với phương án an toàn, vừa sức với một môn học. |

---

# 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| **CP1 Scan** | Nhờ gợi ý thêm vấn đề qua 4 lăng kính cho sinh viên IT. | Khơi gợi được ý tưởng về việc gom log realtime và nghe podcast. | Đề xuất giải pháp quá rộng kiểu "trợ lý học tập toàn năng". | Bỏ qua các ý chung chung, bắt ép AI viết theo định dạng Job Story cho một task cụ thể. |
| **CP2 Problem Card** | Đóng vai PM khó tính để phản biện các card cá nhân. | Chỉ ra rằng baseline 45-60 phút chưa rõ ràng (cho tài liệu dài bao nhiêu). | Xui tôi làm Agent tự động chia task/tạo ticket lên Jira thay cho trưởng nhóm. | Bác bỏ ý AI, giữ lại bước "tự chia task" làm boundary để PM kiểm soát được thực tế. |
| **CP4 Research** | Tìm hiểu cách thế giới giải quyết bài toán đếm khách xe buýt. | Gợi ý ý tưởng dùng Machine Learning kết hợp dữ liệu quét thẻ. | AI đưa ra pattern của nước ngoài (tap-in/tap-out chuẩn chỉnh), không khớp hành vi ở Việt Nam (không tap-out). | Đưa thêm giả định/rule: Dùng ML nội suy số người xuống xe tại các trạm lớn dựa trên lịch sử thay vì đợi tap-out. |
| **CP5 Quy trình** | Hỗ trợ chuyển mô tả bằng lời sang dạng step-by-step. | Trình bày luồng Before/After nhanh và trực quan. | Gộp chung bước AI dự đoán và bước người dùng ra quyết định làm một. | Tách bạch rõ: AI chỉ dừng ở việc "hiển thị màu", con người là người chốt "lên xe hay ở lại". |
| **CP5–6 Problem Statement** | Hoàn thiện cấu trúc bảng và chuẩn hóa wording. | Viết ngắn gọn, súc tích đúng ngôn ngữ Product. | Đưa Success Metric là "Giảm thời gian chờ xe". | Đổi Metric thành "Độ chính xác của thuật toán >80%", vì chờ xe vắng có khi lâu hơn chờ xe đông. |
| **CP6 Mức can thiệp / quyết định** | Lập bảng so sánh 4 mức (No AI, Rule, Workflow, Agent). | Lập luận rất chặt chẽ việc tại sao Rule (cộng trừ đơn thuần) thất bại. | Ở mức Agent, AI gợi ý hệ thống tự động book xe Grab cho sinh viên nếu buýt quá đông. | Gạch bỏ ngay lập tức vì phi thực tế về chi phí, nằm ngoài khả năng của một sinh viên/app buýt. |

---

# 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi nhận ra rằng một "vấn đề tốt" không nhất thiết phải là một vấn đề công nghệ đao to búa lớn. Ban đầu tôi chỉ chăm chăm vào năng suất cá nhân (đọc tài liệu, code, log), nhưng khi nghe bài xe buýt E03 của Minh, tôi hiểu ra những vấn đề có impact cộng đồng cao, đụng chạm đến nỗi đau thường nhật của hàng ngàn sinh viên mới là "mỏ vàng" thực sự để làm Product.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Lúc mới chọn bài E03, cả nhóm lập tức bàn nhau: *"Hay là mình lắp camera AI trên cửa xe để đếm đầu người?"*. Đây là điển hình của solution-first. Nhóm nhận ra sai lầm khi bắt đầu phân tích rủi ro Feasibility: chúng ta không có tiền và quyền để lắp camera lên xe của VinBus. Nhóm lùi lại, nhìn vào lõi vấn đề là "cần biết độ đông", và chuyển hướng sang tận dụng dữ liệu quẹt thẻ sẵn có kết hợp Machine Learning.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi đã thay đổi hoàn toàn quyết định chọn đề tài của mình. Lúc đầu, tôi khăng khăng bảo vệ ý tưởng "Tóm tắt tài liệu môn học" vì thấy nó dễ làm, an toàn và quy trình cực kỳ rõ ràng. Nhưng khi Minh phản biện rằng: *"Bài đó hay nhưng hơi cá nhân, nếu làm bài E03 thì khảo sát được sinh viên"*, tôi đã suy nghĩ lại. Cuối cùng, tôi nhượng bộ và đồng ý chốt bài E03 vì giá trị thực tiễn của nó thuyết phục hơn hẳn.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất khi phỏng vấn là sự đánh đổi của sinh viên. Tôi luôn nghĩ "sợ muộn học/sợ bị điểm danh" là nỗi sợ lớn nhất. Tuy nhiên, 3/4 người được hỏi thú nhận rằng thà đi muộn 10 phút còn hơn nhét lên chuyến E03 đông đúc, vì *"lên trường mệt lả cũng không học nổi"*. Insight này chứng minh việc cung cấp thông tin để họ lùi chuyến là thực sự có giá trị.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Đó là việc xác định Success Metric (Chỉ số thành công) sao cho đúng. Lúc đầu nhóm đo bằng "thời gian chờ giảm đi". Nhưng thực tế, nếu quyết định chờ chuyến sau cho vắng, thời gian chờ lại *tăng lên*. Cuối cùng tôi nhận ra, giá trị lõi hệ thống mang lại là "thông tin đúng", nên metric phải là độ chính xác của dự đoán AI >80% so với thực tế, và sự hài lòng của người dùng vì làm chủ được thời gian.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ phản biện mạnh hơn ở khâu thu thập dữ liệu kiểm chứng. Việc phỏng vấn 4 người hơi ít để kết luận đại trà. Tôi cũng sẽ muốn nhóm thiết kế một form khảo sát gửi lên group sinh viên trường để có định lượng rõ ràng hơn về tỉ lệ phần trăm các bạn sẵn sàng "bỏ chuyến đông chờ chuyến vắng".

**6.7. Hiểu bài:**
Bài toán của nhóm là sinh viên thường xuyên bị nhồi nhét trên tuyến buýt E03 do không biết trước mức độ đông đúc để quyết định đi hay chờ. Quy trình tương lai can thiệp AI bằng cách lấy log quẹt thẻ, dùng Machine Learning dự đoán độ đông và hiển thị màu cảnh báo trên app. Metric thành công được xác định bằng độ chính xác của dự đoán (>80%) và đánh giá từ người dùng. Boundary cốt lõi là AI chỉ cung cấp thông tin, quyền quyết định bước lên xe hay không hoàn toàn thuộc về con người. Do độ phức tạp của bài toán đếm người (nhiều biến số ngầm) nhưng đầu ra rõ ràng (nhãn màu), nhóm chọn mức can thiệp Workflow. Cuối cùng, nhóm quyết định Go bằng cách triển khai một bản Pilot sử dụng dữ liệu giả lập (Mock Data) riêng cho tuyến E03 để chứng minh thuật toán.

---

# 7. Tài liệu tham khảo
- Tài liệu học phần *Discovery & Problem Framing* (Slide bài giảng).
- Google Maps Help - Cơ chế hoạt động của tính năng Transit Crowding.
- Các nghiên cứu về *Alighting Estimation for Smart Card Data* (Dùng ML dự đoán khách xuống xe).