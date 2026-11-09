# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân. Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: ABC
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi khách đã chốt mẫu, số lượng, SĐT và địa chỉ nằm rải rác trong đoạn chat dài, nhân viên sales muốn gom đủ thông tin đặt hàng vào đúng các trường tạo đơn, để không phải cuộn ngược đoạn chat copy-paste từng dòng và tránh nhập sai mã hàng/địa chỉ.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| \#  | Người đưa ra | Candidate (Job Story ngắn)                                                                                                                                                                                                                                         | Actor                     | Bottleneck                                                                                                       | Câu hỏi phản biện nhận được (ai hỏi)                                                                                                                                    |
| --- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------- | ---------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Trọng        | reset mật khẩu                                                                                                                                                                                                                                                     | nhân viên                 | quy trình lặp lại tốn thời gian                                                                                  | Nếu bật tính năng tự lấy lại mật khẩu qua OTP/Email (Self-service Password Reset - No AI) thì đã giảm được 90% ticket chưa, cần gì tới AI? (Khải)                       |
| 2   | Trọng        | onboarding tài khoản dành cho nhân viên mới                                                                                                                                                                                                                        | nhân viên                 | cấp thủ công mất 15-20 phút                                                                                      | Một tuần công ty có bao nhiêu nhân viên mới vào? Nếu chỉ 2–3 người/tuần thì tốn 15 phút/lần có phải pain lớn nhất không? (Thắng)                                        |
| 3   | Trọng        | phân quyền, phê duyệt quyền truy cập tài nguyên                                                                                                                                                                                                                    | nhân viên                 | ảnh hưởng tiến độ các dự án khác                                                                                 | Bước làm chậm tiến độ thực chất là do chờ sếp bấm duyệt (con người) hay do thao tác kỹ thuật cấp quyền? Nếu do chờ sếp duyệt thì AI có tự duyệt thay được không? (Khải) |
| 4   | Khải         | tổng hợp thông tin khách hàng và sản phẩm để tạo đơn hàng                                                                                                                                                                                                          | nhân viên                 | chuyển qua nhiều hệ thống để xử lý đơn hàng                                                                      | Nếu gửi cho khách 1 form mẫu cố định để khách tự điền Tên + SĐT + Địa chỉ (No AI) thì đã giảm được một nửa thời gian chưa? (Thắng)                                      |
| 5   | Khải         | Khi nhiều khách nhắn tin hỏi cùng thông số sản phẩm (size, chất liệu) hoặc chính sách đổi trả trong giờ cao điểm, tôi muốn có ngay thông tin chuẩn xác theo đúng mã hàng khách đang hỏi, để phản hồi dưới 1 phút mà không phải mở file tra cứu và gõ lại nhiều lần | nhân viên                 | tìm thông tin sản phẩm tốn thời gian và lặp lại                                                                  | Dùng bộ câu trả lời nhanh gắn sẵn trên phần mềm chat đã giải quyết được 80% chưa (Thắng)                                                                                |
| 6   | Khải         | Khi khách nhắn tin báo nhận sai hàng hoặc hàng lỗi kèm ảnh/video unbox, tôi muốn kiểm tra nhanh lịch sử tư vấn, mã vận đơn gốc, người đóng gói và tồn kho mã thay thế ở một chỗ, để đưa ra phương án đổi trả cho khách ngay trong một lần trao đổi                 | nhân viên                 | đối chiếu lịch sử chat cũ + nhắn hỏi kho chờ xác nhận tồn thực tế): mất 8–10 phút/ca                             | Số ca lỗi/tuần có đủ nhiều để ưu tiên hơn việc tạo đơn hàng ngày không? (Trọng)                                                                                         |
| 7   | Thắng        | Tổng hợp báo cáo hàng tháng                                                                                                                                                                                                                                        | kế hoạch tổng hợp         | tổng hợp thông tin từ nhiều chuyên khoa mất thời gian                                                            | Mỗi tháng chỉ làm 1 lần thì tần suất có hơi thấp để kiểm chứng trong pilot ngắn không? (Khải)                                                                           |
| 8   | Thắng        | Tóm tắt nội dung các chức năng cần phát triển và phân quyền đến nhân viên                                                                                                                                                                                          | team leader, trưởng phòng | chưa tóm tắt rõ được yêu cầu từ team triển khai nhận được, phân quyền ưu tiên gửi đến nhân viên gây chậm tiến độ | Đo lường chất lượng bản tóm tắt và việc phân việc "đúng người" bằng chỉ số nào? (Trọng)                                                                                 |
| 9   | Thắng        | Bàn giao ca giữa các ca trực của bác sĩ cấp cứu                                                                                                                                                                                                                    | bác sĩ                    | tổng hợp thông tin bàn giao các ca mất thời gian vì theo dõi trên biên bản                                       | Nhóm có tiếp cận được bác sĩ thật và xem biên bản bàn giao thật để kiểm chứng trong buổi học hôm nay không? (Khải)                                                      |

### 2.2. Cluster

| Cluster                                                       | Các candidate                                                                                                                                           | Pattern chung                                                                                                                                             |
| ------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| A — Đọc hội thoại / biên bản rời rạc để trích xuất & bàn giao | #4 (Khải — gom thông tin khách & SP từ chat để tạo đơn), #8 (Thắng — tóm tắt yêu cầu chức năng phân việc), #9 (Thắng — bàn giao ca trực bác sĩ cấp cứu) | Thông tin đầu vào là ngôn ngữ tự nhiên nằm rải rác qua nhiều lượt trao đổi/ghi chép; người làm phải đọc lại, lọc thông tin mới nhất và điền vào mẫu chuẩn |
| B — Tra cứu đa nguồn & tổng hợp báo cáo                       | #5 (Khải — tra thông số SP & chính sách đổi trả), #6 (Khải — tra chéo khiếu nại đổi trả), #7 (Thắng — tổng hợp báo cáo tháng từ nhiều chuyên khoa)      | Dữ liệu nằm phân tán ở nhiều file/hệ thống khác nhau; tốn thời gian chuyển tab tra cứu, đối chiếu và tổng hợp lại                                         |
| C — Xử lý yêu cầu IT / cấp quyền lặp lại                      | #1 (Trọng — reset mật khẩu), #2 (Trọng — onboarding tài khoản nhân viên mới), #3 (Trọng — phân quyền truy cập tài nguyên)                               | Quy trình thao tác hệ thống theo các quy tắc cố định (if/else theo vai trò/phòng ban), nặng tính thủ công lặp lại                                         |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian nhân viên sales tạo đơn từ tin nhắn chốt hàng (từ 4 phút xuống dưới 1 phút/đơn) mà không tăng tỷ lệ nhập sai thông tin
├── Opportunity A: Thông tin khách chốt (mẫu, màu, size, SĐT, địa chỉ) nằm rải rác qua 10–20 tin nhắn chat, phải cuộn ngược lên tìm từng dòng
├── Opportunity B: Khách hay đổi ý (đổi màu/size, sửa địa chỉ) giữa chừng hoặc viết tắt địa chỉ khiến sales dễ copy nhầm tin nhắn cũ
└── Opportunity C: Phải chuyển qua lại giữa khung chat và phần mềm POS để copy-paste từng trường và chọn lại Tỉnh/Quận/Phường thủ công
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- _"Làm chatbot AI tự động chốt đơn và đẩy thẳng sang kho không cần nhân viên"_ (Solution — tự động hóa quá mức, rủi ro sai đơn cao).
- _"Tích hợp API tự động tạo đơn trên POS ngay khi khách nhắn SĐT"_ (Solution — tính năng kỹ thuật, chưa xét việc khách chưa chốt xong mẫu/size).

