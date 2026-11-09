# Báo cáo cá nhân — 2A202603671_PhamQuynhAnh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Phạm Quỳnh Anh 
- MSSV:2A202603671
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:xyz
- Link repo nhóm:https://github.com/ducminh03/K5-L3A-DAY02-xyz-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc tổng hợp nhiều thông tin  |Khi ôn thi cuối kì tôi cần tổng hợp lại toàn bộ kiến thức cốt lõi để có thể ghi nhớ nhanh chóng   |Sinh viên đại học |mất 4-5 tiếng để ngồi xem lại toàn bộ slide bài giảng để tổng hợp công thức |
| 2 |Lặp lại| Khi phát sinh các khoản chi tiêu nhỏ lẻ trong ngày(tiền ăn, tiền gửi xe, tiền mua đồ), tôi muốn ghi nhận lại số tiền và phân loại vào các khoản mục, để kiểm soát chi tiêu hàng tháng mà không phải nhớ lại và cộng trừ lại vào cuối ngày|Cá nhân |Mất khoảng 15-20p mỗi ngày để tổng hợp lại chi tiêu |
| 3 |Lặp lại |Khi khách hàng muốn hỏi thông tin sản phẩm(giá, kích thước,...)tôi muốn cung cấp thông tin cho khách hàng mà không phải trực page  |Chủ cửa hàng | Tỷ lệ rớt đơn khoảng 40% vào khung giờ 22-7h sáng do khách hàng đợi quá lâu không thấy trả lời|
| 4 |Lặp lại |Khi tập gym/giảm cân, tôi muốn ước tính nhanh lượng calo và protein của suất ăn để điều chỉnh lượng chế độ ăn trong ngày   |Cá nhân  | Mất khoảng 15p mỗi bữa ăn để tra cứu calo cho từng món|
| 5 | Cần đọc, tổng hợp nhiều thông tin|Khi đăng ký tín chỉ vào ngày mở cổng, tôi muốn so sánh nhanh thời khóa biểu của 8‑10 lớp để tránh trùng lịch, để có lịch học hợp lý mà không phải ngồi 2 đêm trên Excel.| Sinh viên| Mất ≈ 4 giờ (2 đêm) dò danh sách lớp; 1 lần trùng giờ → phải đổi lớp, gây lãng phí 1 tuần học.|
| 6 |Pain từ người khác | Khi đối chiếu đơn hàng COD với báo cáo vận chuyển hàng tuần, tôi muốn so khớp nhanh mã đơn và số tiền thực nhận để phát hiện sai lệch, để không để mất tiền công ty.| Chủ shop, nhân viên kế toán|Mất 3‑4 giờ mỗi tuần kiểm tra 500 đơn; 2‑3 đơn có sai lệch > 5 % giá trị. |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Trả lời thông tin sản phẩm và tư vấn khách hàng ngoài giờ hành chính (bán hàng online)	 |ảnh hưởng trực tiếp đến doanh thu cửa hàng |Chưa chắc mức độ sẵn sàng mua hàng thực tế của khách|
| 2 |Ghi nhận và phân loại chi tiêu nhỏ lẻ hàng ngày	 |vấn đề ai cũng từng gặp | Chưa chắc người dùng có duy trid thói quen nhập liệu lâu dài hay không |
| 3 |Tổng hợp kiến thức và công thức cốt lõi từ slide bài giảng khi ôn thi| nhu cầu cấp thiết của sinh viên| dữ liệu slide bài giảng nhiều thông tin, lộn xộn|

