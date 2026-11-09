# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyen Minh Duc
- MSSV: 2A202603960
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Vietnam Airline
- Link repo nhóm:

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

|   # | Lăng kính     | Job Story: Khi… tôi muốn… để…                                                                                                  | Ai chịu ảnh hưởng?             | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)           |
| --: | ------------- | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------ | ------------------------------------------------------------------- |
|   1 | Tốn thời gian | Khi viết báo cáo tuần tôi muốn tổng hợp các kết quả số liệu theo đúng format để mang trình bày, báo cáo kịp giờ và dễ đọc      | Sinh viên, giáo viên           | Mỗi tuần một lần, mất ~50-60 phút tổng hợp viết báo cáo             |
|   2 | Đọc tổng hợp  | Khi học, tôi muốn các slide và các references tổng hợp về một chỗ để tiện theo dõi                                             | Sinh viên                      | Mỗi chương trình học có nhiều kênh phân tán (discord, lms, drive)   |
|   3 | Đọc tổng hợp  | Khi học kiến thức mới, tôi muốn các tài liệu phù hợp với ngưỡng năng lực của tôi để học hiệu quả                               | Sinh viên                      | Thường phải đọc thêm hoặc đọc lại 1-2 bài mỗi khi học kiến thức mới |
|   4 | Tốn thời gian | Khi tham gia họp online, tôi muốn một danh sách các ý chính, công việc để tham khảo lại                                        | Sinh viên, Team                | Thường phải có người ghi chú riêng, tốn 20-30p mỗi buổi họp         |
|   5 | Lặp lại       | Khi viết mail công việc, tôi muốn các thông tin liên quan tổng hợp lại một chỗ với các mẫu để viết mail nhanh và chuyên nghiệp | Sinh viên, giáo viên, cấp trên | Thường phải tra lại thông tin từ các nguồn và viết theo mẫu chuẩn   |
|   6 |               |                                                                                                                                |                                |                                                                     |
|   7 |               |                                                                                                                                |                                |                                                                     |
|   8 |               |                                                                                                                                |                                |                                                                     |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.
- AI gợi ý bỏ ý 3 vì "ngưỡng năng lực" quá mơ hồ và không đo được
- AI gợi ý bỏ ý 5 vì công việc quá đơn giản, các AI hiện có đã đơn giản rồi

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                                                | Vì sao chọn                              | Điều còn chưa chắc                                                                                   |
| ---: | ------------------------------------------------------ | ---------------------------------------- | ---------------------------------------------------------------------------------------------------- |
|    1 | Viết báo cáo hàng tuần (1)                             | Mất thời gian                            | Có thể kiểm tra dựa trên các báo cáo cũ, số liệu commit / task hoàn thành trên jira, số liệu kết quả |
|    2 | Viết biên bản cho họp online (4)                       | Vấn đề thật, mất thời gian               | Không có dữ liệu kiểm tra                                                                            |
|    3 | Tổng hợp slide, tài liệu về một chỗ từ nhiều nguồn (2) | Mất thời gian, vấn đề thật, có quy trình | Giới hạn quyền truy cập, cơ chế chống bot                                                            |

### Problem Card #1

| Trường                                    | Nội dung                                                                                                                                                                               |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi đến hạn nộp báo cáo tiến độ tuần, tôi muốn tự động tổng hợp các kết quả thực tế báo cáo đúng cấu trúc, để không mất thời gian tổng hợp lại và tránh báo cáo sót việc.              |
| Actor                                     | Sinh viên làm đồ án                                                                                                                                                                    |
| Thời điểm / bối cảnh                      | Một tuần một lần                                                                                                                                                                       |
| Quy trình hiện tại (3–7 bước)             | - Tổng hợp số liệu chạy thí nghiệm<br>- Tổng hợp lại các tính năng phát triển và commit<br>- Viết lại vào doc<br>- Vẽ sơ đồ, trình bày bảng số liệu<br>- Review và format lại theo mẫu |
| Bottleneck (bước nào, mất bao nhiêu phút) | Viết ngắn gọn ~ 30 phút<br>Vẽ sơ đồ ~ 30 phút<br>Review và format ~ 30 phút                                                                                                            |
| Impact (nếu không giải thì sao)           | 60-90 phút/tuần cho cá nhân, nếu làm theo team thì tiết kiệm ~30 phút/tuần cho mỗi người và 30 phút/tuần cho leader tổng hợp                                                           |
| Success metric (baseline → target)        | Tổng thời gian viết báo cáo từ                                                                                                                                                         |
| Phương án không dùng AI                   | Tự động cào các commit, số liệu và tổng hợp theo template                                                                                                                              |
| Giả thuyết về AI (nếu có)                 | AI tự động nhận diện số liệu để sinh mẫu bảng trình bày, sơ đồ                                                                                                                         |
| Cảm nhận nhanh                            | No AI / Rule / Workflow / **Agent** / Chưa biết                                                                                                                                        |