### 2.4. Chấm điểm shortlist (1–5)

| Candidate                                           | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng   |
| --------------------------------------------------- | -------- | ------------ | ------------------ | -------------- | ----------- | -------------------------------------- | ---------------- | ------ |
| **#4 — Tạo đơn từ hội thoại chat (Khải)**           | 5        | 5            | 4                  | 5              | 5           | 5                                      | 5                | **34** |
| **#2 — Onboarding tài khoản nhân viên mới (Trọng)** | 5        | 5            | 4                  | 4              | 4           | 3                                      | 4                | **29** |
| **#9 — Bàn giao ca trực bác sĩ cấp cứu (Thắng)**    | 5        | 4            | 3                  | 3              | 2           | 4                                      | 3                | **24** |

**Candidate được chọn:** **#4 — Tổng hợp thông tin khách hàng và sản phẩm từ hội thoại chat để tạo đơn hàng (Khải)**.

**Vì sao chọn:**

- Actor và quy trình 6 bước cực kỳ rõ ràng, diễn ra hàng chục lần mỗi ngày (25–40 đơn/ca).
- Có sẵn dữ liệu hội thoại chat mẫu để kiểm chứng ngay trong buổi lab mà không bị vướng rào cản bảo mật hệ thống nội bộ.
- Thể hiện rất rõ ranh giới giữa **No AI** (bắt khách điền form mẫu), **Rule** (dùng Regex bắt SĐT), **Workflow** (AI đọc đoạn chat rải rác để trích xuất JSON các trường tạo đơn + nhân viên kiểm duyệt) và **Agent**.

**Vì sao loại các candidate còn lại:**

- **#2 (Onboarding tài khoản nhân viên mới — Trọng):** Quy trình rất rõ nhưng bản chất là bài toán tự động hóa bằng Rule/Script (theo phòng ban/chức danh cố định), ít độ mơ hồ ngôn ngữ nên không khai thác sâu được bài toán đánh giá mức can thiệp AI.
- **#9 (Bàn giao ca trực bác sĩ cấp cứu — Thắng):** Pain rất lớn và ý nghĩa cao, nhưng rủi ro an toàn y khoa (Viability/Liability) cực kỳ nghiêm trọng và nhóm không thể tiếp cận bác sĩ hay hồ sơ bệnh án thật ngay trong buổi lab để kiểm chứng.

**Xử lý bất đồng (nếu có):**

- Ban đầu Thắng và Trọng ấn tượng với bài **#9 (Bàn giao ca trực bác sĩ)** và **#3 (Phân quyền truy cập)** vì nghe quy mô lớn. Sau khi nhóm thảo luận tiêu chí _"Vừa sức lab"_ và _"Khả năng kiểm chứng thật ngay trong buổi học"_, cả nhóm đồng thuận chọn bài **#4 (Tạo đơn từ hội thoại chat)** vì có người trong nhóm làm thực tế, đo thời gian bấm giờ được ngay và an toàn để chạy pilot.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| \#  | Giả định                                                                                                                                           | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước?      |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------- | ---------------- | ---------------------- | ---------------------- |
| 1   | Nhân viên trực page khác cũng mất trung bình 3–4 phút/đơn và gặp tình trạng nhập nhầm size/địa chỉ khi đơn dồn                                     | Value                                              | 5                | 2                      | ✅                     |
| 2   | Bước tốn thời gian nhất là cuộn đọc lại đoạn chat rải rác (khách đổi ý mẫu/màu/size, viết tắt địa chỉ), chứ không phải bước bấm lưu đơn trên POS   | Value                                              | 5                | 2                      | ✅                     |
| 3   | Bắt khách hàng điền lại vào "Form mẫu 1 tin nhắn" (No AI) sẽ bị phần lớn khách bỏ qua hoặc vẫn nhắn tách lẻ nhiều dòng                             | Usability                                          | 4                | 2                      | ✅                     |
| 4   | Dữ liệu đoạn chat (15–30 tin nhắn gần nhất) và danh mục mã SKU của shop có thể đưa vào prompt/API để trích xuất ra cấu trúc JSON chuẩn             | Feasibility                                        | 4                | 4                      | —                      |
| 5   | Chủ shop chấp nhận việc dùng công cụ AI đọc nội dung tin nhắn đặt hàng và chi phí API trên mỗi đơn không vượt quá lợi ích thời gian tiết kiệm được | Viability                                          | 4                | 2                      | Hỏi chủ shop / quản lý |

Giả định nhóm kiểm chứng trong buổi này: **Giả định #1, #2 và #3** (đều có mức độ Quan trọng cao 4–5 nhưng Bằng chứng ban đầu mới chỉ từ 1 cá nhân trong nhóm).

### 3.2. Kiểm chứng

Cách đã dùng: **Phỏng vấn nhanh (theo The Mom Test)** 2 nhân viên trực page/lên đơn TMĐT + **Kiểm tra log thật** 15 đoạn chat chốt đơn gần nhất của shop.

Interview snapshot — Người thứ 1:

