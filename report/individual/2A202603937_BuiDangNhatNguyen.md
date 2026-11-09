# Báo cáo cá nhân: 2A202603937_BuiDangNhatNguyen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Bùi Đặng Nhật Nguyên
- MSSV: 2A202603937
- Email trường (không bắt buộc, repo có thể để public): không công khai
- Tên nhóm: HEHEHE
- Link repo nhóm: https://github.com/hoangvu1806/K5-L3B-DAY02-HEHEHE-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi dịch vụ nội bộ bị chậm hoặc báo lỗi hàng loạt, tôi muốn khoanh vùng ngay sự cố nằm ở tầng nào (cổng proxy, mạng, ứng dụng hay cơ sở dữ liệu) mà không phải mở dò thủ công hàng chục file log trên nhiều máy chủ, để khôi phục dịch vụ trong vài phút | Kỹ sư vận hành, người dùng hệ thống | Thực tế hạ tầng có rất nhiều nguồn log rời rạc; mỗi lần xảy ra sự cố mất khoảng 60 đến 90 phút đăng nhập nhiều máy chủ và chạy lệnh lọc log thủ công |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi điều tra sự cố lúc cao điểm, tôi muốn lọc bỏ các bản ghi nhiễu (như kết nối giữ phiên, cache) và đối chiếu chéo từ log cổng vào (như Nginx) sang hàng loạt log dịch vụ ứng dụng, DNS và hệ thống phía sau, để tìm đúng nguyên nhân gốc | Kỹ sư vận hành, lập trình viên backend | Mỗi lần lần theo dấu vết qua nhiều tầng log mất khoảng 45 đến 60 phút; các kỹ sư trong ca trực dễ kết luận lệch nhau do mỗi người chỉ nhìn một vài file log |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi giám sát hệ thống ngoài giờ hành chính, tôi muốn phát hiện sớm các chuỗi truy cập bất thường (dò đường dẫn nhạy cảm, thử mật khẩu hoặc gửi request dồn dập) trải rộng trên nhiều file log cổng vào và xác thực, để chặn kịp thời trước khi dịch vụ bị treo | Kỹ sư vận hành, quản trị viên bảo mật | Rà soát thủ công trên nhiều nguồn log sau mỗi đợt bất thường mất 45 đến 60 phút; ca đêm không có người theo dõi màn hình liên tục |
| 4 | Pain từ người khác | Khi một dịch vụ phía sau quá tải kéo theo lỗi dây chuyền sang các dịch vụ khác, người dùng muốn đội kỹ thuật phát hiện và cô lập ngay từ lúc lỗi mới chớm tăng, để công việc không bị gián đoạn và không phải gửi ticket báo lỗi | Người dùng hệ thống, đội trực hỗ trợ | Đội vận hành thường chỉ biết sự cố sau 30 đến 60 phút khi người dùng đã gửi tin nhắn hoặc ticket phàn nàn |
| 5 | Lặp lại | Khi kiểm tra sức khỏe cụm máy chủ hàng tuần, tôi muốn có sẵn bộ chỉ số chuẩn về lưu lượng và tỷ lệ lỗi trên từng dịch vụ, để biết ngay thành phần nào đang suy giảm mà không phải gõ lại lệnh thống kê trên từng máy chủ | Kỹ sư vận hành, quản lý hạ tầng | Đều đặn mỗi tuần mất khoảng 35 đến 45 phút chạy lại các lệnh cắt lọc trên nhiều cụm log để tổng hợp tình trạng hệ thống |
| 6 | Lặp lại | Khi trực ca vào sáng đầu tuần lúc lưu lượng toàn công ty tăng tự nhiên, tôi muốn phân biệt được mức tăng theo chu kỳ làm việc với sự cố thật, để không tốn thời gian kiểm tra các cảnh báo giả kêu liên tục ở nhiều dịch vụ | Kỹ sư trực ca (On-call) | Mỗi sáng thứ Hai nhận nhiều lượt cảnh báo vượt ngưỡng tĩnh từ các máy chủ, mất khoảng 30 đến 40 phút/ca để kiểm tra rồi đóng cảnh báo giả |
| 7 | Tốn thời gian | Khi cần điều tra lại sự cố quá khứ trên diện rộng, tôi muốn gom hàng trăm file log khác định dạng từ nhiều máy chủ về một cấu trúc chung trước khi log tạm bị xoay vòng xóa mất, để không mất dấu vết lỗi | Kỹ sư vận hành, kỹ sư dữ liệu | Mỗi lần gom và đọc tuần tự hàng loạt file log lịch sử từ nhiều nơi mất 45 đến 60 phút; từng gặp trường hợp máy chủ khởi động lại làm mất log tạm |
| 8 | Pain từ người khác | Khi xảy ra lỗi liên hoàn qua nhiều tầng dịch vụ, đội phát triển backend muốn nhận ngay bản tóm tắt nguyên nhân gốc, đúng dịch vụ gây lỗi và mức độ khẩn cấp, để sửa đúng chỗ mà không phải tự đọc log thô của hạ tầng | Lập trình viên backend, kỹ sư trực ca | Kỹ sư trực ca mất thêm 25 đến 30 phút mỗi sự cố để gom các đoạn log liên quan từ nhiều nguồn và viết giải thích bàn giao cho đội ứng dụng |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Cách thực hiện: Tôi tự liệt kê trước 5 vấn đề (#1 đến #5) từ trải nghiệm kiểm tra log hệ thống (bắt đầu từ tầng cổng Nginx đến các dịch vụ ứng dụng phía sau). Sau đó nhờ AI gợi ý thêm góc nhìn theo 4 lăng kính.
- Ý giữ lại: Giữ #6 (kiểm tra cảnh báo giả sáng đầu tuần), #7 (tốn thời gian gom hàng trăm file log khác định dạng từ nhiều máy chủ) và #8 (chậm trễ khi gom bằng chứng đa nguồn bàn giao cho đội backend), viết lại theo thời gian thực tế đã gặp.
- Ý loại bỏ: Bỏ gợi ý "xây dựng hệ thống tự động sửa code backend và khởi động lại toàn bộ cụm máy chủ" vì đó là giải pháp đội lốt vấn đề và quá rủi ro cho môi trường vận hành thật.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Phát hiện chậm, phải lần mò qua nhiều nguồn log rời rạc và phản ứng trễ khi có sự cố hoặc truy cập bất thường (#1, #2, #3, #4) | Mất nhiều thời gian nhất (60 đến 90 phút/sự cố); vì thực tế doanh nghiệp có rất nhiều nguồn log khác nhau nên thấy rất rõ vì sao `Workflow` cố định bị bí và cần tới `Agent` tự chọn nguồn log điều tra kèm ngưỡng `Confidence Score` | Đặt ngưỡng điểm tự tin (`Confidence Score`) bao nhiêu là an toàn để cho phép tự động cô lập tạm thời, và phạm vi log nào nên chọn làm bước thử nghiệm đầu tiên (ví dụ thử trước trên tầng cổng Nginx)? |
| 2 | Mất thời gian kiểm tra cảnh báo giả vào giờ cao điểm đầu tuần và lọc nhiễu log (#6) | Lặp lại hàng tuần trên nhiều dịch vụ, dễ đo lường bằng số phút kiểm tra và tỷ lệ cảnh báo sai | Chỉ cần dùng công thức thống kê theo ngày trong tuần (`Rule`) có giải quyết được hơn 80% vấn đề chưa? |
| 3 | Chậm trễ khi gom bằng chứng từ nhiều tầng log để viết báo cáo bàn giao cho đội backend (#8) | Điểm nghẽn thực tế khi phối hợp giữa đội hạ tầng và các đội phát triển ứng dụng | Đội backend cần bản tóm tắt đầy đủ hay chỉ cần tên dịch vụ lỗi, đường dẫn lỗi và khung giờ? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi hệ thống gặp lỗi hàng loạt hoặc có truy cập bất thường (nhất là ban đêm), tôi muốn phát hiện sớm từ tầng cổng vào, tự động lần ra đúng nguyên nhân gốc giữa hàng chục nguồn log liên quan và cô lập tác nhân gây lỗi theo mức độ tin cậy rõ ràng, để giảm thời gian gián đoạn từ hàng giờ xuống vài phút mà không chặn nhầm người dùng hợp lệ |
| Actor | Kỹ sư trực vận hành hệ thống (IT / NetOps On-call) quản lý hạ tầng nhiều máy chủ và dịch vụ nội bộ |
| Thời điểm / bối cảnh | Khi lưu lượng hoặc tỷ lệ lỗi tăng vọt (biểu hiện đầu tiên thường ở cổng reverse proxy như Nginx nhưng nguyên nhân có thể nằm sâu ở ứng dụng, mạng hoặc database), đặc biệt ngoài giờ hành chính |
| Quy trình hiện tại (3–7 bước) | 1. Nhận báo lỗi trễ từ người dùng · 2. Mở log ở cổng đón lưu lượng (như Nginx access/error log) để xác định triệu chứng ban đầu · 3. Chạy lệnh lọc bỏ bản ghi nhiễu (kết nối giữ phiên, cache) để tìm khung giờ đỉnh lỗi · 4. Tùy dấu hiệu vừa thấy mà đăng nhập tiếp sang các máy chủ khác để đọc log ứng dụng, DNS, container hoặc bảo mật nhằm tìm nguyên nhân gốc · 5. Cân nhắc rủi ro và chạy lệnh xử lý (chặn tạm IP hoặc báo đội phụ trách dịch vụ lỗi) · 6. Kiểm tra lại và viết báo cáo |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 và Bước 4: Lọc nhiễu và phải mở đối chiếu thủ công qua nhiều nguồn log rời rạc trên nhiều máy chủ khác nhau để khoanh vùng đúng nguồn gây lỗi, mất khoảng 50 đến 60 phút/sự cố (chưa tính 30 đến 60 phút phát hiện trễ ban đầu) |
| Impact (nếu không giải thì sao) | Tổng thời gian xử lý kéo dài 90 đến 120 phút (hoặc tới sáng hôm sau nếu lỗi ban đêm), gây gián đoạn dây chuyền trên nhiều dịch vụ nội bộ |
| Success metric (baseline → target) | Giảm thời gian phát hiện và khoanh vùng nguyên nhân gốc từ 60-90 phút xuống dưới 5 phút; tỷ lệ cảnh báo sai dưới 15%; 0 trường hợp chặn nhầm dải IP hoặc dịch vụ hợp lệ |
| Phương án không dùng AI | Gom log về một công cụ tìm kiếm tập trung (như OpenSearch/Loki), đặt bộ quy tắc ngưỡng thống kê (`Rule`) trên từng nguồn log và chuẩn bị sẵn script để kỹ sư tự tra cứu và chạy tay |
| Giả thuyết về AI (nếu có) | Kết hợp bộ lọc ngưỡng với `Agent` hoạt động theo điểm tự tin (`Confidence Score`) và con người kiểm duyệt (`HITL`): từ dấu hiệu bất thường ở cổng vào, Agent tự chọn nguồn log liên quan tiếp theo cần đọc để kết luận nguyên nhân và tính điểm tự tin. Nếu điểm vượt ngưỡng cao (ví dụ từ 85% trở lên) và hành động an toàn có thể hoàn tác (như giới hạn tốc độ tạm thời 1 IP lạ), Agent tự thực thi và báo ngay cho kỹ sư; nếu dưới ngưỡng hoặc đụng tới dịch vụ chung thì bắt buộc chờ kỹ sư bấm duyệt. Khi thử nghiệm thực tế có thể bắt đầu trước với cụm log cổng Nginx rồi mở rộng sang các tầng log khác |
| Cảm nhận nhanh | Agent (vì phải tự quyết định nhánh nguồn log cần tra cứu tiếp theo giữa hàng chục nguồn log công ty, kết hợp khóa an toàn bằng `Confidence Score` và `HITL`) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI (khoảng 90 phút xử lý chủ động + 30-60 phút phát hiện trễ)

[1. Nhận báo lỗi trễ: 30-60p] -> [2. Mở log cổng vào (Nginx) xem triệu chứng: 10p]
-> [3. Lọc bỏ log nhiễu & tìm khung giờ đỉnh lỗi: 20p] (BOTTLENECK)
-> [4. Đăng nhập các server khác đối chiếu log ứng dụng / mạng / DB: 35p] (BOTTLENECK)
-> [5. Chạy lệnh chặn IP / xử lý dịch vụ lỗi: 10p] -> [6. Kiểm tra & báo cáo: 15p]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi trực ca vào giờ cao điểm đầu tuần, tôi muốn phân biệt mức tăng lưu lượng tự nhiên trên các máy chủ với đợt tăng bất thường thật sự, để không tốn thời gian kiểm tra các cảnh báo giả kêu liên tục |
| Actor | Kỹ sư trực ca vận hành (On-call Engineer) |
| Thời điểm / bối cảnh | Buổi sáng đầu tuần (8h30 đến 10h30 thứ Hai) khi toàn bộ nhân viên mở các công cụ làm việc khiến lượng kết nối trên nhiều dịch vụ tăng vọt so với cuối tuần |
| Quy trình hiện tại (3–7 bước) | 1. Nhận hàng loạt cảnh báo lưu lượng vượt ngưỡng cố định · 2. Mở log 30 phút gần nhất của dịch vụ đang báo động · 3. Tách riêng các kết nối giữ phiên (WebSocket) và đếm tỷ lệ lỗi thật · 4. Mở số liệu sáng thứ Hai tuần trước để so sánh bằng mắt · 5. Xác nhận là bình thường và đóng từng cảnh báo |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 và Bước 4: Tách lọc lưu lượng nhiễu và đối chiếu thủ công với cùng khung giờ tuần trước trên nhiều dịch vụ, mất khoảng 25 phút mỗi đợt kiểm tra |
| Impact (nếu không giải thì sao) | Tốn 30 đến 45 phút mỗi ca sáng đầu tuần cho các cảnh báo sai, dễ gây tâm lý chủ quan bỏ sót sự cố thật |
| Success metric (baseline → target) | Giảm tỷ lệ cảnh báo sai xuống dưới 15%; giảm thời gian xác minh cảnh báo đầu tuần từ 35-40 phút/ca xuống dưới 5 phút/ca |
| Phương án không dùng AI | Dùng `Rule` tách bỏ kết nối giữ phiên trước khi đếm, tính ngưỡng chuẩn riêng theo từng thứ trong tuần (cửa sổ trượt) và tắt lặp lại cảnh báo trong 30 phút |
| Giả thuyết về AI (nếu có) | Dùng mô hình học máy không giám sát học chu kỳ lưu lượng theo giờ và ngày trên nhiều dịch vụ để phát hiện các bất thường kết hợp nhiều chỉ số cùng lúc |
| Cảm nhận nhanh | Rule (ngưỡng thống kê theo ngày trong tuần đã giải quyết được phần lớn vấn đề) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI (khoảng 40 phút/ca kiểm tra cảnh báo đầu tuần)

[1. Nhận loạt cảnh báo ngưỡng tĩnh: 3p] -> [2. Mở log các dịch vụ báo động: 7p]
-> [3. Tách lọc log giữ phiên & đếm lỗi thật: 10p] (BOTTLENECK)
-> [4. So sánh tay với sáng thứ Hai tuần trước: 15p] (BOTTLENECK)
-> [5. Đóng các cảnh báo giả: 5p]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi phát hiện lỗi dây chuyền giữa cổng proxy và các dịch vụ phía sau, tôi muốn gom nhanh các đoạn log bằng chứng từ nhiều nguồn thành bản tóm tắt nguyên nhân gốc kèm mức độ khẩn cấp, để chuyển ngay cho đúng đội ứng dụng xử lý mà không mất nửa tiếng viết giải trình |
| Actor | Kỹ sư vận hành (người gửi) và Lập trình viên các đội backend (người nhận xử lý) |
| Thời điểm / bối cảnh | Ngay sau khi phát hiện tỷ lệ lỗi kết nối tăng cao, cần xác định đúng dịch vụ backend nào đang gây nghẽn để bàn giao cho nhóm phụ trách dịch vụ đó |
| Quy trình hiện tại (3–7 bước) | 1. Cắt các dòng lỗi tiêu biểu lúc đỉnh lỗi ở cổng proxy · 2. Tra cứu tiếp sang log của các dịch vụ ứng dụng liên quan để tìm đúng dịch vụ gốc gây treo · 3. Tự ước lượng mức độ khẩn cấp · 4. Viết tin nhắn tóm tắt diễn biến, bằng chứng log và hướng kiểm tra · 5. Gửi cho đội phụ trách ứng dụng đó và trả lời câu hỏi làm rõ |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 và Bước 4: Gom bằng chứng xuyên qua nhiều nguồn log và viết tóm tắt sao cho đội ứng dụng hiểu ngay, mất khoảng 22 phút/sự cố |
| Impact (nếu không giải thì sao) | Chậm thời gian bàn giao sự cố thêm 25 đến 30 phút; nếu khoanh vùng nhầm dịch vụ sẽ gửi nhầm nhóm phát triển làm mất thêm thời gian chuyển tiếp |
| Success metric (baseline → target) | Giảm thời gian soạn bàn giao sự cố từ 25-30 phút xuống dưới 3 phút/lần; 100% thông số khung giờ, tên dịch vụ và đường dẫn lỗi khớp với log gốc |
| Phương án không dùng AI | Tạo biểu mẫu báo cáo sự cố cố định kèm script tự gom khung giờ, mã lỗi và đường dẫn lỗi theo mã định danh truy vết (request ID) |
| Giả thuyết về AI (nếu có) | Sau khi script trích xuất các đoạn log liên quan quanh đỉnh lỗi, mô hình ngôn ngữ chạy nội bộ soạn nháp đoạn tóm tắt nguyên nhân để kỹ sư kiểm tra rồi gửi cho đội ứng dụng |
| Cảm nhận nhanh | Workflow (các bước cố định khi đã biết nguồn log cần lấy, AI hỗ trợ viết nháp tóm tắt, kỹ sư duyệt trước khi gửi) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI (khoảng 35 phút bàn giao sự cố liên tầng)

[1. Cắt dòng lỗi ở cổng proxy: 5p] -> [2. Tra chéo sang log các dịch vụ ứng dụng: 10p] (BOTTLENECK)
-> [3. Ước lượng mức khẩn cấp: 3p] -> [4. Viết tóm tắt nguyên nhân gửi đội phụ trách: 12p] (BOTTLENECK)
-> [5. Giải đáp câu hỏi làm rõ: 5p]
```

### Card muốn pitch nhất

- Card số: Card #1 (Phát hiện chậm, phải lần mò qua nhiều nguồn log rời rạc và phản ứng trễ khi có sự cố hoặc truy cập bất thường).
- Vì sao: Phản ánh đúng thực tế hạ tầng doanh nghiệp có hàng chục nguồn log khác nhau (không thể đọc xuể bằng tay hay viết một luồng cứng nhắc cho mọi tình huống), đồng thời cho phép giới hạn phạm vi thử nghiệm ban đầu ngay trên tầng cổng Nginx trước khi mở rộng.
- Câu hỏi muốn nhóm phản biện: Khi cho phép Agent tự chọn nguồn log điều tra và tự chạy lệnh cô lập ở ngưỡng `Confidence Score` cao (ví dụ từ 85% trở lên), làm sao ngăn rủi ro mô hình tự chấm điểm tự tin sai rồi chặn nhầm cổng kết nối chung của người dùng thật?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Nếu mô tả bài toán như thể chỉ có 2 file log cố định thì một `Workflow` viết sẵn là đủ, không có lý do thuyết phục để dùng `Agent`; ngược lại nếu ôm toàn bộ hàng trăm nguồn log của công ty ngay ngày đầu thì quá sức một buổi thử nghiệm | Đồng ý | Làm rõ bối cảnh thực tế doanh nghiệp có rất nhiều nguồn log phân tán nhiều tầng (nên cần `Agent` tự quyết định nhảy sang nguồn log nào để điều tra tiếp), nhưng khi chạy Pilot sẽ thu hẹp phạm vi thử nghiệm bắt đầu từ tầng cổng Nginx trước |
| Nếu để mô hình ngôn ngữ tự phát biểu con số phần trăm `Confidence Score` thì rất dễ bị ảo giác tự tin cao dù chẩn đoán sai nguyên nhân | Đồng ý | Quy định lại `Confidence Score` phải tính từ các chỉ số định lượng độc lập (mức vượt ngưỡng thống kê, mức khớp kịch bản chuẩn và kiểm tra danh sách trắng); mọi tác động lên dịch vụ dùng chung bắt buộc qua con người duyệt (`HITL`) |
| Chưa làm rõ vì sao không dùng luôn các nền tảng giám sát đám mây thương mại như Datadog | Đồng ý | Bổ sung ràng buộc bảo mật không được gửi log nội bộ ra đám mây bên ngoài và thực tế nhiều máy chủ nội bộ chưa được gom log đồng bộ về một chỗ |

---

## 4. Tôi đã tham gia phần nào (CP3 -> CP7)

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
| CP1 Scan | Rà soát cách viết Job Story theo 4 lăng kính cho bài toán vận hành log hệ thống | Giúp chuẩn hóa câu chữ ngắn gọn theo cấu trúc Job Story và gợi ý thêm góc nhìn về cảnh báo giả đầu tuần | Bản nháp đầu của AI hiểu hẹp rằng hệ thống chỉ có 2 file log cố định (theo file mẫu tôi đưa) và giữ lại các thông số nội bộ nhạy cảm | Chỉnh lại đúng thực tế doanh nghiệp có hàng chục nguồn log đa tầng (Nginx chỉ là cổng vào), viết gọn dễ hiểu và xóa sạch thông số riêng của công ty |
| CP2 Problem Card | Đóng vai Product Manager hoài nghi để phản biện 3 Problem Cards và hướng dùng `Agent` kèm `Confidence Score` | Chỉ ra mâu thuẫn giữa phạm vi dữ liệu với lựa chọn `Agent`, đồng thời cảnh báo nguy cơ ảo giác nếu để mô hình tự chấm điểm tự tin | Có xu hướng gộp bước lọc nhiễu log cổng vào với bước tra cứu log các dịch vụ phía sau thành một bước chung | Tách rõ từng bước kèm số phút, xác định rõ lý do cần `Agent` khi truy vết nhiều nguồn log nhưng thu hẹp Pilot ở tầng Nginx, kết hợp khóa an toàn `HITL` |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5-6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1-6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5-8 câu, không nhìn tài liệu, chuỗi *problem -> quy trình -> metric -> boundary -> mức can thiệp AI -> quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

- [Đề bài CHECKPOINTS](../../CHECKPOINTS.md)
- [Quy định sử dụng AI](../../RULES.md)
- [Tiêu chí chấm điểm RUBRIC](../../RUBRIC.md)
- Anthropic, *Building Effective Agents*: https://www.anthropic.com/research/building-effective-agents
- Google PAIR, *People + AI Guidebook*: https://pair.withgoogle.com/chapter/user-needs/
- OpenSearch Documentation, *Anomaly Detection Plugin*: https://opensearch.org/docs/latest/monitoring-plugins/ad/index/
- Datadog Documentation, *Watchdog Log Anomaly Detection*: https://docs.datadoghq.com/watchdog/
- GoAccess, *Real-time Web Log Analyzer*: https://goaccess.io/
- Grafana Labs, *Grafana Loki Documentation*: https://grafana.com/docs/loki/latest/