Quy trình nháp hiện tại:

```text

```

### Problem Card #2

| Trường                                    | Nội dung                                                                                                                                                                    |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi vừa kết thúc cuộc họp online, tôi muốn có bản nháp tổng hợp về các quyết định đã chốt và các công việc từ transcript, để cả nhóm xác nhận và chỉ cần chỉnh sửa lại ngắn |
| Actor                                     | Nhóm trưởng, thư ký                                                                                                                                                         |
| Thời điểm / bối cảnh                      | Kết thúc cuộc họp                                                                                                                                                           |
| Quy trình hiện tại (3–7 bước)             | Một người hoặc cả nhóm tổng hợp thủ công thành tài liệu                                                                                                                     |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tổng hợp tài liệu, thường mất 30 phút để thống nhất lại                                                                                                                     |
| Impact (nếu không giải thì sao)           | Mỗi thành viên 10 phút                                                                                                                                                      |
| Success metric (baseline → target)        | Bản nháp cuối có các công việc và gạch đầu dòng tương ứng                                                                                                                   |
| Phương án không dùng AI                   | Phân công một người viết                                                                                                                                                    |
| Giả thuyết về AI (nếu có)                 | LLM nhận transcript thô và trích xuất                                                                                                                                       |
| Cảm nhận nhanh                            | No AI / Rule / **Workflow** / **Agent** / Chưa biết                                                                                                                         |

Quy trình nháp hiện tại:

```text

```

### Problem Card #3

| Trường                                    | Nội dung                                                                                                                                                                                                                                  |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi trước và sau các buổi học, tôi muốn tự động gom tất cả slide bài giảng, bài tập và tài liệu tham khảo từ các kênh rải rác về một thư mục duy nhất trên máy, để tiết kiệm thời gian tra cứu và không bị bỏ sót tài liệu được cập nhật. |
| Actor                                     | Sinh viên, học viên                                                                                                                                                                                                                       |
| Thời điểm / bối cảnh                      | Trước và sau buổi học                                                                                                                                                                                                                     |
| Quy trình hiện tại (3–7 bước)             | Truy cập vào từng trang, tải tài liệu, sắp xếp lại, thống nhất tên                                                                                                                                                                        |
| Bottleneck (bước nào, mất bao nhiêu phút) | Truy cập vào mỗi trang và tải tài liệu mất 10-15 phút, mất 10-15 phút để sắp xếp và đặt tên                                                                                                                                               |
| Impact (nếu không giải thì sao)           | Mỗi buổi mất 20-30 phút để tổng hợp tài liệu. Mất thời gian tìm kiếm khi cần thiết.                                                                                                                                                       |
| Success metric (baseline → target)        | Thời gian tập hợp tài liệu giảm từ 20 phút / lần xuống dưới 5 phút                                                                                                                                                                        |
| Phương án không dùng AI                   | Viết script tự động hoá và đặt tên, tuy nhiên nếu file lạ, hoặc thêm nguồn mới sẽ mất thời gian nhận diện                                                                                                                                 |
| Giả thuyết về AI (nếu có)                 | AI tự động tải file theo bộ quy tắc viết tay,                                                                                                                                                                                             |
| Cảm nhận nhanh                            | No AI / Rule / **Workflow** / **Agent** / Chưa biết                                                                                                                                                                                       |
|                                           |                                                                                                                                                                                                                                           |

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì?         | Kết quả / ảnh hưởng tới bài nhóm |
| -------------------------- | ---------------------- | -------------------------------- |
| Pitch Problem Card         |                        |                                  |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:    |                                  |
| Nhận phản biện             | Câu hỏi tôi nhận được: | Tôi đã sửa gì:                   |
| Gom cluster / cây OST      |                        |                                  |
| Chọn candidate problem     |                        |                                  |
| Kiểm chứng / research      |                        |                                  |
| Quy trình nhóm             |                        |                                  |
| Problem Statement          |                        |                                  |
| Mức can thiệp AI           |                        |                                  |
| Quyết định                 |                        |                                  |

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
