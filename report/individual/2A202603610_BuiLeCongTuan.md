# Báo cáo cá nhân — 2A202603610_BuiLeCongTuan


## 1. Thông tin học viên

- Họ tên: Bùi Lê Công Tuấn
- MSSV: 2A202603610
- Email trường:
- Tên nhóm: Phượng Hoàng
- Link repo nhóm: https://github.com/MHuyHoat/K5--L3A--DAY02-PhuongHoang-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi nhận bài tập mới, tôi muốn tìm nhanh toàn bộ tài liệu liên quan để bắt đầu làm bài ngay | Sinh viên | Ước tính mất khoảng 15–20 phút để tìm LMS, GitHub, notebook và tài liệu; cần bấm giờ thêm để xác nhận |
| 2 | Lặp lại | Khi có nhiều bài tập cùng lúc, tôi muốn theo dõi deadline tập trung để không bỏ sót | Sinh viên | Phải kiểm tra deadline ở LMS, Discord và GitHub nhiều lần mỗi tuần |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi làm báo cáo môn học, tôi muốn tổng hợp nội dung nhanh để hoàn thành đúng hạn | Sinh viên | Mỗi báo cáo mất khoảng 1–2 giờ để tổng hợp và định dạng |
| 4 | Pain từ người khác | Khi làm việc nhóm, tôi muốn biết từng thành viên đang làm gì để tránh trùng lặp công việc | Thành viên nhóm | Thường phải nhắn tin hỏi tiến độ nhiều lần |
| 5 | Tốn thời gian | Khi cần sử dụng lại API key hoặc tài khoản đã tạo, tôi muốn tìm lại nhanh để tiếp tục công việc | Sinh viên học AI | Có lúc mất 5–10 phút tìm email hoặc API key |
| 6 | Lặp lại | Khi ghi chép chi tiêu, tôi muốn lưu nhanh các khoản chi để quản lý tài chính cá nhân | Sinh viên | Thường quên ghi chép sau vài ngày |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi học nhiều môn cùng lúc, tôi muốn biết tiến độ từng môn để phân bổ thời gian hợp lý | Sinh viên | Khó xác định môn nào đang bị chậm |
| 8 | Pain từ người khác | Khi tìm phòng trọ, tôi muốn kiểm tra nhanh độ tin cậy của thông tin để tránh mất thời gian | Sinh viên | Nhiều bài đăng thiếu hoặc sai thông tin |

**Nếu có dùng AI để gợi ý thêm:**

- Tôi dùng AI để brainstorm thêm các vấn đề thường gặp của sinh viên. Tôi giữ lại các vấn đề mà bản thân hoặc bạn bè từng gặp như tìm tài liệu học tập, theo dõi deadline và làm việc nhóm. Tôi bỏ các ý quá chung chung hoặc chưa có trải nghiệm thực tế vì chưa có bằng chứng để kiểm chứng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Khó tìm tài liệu học tập | Tôi gặp thường xuyên, quy trình rõ và có thể đo bằng thời gian | Mức độ ảnh hưởng với các sinh viên khác; baseline hiện mới là ước tính |
| 2 | Bỏ sót deadline bài tập | Xảy ra lặp lại trong quá trình học và có hậu quả trực tiếp | Tần suất thực tế của các sinh viên khác |
| 3 | Làm việc nhóm khó theo dõi tiến độ | Gây chậm tiến độ và dễ trùng công việc | No AI như bảng phân công có thể đã giải quyết phần lớn vấn đề hay chưa |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận bài tập mới, tôi muốn tìm nhanh toàn bộ tài liệu liên quan để có thể bắt đầu làm bài ngay |
| Actor | Sinh viên K5 AI Foundation |
| Thời điểm / bối cảnh | Khi bắt đầu một buổi học hoặc bài lab mới |
| Quy trình hiện tại (3–7 bước) | 1. Nhận bài tập → 2. Mở LMS → 3. Tìm GitHub → 4. Tìm notebook → 5. Đọc tài liệu → 6. Bắt đầu làm bài |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước tìm LMS, GitHub và notebook; ước tính khoảng 15–20 phút mỗi buổi lab |
| Impact (nếu không giải thì sao) | Giảm thời gian học và thực hành; nếu có 4 buổi/tuần thì có thể mất khoảng 60–80 phút/tuần chỉ để tìm tài liệu |
| Success metric (baseline → target) | Baseline tạm tính: khoảng 20 phút/lần → Target: dưới 5 phút/lần; đo bằng bấm giờ trước và sau khi thử giải pháp |
| Phương án không dùng AI | Tạo một trang tổng hợp tài liệu theo từng buổi học, có quy tắc đặt tên và link cố định |
| Giả thuyết về AI (nếu có) | AI có thể hỗ trợ tìm kiếm, lọc và tổng hợp tài liệu từ nhiều nguồn |
| Cảm nhận nhanh | Chưa biết; No AI hoặc Rule có thể đã đủ, cần kiểm chứng trước |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ước tính khoảng 20 phút

