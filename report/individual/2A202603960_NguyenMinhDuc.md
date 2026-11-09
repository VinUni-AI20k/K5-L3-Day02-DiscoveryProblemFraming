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

| Trường                                    | Nội dung                                                                                                                                                                  |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi đến hạn nộp báo cáo tiến độ tuần, tôi muốn tự động tổng hợp các kết quả thực tế báo cáo đúng cấu trúc, để không mất thời gian tổng hợp lại và tránh báo cáo sót việc. |
| Actor                                     | Sinh viên làm đồ án                                                                                                                                                       |
| Thời điểm / bối cảnh                      | Một tuần một lần (trước buổi họp báo cáo tiến độ)                                                                                                                         |
| Quy trình hiện tại (3–7 bước)             | 1. Tổng hợp số liệu chạy thí nghiệm · 2. Tổng hợp tính năng và commit Git · 3. Viết nháp vào doc · 4. Vẽ sơ đồ, kẻ bảng số liệu · 5. Review và format theo mẫu            |
| Bottleneck (bước nào, mất bao nhiêu phút) | Viết ngắn gọn ~ 30 phút<br>Vẽ sơ đồ ~ 30 phút<br>Review và format ~ 30 phút                                                                                               |
| Impact (nếu không giải thì sao)           | 60-90 phút/tuần cho cá nhân, nếu làm theo team thì tiết kiệm ~30 phút/tuần cho mỗi người và 30 phút/tuần cho leader tổng hợp                                              |
| Success metric (baseline → target)        | Tổng thời gian viết báo cáo giảm từ baseline ~90 phút/tuần xuống target dưới 30 phút/tuần                                                                                 |
| Phương án không dùng AI                   | Tự động cào các commit, số liệu và tổng hợp theo template                                                                                                                 |
| Giả thuyết về AI (nếu có)                 | AI tự động nhận diện số liệu để sinh mẫu bảng trình bày, sơ đồ                                                                                                            |
| Cảm nhận nhanh                            | No AI / Rule / Workflow / **Agent** / Chưa biết                                                                                                                           |

Quy trình nháp hiện tại:

```text
[1. Lấy số liệu thí nghiệm & commit: 15']
→ [2. Viết nháp kết quả vào Doc: 30'] ← BOTTLENECK
→ [3. Vẽ sơ đồ & kẻ bảng số liệu: 30'] ← BOTTLENECK
→ [4. Review & căn chỉnh format: 15']
Tổng: ~90 phút/tuần (hoàn toàn thủ công)
```

### Problem Card #2

| Trường                                    | Nội dung                                                                                                                                                                    |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi vừa kết thúc cuộc họp online, tôi muốn có bản nháp tổng hợp về các quyết định đã chốt và các công việc từ transcript, để cả nhóm xác nhận và chỉ cần chỉnh sửa lại ngắn |
| Actor                                     | Nhóm trưởng, thư ký                                                                                                                                                         |
| Thời điểm / bối cảnh                      | Ngay sau khi kết thúc cuộc họp online                                                                                                                                       |
| Quy trình hiện tại (3–7 bước)             | 1. Tải transcript cuộc họp · 2. Đọc lại lọc việc cần làm · 3. Soạn nháp quyết định và to-do · 4. Gửi nhóm xin xác nhận · 5. Thảo luận thống nhất bản cuối                 |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tổng hợp tài liệu và thống nhất lại, thường mất ~30 phút                                                                                                                    |
| Impact (nếu không giải thì sao)           | Thư ký mất 30 phút/buổi, các thành viên khác mất thêm ~10 phút đọc lại do biên bản không rõ, dễ trễ việc                                                                    |
| Success metric (baseline → target)        | Thời gian từ lúc họp xong đến khi có biên bản chốt giảm từ ~40 phút xuống dưới 10 phút                                                                                      |
| Phương án không dùng AI                   | Phân công một người viết tay theo template cố định                                                                                                                          |
| Giả thuyết về AI (nếu có)                 | LLM nhận transcript thô và trích xuất action items                                                                                                                         |
| Cảm nhận nhanh                            | No AI / Rule / **Workflow** / **Agent** / Chưa biết                                                                                                                         |

