# Báo cáo cá nhân — 03427_NguyenVuKhanh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Vũ Khanh
- MSSV: 2A202603427
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:CodeX
- Link repo nhóm:https://github.com/cuong-sadboi/K5-L3A-DAY02-CodeX-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Tốn thời gian|Khi vừa code xong môt bài tập lớn, tôi muốn công cụ tự động đọc thư mục code để tạo sẵn file readme.md và tóm tắt các hàm chính để nộp bài mà không cần phải gõ tài liệu từ đầu|Cá nhân tôi, giảng viên, bạn cùng nhóm|Mất 1-2 tiếng để gõ cấu trúc code, file hướng dẫn mỗi khi hoàn thành|
| 2 |Lặp lại|Khi tải code về máy hoặc chuyển sang làm bài tập môn khác, tôi muốn một công cụ tự động kiểm tra thiếu thư viện nào và cài sẵn và tạo file cấu hình mẫu .env để bấm chạy được ngay|Cá nhân tôi và các bạn trong nhóm|Mất 15-20 phút mỗi lần pull code mới về dò lỗi|
| 3 |Pain từ người khác|Khi bạn trong nhóm đẩy code lên Git, tôi muốn nhận được một bản tóm tắt ngắn gọn về những thay đổi mà hành viên trong nhóm đã sửa và nó có ảnh hưởng gì đến các feature của tôi không|Cá nhân tôi và thành viên nhóm|Tin nhắn commit trên GitHub chỉ ghi đơn giản (update, fix bug) khiến người khác không biết sửa gì|
| 4 |Tốn thời gian|Khi chọn thử nghiệm code với các tham số khác nhau, tôi muốn tự động gom các kết quả in ra màn hình thành một bảng so sánh gọn gàng để tiện sử dụng để so sánh hoặc được vào slide, báo cáo|Cá nhân tôi|Mất 20-30 phút để lướt lại màn hình console, copy số liệu vào note|
| 5 |Cần đọc, tổng hợp nhiều thông tin|Khi chuẩn bị đi xin intern hoặc tìm việc làm, tôi muốn AI đọc trực tiếp các dự án tôi đã làm trong local và viết thành mục trong cv để cập nhật cv mà tôi không cần tự mình tổng hợp|Cá nhân tôi|Các dự án làm rất kỹ nhưng đã lâu rồi không xem lại nên việc viết vào cv khá khăn, có thể thiếu sót các thông tin|
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
| 1 |Tự động tạo file README.md và tóm tắt báo cáo từ thư mục code|Dễ đưa vào thực thi, đầu vào là các repo bài tập có sẵn|Đối với các project có quá nhiều file hoặc thư mục lồng với nhau phức tạp , nếu đưa vào prompt có thể bị tràn giới hạn từ hoặc tốn nhiều token|
| 2 |Tóm tắt thay đổi khi người trong nhóm đẩy code mới lên Git|Giải quyết nỗi đau làm đồ án nhóm |AI có thể chỉ nhìn vào mỗi đoạn code thay đổi nên có khả năng cảnh bào nhầm nếu không năm được luồng của cả hệ thống|
| 3 |Đọc dự án trong máy để viết mục kinh nghiệm dự án trong cv để khớp jd|Giá trị sử dụng cao cho những người tìm việc làm|Khó đánh giá tự động câu chữ viết ra đã tốt và thuyết phục được nhà tuyển dụng không|

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa code xong môt bài tập lớn, tôi muốn công cụ tự động đọc thư mục code để tạo sẵn file readme.md và tóm tắt các hàm chính để nộp bài mà không cần phải gõ tài liệu từ đầu |
| Actor | Sinh viên, coder |
| Thời điểm / bối cảnh | Khi code chạy được nhưng kho lưu trữ vẫn trống, chưa có hướng dẫn cài đặt hay mô tả cấu trúc |
| Quy trình hiện tại (3–7 bước) | Bước 1: Mở lại từng thư mục để xem cấu trúc dự án.<br>Bước 2: Kiểm tra các thư viện đã dùng để ghi lại requirements.txt<br>Bước 3: Mở các file code chính để nhớ lại luồng chạy, tham số đầu vào và tên các hàm quan trọng.<br>Bước 4: Chạy thử lại các lệnh trên Terminal để copy câu lệnh mẫu và kết quả in ra màn hình.<br>Bước 5: Mở file README.md, tự gõ mô tả dự án, kẻ khung cây thư mục và định dạng cú pháp Markdown thủ công.<br>Bước 6: Đọc soát lại, lưu file và git push|
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 3 và 5 mất 45-60 phút|
| Impact (nếu không giải thì sao) | Gây ra bất đồng bộ trong nhóm các bạn cùng nhóm kéo code về nhưng không hiểu cấu trúc thư mục và cách dùng hàm |
| Success metric (baseline → target) | Thời gian viết tài liệu cho 1 repo giảm từ 60-70 phút xuống còn 5-10 phút, Người khác làm theo REAMDE.md chạy được code ngay lần đầu|
| Phương án không dùng AI | Tạo sẵn template cố định cho README.md, dùng lệnh có sẵn trên máy để xuất nhanh cấu trúc thư mục và danh sách thư viện|
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | Workflow / Agent |