[Nhận bài tập]
→ [Mở LMS: 3']
→ [Tìm repo GitHub: 5']
→ [Tìm notebook/tài liệu hướng dẫn: 7'] ← BOTTLENECK
→ [Đọc yêu cầu: 3']
→ [Bắt đầu làm bài: 2']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhiều bài tập cùng lúc, tôi muốn theo dõi deadline tập trung để không bỏ sót bài nộp |
| Actor | Sinh viên |
| Thời điểm / bối cảnh | Khi học nhiều môn và nhận thông báo từ nhiều kênh |
| Quy trình hiện tại (3–7 bước) | 1. Nhận thông báo → 2. Ghi nhớ hoặc lưu lại → 3. Kiểm tra nhiều nguồn → 4. Làm bài → 5. Nộp bài |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước kiểm tra lại deadline ở LMS, GitHub, Discord và nhóm chat; diễn ra nhiều lần mỗi tuần |
| Impact (nếu không giải thì sao) | Có nguy cơ quên bài, nộp muộn hoặc phải hỏi lại deadline |
| Success metric (baseline → target) | Baseline tạm tính: 2–3 lần quên hoặc hỏi lại/tháng → Target: 0 lần/tháng |
| Phương án không dùng AI | Dùng Google Calendar hoặc Microsoft To Do làm nơi lưu deadline tập trung |
| Giả thuyết về AI (nếu có) | AI có thể trích xuất deadline từ thông báo và gợi ý lịch nhắc |
| Cảm nhận nhanh | Rule có thể đủ; chưa chắc cần AI |

Quy trình nháp hiện tại:

```text
[Nhận thông báo]
→ [Ghi nhớ hoặc lưu lại]
→ [Kiểm tra deadline ở nhiều nguồn] ← BOTTLENECK
→ [Làm bài]
→ [Nộp bài]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm việc nhóm, tôi muốn biết từng thành viên đang làm gì và hạn hoàn thành là khi nào để tránh trùng lặp hoặc chậm tiến độ |
| Actor | Thành viên nhóm và nhóm trưởng |
| Thời điểm / bối cảnh | Trong quá trình thực hiện bài tập nhóm |
| Quy trình hiện tại (3–7 bước) | 1. Chia việc trong nhóm chat → 2. Mỗi người làm phần riêng → 3. Hỏi tiến độ → 4. Tổng hợp → 5. Kiểm tra và nộp |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước hỏi và cập nhật tiến độ; thông tin phân công dễ bị trôi trong chat |
| Impact (nếu không giải thì sao) | Dễ trùng công việc, bỏ sót nhiệm vụ hoặc chậm deadline chung |
| Success metric (baseline → target) | Baseline: phải hỏi tiến độ nhiều lần mỗi tuần → Target: dưới 2 lần/tuần |
| Phương án không dùng AI | Dùng Trello, Notion, GitHub Projects hoặc Google Sheets làm bảng phân công chung |
| Giả thuyết về AI (nếu có) | AI có thể trích xuất nhiệm vụ và tổng hợp trạng thái từ nội dung trao đổi |
| Cảm nhận nhanh | No AI hoặc Rule có thể đủ |

Quy trình nháp hiện tại:

```text
[Chia việc trong nhóm chat]
→ [Thành viên làm phần riêng]
→ [Thông tin phân công bị trôi]
→ [Hỏi lại tiến độ/deadline] ← BOTTLENECK
→ [Tổng hợp kết quả]
→ [Nộp bài]
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Đây là vấn đề tôi gặp thường xuyên, có quy trình rõ, có thể đo bằng thời gian và dễ kiểm chứng với sinh viên khác.
- Câu hỏi muốn nhóm phản biện: Vấn đề này có thực sự đủ lớn để giải quyết không, hay chỉ cần tổ chức tài liệu tốt hơn là đủ?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline thời gian mới dựa trên ước tính cá nhân | Đồng ý | Ghi rõ đây là baseline tạm và cần bấm giờ thực tế |
| Có thể chỉ cần tổ chức tài liệu, không cần AI | Đồng ý | Bổ sung phương án No AI và đổi cảm nhận nhanh thành “Chưa biết” |
| Chưa có bằng chứng từ sinh viên khác | Đồng ý | Đưa vào danh sách giả định cần kiểm chứng |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày bài toán khó tìm tài liệu học tập và hướng dẫn lab | Đóng góp một candidate để nhóm so sánh |
| Phản biện bài của bạn khác | Đặt câu hỏi: “Dữ liệu giao dịch có được ghi nhận đầy đủ không? Nếu dữ liệu chưa có thì AI sẽ dựa vào đâu để trả lời?” | Giúp nhóm nhận ra chất lượng dữ liệu là giả định quan trọng của đề tài được chọn |
| Nhận phản biện | Nhận câu hỏi: “Việc tìm tài liệu có cần công cụ mới hay chỉ cần tổ chức lại?” | Bổ sung phương án No AI và không kết luận Workflow quá sớm |
| Gom cluster / cây OST | Tham gia gom các candidate thành nhóm tìm kiếm thông tin, quản lý công việc và quản lý dữ liệu kinh doanh | Giúp nhóm nhìn thấy pattern chung và thu hẹp shortlist |
| Chọn candidate problem | Đồng ý chọn bài toán quản lý hàng hóa và giao dịch bán hàng tại cửa hàng điện tử của gia đình Nguyễn Vũ Thành Long | Nhóm có một candidate thực tế, có actor và quy trình rõ để tiếp tục |
| Kiểm chứng / research | Góp ý câu hỏi phỏng vấn về lần tra cứu gần nhất, thời gian tra cứu, sai lệch tồn kho và cách ghi chép hiện tại | Hướng CP4 tập trung vào hành vi đã xảy ra thay vì hỏi người dùng có thích AI không |
| Quy trình nhóm | Phụ trách xây dựng quy trình hiện tại, quy trình tương lai và bảng Before/After | Hoàn thiện phần CP5 của `group_report.md` |
| Problem Statement | Góp ý Actor, Quy trình, Bottleneck, Impact, Success Metric và Boundary | Hoàn thiện Problem Statement v0, nhấn mạnh gốc rễ là dữ liệu chưa đầy đủ |
| Mức can thiệp AI | Đề xuất ưu tiên biểu mẫu chuẩn và Rule cập nhật tồn kho trước khi cân nhắc AI | Giúp nhóm tránh solution-first |
| Quyết định | Đề xuất quyết định tạm thời **Not Yet đối với AI**, nhưng **Go cho pilot No AI/Rule** | Nhóm có hướng thử nghiệm nhỏ, ít rủi ro và đo được |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Brainstorm thêm vấn đề theo 4 lăng kính | Giúp mở rộng danh sách và chuẩn hóa Job Story | Một số ý quá chung hoặc không có bằng chứng | Chỉ giữ vấn đề có trải nghiệm thực tế; ghi rõ số nào mới là ước tính |
| CP2 Problem Card | Cấu trúc hóa actor, quy trình, bottleneck và metric | Giúp card dễ so sánh và phản biện | Ban đầu kết luận Workflow quá sớm | Đổi thành Chưa biết/No AI/Rule có thể đủ |
| CP4 Research | Gợi ý Assumption Map và câu hỏi The Mom Test | Giúp tập trung vào hành vi đã xảy ra | Có xu hướng đề xuất chatbot quản lý kho trước khi đủ dữ liệu | Bỏ solution sớm, ưu tiên kiểm tra dữ liệu giao dịch và tồn kho |
| CP5 Quy trình | Chuyển mô tả thành quy trình hiện tại/tương lai và bảng Before/After | Giúp nhìn rõ handoff, bước thủ công và boundary | AI đưa ra thời gian chưa được đo thực tế | Ghi các mốc là ước lượng, yêu cầu thay bằng dữ liệu CP4 |
| CP5–6 Problem Statement | Rà soát 6 trường của v0 và phần mở rộng của v1 | Chỉ ra gốc rễ có thể là dữ liệu chưa được ghi đủ | Có lúc lẫn giải pháp “hệ thống AI” vào Problem Statement | Loại tên công cụ và AI khỏi phần mô tả vấn đề |
| CP6 Mức can thiệp / quyết định | So sánh No AI, Rule, Workflow và Agent | Giúp thấy Rule giải quyết phần lớn bài toán nhập liệu và tồn kho | AI thường đề xuất Workflow khi chưa đủ dữ liệu | Chọn Not Yet cho AI; chỉ pilot No AI/Rule trước |

---

## 6. Reflection (CP7)


### 6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?

Khi nghe các thành viên trình bày top 3 problems, tôi nhận ra một problem mạnh không cần phải có công nghệ phức tạp. Những đề tài như quản lý hàng hóa, tìm phòng, sửa CV, điểm danh hay tra cứu tài liệu kỹ thuật đều mạnh hơn khi actor cụ thể, quy trình thật và bottleneck đo được. Tôi cũng thấy các bạn có domain thực tế thường mô tả tác động rõ hơn, nhưng một bài có impact lớn chưa chắc phù hợp nếu nhóm không tiếp cận được người dùng hoặc dữ liệu. Điều này giúp tôi hiểu rằng nhóm phải cân bằng giữa giá trị của vấn đề, khả năng kiểm chứng và phạm vi của buổi lab.

### 6.2. Nhóm có lúc nào bị “solution-first” không? Lúc đó nhóm nhận ra và xử lý thế nào?

Có. Khi nghe bài toán quản lý hàng hóa, nhóm dễ nghĩ ngay đến chatbot hoặc AI tra cứu tồn kho. Sau khi phân tích, nhóm nhận ra dữ liệu nhập, xuất và giá bán hiện chưa được ghi nhận đầy đủ. Nếu dữ liệu gốc thiếu thì AI không thể trả lời chính xác. Nhóm quay lại quy trình, tách cơ hội khỏi giải pháp và ưu tiên biểu mẫu chuẩn, trường bắt buộc cùng Rule tự cộng trừ tồn kho. AI chỉ được xem là bước tùy chọn sau khi dữ liệu đủ tin cậy.

### 6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.

Tôi có đổi ý về chính Problem Card của mình. Ban đầu tôi ghi cảm nhận nhanh là Workflow vì nghĩ AI có thể tìm và tổng hợp tài liệu. Sau phản biện “chỉ cần gom link vào một nơi có đủ không?”, tôi thấy No AI hoặc Rule có thể giải quyết phần lớn vấn đề. Tôi sửa card bằng cách thêm phương án trang tổng hợp tài liệu, đổi mức can thiệp thành “Chưa biết” và ghi rõ cần đo thời gian thật trước khi kết luận.

### 6.4. Kết quả kiểm chứng có làm tôi bất ngờ không? Điều gì?

Điều đáng chú ý nhất là vấn đề của cửa hàng không bắt đầu từ khả năng tìm kiếm thông minh mà từ việc giao dịch chưa được ghi đầy đủ và thống nhất. Điều này làm thay đổi hướng giải quyết: thay vì xây AI trả lời câu hỏi về tồn kho, nhóm cần cải thiện dữ liệu đầu vào trước. Tôi hiểu rằng một kết quả kiểm chứng phản bác giả định ban đầu vẫn có giá trị, vì nó giúp nhóm tránh xây một giải pháp phức tạp trên nền dữ liệu yếu. Phần này cần được cập nhật thêm bằng số liệu phỏng vấn thật trong báo cáo nhóm.

### 6.5. Điều khó nhất khi viết Problem Statement là gì?

Điều khó nhất là giữ Problem Statement không chứa giải pháp, đồng thời metric vẫn đủ cụ thể. Khi viết, tôi thường muốn đưa ngay Google Sheets, phần mềm kho hoặc AI vào nội dung. Tuy nhiên Problem Statement chỉ nên mô tả actor, quy trình, bottleneck, impact, success metric và boundary. Một khó khăn khác là không biến số liệu ước tính thành sự thật. Vì vậy tôi ghi rõ baseline nào là tạm tính và cách sẽ đo lại trong pilot.

### 6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?

Nếu làm lại, tôi sẽ bấm giờ và ghi ví dụ thật ngay từ CP1 thay vì dựa vào trí nhớ. Trong phần nhóm, tôi sẽ yêu cầu phân biệt rõ ba vấn đề: dữ liệu không được ghi, dữ liệu ghi sai và dữ liệu có nhưng khó tìm. Ba trường hợp này dẫn đến ba hướng giải quyết khác nhau. Tôi cũng sẽ phản biện mạnh hơn khi nhóm đưa ra target chưa có baseline, hoặc khi gọi một tính năng là AI dù Rule đã đủ. Cuối cùng, tôi sẽ yêu cầu mọi claim quan trọng có nguồn hoặc được đánh dấu là giả định.

### 6.7. Hiểu bài

Bài nhóm bắt đầu từ problem quản lý hàng hóa và giao dịch chưa hiệu quả tại một cửa hàng điện tử. Nhóm vẽ quy trình hiện tại để thấy bottleneck nằm ở việc tìm, đối chiếu sổ sách và kiểm hàng thực tế. Metric cần đo là thời gian tra cứu, số lần phải kiểm kê lại và mức sai lệch tồn kho. Boundary là hệ thống hoặc AI không được tự sửa giao dịch, tồn kho hay giá bán nếu chưa có người quản lý xác nhận. Vì dữ liệu đầu vào chưa đầy đủ, nhóm ưu tiên No AI/Rule để chuẩn hóa nhập liệu và tự động cộng trừ tồn kho. Quyết định tạm thời là Not Yet đối với AI, nhưng Go cho một pilot nhỏ bằng biểu mẫu chuẩn và bảng dữ liệu tập trung. Sau pilot, nếu dữ liệu đủ và nhu cầu hỏi bằng ngôn ngữ tự nhiên vẫn có giá trị, nhóm mới cân nhắc Workflow có AI.

---

## 7. Tài liệu tham khảo

- `RULES.md`
- `CHECKPOINTS.md`
- `docs/01-worksheet.md`
- `docs/02-deliverable-example.md`
- `docs/03-international-frameworks.md`
- `report/team/group_report.md`
- Microsoft Copilot / ChatGPT, dùng để brainstorming, phản biện Problem Card, mô tả quy trình và so sánh mức can thiệp
- Trải nghiệm cá nhân trong quá trình học tập và làm việc nhóm
- Trao đổi, phản biện và kết quả làm việc của nhóm Phượng Hoàng