### Problem Card #1 — Trả lời thông tin sản phẩm và tư vấn khách hàng ngoài giờ hành chính

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách hàng nhắn tin hỏi thông tin sản phẩm (giá, kích thước, tình trạng còn hàng) ngoài giờ hành chính (22h–7h), tôi (chủ shop) muốn cung cấp thông tin chính xác và tư vấn tức thì cho khách, để giữ chân khách mua hàng mà tôi không phải thức đêm trực page. |
| Actor | Chủ cửa hàng online, nhân viên trực page, khách mua hàng ban đêm |
| Thời điểm / bối cảnh | Khung giờ từ 22h đêm đến 7h sáng hôm sau, khi chủ shop ngủ hoặc không có nhân viên trực ca |
| Quy trình hiện tại (3–7 bước) | 1. Khách gửi tin nhắn hỏi thông tin món hàng qua Messenger/Zalo.<br>2. Sáng hôm sau (8h–9h), chủ shop/nhân viên mở tin nhắn đọc.<br>3. Kiểm tra kho/bảng giá xem còn hàng không.<br>4. Soạn tin nhắn trả lời khách kèm hình ảnh và báo giá.<br>5. Chờ khách phản hồi (thường khách đã xem nơi khác hoặc đổi ý). |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2 và Bước 4**: Độ trễ phản hồi qua đêm quá lớn (chậm từ 6–8 tiếng). Khách hàng mua sắm theo cảm xúc ban đêm, đợi quá 15 phút không thấy phản hồi là chuyển sang shop đối thủ. |
| Impact (nếu không giải thì sao) | Mất 40% khách hàng tiềm năng vào ban đêm; làm giảm doanh thu của cửa hàng ước tính khoảng 10–20% doanh thu tháng; lãng phí ngân sách chạy quảng cáo vì khách click vào nhưng không được tư vấn kịp thời. |
| Success metric (baseline → target) | - Thời gian phản hồi lần đầu (FRT): Từ 6–8 tiếng → giảm xuống dưới 1 phút.<br>- Tỷ lệ rớt đơn ban đêm: Từ 40% → giảm xuống dưới 15%. |
| Phương án không dùng AI | Dùng tính năng tin nhắn tự động có sẵn của Facebook/Zalo (Auto-responder) với menu nút bấm cố định theo danh mục (Bảng giá, Bảng size, Địa chỉ cửa hàng). |
| Giả thuyết về AI (nếu có) | AI (Workflow) đọc hiểu câu hỏi ngôn ngữ tự nhiên của khách (kể cả viết tắt, hỏi phối đồ), tra cứu bảng tồn kho và giá hiện tại để trả lời chuẩn xác, trường hợp phức tạp thì gắn tag để nhân viên xử lý vào sáng hôm sau. |
| Cảm nhận nhanh | **Workflow** (kết hợp Rule tra kho + AI xử lý ngôn ngữ tự nhiên câu hỏi của khách) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — Trễ 6–8 tiếng (mất khách ban đêm)

[1. Khách nhắn hỏi sản phẩm lúc 23h] 
    │
    ▼ (Chờ qua đêm 6–8 tiếng — BOTTLENECK)
[2. 08:00 Sáng hôm sau: Nhân viên mở tin nhắn] ──(2 phút)──▶ [3. Tra kho & bảng giá] 
    │
    ▼