Quy trình nháp hiện tại:

```text
[1. Tải transcript cuộc họp: 5']
→ [2. Đọc lại và trích xuất to-do: 15']
→ [3. Soạn nháp quyết định: 10']
→ [4. Gửi nhóm tranh luận thống nhất lại: 10'] ← BOTTLENECK
Tổng: ~40 phút/buổi họp (dễ bỏ sót việc đã chốt)
```

### Problem Card #3

| Trường                                    | Nội dung                                                                                                                                                                                                                                  |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi trước và sau các buổi học, tôi muốn tự động gom tất cả slide bài giảng, bài tập và tài liệu tham khảo từ các kênh rải rác về một thư mục duy nhất trên máy, để tiết kiệm thời gian tra cứu và không bị bỏ sót tài liệu được cập nhật. |
| Actor                                     | Sinh viên, học viên                                                                                                                                                                                                                       |
| Thời điểm / bối cảnh                      | Trước và sau buổi học                                                                                                                                                                                                                     |
| Quy trình hiện tại (3–7 bước)             | 1. Vào LMS tải slide · 2. Vào Discord tải tài liệu bổ trợ · 3. Vào GitHub tải starter code · 4. Đổi tên file chuẩn · 5. Phân loại vào folder máy                                                                                        |
| Bottleneck (bước nào, mất bao nhiêu phút) | Truy cập vào mỗi trang và tải tài liệu mất 10-15 phút, mất 10-15 phút để sắp xếp và đặt tên                                                                                                                                               |
| Impact (nếu không giải thì sao)           | Mỗi buổi mất 20-30 phút để tổng hợp tài liệu. Mất thời gian tìm kiếm khi cần thiết.                                                                                                                                                       |
| Success metric (baseline → target)        | Thời gian tập hợp tài liệu giảm từ baseline 20-30 phút/lần xuống dưới 5 phút                                                                                                                                                              |
| Phương án không dùng AI                   | Viết script tự động hoá và đặt tên, tuy nhiên nếu file lạ, hoặc thêm nguồn mới sẽ mất thời gian nhận diện                                                                                                                                 |
| Giả thuyết về AI (nếu có)                 | AI tự động nhận diện loại tài liệu và gom file theo bộ quy tắc đặt tên                                                                                                                                                                    |
| Cảm nhận nhanh                            | No AI / Rule / **Workflow** / **Agent** / Chưa biết                                                                                                                                                                                       |

Quy trình nháp hiện tại:

```text
[1. Vào LMS tải slide: 5']
→ [2. Vào Discord tải tài liệu bổ trợ: 5']
→ [3. Lọc và đổi tên file chuẩn: 10'] ← BOTTLENECK
→ [4. Di chuyển vào đúng folder môn học: 5']
Tổng: ~25 phút/buổi (rải rác ở nhiều nguồn)
```

### Card muốn pitch nhất