| Trường                                            | Nội dung                                                                                                                                                                                                                                 |
| ------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Người được hỏi (vai trò, không ghi tên thật)      | Nhân viên trực page & lên đơn tại một shop thời trang nữ (quy mô 80–120 đơn/ngày trên Facebook & Shopee)                                                                                                                                 |
| Câu nói đáng nhớ nhất (nguyên văn)                | _"SĐT thì phần mềm nó tự bắt màu xanh rồi, cực nhất là khách hỏi 5 mẫu xong chốt 'lấy chị cái áo trắng đầu tiên nha nhưng đổi qua size L, còn quần thì giữ size M', lúc đông khách lướt lên tìm lại ảnh cái áo đầu tiên là hoa cả mắt."_ |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tối hôm qua (ca sale 20h–22h), lên nhầm màu Be sang màu Trắng cho khách vì khách nhắn đổi ý ở tin nhắn thứ 12 mà sales nhìn tin nhắn đầu                                                                                                 |
| Hiện đang xử lý bằng cách nào (workaround)?       | Mở 2 nửa màn hình (1 bên chat, 1 bên POS), vừa cuộn chat vừa gõ nháp mã hàng ra thanh chat trước rồi mới nhập vào đơn                                                                                                                    |
| Mất bao lâu, bao lần?                             | Đơn khách nhắn gọn mất \~1 phút; đơn khách tư vấn qua lại nhiều mẫu mất 3,5–5 phút/đơn (chiếm khoảng 60% số đơn trên Fanpage)                                                                                                            |
| Insight / opportunity rút ra                      | Phần mềm hiện tại đã tự bắt được SĐT (Rule), nhưng **hoàn toàn mù ngữ cảnh** khi khách chốt hàng bằng cách tham chiếu ngược (_"lấy mẫu đầu tiên"_, _"đổi cái kia sang size L"_) hoặc ghi chú giao hàng rải rác                           |

Interview snapshot — Người thứ 2:

| Trường                                            | Nội dung                                                                                                                                                                            |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Người được hỏi (vai trò, không ghi tên thật)      | Nhân viên CSKH kiêm tạo đơn tại shop phụ kiện & đồ gia dụng (40–60 đơn/ngày)                                                                                                        |
| Câu nói đáng nhớ nhất (nguyên văn)                | _"Mình từng gửi form mẫu kêu khách điền Họ tên - SĐT - Địa chỉ rồi, mà 10 người thì 7 người chỉ gõ mỗi SĐT với câu 'giao về địa chỉ cũ nha em' hoặc chụp ảnh danh thiếp gửi qua."_  |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Sáng nay, khách nhắn địa chỉ viết tắt tên phường/quận và dặn _"sau 5h chiều chuyển qua địa chỉ công ty"_, bạn sales bỏ sót câu dặn sau nên kho đóng đơn giao giờ hành chính bị hoàn |
| Hiện đang xử lý bằng cách nào (workaround)?       | Tự cuộn đọc lại từ đầu cuộc trò chuyện và copy từng câu ghép vào ô Ghi chú giao hàng                                                                                                |
| Mất bao lâu, bao lần?                             | Trung bình 3 phút/đơn; mỗi tuần bị sót ghi chú hoặc nhầm phân loại khoảng 2–3 đơn                                                                                                   |
| Insight / opportunity rút ra                      | Phương án No AI (gửi form bắt khách điền) chỉ hiệu quả với \~30% khách; 70% khách vẫn nhắn tự nhiên theo thói quen hội thoại                                                        |

Tổng hợp:

| Nguồn                          | Số người / số mẫu                 | Tín hiệu xác nhận                                                                                                                                          | Tín hiệu phản bác                                                                                                                                      |
| ------------------------------ | --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Phỏng vấn trực tiếp (Mom Test) | 2 nhân viên trực page/CSKH        | Cả 2 xác nhận mất 3–5 phút với các đơn tư vấn nhiều mẫu/đổi ý; gửi form mẫu (No AI) khách ít chịu điền theo chuẩn                                          | SĐT và khách cũ đã có phần mềm POS hỗ trợ bắt tự động bằng Rule; những đơn khách chỉ mua 1 mẫu cố định từ bài post chỉ mất \~45–60 giây (không cần AI) |
| Đếm từ log hội thoại thật      | 15 đơn chốt gần nhất trên Fanpage | 9/15 đơn (60%) thông tin mẫu/size/địa chỉ/ghi chú nằm rải rác từ 6 tin nhắn trở lên; 4/15 đơn khách có sửa lại màu/size hoặc địa chỉ sau khi đã chốt lần 1 | 6/15 đơn (40%) khách nhắn gọn trong 1–2 tin nhắn, dùng tính năng click-to-fill có sẵn của POS là đủ nhanh                                              |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