[4. Soạn tin nhắn trả lời] ──(3 phút)──▶ [5. Khách đã mua shop khác / Không xem tin nhắn]
Tổng thời gian trễ: ~8 tiếng
```

### Problem Card #2 — Ghi nhận và phân loại chi tiêu nhỏ lẻ hàng ngày

| Trường | Nội dung |
|---|---|
| Job Story | Khi phát sinh các khoản chi tiêu nhỏ lẻ trong ngày (tiền ăn, gửi xe, cà phê, tạp hóa), tôi muốn ghi nhận lại số tiền và danh mục chi tiêu chỉ trong vài giây, để kiểm soát ngân sách tháng mà không phải mất công nhớ lại và cộng trừ thủ công vào cuối ngày. |
| Actor | Cá nhân, sinh viên, người mới đi làm |
| Thời điểm / bối cảnh | Ngay sau khi vừa rút tiền mặt hoặc chuyển khoản quét mã QR thanh toán |
| Quy trình hiện tại (3–7 bước) | 1. Thanh toán tiền (tiền mặt hoặc chuyển khoản QR).<br>2. Cất ví/điện thoại, tiếp tục công việc.<br>3. Đến tối trước khi ngủ, cố gắng nhớ lại hôm nay đã tiêu những gì.<br>4. Mở app ghi chú hoặc file Excel cá nhân.<br>5. Gõ từng dòng chi tiêu và tự cộng tổng số tiền.<br>6. So sánh với số dư thực tế trong tài khoản (thường bị lệch). |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 3 và Bước 5**: Mất 15–20 phút mỗi tối để nhớ lại và nhập liệu; thường xuyên quên mất các khoản lặt vặt (5k gửi xe, 15k nước mía), dẫn đến nản lòng và bỏ cuộc sau vài ngày. |
| Impact (nếu không giải thì sao) | Bị "cháy túi" vào cuối tháng mà không hiểu tiền đi đâu; không có thói quen quản lý tài chính; căng thẳng khi phát sinh chi phí đột xuất. |
| Success metric (baseline → target) | - Thời gian ghi nhận mỗi giao dịch: Từ 15 phút tổng hợp buổi tối → giảm xuống dưới 10 giây ngay lúc tiêu.<br>- Tỷ lệ duy trì ghi chép liên tục: Từ bỏ cuộc sau 1 tuần → duy trì đều đặn trên 30 ngày. |
| Phương án không dùng AI | Dùng app quản lý tài chính truyền thống (Money Lover, Sổ Thu Chi) tự nhập tay, hoặc tạo form Google Form gắn phím tắt trên màn hình điện thoại. |
| Giả thuyết về AI (nếu có) | Người dùng chỉ cần chụp ảnh hóa đơn/ảnh chụp màn hình chuyển khoản hoặc nói 1 câu vào tin nhắn ("hôm nay ăn phở 40k"), AI tự trích xuất số tiền, ngày giờ và phân loại danh mục vào bảng tính. |
| Cảm nhận nhanh | **Rule** (tự động hóa đọc biến động số dư) hoặc **Workflow** (OCR ảnh bill + phân loại danh mục) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 15–20 phút/ngày

[1. Thanh toán tiền] ──▶ [2. Không ghi lại ngay, tiếp tục sinh hoạt]
                             │
                             ▼ (Đến tối trước khi đi ngủ)
[3. Ngồi nhớ lại các khoản chi] ──(10 phút — BOTTLENECK)──▶ [4. Mở Excel/Note gõ tay] 
                             │
                             ▼ (5 phút)
[5. Soi lại số dư thấy lệch tiền] ──▶ [6. Nản lòng, bỏ cuộc sau 1 tuần]
Tổng thời gian: 15–20 phút/ngày
```

### Problem Card #3 — Tổng hợp kiến thức và công thức cốt lõi từ slide bài giảng khi ôn thi

| Trường | Nội dung |
|---|---|
| Job Story | Khi bước vào đợt ôn thi cuối kỳ với khối lượng tài liệu khổng lồ (200–300 slide bài giảng), tôi muốn trích xuất các công thức, định nghĩa và dạng bài tập cốt lõi thành bản tóm tắt (cheat sheet) có hệ thống, để tập trung luyện bài mà không mất 4–5 tiếng lật giở từng trang slide. |
| Actor | Sinh viên đại học |
| Thời điểm / bối cảnh | 1–2 tuần trước kỳ thi giữa kỳ hoặc cuối kỳ |
| Quy trình hiện tại (3–7 bước) | 1. Tải toàn bộ file slide bài giảng từ Teams/Drive về máy.<br>2. Mở từng file PDF/PowerPoint đọc lướt qua.<br>3. Tìm các trang có đóng khung định lý, công thức quan trọng.<br>4. Dùng Snipping Tool chụp ảnh hoặc gõ lại công thức sang file Word.<br>5. Sắp xếp lại thứ tự các chương để in ra học. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2 và Bước 4**: Mất 3–4 tiếng ngồi lật từng trang, copy-paste và gõ lại công thức Toán/Lý/Kỹ thuật rất chậm chạp. |
| Impact (nếu không giải thì sao) | Mất quá nhiều thời gian cho khâu chuẩn bị tài liệu, không còn đủ thời gian để giải bài tập; dễ học lệch hoặc bỏ sót các chú ý quan trọng của giảng viên. |
| Success metric (baseline → target) | - Thời gian tạo bản tóm tắt ôn thi: Từ 4–5 tiếng/môn → giảm xuống còn 30–45 phút.<br>- Độ bao phủ kiến thức: Đảm bảo trích xuất đủ 100% các công thức và thuật ngữ chính trong đề cương môn học. |
| Phương án không dùng AI | Xin lại bản tóm tắt hoặc vở ghi chép của sinh viên khóa trước được điểm A; lập nhóm mỗi người tóm tắt 1 chương rồi ghép lại. |
| Giả thuyết về AI (nếu có) | AI phân tích cấu trúc tài liệu PDF bài giảng, tự động gom các slide chứa định nghĩa/công thức và sinh ra bảng tổng hợp kèm ví dụ minh họa tương ứng. |
| Cảm nhận nhanh | **Workflow** (Trích xuất văn bản từ tài liệu + LLM tổng hợp dạng bảng) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 4–5 tiếng/môn

