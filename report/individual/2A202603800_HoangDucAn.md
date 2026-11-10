# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Hoàng Đức An
- MSSV: 2A202603800
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: I3
- Link repo nhóm: https://github.com/QuangNEU/K5-L3B-Day02-K3-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Khi hoàn thành buổi họp, tôi muốn hệ thống tự động tổng hợp toàn bộ buổi họp để tôi không bị quên nội dung và tiết kiếm thời gian xem lại buổi họp |CEO, Nhân viên văn phòng |Khảo sát 20 nhân viên, có 13 nhân viên chỉ nhớ 50% nội dung buổi họp, tốn khoảng 40 phút để xem lại nội dung họp |
| 2 |Tốn thời gian |Khi hoàn thành xong bài tập, tôi muốn hệ thống tổng hợp các câu hỏi sai và đưa ra các kiến thức liên quan để tôi củng cố lại kiến thức |Học sinh, sinh viên |Mất 15 phút để xem câu sai và tìm kiến thức |
| 3 |Lặp lại |Khi tìm quán ăn, tôi muốn hệ thống tổng hợp các đánh giá của quán ăn đó để tôi biết quán nào nên ăn |Người dùng muốn tìm quán ăn |Mất 10 phút/quán |
| 4 |Lặp lại |Khi có khách hàng gửi yêu cầu hỗ trợ, tôi muốn hệ thống tự phân loại và chuyển đúng bộ phận, để giảm thời gian xử lý thủ công |CSKH, quản lý dịch vụ |Kiểm tra 100 ticket gần nhất, có 40 ticket phải chuyển bộ phận thủ công |
| 5 |Tốn thời gian |Khi cần tìm căn hộ phù hợp với khách hàng, tôi muốn hệ thống đề xuất các căn đáp ứng vị trí, giá tiền và tiện ích, để không phải lọc thủ công từng căn |Người muốn tìm căn hộ |Mất 5 phút để lọc và tìm ra 3 căn phù hợp |
| 6 |Cần đọc và tổng hợp nhiều thông tin |Khi cần đánh giá hiệu quả kinh doanh, tôi muốn hệ thống tổng hợp doanh thu, chi phí, khách hàng và hiệu suất từ nhiều nguồn dữ liệu, để nhanh chóng xác định vấn đề |Giám đốc kinh doanh, chuyên viên phân tích |Kiểm tra 10 báo cáo gần nhất, thống kê có 2 báo cáo phải chỉnh sửa hoặc yêu cầu bổ sung |