- **Thu hẹp phạm vi (Scope down):** Bỏ ý định "xây dựng hệ thống tạo đơn mới thay thế POS" hay "dùng AI bắt SĐT". Nhóm thu hẹp bài toán thành: **"Tổng hợp và chuẩn hóa thông tin chốt đơn cuối cùng (danh sách SKU + màu/size sau khi khách đã đổi ý, địa chỉ đầy đủ Tỉnh/Quận/Phường, và ghi chú giao hàng) từ các cuộc hội thoại tư vấn kéo dài"**.
- Phân tách rõ: Với \~40% đơn khách nhắn gọn 1 tin nhắn → dùng luôn tính năng Rule có sẵn của POS; chỉ dùng AI hỗ trợ cho \~60% đơn hội thoại dài/rải rác.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern                                                               | Link                                                       | Giải bước nào trong quy trình?                                                                                                                        | Điểm mạnh                                                                                                                                               | Khoảng trống / rủi ro                                                                                                                                   | Bài học cho nhóm                                                                                                                                             |
| -------------------------------------------------------------------------------------- | ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Pancake POS / Vpage** (Tính năng tạo đơn ngay trên khung chat & tự quét SĐT/Địa chỉ) | https://pancake.vn                                         | Bước 2 & một phần Bước 3: Đặt khung tạo đơn cạnh khung chat; dùng Rule/Regex tô sáng SĐT và click vào 1 tin nhắn để điền địa chỉ                      | Phổ biến tại VN, đồng bộ thẳng với kho và các ĐVVC (GHN, GHTK); bắt SĐT bằng Regex cực nhanh và chính xác                                               | Chỉ lấy được địa chỉ khi nằm gọn trong 1 tin nhắn; không tự đọc hiểu được khách chốt mẫu/màu/size nào trong đoạn chat dài hay khi khách đổi ý nhiều lần | Không tự xây lại giao diện POS hay bộ bắt SĐT. Tận dụng Rule cho SĐT, chỉ dùng AI cho phần đọc hiểu ngữ cảnh chốt SKU & chuẩn hóa địa chỉ/ghi chú            |
| **Sapo Social (Sapo Omni)** — Tạo đơn trên khung chat Facebook (phím tắt F1)           | https://www.sapo.vn/quan-ly-ban-hang-online.html           | Bước 2, 3 & 5: Tự đồng bộ thông tin nếu là khách cũ; xem tồn kho ngay khi gõ tìm SKU; gửi hóa đơn xác nhận vào chat                                   | Tự động lưu lịch sử địa chỉ khách cũ, tính phí ship các hãng vận chuyển ngay trên màn hình chat                                                         | Với khách mới hoặc khách mua nhiều phân loại rải rác trong chat, nhân viên vẫn phải tự đọc ngược hội thoại và gõ tìm từng mã SKU thủ công               | Cần tận dụng tính năng lưu khách cũ của POS và bước "Gửi hóa đơn xác nhận vào chat" làm chốt chặn kiểm tra cùng khách hàng                                   |
| **OpenAI Structured Outputs / Function Calling** (kết hợp n8n hoặc Chrome Extension)   | https://platform.openai.com/docs/guides/structured-outputs | Bước 1, 3, 4 & 5: Đọc 20 tin nhắn gần nhất → trích xuất ra đúng JSON Schema (`items[{sku, color, size, qty}]`, `address`, `note`, `confirmation_msg`) | Đảm bảo đầu ra luôn đúng 100% định dạng các trường dữ liệu cần điền; hiểu tốt ngữ cảnh tiếng Việt viết tắt và trường hợp khách đổi ý ở các tin nhắn sau | Rủi ro AI đoán nhầm mã SKU nếu tên sản phẩm trong chat quá chung chung (_"áo hôm qua"_); tốn độ trễ 2–3 giây                                            | Thiết kế dưới dạng Workflow (Augment): AI trích xuất ra bảng nháp + câu xác nhận đơn, nhưng nhân viên sales phải kiểm và bấm nút Lưu đơn (Human-in-the-loop) |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 6 bước, trung bình 240 giây (4 phút)/đơn hội thoại dài, 5/6 bước thủ công

[1 Cuộn ngược 15–30 câu chat tìm mẫu, màu, size cuối cùng & ghi chú: 75s] ← BOTTLENECK 1
→ [2 Mở khung POS & bắt SĐT tự động: 15s] (Rule có sẵn của POS)
→ [3 Đọc chat tìm địa chỉ viết tắt + chọn Tỉnh/Quận/Phường trên POS: 60s] ← BOTTLENECK 2
→ [4 Gõ tìm từng mã SKU, chọn phân loại màu/size, số lượng & ghi chú: 45s]
→ [5 Gõ lại tin nhắn tóm tắt đơn gửi vào chat để khách xác nhận: 30s]
→ [6 Bấm lưu đơn & đẩy sang kho/ĐVVC: 15s]
```

| Bước | Actor                | Input                                                                   | Output                                                                    | Thời gian / tần suất         | Ghi chú                                                           |
| ---- | -------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------- | ---------------------------- | ----------------------------------------------------------------- |
| 1    | Nhân viên sales      | Đoạn hội thoại chat (15–30 tin nhắn qua lại)                            | Xác định trong đầu (hoặc ghi nháp) mẫu, màu, size cuối cùng khách chốt    | \~75 giây/đơn · 25–40 đơn/ca | Hay nhìn nhầm tin nhắn cũ nếu khách đổi ý màu/size ở câu sau      |
| 2    | Phần mềm POS + Sales | Tin nhắn chứa SĐT của khách                                             | Điền SĐT và tên khách (nếu là khách cũ) vào khung tạo đơn                 | \~15 giây/đơn                | POS đã có sẵn Rule/Regex tự bắt SĐT                               |
| 3    | Nhân viên sales      | Tin nhắn địa chỉ (thường viết tắt tên phường/quận hoặc tách nhiều dòng) | Các trường Địa chỉ chi tiết, Tỉnh/Thành, Quận/Huyện, Phường/Xã trên POS   | \~60 giây/đơn                | Phải vừa nhìn chat vừa chọn lại từ 3 dropdown địa giới hành chính |
| 4    | Nhân viên sales      | Tên mẫu/màu/size đã xác định ở Bước 1 + yêu cầu giao hàng               | Giỏ hàng trên POS (đúng mã SKU, phân loại, số lượng) + ô Ghi chú kho/ship | \~45 giây/đơn                | Dễ gõ nhầm mã tương tự hoặc quên ghi chú giao hàng                |
| 5    | Nhân viên sales      | Thông tin đơn vừa nhập trên POS                                         | Tin nhắn tóm tắt đơn gửi lại cho khách trong khung chat                   | \~30 giây/đơn                | Gõ tay hoặc copy-paste lại từng dòng                              |
| 6    | Nhân viên sales      | Khách bấm OK xác nhận (hoặc chốt trên chat)                             | Đơn hàng trạng thái "Chờ xuất kho" chuyển sang bộ phận Kho                | \~15 giây/đơn                | Handoff sang Nhân viên kho đóng gói                               |

**Bottleneck chính:** **Bước 1 & Bước 3–4** (mất \~180 giây/240 giây): Nhân viên phải tự đọc ngược đoạn hội thoại dài để lọc ra lựa chọn **cuối cùng** của khách (sau khi đã hỏi nhiều mẫu, đổi màu/size) và chuyển đổi địa chỉ viết tắt sang đúng trường trên POS.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 5 bước, khoảng 55 giây/đơn hội thoại dài, 2/5 bước thủ công

[1 Tự bắt SĐT + lấy lịch sử khách cũ + gom 25 tin nhắn gần nhất: 3s] ← RULE / SCRIPT
→ [2 Trích xuất JSON đơn nháp (SKU, màu, size cuối, Địa chỉ 3 cấp, Ghi chú) + Soạn câu xác nhận: 4s] ← AI (Structured Outputs)
→ [3 Điền sẵn vào form nháp POS & highlight trường thiếu/mơ hồ: 3s] ← RULE
→ [4 Sales kiểm tra bảng nháp, gửi câu xác nhận cho khách & bấm Lưu đơn: 35s] ← CON NGƯỜI (HITL)
→ [5 Đẩy đơn sang kho: 10s] ← RULE / CON NGƯỜI

BOUNDARY:
- AI KHÔNG tự động bấm "Tạo đơn / Đẩy sang kho" và KHÔNG tự sửa giá bán/phí ship hay tồn kho.
- Nếu khách chưa nói rõ màu/size hoặc địa chỉ thiếu Phường/Xã, AI phải để trống (`null`) kèm cảnh báo đỏ để Sales hỏi lại khách, tuyệt đối không tự đoán.

PHƯƠNG ÁN QUAY VỀ (Fallback):
- Nếu AI trích xuất sai hoặc API quá 5 giây không phản hồi → Sales tắt gợi ý nháp và dùng thao tác click-to-fill + chọn SKU thủ công trên POS như quy trình cũ.
```