- Card số: 1 (Báo cáo tiến độ tuần)
- Vì sao: Vấn đề lặp lại đều đặn mỗi tuần, có số liệu thời gian đo lường cụ thể (~90 phút/tuần), ảnh hưởng trực tiếp đến cả cá nhân và nhóm đồ án, có sẵn dữ liệu đối soát từ commit log và Jira.
- Câu hỏi muốn nhóm phản biện: "Nếu chỉ cần script tự động cào số liệu commit và điền vào template Doc sẵn thì có thực sự cần đến AI không?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                                                                         | Đồng ý? | Đã sửa gì                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------- |
| Đòi hỏi AI Agent tự động vẽ sơ đồ và viết toàn bộ báo cáo là phi thực tế, rủi ro hallucination số liệu cao | Đồng ý  | Hạ kỳ vọng từ Agent xuống Workflow                                                                                        |
| Success metric chưa có baseline định lượng cụ thể và thiếu phương thức đo lường kiểm chứng                 | Đồng ý  | Bổ sung baseline đo thật (90 phút/tuần) và target giảm xuống dưới 30 phút, đo bằng cách tự bấm giờ trong 2 tuần           |
| Chưa có ranh giới vận hành (Boundary): AI có thể tự ý bịa thêm kết quả thí nghiệm chưa chạy                | Đồng ý  | Thêm boundary nghiêm ngặt: AI chỉ trích xuất từ commit/log có sẵn, bắt buộc gắn nhãn `[DRAFT_ONLY]` để sinh viên kiểm tra |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì?                                                     | Kết quả / ảnh hưởng tới bài nhóm                          |
| -------------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| Pitch Problem Card         | Tôi pitch card của tôi và cùng vote lựa chọn                       | Đóng góp 3 bài toán vào danh sách chung để nhóm lựa chọn  |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Discord đã có AI chatbot cho hỏi đáp rồi mà?" | Nhóm nhận ra bài đó AI chưa hiệu quả và đổi thành workflơ |
| Nhận phản biện             | Câu hỏi tôi nhận được: Bài của tôi bị trùng với ví dụ mẫu          | Tôi đã sửa gì: Tôi chọn ý khác thực tế hơn                |
| Gom cluster / cây OST      | Tôi đọc ví dụ và giao việc cho các bạn khác                        |                                                           |
| Chọn candidate problem     | Tôi vote với cả nhóm để quyết định                                 | Chốt bài toán tìm câu trả lời trên Discord                |
| Kiểm chứng / research      | Tôi làm phỏng vấn và tôi viết research các giải pháp đã có         | Tạo 2 file snapshot và bảng so sánh 3 công cụ             |
| Quy trình nhóm             | Tôi đóng góp ý kiến và phân công công việc vẽ quy trình            |                                                           |
| Problem Statement          | Tôi đóng góp ý kiến và phân công công việc hoàn thiện bảng         |                                                           |
| Mức can thiệp AI           | Tôi đóng góp ý kiến và phân công công việc phân tích 4 mức         | Nhóm thống nhất chọn mức Workflow thay vì Agent           |
| Quyết định                 | Tôi ra quyết định Go kèm thời gian pilot và ngưỡng dừng            | Quyết định Go                                             |

---

## 5. Dùng AI

| Checkpoint                     | Tôi dùng AI để làm gì?            | AI hữu ích ở đâu?                                    | AI sai hoặc hời hợt ở đâu?                           | Tôi sửa gì bằng nhận định của mình?                       |
| ------------------------------ | --------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | --------------------------------------------------------- |
| CP1 Scan                       | Phản biện lại ý của mình          | Đưa ra phản biện để tôi làm rõ scope                 | Gợi ý phạm vi ban đầu còn quá rộng                   | Sửa rõ lại scope từ tool tổng hợp thành workflow tổng hợp |
| CP2 Problem Card               | Không dùng                        |                                                      |                                                      |                                                           |
| CP4 Research                   | Tìm kiếm các giải pháp tương đồng | Gợi ý các ý tưởng giải pháp phù hợp để tìm hiểu thêm | Các đường link nguồn dẫn ra bị hallucinate (link ảo) | Tự kiểm tra lại và tìm kiếm link tài liệu chuẩn           |
| CP5 Quy trình                  | Không làm phần này                |                                                      |                                                      |                                                           |
| CP5–6 Problem Statement        | Không làm phần này                |                                                      |                                                      |                                                           |
| CP6 Mức can thiệp / quyết định | Không dùng                        |                                                      |                                                      |                                                           |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
- Chưa có thuyết trình
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
- Khi nêu problem card của nhau
- Do phản biện của nhau nên đã nhận ra
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
- Có
- Khi bị phản biện là bỏ ý 3 vì "ngưỡng năng lực quá mơ hồi", tôi đã bỏ
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
- Không
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
- Xác định quy trình
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
- Chưa có thuyết trình
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
- Problem: Học viên gặp vấn đề với hệ thông
- Quy trình: Học viên tự tìm kiếm trên Discord hoặc viết ticket cho lab coach
- Metric: Thời gian xử lý 1 vấn đề
- Boundary: AI chỉ tổng hợp từ dữ liệu được cấp quyền
- Mức can thiệp AI: AI không được trả lời thay coach
- Quyết định: Workflow

---

## 7. Tài liệu tham khảo

-
