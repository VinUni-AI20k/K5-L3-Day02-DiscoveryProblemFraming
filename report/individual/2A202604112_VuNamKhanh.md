# Báo cáo cá nhân — 2A202604112_VuNamKhanh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Vũ Nam Khánh
- MSSV: 2A202604112
- Email trường: 26ai.khanhvn@vinuni.edu.vn
- Tên nhóm: 4Ward
- Link repo nhóm: https://github.com/phungtr/K5-L3B-Day02-4Ward-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi đến hạn nộp báo cáo tuần/tháng, tôi muốn tự động gom các thông tin/task đã làm, để không phải lục lại lịch sử chat và bảng công việc | Bản thân | Mất 60-90 phút mỗi tuần |
| 2 | Lặp lại | Khi cần viết tài liệu cho một API/service mới, tôi muốn có cấu trúc tài liệu nhất quán từ source/config, để không phải viết thủ công từ đầu | Backend Dev | 15 API/tháng, 20 phút/API |
| 3 | Tốn thời gian | Khi vừa kết thúc cuộc họp dài 1 tiếng, tôi muốn tổng hợp lại danh sách công việc (action items) kèm người phụ trách, để gửi cho từng người trong team | Bản thân, Team | Mất 30 phút viết lại notes sau mỗi buổi họp (2-3 buổi/tuần) |
| 4 | Tốn thời gian | Khi nhận được tài liệu/nghiên cứu dài (20-30 trang), tôi muốn nắm nhanh các ý chính và rủi ro quan trọng, để quyết định có đọc sâu hay không mà không trễ deadline | Bản thân, Đồng nghiệp | Mất 45-60 phút/bản tài liệu, trung bình 3 bài/tuần |
| 5 | Đọc & Tổng hợp | Khi cần so sánh giải pháp/sản phẩm từ 4-5 nguồn tài liệu khác nhau, tôi muốn có bảng tổng hợp ưu/nhược điểm theo tiêu chuẩn chung, để đưa ra đề xuất nhanh chóng | Bản thân, Team, Mentor | Mất 2-3 tiếng gom thông tin rải rác mỗi khi làm đề xuất mới |
| 6 | Đọc & Tổng hợp | Khi cần tìm lại lý do vì sao team đã đưa ra một quyết định chuyên môn cũ, tôi muốn truy xuất đúng đoạn thảo luận lịch sử, để không phải tranh luận lại từ đầu | Team | Tìm kiếm thủ công mất 15-20 phút/lần, xảy ra 2-3 lần/tuần trên kênh chat |
| 7 | Pain từ người khác | Khi tôi gửi yêu cầu/assignment cho thành viên khác, họ muốn hiểu rõ tiêu chí đánh giá ngay lần đầu, để không phải nhắn tin hỏi đi hỏi lại | Bản thân, Team | Nhắn tin qua lại hỏi làm rõ yêu cầu 3-4 lần/task |
| 8 | Pain từ người khác | Khi mentor cần theo dõi tiến độ công việc, họ muốn thấy báo cáo dạng hình ảnh/bảng tổng quan ngắn gọn, để nắm tình hình mà không phải nhắn hỏi từng người | Mentor, Bản thân, Team | 2-3 lần/tuần |