### 4.3. Before / after

| Chỉ số               | Trước                                                     | Sau (kỳ vọng)                                                                    | Ghi chú                                                                                             |
| -------------------- | --------------------------------------------------------- | -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Số bước              | 6 bước                                                    | 5 bước                                                                           | Gộp bước đọc lọc hội thoại, chuẩn hóa địa chỉ và soạn tin nhắn xác nhận                             |
| Tổng thời gian       | \~240 giây (4 phút)/đơn                                   | \~55 giây (&lt; 1 phút)/đơn                                                      | Áp dụng cho nhóm đơn hội thoại dài (\~60% tổng đơn Fanpage)                                         |
| Số bước thủ công     | 5/6 bước                                                  | 2/5 bước                                                                         | Sales chỉ kiểm tra bản nháp và bấm xác nhận tạo đơn                                                 |
| Bottleneck chính     | Cuộn đọc chat tìm chốt cuối & nhập lại địa chỉ/SKU (180s) | Sales đọc kiểm tra bảng nháp & chờ khách xác nhận (35s)                          | Bottleneck chuyển sang bước kiểm soát chất lượng (chấp nhận được)                                   |
| Rủi ro mới phát sinh | —                                                         | AI map nhầm mã SKU gần giống tên hoặc lấy nhầm tin nhắn cũ trước khi khách đổi ý | Kiểm soát bằng Boundary (không tự lưu đơn), hiển thị trích dẫn câu chat gốc và bắt buộc Sales duyệt |

---

## 5. Problem Statement v0 (CP5)

| Trường                                                                     | Nội dung                                                                                                                                                                                 |
| -------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Actor**                                                                  | Nhân viên sales trực page kiêm lên đơn tại các shop thương mại điện tử bán qua Fanpage/Zalo                                                                                              |
| **Quy trình**                                                              | Trong ca trực: đọc ngược đoạn chat tư vấn → bắt SĐT → nhập địa chỉ Tỉnh/Quận/Phường → tìm chọn mã SKU/màu/size và ghi chú trên POS → nhắn lại khách xác nhận → bấm lưu đơn chuyển kho    |
| **Bottleneck**                                                             | Bước cuộn đọc lại 15–30 tin nhắn rời rạc để xác định đúng sản phẩm/màu/size cuối cùng khách chốt và chuẩn hóa địa chỉ viết tắt sang POS (mất \~3 phút/đơn)                               |
| **Impact**                                                                 | Mất \~100–120 phút/ca cho 30 đơn; gây ùn ứ tin nhắn giờ cao điểm (12h–14h, 20h–22h); trung bình 2–3 đơn/tuần bị nhập nhầm phân loại màu/size hoặc sót ghi chú giao hàng dẫn đến hoàn đơn |
| **Success Metric** (baseline → target, cách đo)                            | Thời gian tạo 1 đơn giảm từ trung bình 4 phút (đo bằng bấm giờ 15 đơn gần nhất) xuống dưới 1 phút, đo bằng tự bấm giờ trong 2 tuần pilot                                                 |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ tạo bản nháp đơn hàng và câu nhắn xác nhận; không tự động lưu đơn đẩy sang kho, không tự đoán màu/size khi khách chưa nói rõ; nhân viên sales bắt buộc kiểm tra và bấm lưu        |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **Phản biện 1 (từ AI đóng vai PM hoài nghi):** _"Actor đang viết cho mọi đơn hàng trên Fanpage, nhưng ở CP4 nhóm đã thấy 40% đơn khách nhắn gọn 1 dòng chỉ mất 45–60 giây bằng Rule có sẵn của POS. Nếu gộp chung vào baseline thì metric sẽ bị nhiễu."_ → **Nhóm đồng ý:** Sửa lại Actor và phạm vi ở v1, chỉ tập trung vào các cuộc hội thoại tư vấn kéo dài (≥ 6 tin nhắn hoặc có nhiều mẫu/đổi ý).
- **Phản biện 2 (từ AI & thành viên nhóm):** _"Success Metric ở v0 mới chỉ đo tốc độ (từ 4 phút xuống dưới 1 phút). Nếu nhân viên ỷ lại vào bản nháp AI, bấm duyệt nhanh mà không đọc kỹ làm tăng số đơn giao sai màu/size thì sao?"_ → **Nhóm đồng ý:** Bổ sung thêm 2 chỉ số chất lượng ở v1: (1) Tỷ lệ trường thông tin AI trích xuất đúng ngay lần đầu (không phải sửa tay) đạt ≥ 85%; (2) Số đơn bị nhập sai SKU/địa chỉ giảm từ 2–3 đơn/tuần xuống ≤ 1 đơn/tuần.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ CAO × Độ phức tạp THẤP–TRUNG BÌNH**.

Vì sao:

- **Độ mơ hồ cao ở đầu vào ngôn ngữ:** Khách hàng Việt Nam nhắn tin chốt đơn không theo cấu trúc cố định (viết tắt _"đc: 12 ngõ 5 CG, HN"_, tham chiếu ngược _"lấy cái màu đen lúc đầu nhưng lên size L nhé"_, dặn dò rải rác _"giao sau 18h giúp chị"_), nên Rule/Regex thông thường không bắt hết được.
- **Độ phức tạp quy trình thấp–trung bình:** Luồng công việc cố định (Đọc đoạn chat → Trích xuất ra đúng 6 trường dữ liệu của đơn → Kiểm tra tồn kho/SKU → Nhân viên duyệt → Lưu đơn). Không cần hệ thống tự lập kế hoạch nhiều vòng hay tự gọi công cụ ngoài phạm vi.

### 6.2. So sánh 4 mức