Quy trình nháp hiện tại:

```text
[1. Code xong dự án] 
       │
       ▼
[2. Mở Code rà soát thủ công từng thư mục & danh sách thư viện] (10-15 phút)
       │
       ▼
[3. Đọc lại các file code chính để nhớ luồng chạy & chức năng từng hàm] (20-25 phút) 
       │
       ▼
[4. Chạy lại lệnh trên Terminal để copy câu lệnh mẫu & kết quả đầu ra] (10 phút)
       │
       ▼
[5. Tự gõ nội dung, vẽ cây thư mục & căn chỉnh Markdown trong README.md] (25-35 phút) 
       │
       ▼
[6. Kiểm tra lại, lưu file và git push lên GitHub] (5 phút)

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi bạn trong nhóm đẩy code lên Git, tôi muốn nhận được một bản tóm tắt ngắn gọn về những thay đổi mà hành viên trong nhóm đã sửa và nó có ảnh hưởng gì đến các feature của tôi không |
| Actor | Thành viên trong nhóm làm dự án |
| Thời điểm / bối cảnh | Trong giai đoạn chạy nước rút làm đồ án môn học, khi các thành viên liên tục git push code lên nhánh chung vào buổi tối trước ngày báo cáo tiến độ nhưng chỉ ghi lời nhắn commit ngắn như "update", "fix bug". |
| Quy trình hiện tại (3–7 bước) | Bước 1: Kéo (git pull) code mới của bạn cùng nhóm về máy cục bộ.<br>Bước 2: Chạy thử chương trình và phát hiện lỗi đỏ màn hình .<br>Bước 3: Mở lịch sử GitHub hoặc VS Code Git Graph để dò xem ai vừa sửa những file nào.<br>Bước 4: Mở từng file có dấu cộng/trừ để đọc bằng mắt thường xem bạn đã đổi logic gì.<br>Bước 5: Nhắn tin vào nhóm  hỏi lại bạn cho chắc chắn và chờ phản hồi.<br>Bước 6: Tự sửa lại các file code của mình cho khớp với thay đổi của bạn.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4,5 mất 30-60 phút |
| Impact (nếu không giải thì sao) | Chậm tiến độ cả nhóm: Mất cả buổi tối chỉ để sửa lỗi ghép nối thay vì code tính năng mới |
| Success metric (baseline → target) |  Thời gian hiểu thay đổi & xử lý lỗi ghép code: Giảm từ 30–60 phút/lần pull → xuống còn dưới 5 phút |
| Phương án không dùng AI | Đặt quy tắc bắt buộc trong nhóm: Ai sửa API/Database phải viết tin nhắn báo vào nhóm chat và ghi commit theo mẫu cố định,dùng tính năng GitHub Branch Protection bắt buộc phải có 1 người đọc duyệt (Review) trước khi gộp code |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | Workflow / Agent |

Quy trình nháp hiện tại:

```text
[1. Kéo code mới của bạn về máy (git pull)] 
       │
       ▼
[2. Chạy thử project -> Phát sinh lỗi bất ngờ do lệch biến/API] (5 phút)
       │
       ▼
[3. Mở lịch sử Git tìm xem ai vừa sửa những file nào] (5-10 phút)
       │
       ▼
[4. Đọc dò từng dòng xanh/đỏ trong git diff để tìm nguyên nhân] (15-25 phút) 
       │
       ▼
[5. Nhắn tin hỏi bạn cùng nhóm và chờ trả lời] (15-30 phút)
       ▼