[1. Tải 10 chương slide PDF] ──▶ [2. Mở từng file đọc lướt tìm nội dung] (60 phút)
                                    │
                                    ▼ (BOTTLENECK — 180 phút)
                    [3-4. Chụp ảnh / Gõ lại công thức sang Word]
                                    │
                                    ▼ (30 phút)
                    [5. Căn chỉnh lề & In tài liệu ôn thi]
Tổng thời gian: 4–5 tiếng/môn
```

### Card muốn pitch nhất

- **Card số:** **Card #1 — Trả lời thông tin sản phẩm và tư vấn khách hàng ngoài giờ hành chính (bán hàng online)**
- **Vì sao:** Đây là bài toán gắn liền trực tiếp với lợi ích kinh tế (doanh thu cửa hàng và tỷ lệ chốt đơn), có quy trình trước/sau rất rõ ràng và đo lường được bằng số liệu thực tế (thời gian trễ 6–8 tiếng → rớt 40% đơn hàng ban đêm). Bài toán cũng rất thực tế để so sánh giữa phương án No AI (menu nút bấm tĩnh) và Workflow AI.
- **Câu hỏi muốn nhóm phản biện:** *"Làm thế nào để phân biệt khách chỉ hỏi dạo lúc nửa đêm với khách thật sự có nhu cầu mua hàng, và liệu khách hàng có cảm thấy khó chịu khi nhận ra mình đang tương tác với hệ thống tự động không?"*

### AI đã phản biện card thế nào

Tôi đã đưa Problem Card #1 cho AI đóng vai "Product Manager hoài nghi" phản biện theo prompt mẫu của `docs/01-worksheet.md`:

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card ban đầu ghi chung chung là "chăm sóc khách hàng", dễ bị biến thành chatbot trò chuyện lan man, không ra đơn mà tốn chi phí token. | **Đồng ý hoàn toàn** | Đã giới hạn rõ bối cảnh là **ngoài giờ hành chính (22h–7h)** và mục tiêu cụ thể là **cung cấp thông tin giá/size/tồn kho để giảm tỷ lệ rớt đơn**. |
| Đưa ra giả định AI quá sớm mà chưa xem xét các công cụ miễn phí có sẵn (Facebook Auto-responder). | **Đồng ý** | Đã bổ sung mục **Phương án không dùng AI**: Dùng menu nút bấm cố định có sẵn của Facebook/Zalo để đối chiếu, và chỉ dùng AI cho khâu đọc hiểu câu hỏi ngôn ngữ tự nhiên viết tắt. |
| Bottleneck ban đầu ghi "mất thời gian khá lớn" là mơ hồ, không có số liệu đo lường cụ thể. | **Đồng ý** | Đã sửa lại định lượng chính xác: **Độ trễ phản hồi từ 6–8 tiếng qua đêm**, dẫn đến **tỷ lệ rớt đơn 40%**, target cải thiện là phản hồi dưới 1 phút. |

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