| Mức                       | Phương án cho bài của nhóm                                                                                                                             | Đủ khi nào                                                                                               | Rủi ro                                                                                                                    | Chọn?                                    |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| **No AI** (sửa quy trình) | Gửi tin nhắn Form mẫu cố định (_Họ tên - SĐT - Địa chỉ - Màu/Size_) yêu cầu khách điền lại trước khi chốt                                              | Khi khách hàng chịu hợp tác điền đúng form 1 tin nhắn (\~30% khách)                                      | 70% khách ngại gõ lại form hoặc vẫn nhắn tách lẻ nhiều câu; gây cảm giác cứng nhắc làm giảm tỷ lệ chốt                    | Chỉ dùng bổ trợ                          |
| **Rule**                  | Dùng Regex có sẵn của Pancake/Sapo để tự bắt SĐT 10 số, tự lấy lại địa chỉ khách cũ và click-to-fill 1 dòng                                            | Khi khách cũ mua lại hoặc khách chỉ mua 1 sản phẩm cố định và nhắn gọn trong 1–2 tin nhắn (\~40% số đơn) | Không hiểu được khi khách đổi ý màu/size giữa chừng hoặc địa chỉ chia nhiều tin nhắn                                      | **Dùng cho Bước 1** (bắt SĐT & khách cũ) |
| **Workflow**              | Rule lấy SĐT + gom 25 câu chat → **AI trích xuất ra JSON chuẩn** (SKU, màu, size cuối, địa chỉ 3 cấp, ghi chú) + câu xác nhận → Sales duyệt và bấm lưu | Khi hội thoại tư vấn kéo dài, khách hỏi nhiều mẫu hoặc thay đổi lựa chọn trước khi chốt (\~60% số đơn)   | AI có thể ánh xạ nhầm tên gọi thông thường trong chat sang mã SKU nếu danh mục tên SP quá giống nhau                      | **Chọn (Mức chính)**                     |
| **Agent**                 | Chatbot AI tự động tư vấn, tự mặc cả, tự chốt đơn và đẩy thẳng đơn sang kho/vận chuyển không cần nhân viên                                             | Khi shop bán mặt hàng đồng nhất 100%, không cần tư vấn cá nhân hóa và chấp nhận rủi ro đơn ảo/sai đơn    | Rủi ro rất cao: tự tạo đơn sai màu/size đẩy sang kho gây tốn phí ship 2 chiều; mất kiểm soát khi khách hỏi ngoài kịch bản | Không chọn                               |

**Mức chọn:** **Workflow** (kết hợp **Rule** ở bước bắt SĐT/khách cũ và **AI** ở bước trích xuất thông tin chốt đơn từ đoạn hội thoại sang JSON, có **Con người** duyệt cuối).

**Vì sao không chọn mức đơn giản hơn:**

- Kiểm chứng ở CP4 (phỏng vấn 2 nhân viên + kiểm 15 đơn thật) cho thấy **Rule** có sẵn trên Pancake/Sapo đã giải quyết tốt phần bắt SĐT và \~40% đơn nhắn gọn, nhưng bất lực trước **60% đơn có hội thoại tư vấn dài** (khách đổi ý màu/size hoặc nhắn rải rác). Trong khi đó, phương án **No AI** (gửi form bắt khách điền lại) bị \~70% khách bỏ qua. Vì vậy cần **Workflow có AI ở bước đọc hiểu hội thoại** để giải quyết đúng nút thắt 180 giây này mà vẫn an toàn hơn **Agent**.

### 6.3. AI Canvas rút gọn

| Thành phần                                                        | Nội dung                                                                                                                                                                                                                                                                                              |
| ----------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Prediction** — AI dự đoán / tạo ra gì?                          | Trích xuất từ đoạn chat ra đối tượng JSON chuẩn gồm: (1) Danh sách sản phẩm chốt cuối (`sku`, `color`, `size`, `quantity`), (2) Địa chỉ chuẩn hóa 3 cấp (`tinh`, `quan`, `phuong`, `so_nha`), (3) `ghi_chu_giao_hang`, (4) Trường còn thiếu (`missing_fields`), và (5) Tin nhắn tóm tắt đơn gửi khách |
| **Judgment** — con người cân nhắc, quyết định gì?                 | Nhân viên sales đối chiếu nhanh bảng nháp với câu chat được trích dẫn, kiểm tra các trường AI báo thiếu/mơ hồ và quyết định có áp dụng ưu đãi/freeship riêng cho khách hay không                                                                                                                      |
| **Action** — hành động cuối cùng là gì, ai làm?                   | Nhân viên sales gửi tin nhắn xác nhận cho khách và bấm nút **"Tạo đơn"** trên POS để đẩy sang kho                                                                                                                                                                                                     |
| **Outcome** — đo kết quả bằng gì?                                 | (1) Thời gian trung bình tạo 1 đơn hội thoại dài; (2) Tỷ lệ trường thông tin AI điền đúng không cần sửa tay; (3) Số đơn giao sai màu/size/địa chỉ mỗi tuần                                                                                                                                            |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | (1) Text 20–25 tin nhắn gần nhất của hội thoại hiện tại; (2) Danh mục SKU rút gọn của các sản phẩm đang bán trong chiến dịch (Mã SKU, Tên gọi, Màu, Size). **Đều có sẵn** ngay trên trình duyệt/POS                                                                                                   |
| **Feedback** — lấy phản hồi ở đâu để cải thiện?                   | Ghi log những trường mà nhân viên sales phải sửa lại bằng tay trên bảng nháp (ví dụ: AI chọn sai mã SKU hoặc tách sai Phường/Xã) để cập nhật từ điển đồng nghĩa sản phẩm trong prompt                                                                                                                 |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
    - **Augment (Hỗ trợ điền sẵn bản nháp để duyệt).** Cả 2 nhân viên được phỏng vấn ở CP4 đều khẳng định không dám để công cụ tự đẩy đơn thẳng sang kho vì chỉ cần sai 1 chữ số điện thoại hoặc nhầm size M sang L là shop mất ngay 30.000–60.000đ phí ship hoàn 2 chiều và bị khách mắng. Họ chỉ muốn có bảng điền sẵn để đọc lướt 10 giây rồi tự bấm Tạo đơn.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
    - **Điền nhầm (False Positive — tự đoán bừa màu/size/địa chỉ khi khách nói mơ hồ) tệ hơn nhiều so với Để trống báo thiếu (False Negative).**
    - _Vì sao:_ Nếu AI không chắc mà để trống và tô vàng ô "Size", nhân viên sales nhìn thấy ngay trong 2 giây để hỏi lại khách. Ngược lại, nếu AI tự đoán điền đại "Size M" vào ô nhìn giống như đã đủ thông tin, nhân viên dễ chủ quan bấm duyệt luôn → đóng gói giao sai hàng.
    - _Thiết kế xử lý:_ Ràng buộc trong System Prompt & JSON Schema: mọi trường không có thông tin rõ ràng trong chat phải trả về `null` kèm mảng `missing_fields` tô màu cảnh báo đỏ; đồng thời hiển thị câu chat gốc (`source_quote`) ngay dưới mỗi sản phẩm được trích xuất để sales đối chiếu mắt.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường                                          | Nội dung                                                                                                                                                                                                                                                                      |
| ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Actor**                                       | Nhân viên sales trực page kiêm lên đơn tại shop TMĐT (Fanpage/Zalo), xét riêng khi xử lý các cuộc hội thoại tư vấn kéo dài (≥ 6 tin nhắn hoặc khách hỏi nhiều mẫu/đổi ý)                                                                                                      |
| **Quy trình**                                   | Bắt SĐT tự động (Rule) → Gom đoạn hội thoại + trích xuất thông tin chốt đơn (AI) → Điền nháp vào form tạo đơn → Nhân viên kiểm tra, gửi xác nhận cho khách & bấm lưu đơn chuyển kho                                                                                           |
| **Bottleneck**                                  | Đọc ngược 15–30 tin nhắn rời rạc để lọc ra đúng sản phẩm/màu/size cuối cùng khách chốt và chuẩn hóa địa chỉ viết tắt sang POS (mất \~3 phút/đơn)                                                                                                                              |
| **Impact**                                      | Mất \~100–120 phút/ca trực; ùn ứ phản hồi giờ cao điểm; trung bình 2–3 đơn/tuần bị nhập nhầm màu/size hoặc sót ghi chú giao hàng gây tốn phí hoàn đơn                                                                                                                         |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian tạo đơn hội thoại dài giảm từ **4 phút xuống dưới 1 phút/đơn**; (2) **≥ 85% số đơn nháp** nhân viên chỉ cần sửa tối đa 1 trường trước khi lưu; (3) Số đơn nhập sai SKU/địa chỉ giảm từ **2–3 đơn/tuần xuống ≤ 1 đơn/tuần** (đo trong 2 tuần pilot trên 100 đơn) |
| **Boundary**                                    | AI không tự động bấm lưu đơn/đẩy kho, không tự sửa giá bán/khuyến mãi, không tự đoán màu/size/địa chỉ khi khách chưa nhắn rõ (phải trả về `null` và cảnh báo)                                                                                                                 |
| **AI intervention point**                       | Ngay sau khi khách nhắn chốt mua (và Rule đã bắt được SĐT), trước bước nhân viên sales nhập các trường Sản phẩm, Địa chỉ, Ghi chú vào POS                                                                                                                                     |
| **Mức chọn**                                    | **Workflow** (Rule bắt SĐT + AI trích xuất JSON từ đoạn chat + Con người kiểm duyệt)                                                                                                                                                                                          |
| **Rủi ro & người kiểm tra**                     | Rủi ro AI lấy nhầm phân loại ở tin nhắn cũ (trước khi khách đổi ý) hoặc map nhầm tên sản phẩm gần giống → **Nhân viên sales** kiểm tra qua dòng trích dẫn câu chat gốc (`source_quote`) và tin nhắn xác nhận gửi khách trước khi bấm Lưu đơn                                  |

**Thay đổi so với v0 và lý do:**

| Trường              | v0                                                     | v1                                                                                                        | Vì sao đổi                                                                                                           |
| ------------------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **Actor / Phạm vi** | Nhân viên sales trực page khi tạo mọi đơn hàng từ chat | Thu hẹp vào các cuộc hội thoại tư vấn kéo dài (≥ 6 tin nhắn hoặc có đổi ý)                                | Kiểm chứng CP4 cho thấy 40% đơn nhắn gọn 1 dòng chỉ mất 45–60s bằng Rule có sẵn của POS, không cần gọi AI            |
| **Success Metric**  | Chỉ đo thời gian tạo đơn (4 phút → dưới 1 phút)        | Thêm tỷ lệ đơn nháp điền đúng (≥ 85%) và số đơn sai thông tin/tuần (≤ 1 đơn)                              | Phản biện CP5 chỉ ra nếu làm nhanh nhưng nhân viên phải sửa lại nhiều hoặc tăng tỷ lệ sai đơn thì giải pháp thất bại |
| **Boundary**        | Không tự lưu đơn, không tự đoán màu/size               | Cụ thể hóa cơ chế kỹ thuật: trả về `null` + tô đỏ `missing_fields` + kèm câu trích dẫn gốc `source_quote` | Trả lời câu hỏi Google PAIR: tránh lỗi "điền nhầm" gây chủ quan cho người duyệt                                      |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| \#  | Tiêu chí                                              | Đạt khi                                                                                                                            | Không đạt khi                                                                                                    |
| --- | ----------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 1   | **Đúng lựa chọn cuối cùng (Latest Intent)**           | Lấy đúng mẫu, màu, size, số lượng ở tin nhắn chốt **cuối cùng** của khách (bỏ qua các mẫu khách chỉ hỏi hoặc đã đổi ý trước đó)    | Lấy nhầm màu/size ở tin nhắn cũ trước khi khách đổi ý hoặc gộp cả mẫu khách chỉ hỏi giá vào đơn                  |
| 2   | **Không tự bịa thông tin thiếu (Zero Hallucination)** | Mọi trường khách chưa nói rõ (ví dụ: mới nói "lấy áo sơ mi trắng" nhưng chưa báo size) đều để `null` và liệt kê vào `missing_fields` | Tự ý điền đại một giá trị (size M, màu đen, hoặc tự thêm tên Phường/Xã không có trong chat)                      |
| 3   | **Chuẩn hóa đúng địa chỉ & ghi chú**                  | Tách đúng Số nhà/Đường, Phường/Xã, Quận/Huyện, Tỉnh/Thành phố từ câu viết tắt và gom đủ yêu cầu giao hàng vào ô `ghi_chu`          | Làm mất số nhà/ngõ hoặc bỏ sót lời dặn giao hàng của khách (như _"giao giờ hành chính"_, _"gọi trước khi giao"_) |
| 4   | **Đúng định dạng JSON & tốc độ phản hồi**             | Trả về đúng 100% JSON Schema quy định kèm tin nhắn xác nhận lịch sự trong thời gian **≤ 4 giây**                                   | Lỗi cú pháp JSON, thiếu trường bắt buộc hoặc thời gian chờ &gt; 5 giây làm ngắt mạch thao tác của sales          |