[6. Sửa lại code của mình cho khớp và chạy thử lại] (10-15 phút)

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị đi xin intern hoặc tìm việc làm, tôi muốn AI đọc trực tiếp các dự án tôi đã làm trong local và viết thành mục trong cv để cập nhật cv mà tôi không cần tự mình tổng hợp |
| Actor | Người cần chuẩn bị cv để xin việc |
| Thời điểm / bối cảnh | Mùa tuyển dụng; khi tìm thấy một tin tuyển dụng (JD) ưng ý nhưng nhận ra CV hiện tại đang viết quá sơ sài, hoặc phải sửa lại cách mô tả các đồ án ở trường sao cho trúng các từ khóa kỹ thuật mà công ty đó yêu cầu |
| Quy trình hiện tại (3–7 bước) | Bước 1: Đọc bản Mô tả công việc (JD) để gạch chân các kỹ năng và công nghệ công ty yêu cầu.<br>Bước 2: Lục lại các thư mục code bài tập lớn/đồ án cũ trong máy tính hoặc trên GitHub.<br>Bước 3: Mở lại code, file requirements.txt và báo cáo cũ để nhớ xem hồi đó mình dùng thư viện gì, giải quyết bài toán gì và kết quả (độ chính xác, tốc độ) ra sao.<br>Bước 4: Mở file CV , tự viết thành 3–4 câu mô tả theo văn phong chuyên nghiệp.<br>Bước 5: So sánh lại với JD xem đã đủ từ khóa chưa, chỉnh sửa độ dài câu cho vừa trang giấy rồi xuất file PDF.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3,4 mất 30-45 phút |
| Impact (nếu không giải thì sao) | Ngại cá nhân hóa CV: Vì sửa mỗi bản CV mất gần cả tiếng đồng hồ nên sinh viên thường dùng 1 bản CV duy nhất rải cho mọi công ty |
| Success metric (baseline → target) | Thời gian điều chỉnh mục Dự án trong CV theo 1 JD mới: Giảm từ 45–60 phút → xuống còn 5–10 phút, độ khớp từ khóa với JD: Đạt trên 80% các kỹ năng thực tế có trong code. |
| Phương án không dùng AI | Tự lập một bảng Excel lưu trữ sẵn thông tin mọi đồ án đã làm (tên môn, thư viện đã dùng, số liệu kết quả, câu mô tả mẫu) ngay sau khi kết thúc mỗi học kỳ để lúc làm CV chỉ việc copy ra. |
| Giả thuyết về AI (nếu có) | Nếu dùng một AI Agent tự động quét repo dự án để lấy đúng danh sách thư viện + số liệu thực nghiệm, sau đó đối chiếu với văn bản JD để gợi ý 3 phương án viết gạch đầu dòng (có bước Human-in-the-Loop để tôi kiểm tra số liệu và chọn câu ưng ý nhất), thì sẽ tạo ra bản CV vừa trúng từ khóa tuyển dụng vừa bám sát 100% những gì tôi đã code. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
[1. Đọc tin tuyển dụng (JD) và lọc ra các từ khóa kỹ năng] (5-10 phút)
       │
       ▼
[2. Lục tìm lại các thư mục đồ án / bài tập lớn phù hợp trong máy] (5 phút)
       │
       ▼
[3. Mở đọc lại code & báo cáo cũ để tìm tên thư viện và số liệu kết quả] (15-20 phút) 
       │
       ▼
[4. Tự nghĩ câu chữ viết thành 3-4 gạch đầu dòng khớp với từ khóa JD] (20-25 phút) 
       │
       ▼
[5. Căn chỉnh lại độ dài trong CV, kiểm tra lỗi và xuất file PDF] (5-10 phút)

```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Mang tính ứng dụng cao
- Câu hỏi muốn nhóm phản biện: Đã có GitHub Copilot hay ChatGPT hỗ trợ viết tài liệu rồi, vậy công cụ này có điểm gì vượt trội hơn hẳn để sinh viên chịu dùng thay vì copy-paste code lên web hỏi?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|Nguy cơ tràn bộ nhớ (Context Limit) và tốn token: Nếu thiết kế ngây thơ cho AI đọc toàn bộ mọi file trong thư mục dự án, khi gặp các thư mục như node_modules, .venv, .git hoặc file dữ liệu .csv nặng hàng chục MB thì hệ thống sẽ bị treo hoặc hết sạch quota API ngay lập tức|Đồng ý|Thiết kế lại luồng xử lý tách làm 2 bước (Workflow + Agent):
Bước 1 (Rule-based, không dùng AI): Dùng script Python quét cây thư mục và tự động loại bỏ các thư mục rác/môi trường ảo (.venv, __pycache__, .git, file dữ liệu lớn).
Bước 2 (Agent): Chỉ gửi cây thư mục gọn nhẹ cho AI xem trước để AI tự chọn đúng 3–5 file cốt lõi (requirements.txt, main.py, config.py) cần đọc nội dung chi tiết.|
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
