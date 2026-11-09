# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Tuấn Dũng
- MSSV: 2A202603608
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhóm T Liệt
- Link repo nhóm: https://github.com/dzungapr6th99/K5-L3A-Day02-NhomTLiet-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Cần đọc, tổng hợp nhiều thông tin | tôi từng vào 1 team, khoảng 10 người. dự án đã chạy 1,5 năm. là 1 đề tài hoàn toàn mới ngoài thị trường, không ai có kinh nghiệm thực tế với mảng này mà chỉ có thể dùng kinh nghiệm cá nhân. khi người mới vào lại, có khá nhiều bottleneck. muốn phản biện 1 chức năng nào đó, hỏi ra mới biết là lãnh đạo yêu cầu, hoặc một nguyên do ngoài khác. đồng thời hệ thống quá lớn và cũng rất nhiều chức năng, việc hỏi tại sao theo phương án này, đi hỏi PIC của chức năng đó cũng gây mất thời gian
|Người mới tiếp cận công việc, Người phụ trách training | Mất thời gian, không cải thiện được bottleneck mặc dù bàn nhiều lần|
| 2 |Lặp lại, Pain từ người khác |  bị miss thông tin khi trong 1 ngày có quá nhiều đầu việc phát sinh, 1 đầu việc bị pending từ hôm qua nhưng tự dưng hôm nay leader cần gấp, xử ly sự cố, ... leader cũng ra khá nhiều đầu việc cho các thành viên, đồng thời cũng phải feedback cho ceo. và hay bị vấn đề hỏi thông tin việc A nay xong chưa trong khi công việc này mới bị pending hôm qua
| toàn team, leader| |
| 3 |Tốn thời gian | một bottleneck cần cải thiện,  nhưng sau nhiều lần bàn đi bàn lại, làm đi làm lại, chức năng vẫn sai, vẫn phải làm lại. chỉ 1 thay đổi nhỏ cũng ảnh hưởng đến toàn hệ thống chức năng. vấn đề ở đây là hệ thống sai hay con người sai? khi không ai phản biện được hệ thống, nhưng liệu có phải vì theo hệ thống mà người làm không control được code mình viết ra không?
| toàn bộ team| |
| 4 | Lặp lại, Tốn thời gian | Khi quay lại một đầu việc sau khi phải chuyển sang xử lý sự cố, tôi muốn nắm lại mình đã làm đến đâu và bước tiếp theo là gì, để tiếp tục công việc mà không phải đọc lại toàn bộ thông tin từ đầu. | Lập trình viên phải chuyển đổi giữa nhiều đầu việc | Gợi ý từ AI, chưa xác nhận bằng trải nghiệm cá nhân. Cần bổ sung một lần bị gián đoạn thật, thời gian khôi phục ngữ cảnh và số lần xảy ra trong tuần. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị kiểm tra một bản sửa chức năng, tôi muốn xác định đúng phiên bản yêu cầu đã được thống nhất, để không kiểm tra theo tài liệu cũ hoặc bỏ sót thay đổi trong các đoạn chat. | Lập trình viên, người kiểm thử, người chốt yêu cầu | Gợi ý từ AI, chưa xác nhận bằng trải nghiệm cá nhân. Cần bổ sung một lần có yêu cầu khác nhau giữa tài liệu và chat, thời gian đối chiếu và hậu quả thực tế. |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- AI gợi ý thêm ý #4 (khôi phục ngữ cảnh sau gián đoạn) và #5 (xác định phiên bản yêu cầu đã chốt), dựa trên bối cảnh làm việc của ba ý đầu. Hai ý này đang là candidate để cân nhắc, chưa xác nhận giữ lại. Chỉ giữ khi đối chiếu được với trải nghiệm thật và bổ sung dấu hiệu cụ thể.
- Khi chọn, cần phân biệt #4 với #2: #4 tập trung vào thời gian cá nhân khôi phục ngữ cảnh; #2 tập trung vào việc các bên không nắm cùng trạng thái và ưu tiên. Phân biệt #5 với #3: #5 tập trung vào việc xác định yêu cầu hiện hành; #3 hiện còn nhiều nguyên nhân làm lại cần tách rõ.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

Phản biện dưới đây dựa trên ba mô tả ở CP1, tương ứng dự kiến với Card #1–#3; các card chi tiết chưa được điền. Cột “Đồng ý?” và “Đã sửa gì” cần người viết tự xác nhận sau khi đối chiếu sự việc thật.

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: Đang gộp việc học hệ thống, tìm PIC và truy lại lý do quyết định. Bước nào thực sự gây mất thời gian nhất? | Chưa xác nhận | Chưa ghi nhận thay đổi. Gợi ý: chọn một lần cần truy lại căn cứ quyết định, tách thời gian tìm người, chờ phản hồi và đọc thông tin. |
| Card #1: Chưa biết lý do thiết kế đã được ghi nhưng khó tìm hay chưa từng được ghi. Nếu chưa có dữ liệu, công cụ tìm kiếm cũng không thể trả lời đáng tin cậy. | Chưa xác nhận | Chưa ghi nhận thay đổi. Gợi ý: kiểm tra một quyết định cụ thể và nguồn lưu; đối chiếu phương án không dùng AI như nhật ký quyết định có người cập nhật. |
| Card #2: “Miss thông tin” và “pending” chưa cụ thể. Leader hỏi lại có thể do trạng thái chưa cập nhật, chưa được đọc hoặc ưu tiên vừa thay đổi. | Chưa xác nhận | Chưa ghi nhận thay đổi. Gợi ý: chọn một task thật, ghi ai quyết định dừng, lý do dừng, nơi cập nhật và thời điểm đổi ưu tiên. |
| Card #2: Chưa rõ hậu quả chính và cách đo; hỏi lại tiến độ chưa đủ chứng minh có việc bị bỏ sót. | Chưa xác nhận | Chưa ghi nhận thay đổi. Gợi ý: chọn một chỉ số như thời gian báo cáo lại, số lần làm nhầm ưu tiên hoặc số việc trễ; đối chiếu bảng task chung trước khi cân nhắc AI. |
| Card #3: Câu hỏi “hệ thống sai hay con người sai?” quá rộng. Chưa đủ căn cứ phân biệt yêu cầu thay đổi, hiểu sai nghiệp vụ, bỏ sót phụ thuộc hay thiếu kiểm thử. | Chưa xác nhận | Chưa ghi nhận thay đổi. Gợi ý: chọn một lần sửa cụ thể, mô tả kết quả mong đợi, kết quả thực tế và bước phát hiện sai. |
| Card #3: “Thay đổi nhỏ ảnh hưởng toàn hệ thống” chưa chỉ ra chức năng bị ảnh hưởng và thời gian làm lại. Chưa có căn cứ kết luận người viết không kiểm soát được code. | Chưa xác nhận | Chưa ghi nhận thay đổi. Gợi ý: chỉ rõ phần phụ thuộc bị bỏ sót, số vòng sửa và thời gian từng vòng; thu hẹp card về một nguyên nhân có bằng chứng. |
| Cả ba card: Chưa có quy trình 3–7 bước kèm thời gian, baseline và target. Chưa thể xác định chắc bottleneck hoặc chọn mức can thiệp. | Chưa xác nhận | Chưa ghi nhận thay đổi. Gợi ý: dựng quy trình từ từng sự việc thật, ghi rõ số đo hay ước lượng, bổ sung phương án không dùng AI và cách đo thành công. |

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