**Bộ Eval mẫu (10 cặp Input/Output kiểm thử thực tế):** xem chi tiết tại [report/assets/cp6-eval-dataset.md](../assets/cp6-eval-dataset.md).

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro          | Câu hỏi                                                           | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng                                                                                                                                                                              |
| --------------- | ----------------------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Value**       | Người dùng có thật sự cần và sẽ dùng không?                       | **Thấp**                                              | Đã kiểm chứng qua log 15 đơn thật (60% là hội thoại dài) và phỏng vấn 2 sales trực page đều xác nhận đây là bước mỏi mắt, dễ nhầm nhất trong ca trực                                            |
| **Usability**   | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Thấp**                                              | Đầu ra là bảng các trường tạo đơn quen thuộc kèm câu trích dẫn ngắn và tin nhắn xác nhận; sales chỉ đọc lướt và sửa trực tiếp nếu cần                                                           |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không?                     | **Thấp**                                              | Đoạn hội thoại và bảng mã SKU đã có sẵn; API LLM hỗ trợ Structured Outputs (JSON Schema) giải quyết rất tốt bài toán trích xuất thực thể tiếng Việt                                             |
| **Viability**   | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành?     | **Trung bình**                                        | Chi phí API rất thấp (\~20–40đ/đơn với model nhỏ như GPT-4o-mini / Gemini Flash), nhưng cần chủ shop đồng ý cho phép gửi đoạn text chat chốt đơn qua API (đã che/ẩn thông tin nhạy cảm nếu cần) |

### 8.2. Kết luận

**Quyết định:** **Go** (triển khai thử nghiệm phạm vi nhỏ — Pilot trong 2 tuần).

**Lý do:**

- Cả 3 rủi ro Value, Usability, Feasibility đều ở mức **Thấp** (đã có bằng chứng từ log đơn hàng thật và phỏng vấn). Rủi ro Viability ở mức **Trung bình** nhưng hoàn toàn kiểm soát được bằng cách chỉ gửi 20 câu chat cuối (không lưu trữ dữ liệu khách hàng bên ngoài) và dùng model chi phí thấp.

**Nếu Go — pilot nhỏ nhất:**

- **Phạm vi Pilot (2 tuần, không cần tích hợp sâu vào mã nguồn POS ngay):**
    - Tuần 1 (30 đơn hội thoại dài): Nhân viên sales bôi đen đoạn chat tư vấn → bấm phím tắt (qua tiện ích bookmarklet/extension nhỏ hoặc khung prompt chuẩn đã nạp sẵn danh mục 50 SKU chủ lực của shop) → nhận bảng thông tin trích xuất + câu nhắn xác nhận đơn để paste vào POS và gửi khách.
    - Tuần 2 (70 đơn tiếp theo): Đo thời gian bấm giờ thực tế, đếm số trường phải sửa tay và số đơn bị khiếu nại sai màu/size/địa chỉ.

**Nếu Not Yet — cần kiểm chứng gì trước:**

- _(Không áp dụng vì nhóm chọn Go phạm vi nhỏ; tuy nhiên trước ngày chạy Pilot cần xác nhận với chủ shop về quy định bảo mật thông tin SĐT/địa chỉ khách hàng khi gọi API)._

**Nếu No-Go — nên làm gì thay AI:**

- _(Không áp dụng)._

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

- Nếu sau **50 đơn đầu tiên trong tuần 1**, có **trên 25% số đơn nháp** nhân viên sales phải sửa lại từ 2 trường trở lên, HOẶC thời gian trung bình vẫn **trên 2 phút/đơn** → **Dừng Pilot**, quay về phương án sử dụng tính năng click-to-fill có sẵn của Pancake/Sapo kết hợp bảng phím tắt mã SKU chuẩn.
- Nếu phát sinh **bất kỳ đơn hàng nào** bị giao sai sản phẩm/địa chỉ do lỗi trích xuất của AI mà nhân viên không phát hiện ra ở bước duyệt → **Dừng ngay lập tức** để thiết kế lại giao diện cảnh báo bắt buộc tick xác nhận từng dòng SKU.

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế hiện tại:**
    - Mẫu kiểm chứng ở CP4 mới thực hiện trên 15 đơn hàng thật của 1 shop và phỏng vấn 2 nhân viên trực page, cần đo thêm ở các ngành hàng có số lượng SKU lớn hơn (như mỹ phẩm, linh kiện điện tử).
    - Pilot hiện tại mới xử lý tin nhắn văn bản (text), chưa xử lý trường hợp khách hàng gửi ảnh chụp màn hình sản phẩm hoặc gửi ảnh chụp danh thiếp ghi địa chỉ mà không gõ chữ.
- **Hướng tiếp theo:**
    - Sau 2 tuần pilot đạt target (&lt; 1 phút/đơn, ≥ 85% đơn nháp đúng), đóng gói thành Chrome Extension gắn trực tiếp cạnh màn hình Pancake/Sapo để tự động điền vào ô input của POS chỉ bằng 1 cú click.
    - Mở rộng sang candidate **#5 (Gợi ý câu trả lời thông số sản phẩm & tư vấn size)** và **#6 (Tra cứu chéo khi xử lý khiếu nại đổi trả)** đã xác định ở CP3.

## 10. Tài liệu tham khảo

- Tài liệu hướng dẫn Pancake POS & Vpage — Quản lý hội thoại và tạo đơn từ tin nhắn Fanpage: https://pancake.vn
- Sapo Social (Sapo Omni) — Tính năng tạo đơn hàng trực tiếp trên khung chat Facebook: https://www.sapo.vn/quan-ly-ban-hang-online.html
- OpenAI Platform Documentation — Structured Outputs (đảm bảo phản hồi tuân thủ JSON Schema): https://platform.openai.com/docs/guides/structured-outputs
- Anthropic — _Building Effective Agents_ (phân biệt Workflow và Agent): https://www.anthropic.com/research/building-effective-agents
- Rob Fitzpatrick — _The Mom Test_ (nguyên tắc phỏng vấn kiểm chứng vấn đề thực tế).
- Teresa Torres — _Continuous Discovery Habits_ (Opportunity Solution Tree & Interview Snapshot).
