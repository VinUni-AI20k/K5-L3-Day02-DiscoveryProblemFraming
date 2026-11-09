# Báo cáo cá nhân — 2A202603418_TranThanhTung

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Thanh Tùng
- MSSV: 2A202603418
- Email trường: 26ai.tungtt@vinuni.edu.vn
- Tên nhóm: AZEZ
- Link repo nhóm: https://github.com/hhuydaugg/K5-L3A-DAY02-AZEZ-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị nộp bài lab lúc 23h, tôi muốn tự đối chiếu cấu trúc các file báo cáo và tên branch với rubric checklist, để không bị trừ điểm vì sai quy cách nộp bài | Sinh viên làm bài lab thực hành công nghệ (bản thân tôi và các bạn trong nhóm) | Tự bấm giờ 2 lần nộp lab gần nhất: mất 21 phút và 25 phút ngồi mở qua lại 3 file markdown để soát; đợt trước nhóm từng bị trừ điểm do quên xóa file template mẫu |
| 2 | Lặp lại | Khi bắt đầu tuần học mới, tôi muốn gom các hạn nộp bài tập lớn từ nhiều kênh thông báo (LMS, Discord môn học, Zalo nhóm) vào một lịch thống nhất, để không bị trễ deadline đột xuất | Sinh viên đang học 4–5 môn chuyên ngành song song | Sáng Chủ nhật nào cũng mất 30–35 phút lội tin nhắn ở 4 nhóm Zalo và 2 server Discord; tuần trước suýt bỏ lỡ 1 bài quiz 15 phút mở trên LMS do trôi thông báo |
| 3 | Tốn thời gian | Khi cần trích xuất thông số kỹ thuật và phương pháp đánh giá từ tài liệu nghiên cứu/paper dài 15–20 trang tiếng Anh, tôi muốn có bảng tóm tắt so sánh phương pháp, để chọn hướng làm bài tập lớn kịp buổi thảo luận nhóm | Sinh viên làm đồ án, thành viên nhóm phụ trách đọc lý thuyết | Mỗi bài paper mất từ 60 đến 90 phút ngồi dịch và note lại; mỗi đồ án phải đọc 4–5 bài nên đợt làm đề cương vừa rồi nhóm bị trễ hạn nộp 2 ngày |
| 4 | Tốn thời gian | Khi gặp lỗi xung đột môi trường ảo (CUDA/PyTorch hoặc thư viện pip) trước giờ chạy code, tôi muốn tra nhanh nguyên nhân không tương thích giữa driver và thư viện, để máy chạy được code mẫu mà không phải cài lại từ đầu | Sinh viên thực hành mô hình học máy trên máy cá nhân và máy lab trường | Ghi chép thực tế 2 lần cài máy gần nhất: 1 lần mất 80 phút mò StackOverflow, 1 lần mất gần 2 tiếng do cài nhầm bản CUDA toolkit không khớp với cuDNN |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận đề tài mở từ giảng viên kèm rubric chấm điểm dài nhiều trang, tôi muốn phân rã đề bài thành danh sách task cụ thể kèm mức độ ưu tiên, để phân công thành viên trong nhóm không bị trùng việc hay bỏ sót tiêu chí | Các thành viên trong nhóm làm bài tập lớn (3–4 người) | Buổi họp chia task đầu kỳ kéo dài hơn 2 tiếng vẫn chưa thống nhất xong; kỳ trước nhóm từng bị tình trạng 2 bạn cùng làm phần khảo sát do đọc lướt rubric |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi cần tổng hợp ghi chú từ buổi họp nhóm kéo dài 1 tiếng (nhiều ý kiến ngắt quãng và chatbox rời rạc), tôi muốn có danh sách quyết định cuối cùng kèm người phụ trách, để cả nhóm thống nhất hành động sau cuộc họp | Thư ký cuộc họp và các thành viên trong nhóm đồ án | Sau mỗi buổi họp online mất 30–40 phút ngồi nghe lại đoạn record hoặc đọc chatbox để gõ biên bản; nhóm vẫn hay phải nhắn tin hỏi lại "task này ai chốt làm" |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi gặp lỗi ngoại lệ (exception) trong file log lớn, tôi muốn xác định chính xác dòng dữ liệu gây lỗi và ngữ cảnh biến số, để sửa đúng chỗ mà không phải in log thủ công hàng nghìn dòng | Sinh viên làm bài lab thực hành xử lý dữ liệu | Trung bình mất 40–45 phút mỗi lần lần vết lỗi từ file log server hơn 10.000 dòng; tuần trước phải nhờ bạn cùng lớp soi hộ mới tìm ra giá trị bị null ở dòng 4.200 |
| 8 | Pain từ người khác | Khi gửi bản nháp báo cáo tiến độ cho giảng viên hướng dẫn, tôi muốn nhận được phản hồi định hướng vào đúng các mục trọng tâm, để sửa bài đúng ý mà không phải chờ đến buổi gặp trực tiếp | Giảng viên hướng dẫn (ngại đọc bản nháp dài dòng) và sinh viên làm đồ án | Thầy hướng dẫn nhận xét thẳng là 2 bản nháp trước viết lan man khó theo dõi, thầy phải hẹn gặp trực tiếp 45 phút để nắn lại cấu trúc |
| 9 | Pain từ người khác | Khi người dùng gửi phản hồi lỗi giao diện hoặc tính năng qua form khảo sát tự do, người làm sản phẩm muốn gom nhóm nhanh các phản ánh cùng lỗi, để ưu tiên sửa lỗi gây ức chế nhất trước | Sinh viên phụ trách sản phẩm/testing trong dự án môn học | Đợt thử nghiệm nội bộ vừa rồi thu về 42 câu trả lời ngắn, tôi phải ngồi đọc từng dòng trên Google Sheets mất hơn 2 tiếng mới gom cụm được các lỗi giao diện |
| 10 | Pain từ người khác | Khi tài xế xe taxi điện báo sự cố cạn pin khẩn cấp (< 5%) trên đường, điều phối viên muốn có ngay danh sách trạm sạc khả dụng gần nhất kèm chỉ dẫn an toàn, để hướng dẫn tài xế kịp thời tránh xe chết máy giữa đường | Điều phối viên tổng đài nội bộ và tài xế taxi điện | Số liệu thực tế từ phỏng vấn anh N. (điều phối viên vận hành GSM): mỗi ca mất 12–15 phút xử lý thủ công (tra bản đồ, đo km, gõ tin nhắn); ca cao điểm gặp 3–4 ca khẩn cấp. Khớp với chính sách cứu hộ xe hết pin của VinFast ([VinFast Cứu hộ 24/7](https://vinfastauto.com/vn_vi/dich-vu-cuu-ho-xe-dien-vinfast-247)) và áp lực trạm sạc theo chính sách V-Green ([vgreen.net](https://vgreen.net)) |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Tôi tự nghĩ ra 8 ý đầu từ trải nghiệm học tập và làm đồ án hàng tuần của mình. Sau đó tôi hỏi AI để gợi ý thêm bài toán ở góc nhìn "Pain từ người khác". Tôi giữ lại ý #9 (gom feedback người dùng) và ý #10 (điều phối cứu hộ sạc pin taxi điện) vì đây là những bài toán tôi từng gặp trong dự án môn học và có bạn bè/người quen làm thực tế chia sẻ số liệu đo lường cụ thể.
- **Ý bỏ qua:** Tôi loại bỏ 2 gợi ý của AI là "Hệ thống AI tự động sinh slide thuyết trình môn học" (quá chung chung, nội dung thường sáo rỗng không dùng được) và "Chatbot trả lời thay toàn bộ thắc mắc sinh viên" (phạm vi quá rộng, không kiểm soát được nguồn dữ liệu và dễ bị ảo giác).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Hỗ trợ điều phối viên tra cứu trạm sạc và gửi chỉ dẫn an toàn khi xe taxi điện cạn pin khẩn cấp (< 5%) (#10) | Vấn đề vận hành thực tế rất rõ ràng, ảnh hưởng trực tiếp đến xe và an toàn giao thông; thời gian xử lý thủ công đang quá lâu (14–17 phút); phân định rõ phần nào làm bằng công thức/rule và phần nào cần AI hỗ trợ soạn tin | Dữ liệu số trụ sạc còn trống trên hệ thống trạm sạc có độ trễ không (nếu trạm báo còn chỗ nhưng xe đến nơi thì vừa kín) |
| 2 | Tự đối chiếu cấu trúc file nộp bài lab và checklist rubric trước hạn nộp 23h59 (#1) | Trải nghiệm thật của chính tôi tuần nào cũng gặp; giảm hẳn nỗi lo bị trừ điểm oan do sai sót tên file hay thiếu folder | Phần lớn việc kiểm tra tên file, folder chỉ cần viết script regex là đủ, chưa chắc đã cần dùng đến AI |
| 3 | Tổng hợp biên bản thảo luận và danh sách việc cần làm sau buổi họp nhóm đồ án kéo dài 1 tiếng (#6) | Tuần nào nhóm cũng họp và đều mất thời gian ngồi gõ lại biên bản; dễ xảy ra tranh cãi do nhớ nhầm việc | Khi các bạn trong nhóm nói chèn nhau hoặc chat tiếng Việt viết tắt thì trích xuất danh sách việc có chính xác không |

---

### Problem Card #1 — Xử lý sự cố taxi điện cạn pin khẩn cấp (Card ưu tiên số 1)

| Trường | Nội dung |
|---|---|
| Job Story | Khi tài xế xe taxi điện báo sự cố cạn pin khẩn cấp (< 5%) trên đường, điều phối viên muốn có ngay danh sách trạm sạc khả dụng gần nhất kèm chỉ dẫn an toàn, để hướng dẫn tài xế kịp thời tránh xe chết máy giữa đường |
| Actor | Điều phối viên tổng đài vận hành đội xe taxi điện (Fleet Dispatcher) |
| Thời điểm / bối cảnh | Trong ca trực, khi tài xế đang chạy đón khách thì xe tụt pin xuống dưới 5%, tài xế hoảng gọi về tổng đài nhờ cứu hộ |
| Quy trình hiện tại (5 bước) | 1. Nghe máy tiếp nhận cuộc gọi khẩn cấp từ tài xế (khoảng 2 phút)<br>2. Nhập biển số lên màn hình quản lý xe để xem toạ độ GPS và mức pin còn lại (khoảng 2 phút)<br>3. Mở app bản đồ trạm sạc trên điện thoại/web khác, tự đo khoảng cách và tìm xem trạm nào gần nhất còn trụ sạc trống (5–6 phút) ← **BOTTLENECK 1**<br>4. Tự gõ tay tin nhắn SMS chỉ dẫn địa chỉ trạm sạc và các lưu ý an toàn như tắt điều hoà, đi chậm (3–4 phút) ← **BOTTLENECK 2**<br>5. Bấm gửi SMS hoặc gọi lại đọc đường đi cho tài xế, sau đó theo dõi xe trên màn hình (2 phút) |
| Bottleneck | Bước 3 (tra cứu thủ công trạm sạc còn trụ trống: mất 5–6 phút do phải chuyển qua lại giữa 2 hệ thống) và Bước 4 (ngồi gõ tay từng chữ tin nhắn chỉ dẫn an toàn: mất 3–4 phút). Tổng cộng xử lý một ca mất 14–17 phút |
| Impact | Mất 14–17 phút cho mỗi xe gặp nạn; giờ cao điểm một ca trực có thể gặp 3–4 ca; nếu xe chết máy giữa đường sẽ gây ùn tắc giao thông, tốn 500k–1 triệu tiền cẩu xe về xưởng theo quy trình cứu hộ xe kéo RSA ([Chính sách cứu hộ VinFast](https://vinfastauto.com/vn_vi/dich-vu-cuu-ho-xe-dien-vinfast-247)), tài xế bị trừ điểm phục vụ và khách hủy chuyến |
| Success metric | **Baseline:** 15 phút cho mỗi ca xử lý sự cố (ghi nhận phỏng vấn điều phối viên ca trực; đối chiếu với quy trình tiếp nhận tổng đài cứu hộ VinFast 1900 23 23 89).<br>**Target:** Giảm tổng thời gian xử lý xuống dưới 5 phút; thời gian soạn chỉ dẫn an toàn giảm xuống dưới 30 giây.<br>**Cách đo:** Đồng hồ hệ thống bấm giờ từ lúc mở ticket sự cố đến khi tin nhắn chỉ dẫn được bấm gửi đi |
| Phương án không dùng AI | In sẵn danh sách địa chỉ các trạm sạc theo từng khu vực ra bảng giấy: chỉ giúp nhớ địa chỉ nhanh hơn một chút, nhưng hoàn toàn không biết trạm đó lúc này còn trụ trống hay không và vẫn phải tự gõ tin nhắn |
| Giả thuyết về AI | Hệ thống dùng Rule tính khoảng cách để lọc ra 2 trạm sạc gần nhất còn trụ trống $\rightarrow$ AI đọc thông tin xe (dòng xe VF5/VF e34, mức pin, vị trí đường) để soạn sẵn 1 đoạn tin nhắn chỉ dẫn an toàn ngắn gọn $\rightarrow$ Điều phối viên nhìn lướt kiểm tra 15 giây rồi bấm nút gửi luôn |
| Cảm nhận nhanh | **Workflow** (Dùng Rule lọc trạm sạc theo khoảng cách + AI điền sẵn nội dung tin nhắn + Điều phối viên duyệt và gửi) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 5 bước, tổng thời gian: 14 - 17 phút (100% thủ công)

[1. Nghe điện thoại khẩn: 2'] 
  └──> [2. Tra GPS & % pin trên web: 2'] 
        └──> [3. Mở app tìm trạm sạc còn chỗ & đo km: 5-6']  <── 🔴 BOTTLENECK 1 (Tra cứu 2 màn hình)
              └──> [4. Tự gõ tin nhắn chỉ dẫn an toàn: 3-4'] <── 🔴 BOTTLENECK 2 (Gõ tay lâu và dễ sót)
                    └──> [5. Gửi SMS & theo dõi xe: 2']
```

---

### Problem Card #2 — Kiểm tra và đối chiếu quy cách nộp bài lab

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài lab lúc 23h, tôi muốn tự đối chiếu cấu trúc các file báo cáo và tên branch với rubric checklist, để không bị trừ điểm vì sai quy cách nộp bài |
| Actor | Sinh viên các lớp thực hành AI/CNTT (bản thân tôi và các bạn trong nhóm) |
| Thời điểm / bối cảnh | Khoảng 23h đến 23h30 trước giờ đóng cổng nộp bài LMS |
| Quy trình hiện tại (4 bước) | 1. Mở file SUBMISSION.md và RUBRIC.md lên đọc lại các dòng checklist (3 phút)<br>2. Kiểm tra xem tên repo, tên branch, các thư mục cá nhân đã đặt đúng cú pháp chưa (5 phút)<br>3. Mở từng file báo cáo đọc đối chiếu thủ công xem các bảng biểu đã điền đủ chưa, ảnh có bị lỗi link không (10–12 phút) ← **BOTTLENECK**<br>4. Gõ lệnh git commit, push lên GitHub và dán link nộp bài lên LMS (3 phút) |
| Bottleneck | Bước 3: Mở từng file markdown đọc dò từng mục xem có sót bảng nào hay thiếu ảnh nào không (mất 10–12 phút, lúc đêm muộn mắt mỏi rất dễ nhìn sót) |
| Impact | Mất hơn 20 phút trước hạn chót; nếu lỡ quên xóa một file template mẫu hoặc đặt sai tên file là bị trừ ngay 5 điểm theo quy chế của lớp |
| Success metric | **Baseline:** 20–25 phút ngồi kiểm tra thủ công trước mỗi hạn nộp (tự bấm giờ 2 lab trước).<br>**Target:** Giảm thời gian soát bài xuống dưới 3 phút; không bị trừ điểm lỗi hình thức.<br>**Cách đo:** Bấm giờ từ lúc bắt đầu kiểm tra đến lúc bấm nút nộp bài trên LMS |
| Phương án không dùng AI | Viết một đoạn script bash hoặc Python ngắn chạy kiểm tra regex tên file và kiểm tra sự tồn tại của thư mục: rất nhanh và hiệu quả với các quy tắc cứng |
| Giả thuyết về AI | Script làm phần kiểm tra tên file/thư mục; AI chỉ cần hỗ trợ đọc nội dung để cảnh báo xem các ô trả lời có bị quá ngắn (dưới 200 từ) hay không |
| Cảm nhận nhanh | **Rule** (Chủ yếu dùng script kiểm tra quy tắc cứng là đủ giải quyết 80% vấn đề) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 4 bước, tổng thời gian: 20 - 25 phút

[1. Mở SUBMISSION & RUBRIC: 3'] 
  └──> [2. Kiểm tra tên repo, folder, branch: 5'] 
        └──> [3. Đọc dò từng bảng và link ảnh trong file: 10-12'] <── 🔴 BOTTLENECK (Dò thủ công mỏi mắt)
              └──> [4. Commit, push & nộp LMS: 3']
```

---

### Problem Card #3 — Tổng hợp biên bản và danh sách việc sau họp nhóm

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tổng hợp ghi chú thảo luận từ buổi họp nhóm kéo dài 1 tiếng, tôi muốn có danh sách quyết định cuối cùng kèm người phụ trách, để cả nhóm thống nhất hành động sau cuộc họp |
| Actor | Bạn phụ trách ghi chép (thư ký buổi họp) và các thành viên nhóm đồ án |
| Thời điểm / bối cảnh | Ngay sau khi tắt cuộc gọi họp nhóm online trên Google Meet hoặc Discord |
| Quy trình hiện tại (4 bước) | 1. Trong lúc họp tranh thủ gõ nháp các ý kiến vào Google Docs (diễn ra trong lúc họp)<br>2. Họp xong ngồi đọc lại đống ghi chép nháp và lướt lại các tin nhắn trong ô chat (10 phút)<br>3. Ngồi lọc ra xem chốt lại việc gì, ai làm phần nào, hạn nộp khi nào (20–25 phút) ← **BOTTLENECK**<br>4. Format lại cho gọn rồi gửi tin nhắn tổng kết vào nhóm Zalo/Discord (5 phút) |
| Bottleneck | Bước 3: Phải ngồi chắt lọc từ đống ghi chép lộn xộn để gom thành danh sách việc rõ ràng (mất 20–25 phút) |
| Impact | Mất thêm nửa tiếng sau cuộc họp; nhiều hôm mệt không ai ghi lại biên bản là y như rằng hôm sau có bạn nhớ nhầm việc, làm trùng nhau hoặc quên task |
| Success metric | **Baseline:** Mất khoảng 35 phút sau cuộc họp mới gửi được biên bản.<br>**Target:** Giảm xuống dưới 10 phút sau họp là có to-do list gửi vào nhóm; 100% việc có tên người nhận rõ ràng.<br>**Cách đo:** Bấm giờ từ lúc kết thúc cuộc gọi họp đến lúc tin nhắn tóm tắt được gửi lên nhóm Zalo |
| Phương án không dùng AI | Dùng sẵn template bảng phân công việc trên Notion: trong lúc họp thống nhất đến đâu thì gõ thẳng vào bảng đến đó |
| Giả thuyết về AI | AI nhận bản nháp ghi chú hoặc bản ghi âm cuộc họp $\rightarrow$ tự lọc ra các đầu việc cần làm kèm tên người phụ trách $\rightarrow$ thư ký đọc lướt kiểm tra lại rồi bấm gửi |
| Cảm nhận nhanh | **Workflow** (AI trích xuất danh sách việc từ ghi chép $\rightarrow$ Con người duyệt lại) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 4 bước, tổng thời gian: 35 - 40 phút sau họp

[1. Mở lại bản ghi chép nháp: 3'] 
  └──> [2. Đọc lại nháp và tin nhắn chatbox: 10'] 
        └──> [3. Ngồi lọc quyết định và chia task: 20-25'] <── 🔴 BOTTLENECK (Lọc thông tin tốn thời gian)
              └──> [4. Format & gửi vào nhóm Zalo: 5']
```

---

### Card muốn pitch nhất

- **Card số:** Card #1 (Hỗ trợ điều phối xử lý sự cố xe taxi điện cạn pin khẩn cấp).
- **Vì sao:** Bài này có nghiệp vụ vận hành rất thực tế, tính cấp bách cao và hậu quả nhãn tiền (xe chết máy giữa đường là bị kéo xe, phạt tiền và ách tắc giao thông). Các bước đo thời gian rất rõ: mất 5–6 phút tìm trạm sạc và 3–4 phút gõ tin nhắn. Ngoài ra, bài này thể hiện rất rõ sự phân công hợp lý: việc tìm trạm sạc gần nhất chỉ cần Rule tính khoảng cách số học, còn AI chỉ nên hỗ trợ soạn sẵn câu chữ chỉ dẫn, cuối cùng con người vẫn phải kiểm tra và bấm gửi để đảm bảo an toàn.
- **Câu hỏi muốn nhóm phản biện:** *"Khi xe taxi điện đang còn dưới 5% pin thì tình huống rất gấp, liệu người điều phối có dám tin vào trạm sạc và câu chỉ dẫn do AI gợi ý không? Nếu gợi ý trạm mà xe đến nơi lại vừa kín chỗ thì phương án dự phòng xử lý thế nào để xe không bị chết máy giữa đường?"*

---

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI nhận xét rằng trạng thái trạm sạc có thể bị trễ vài phút: nếu gợi ý xe đến trạm mà đến nơi vừa có xe khác cắm vào sạc thì xe sẽ chết máy | **Đồng ý** | Tôi sửa lại quy trình: Hệ thống không được chỉ đưa 1 trạm duy nhất, mà bắt buộc phải hiển thị **1 trạm chính + 1 trạm dự phòng** gần đó, kèm số hotline của trạm để điều phối viên có thể gọi kiểm tra nhanh |
| AI đề xuất tự động gửi thẳng tin nhắn chỉ đường cho tài xế luôn (làm Agent tự động hoàn toàn) để đỡ mất công người điều phối | **Không đồng ý** | Tôi kiên quyết từ chối ý này: Đây là tình huống an toàn giao thông và ảnh hưởng tài sản xe, không thể để AI tự quyết hoàn toàn. Điều phối viên bắt buộc phải là người nhìn lướt kiểm tra và bấm nút gửi (Human-in-the-loop) để chịu trách nhiệm |
| AI chỉ ra rằng mục tiêu ban đầu chỉ mới đo thời gian xử lý nhanh hay chậm, chưa đo xem nội dung hướng dẫn có chính xác không | **Đồng ý** | Tôi bổ sung thêm tiêu chí chất lượng: 100% tin nhắn gửi đi phải đúng loại cổng sạc của xe (ví dụ xe dùng sạc nhanh DC hay sạc AC), và tỷ lệ tin nhắn bị điều phối viên phải ngồi gõ lại câu chữ phải dưới 10% |

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

1. **Chính sách Dịch vụ Cứu hộ Xe điện VinFast 24/7:** Quy trình tiếp nhận cứu hộ qua tổng đài 1900 23 23 89 và dịch vụ xe kéo cứu hộ RSA khi xe cạn pin trên đường: https://vinfastauto.com/vn_vi/dich-vu-cuu-ho-xe-dien-vinfast-247
2. **Công ty Phát triển Trạm sạc Toàn cầu V-Green:** Quy định hạ tầng trạm sạc, phí sạc quá giờ chống chiếm dụng trụ và chính sách sạc ưu đãi giờ thấp điểm (22h–6h) cho taxi điện GSM: https://vgreen.net
3. **Bài báo CafeF về hạ tầng và áp lực trạm sạc xe điện tại Việt Nam:** Phân tích nhu cầu sạc của các hãng xe dịch vụ và xung đột giờ cao điểm tại đô thị: https://cafef.vn/cuoc-dua-tram-sac-xe-dien-tai-viet-nam-188240405101524319.chn
4. **Quy chế và Rubric môn học K5-L3 Discovery & Problem Framing:** Repo đề bài và hướng dẫn chuẩn mực đánh giá: https://github.com/VinUni-AI20k/K5-L3-Day02-DiscoveryProblemFraming.git