**Nếu có dùng AI để gợi ý thêm:** Sau khi tự scan 5 ý, mình hỏi AI và giữ lại ý 6

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tóm tắt nội dung họp (#1) |Tốn thời gian, nhiều người gặp |Chi phí triển khai và tính bảo mật |
| 2 |Phân loại yêu cầu người dùng (#4) |Pain thật, tính ứng dụng cao |Chi phí so với quy trình thông thường |
| 3 |Tìm căn hộ (#5) |Pain thật, nhiều người gặp |Chi phí triển khai |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi hoàn thành buổi họp, tôi muốn hệ thống tự động tổng hợp toàn bộ buổi họp để tôi không bị quên nội dung và tiết kiếm thời gian xem lại buổi họp |
| Actor |Người tham gia cuộc họp |
| Thời điểm / bối cảnh |Sau các cuộc họp dự án, họp sprint, họp giao ban hoặc họp với khách hàng. |
| Quy trình hiện tại (3–7 bước) |Ghi âm buổi họp -> Mở lại bản ghi -> Đọc ghi chú, đối chiếu nội dung -> Tổng hợp nội dung và các quyết định -> Xác định action item, người phụ trách và deadline -> Soạn biên bản họp |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2-3 Nghe lại bản ghi, đọc ghi chú và xác định action item. Ước tính 30–60 phút cho mỗi cuộc họp.|
| Impact (nếu không giải thì sao) |Tốn thời gian của nhân viên; bỏ sót đầu việc; nhầm người phụ trách; chậm tiến độ do các thành viên không nắm rõ quyết định sau cuộc họp. |
| Success metric (baseline → target) |Thời gian làm biên bản: 30–60 phút → dưới 10 phút. Tỷ lệ đầu việc được ghi nhận đầy đủ: đo baseline → mục tiêu trên 95%. |
| Phương án không dùng AI |	Sử dụng mẫu biên bản họp chuẩn; phân công một người ghi chép; sử dụng công cụ ghi âm và checklist action item. |
| Giả thuyết về AI (nếu có) |Sử dụng Speech-to-Text để chuyển giọng nói thành văn bản, kết hợp LLM để tóm tắt nội dung, trích xuất quyết định, người phụ trách và deadline; tự động tạo biên bản họp. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
    HIỆN TẠI — 30–60 phút

    [1 Ghi âm buổi họp] → [2 Mở và nghe lại bản ghi: 15–30'] → [3 Đọc ghi chú, đối chiếu nội dung: 5–10'] → [4 Tổng hợp nội dung và các quyết định: 5–10'] <- BOTTLENECK 
    → [5 Xác định action item, người phụ trách và deadline: 5–10'] → [6 Soạn biên bản họp: 5–10']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi có khách hàng gửi yêu cầu hỗ trợ, tôi muốn hệ thống tự phân loại và chuyển đúng bộ phận, để giảm thời gian xử lý thủ công |
| Actor |CSKH, quản lý dịch vụ   |
| Thời điểm / bối cảnh |Khi khách hàng gửi yêu cầu qua hotline, email, chatbot, website hoặc ứng dụng chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |Tiếp nhận yêu cầu từ khách hàng. -> Đọc nội dung và xác định vấn đề. -> Phân loại yêu cầu (kỹ thuật, thanh toán, bảo hành, khiếu nại...). -> Chuyển yêu cầu đến bộ phận phụ trách. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2-3, mất 5 phút/yêu cầu |
| Impact (nếu không giải thì sao) |Phản hồi khách hàng chậm; chuyển nhầm bộ phận |
| Success metric (baseline → target) |Thời gian phân loại ticket: 5–15 phút → dưới 2 phút, Tỷ lệ phân loại đúng: đo baseline → mục tiêu trên 90%, Thời gian phản hồi đầu tiên: đo baseline → giảm ít nhất 30%. |
| Phương án không dùng AI |Xây dựng bộ quy tắc phân loại ticket; tạo biểu mẫu yêu cầu chuẩn;|
| Giả thuyết về AI (nếu có) |Sử dụng LLM/NLP để hiểu ngôn ngữ tự nhiên, tự động phân loại ticket, nhận diện mức độ ưu tiên, tìm kiếm thông tin trong kho tri thức và đề xuất câu trả lời cho nhân viên CSKH. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
    HIỆN TẠI — 5 phút/yêu cầu

    [1 Tiếp nhận yêu cầu từ khách hàng: 1'] → [2 Đọc nội dung và xác định vấn đề: 2']
    → [3 Phân loại yêu cầu (kỹ thuật, thanh toán, bảo hành, khiếu nại...): 3'] ← BOTTLENECK
    → [4 Xác định bộ phận phụ trách: 1'] → [5 Chuyển ticket đến bộ phận xử lý: 1']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhu cầu mua hoặc thuê căn hộ, tôi muốn tìm được những căn phù hợp với ngân sách, vị trí, diện tích và tiện ích mong muốn, để không phải tự tìm kiếm và so sánh hàng trăm căn hộ. |
| Actor | Người mua nhà |
| Thời điểm / bối cảnh | Khi khách hàng bắt đầu tìm kiếm căn hộ, có nhu cầu so sánh các dự án hoặc muốn tìm căn phù hợp với khả năng tài chính. |
| Quy trình hiện tại (3–7 bước) | Khách hàng xác định nhu cầu -> Lọc căn hộ -> Kiểm tra tình trạng căn hộ còn bán hoặc cho thuê. -> In danh sách căn hộ cho khách hàng.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 - 3 Lọc căn hộ, khoảng 5 phút/lần |
| Impact (nếu không giải thì sao) | Khách hàng mất nhiều thời gian tìm nhà |
| Success metric (baseline → target) | Thời gian tìm 3–5 căn phù hợp: 20–45 phút → dưới 5 phút. |
| Phương án không dùng AI | Xây dựng bộ lọc tìm kiếm nâng cao theo giá, vị trí, diện tích, số phòng ngủ, tiện ích và trạng thái căn hộ |
| Giả thuyết về AI (nếu có) | Dùng LLM để hiểu nhu cầu bằng ngôn ngữ tự nhiên, chuyển thành bộ tiêu chí tìm kiếm, đề xuất căn hộ phù hợp và giải thích lý do đề xuất. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
    HIỆN TẠI — 20–45 phút/lần tìm kiếm

    [1 Xác định nhu cầu khách hàng: 3–5'] → [2 Lọc căn hộ theo ngân sách, vị trí, diện tích và tiện ích: 5–15'] ← BOTTLENECK 
    → [3 Kiểm tra tình trạng căn hộ còn bán/cho thuê: 5–15'] → [4 So sánh và chọn các căn phù hợp: 5–10'] → [5 Tổng hợp và gửi danh sách căn hộ cho khách hàng: 2–5']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Trong một buổi họp thường có rất nhiều thông tin, nhân viên văn phòng và CEO khó có thể tổng hợp và ghi nhớ toàn bộ.
- Câu hỏi muốn nhóm phản biện: Có phương án để đảm bảo tính bảo mật không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|CEO và nhân viên văn phòng là hai nhóm có nhu cầu rất khác nhau. Chưa xác định ai là người trực tiếp ghi biên bản, ai là người sử dụng kết quả và ai chịu trách nhiệm theo dõi action item. | Đồng ý |Người tham gia cuộc họp |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Tóm tắt cuộc họp, Phân loại yêu cầu CSKH, Lọc tìm tự động căn hộ | Vào shortlist |
| Nhận phản biện | Câu hỏi tôi nhận được: CSKH có scope quá rộng| Tôi đã sửa gì: Thu hẹp lại với chỉ CSKH phòng khách sạn|
| Chọn candidate problem | Đánh giá điểm theo tiêu chí | Nhóm chọn được problem phù hợp |
| Quy trình nhóm | Vẽ quy trình hiện tại và tương lai | Nhóm dùng làm bản cuối |
| Problem Statement v0 | Ghi nội dung Problem Statement v0 | Bảng có đầy đủ thông tin |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm problem | Nêu rõ problem | Thiếu dẫn chứng thực tế |  |
| CP2 Problem Card | Phản biện | Chỉ ra đúng lỗi sai | Có một số câu hỏi không nằm problem | |
| CP5 Quy trình | Gợi ý quy trình cải thiện | Chỉ ra các phần mà AI có thể tác động | AI dự đoán thời gian không thực tế | Dự đoán thời gian xe đến chỉ mất 5 giây |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?** Cách mọi người quan sát mọi người xung quanh để nắm bắt được vấn đề cần giải quyết

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?** Nhóm dường như không bị solution-first. Nhóm luôn nhìn nhận vấn đề thực tế trước rồi đưa ra giải pháp.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.** Có, **AI phản biện**: CEO và nhân viên văn phòng là hai nhóm có nhu cầu rất khác nhau. Chưa xác định ai là người trực tiếp ghi biên bản, ai là người sử dụng kết quả và ai chịu trách nhiệm theo dõi action item. **Đón nhận**: Đồng ý và thay đổi thành Người tham giac cuộc họp

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?** Có, cùng một bối cảnh tuy nhiên với một số người thì đó là vấn đề cần xử lí, một số người khác thì không

**6.5. Điều khó nhất khi viết Problem Statement là gì?** Đưa vào Problem Statement giá trị đo được thực tế (như đo thời gian chờ xe, thời gian tìm kiếm căn hộ,...)

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?** Nếu làm lại, tôi sẽ mở rộng góc nhìn thành toàn bộ tuyến xe, chọn ra tuyến xe hợp lí (tối ưu giữa việc chờ đợi xe, mức độ đông đúc và tuyến đường di chuyển). Tôi sẽ phản biện nhóm mạnh hơn ở tính khả thi và tính cấp thiết của vấn đề

**6.7. Hiểu bài:** Vấn đề đặt ra là khi đi tuyến xe buýt E03, cần biết mức độ đông đúc có thể chấp nhận được để di chuyển trong khoảng thời gian chấp nhận được. Quy trình hiện tại phải đứng chờ để lên chuyến xe ít đông đúc. Quy trình đưa ra là để AI dự đoán thời gian xe đến và mức độ đông đúc. Đo bằng cách bắt đầu từ thời gian chờ xe đến khi xuống xe. AI không đảm bảo xe còn chỗ và tự quyết chuyến xe.

---

## 7. Tài liệu tham khảo

-