**Nếu có dùng AI để gợi ý thêm:** Đã lọc chọn hai gợi ý của AI là ý #2 (viết docs API) và ý #8 (báo cáo tiến độ cho Mentor) vì có lăng kính, actor và con số đo lường cụ thể. Đồng thời, loại bỏ hai ý AI đưa ra về "trợ lý quản lý toàn năng" và "tự động trả lời chat" do phạm vi quá rộng, bị lẫn giải pháp AI và thiếu quy trình thực tế để kiểm chứng rủi ro.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp action items sau họp (#3) | Baseline thời gian rõ (30'/buổi), đau thật (2-3 họp/tuần), bottleneck rõ ở bước phân loại & trích xuất note rải rác | Làm sao AI trích xuất đúng tên người phụ trách nếu hội thoại họp không gọi tên rõ ràng? |
| 2 | Viết tài liệu API/service từ source (#2) | Tần suất lớn (15 API/tháng), quy trình chuẩn hóa cao, vừa sức làm trong 1 buổi lab | Liệu dùng Script/Rule (như Swagger/OpenAPI spec) đã giải quyết trọn vẹn chưa hay thực sự cần AI? |
| 3 | Báo cáo tiến độ cho Mentor (#8) | Giải quyết nỗi đau trực tiếp của Mentor/Lead, dễ đo lường bằng số lần nhắn tin hỏi lại | Dữ liệu đầu vào lấy từ đâu để AI tạo được bảng tổng quan trực quan mà không tốn công nhập liệu tay? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa kết thúc cuộc họp dài 1 tiếng, tôi muốn tổng hợp lại danh sách công việc (action items) kèm người phụ trách, để gửi cho từng người trong team xác nhận ngay |
| Actor | Bản thân, Team |
| Thời điểm / bối cảnh | Ngay sau các buổi họp team (2-3 lần/tuần) |
| Quy trình hiện tại (3–7 bước) | 1. Mở file ghi chép thô trong họp → 2. Đọc lại và phân loại đoạn nào là ý kiến, đoạn nào là công việc → 3. Trích xuất tên người phụ trách và deadline → 4. Định dạng lại danh sách action items ngăn nắp → 5. Gửi lên kênh chat/email cho team |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 + 3 (Phân loại & trích xuất việc/người): mất 20 phút/buổi do hội thoại họp lan man, không đúng cấu trúc |
| Impact (nếu không giải thì sao) | Mất 60-90 phút/tuần; trễ gửi recap khiến team bỏ sót công việc, phải hỏi lại thông tin |
| Success metric (baseline → target) | Tổng thời gian tổng hợp từ 30 phút xuống dưới 8 phút/buổi họp; 100% action items có người phụ trách rõ ràng |
| Phương án không dùng AI | Dùng sẵn template Notion/Docs + phân công 1 người ghi chép trực tiếp vào template ngay trong lúc họp |
| Giả thuyết về AI (nếu có) | AI đọc bản ghi âm/transcript cuộc họp, trích xuất danh sách công việc theo dạng bảng |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 30 phút/buổi họp

[1] Mở note thô: 2'
[2] Đọc & lọc nội dung: 12'
[3] Trích xuất Task + Assignee: 8' ← BOTTLENECK
[4] Format lại danh sách: 5'
[5] Gửi lên Slack/Email: 3'
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần viết tài liệu cho một API/service mới, tôi muốn có cấu trúc tài liệu nhất quán từ source/config, để không phải viết thủ công từ đầu |
| Actor | Backend Developer |
| Thời điểm / bối cảnh | Khi hoàn thành xong một Endpoint/API mới và chuẩn bị bàn giao cho Frontend/Partner |
| Quy trình hiện tại (3–7 bước) | 1. Đọc source code và file config → 2. Tạo file tài liệu theo template → 3. Viết mô tả input/output parameter → 4. Viết ví dụ response (200, 400, 500) → 5. Tự kiểm tra và gửi cho Dev khác review |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 + 4 (Viết mô tả tham số & response mẫu): mất 12 phút/API vì phải copy-paste và format JSON thủ công |
| Impact (nếu không giải thì sao) | Mất 300 phút (5 tiếng)/tháng (15 API); Dev lười viết tài liệu dẫn đến tài liệu bị out-of-date, Frontend phải hỏi lại nhiều lần |
| Success metric (baseline → target) | Thời gian viết từ 20 phút xuống dưới 5 phút/API; 100% API ra mắt đều có tài liệu chuẩn cấu trúc |
| Phương án không dùng AI | Dùng thư viện Rule/Script tự động sinh UI/Docs từ code annotation (như Swagger/OpenAPI code generator) |
| Giả thuyết về AI (nếu có) | AI phân tích đoạn code handler/DTO, tự động viết mô tả tiếng Việt diễn giải ý nghĩa các tham số và tạo response mẫu |
| Cảm nhận nhanh | Rule hoặc Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 20 phút/API

[1] Đọc code/config: 3'
[2] Mở template: 2'
[3] Viết mô tả param + response mẫu: 12' ← BOTTLENECK
[4] Tự review format: 2'
[5] Gửi bàn giao: 1'
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi mentor cần theo dõi tiến độ công việc, họ muốn thấy báo cáo dạng hình ảnh/bảng tổng quan ngắn gọn, để nắm tình hình mà không phải nhắn hỏi từng người |
| Actor | Mentor, Team |
| Thời điểm / bối cảnh | Trước các buổi check-in định kỳ hoặc cuối tuần (2-3 lần/tuần) |
| Quy trình hiện tại (3–7 bước) | 1. Gom task từ Trello/Jira/Git → 2. Tổng hợp các việc đã xong và việc bị nghẽn (blocker) → 3. Viết nhận định/tiến độ chung → 4. Chụp màn hình/vẽ lại dashboard → 5. Gửi cho Mentor |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 + 3 (Gom việc & viết nhận định rủi ro): mất 15 phút/lần do thông tin nằm ở nhiều công cụ khác nhau |
| Impact (nếu không giải thì sao) | Mentor phải nhắn tin đôn đốc 2-3 lần/tuần; báo cáo thủ công bị chậm, thiếu thông tin rủi ro chính |
| Success metric (baseline → target) | Thời gian tạo báo cáo từ 25 phút xuống dưới 5 phút/lần; Mentor không còn phải nhắn tin hỏi tiến độ thủ công |
| Phương án không dùng AI | Cấu hình Widget Dashboard tự động trên Jira/Notion gom toàn bộ task theo trạng thái |
| Giả thuyết về AI (nếu có) | AI đọc log công việc trên bảng task, tự động tóm tắt 3 việc nổi bật + 1 rủi ro chính thành khung visual ngắn gọn |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 25 phút/lần báo cáo

[1] Gom task rải rác: 5'
[2] Lọc task xong & blocker: 10' ← BOTTLENECK
[3] Viết nhận định tiến độ: 5'
[4] Chụp ảnh/format: 3'
[5] Gửi Mentor: 2'
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Đau thật và lặp lại đều đặn (2-3 lần/tuần); quy trình hiện tại có baseline đo thời gian rõ ràng (30 phút); dễ nhận thấy ranh giới giữa việc AI trích xuất nháp và con người kiểm tra trước khi gửi.
- Câu hỏi muốn nhóm phản biện:
    - Nếu transcript họp bị nhiễu hoặc mọi người nói xen ngang, AI trích xuất sai người phụ trách thì cách kiểm tra nhanh nhất là gì?
    - Liệu một checklist/template Notion cố định điền ngay trong lúc họp có giải quyết được 70% bài toán này mà không cần dùng AI không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: Nhầm lẫn giữa việc ghi chép toàn bộ buổi họp với việc trích xuất action items | Đồng ý | Thu hẹp phạm vi bài toán: chỉ tập trung trích xuất Action Items + Assignee, không làm tóm tắt toàn bộ nội dung cuộc họp |
| Card #2: Bài toán viết docs API có thể xử lý 80% bằng Rule/Script (Swagger) mà không cần AI | Đồng ý | Đưa "Swagger/OpenAPI script" vào ô Phương án không dùng AI để so sánh hiệu quả ở CP4 |
| Card #3: Target metric "Mentor không nhắn hỏi" khó đo lường trực tiếp | Đồng ý | Đổi metric thành: "Thời gian tạo báo cáo từ 25' xuống <5', % rủi ro/blocker được phát hiện trước buổi check-in" |

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
