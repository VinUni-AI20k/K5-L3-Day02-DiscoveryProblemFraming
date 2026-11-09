# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Nguyễn Thành Công
- MSSV:2A202603789
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:D3
- Link repo nhóm:https://github.com/congnt180263/K5-L3B-Day02-D3-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại · Tốn thời gian · Cần đọc, tổng hợp nhiều thông tin |Khi nhận được hàng trăm CV cho một vị trí tuyển dụng, tôi muốn đánh giá mức độ phù hợp của từng ứng viên dựa trên yêu cầu công việc và kinh nghiệm, để không bỏ sót ứng viên tiềm năng và giảm thời gian sàng lọc. |Recruiter, HR Manager, ứng viên. |100–300 CV/vị trí; 3–5 phút/CV; tổng cộng 5–25 giờ sàng lọc/vị trí. |
| 2 |Lặp lại · Tốn thời gian · Pain từ người khác |Khi phải chấm nhiều bài tự luận, tôi muốn đánh giá bài làm theo các tiêu chí thống nhất, để đảm bảo tính công bằng và giúp học sinh nhận phản hồi kịp thời. |Giáo viên, học sinh, phụ huynh. |150–200 bài/tháng; 5–10 phút/bài; tương đương 12,5–33 giờ chấm bài/tháng. |
| 3 |Lặp lại · Tốn thời gian · Pain từ người khác |Khi tiếp nhận nhiều yêu cầu đổi trả, hoàn tiền và tra cứu đơn hàng, tôi muốn xác định chính xác vấn đề của từng khách hàng, để giảm thời gian xử lý và hạn chế khiếu nại. |Nhân viên CSKH, khách hàng, bộ phận kho. |30–80 ticket/ngày; 5–10 phút/ticket; khoảng 2,5–13,3 giờ xử lý/ngày. |
| 4 |Tốn thời gian · Tổng hợp thông tin · Pain từ người khác |Khi phát sinh sự cố giao hàng, tôi muốn nắm được thông tin từ tài xế, kho và đơn vị vận chuyển, để xác định nguyên nhân và cập nhật tình trạng cho khách hàng. |Nhân viên điều phối, tài xế, nhân viên kho, khách hàng. |10–30 sự cố/tuần; 15–30 phút xác minh/sự cố; khoảng 2,5–15 giờ/tuần. |
| 5 |Lặp lại · Tốn thời gian · Tổng hợp thông tin |Khi đối chiếu hóa đơn với đơn đặt hàng và biên bản giao nhận, tôi muốn xác định các thông tin sai lệch hoặc chứng từ còn thiếu, để hạn chế sai sót trong thanh toán. |Kế toán công nợ, bộ phận mua hàng, nhà cung cấp. |30–100 hóa đơn/ngày; 3–7 phút/hóa đơn; khoảng 1,5–11,7 giờ đối chiếu/ngày. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-Sau khi tự scan 3 ý #1,#2 và #4, Minh hỏi AI và giữ lại ý #3 và #5. Bỏ ý "trợ lý AI hỗ trợ tổng hợp thông tin của bệnh nhân trước khi đổi ca" vì chưa nắm chắc được tỷ lệ hồ sơ phải bổ sung, xử lý lại hoặc phát sinh thông tin thiếu.
---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Kế toán – Đối chiếu hóa đơn, đơn đặt hàng và biên bản giao nhận|Quy trình rõ ràng, thao tác lặp lại, bottleneck cụ thể ở bước đối chiếu nhiều chứng từ. Có thể đo thời gian và tỷ lệ sai lệch. |Cần xác minh định dạng chứng từ, quy tắc đối chiếu và số lượng hóa đơn thực tế. |
| 2 |Thương mại điện tử – Phân loại và xử lý yêu cầu khách hàng |Số lượng yêu cầu lớn, xử lý lặp lại, có dữ liệu ticket và thời gian xử lý để đánh giá. |Cần xác minh hệ thống phân loại ticket, quy trình CSKH và dữ liệu lịch sử. |
| 3 |Nhân sự – Sàng lọc CV ứng viên |Actor rõ, quy trình tuyển dụng dễ vẽ, cần đọc và đối chiếu nhiều thông tin. Có thể đo thời gian và độ chính xác đánh giá. |Cần xác minh tiêu chí tuyển dụng, dữ liệu CV và cách đánh giá mức độ phù hợp. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận được hóa đơn từ nhà cung cấp, tôi muốn đối chiếu thông tin với đơn đặt hàng và biên bản giao nhận, để đảm bảo tính chính xác trước khi thanh toán.|
| Actor |Nhân viên kế toán công nợ |
| Thời điểm / bối cảnh |Khi tiếp nhận và kiểm tra hóa đơn trước khi thực hiện thanh toán cho nhà cung cấp. |
| Quy trình hiện tại (3–7 bước) |1. Tiếp nhận hóa đơn. 2. Tìm đơn đặt hàng tương ứng. 3. Tìm biên bản giao nhận. 4. Đối chiếu nhà cung cấp, số lượng, đơn giá, thuế và tổng tiền. 5. Ghi nhận sai lệch hoặc xác nhận hồ sơ hợp lệ. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 4 – Đối chiếu thông tin giữa 3 loại chứng từ, khoảng 3–7 phút/hóa đơn (ước tính). |
| Impact (nếu không giải thì sao) |Với 30–100 hóa đơn/ngày, có thể tiêu tốn khoảng 1,5–11,7 giờ công/ngày. Sai lệch có thể gây chậm thanh toán và phát sinh xử lý lại. |
| Success metric (baseline → target) |Thời gian đối chiếu: 3–7 phút → ≤ 2 phút/hóa đơn. Tỷ lệ phát hiện sai lệch trên bộ dữ liệu kiểm thử: mục tiêu ≥ 95%. |
| Phương án không dùng AI |Sử dụng checklist đối chiếu và bảng tính Excel với các công thức, quy tắc kiểm tra cố định. |
| Giả thuyết về AI (nếu có) |AI có thể đọc và trích xuất thông tin từ nhiều chứng từ có định dạng khác nhau, sau đó hỗ trợ phát hiện các trường dữ liệu không khớp. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[Nhận hóa đơn]
       |
       v
[Tìm đơn đặt hàng (PO)]
       |
       v
[Tìm biên bản giao nhận (GRN)]
       |
       v
[Đối chiếu 3 loại chứng từ]
       |
       |  BOTTLENECK: 3–7 phút
       v
[Phát hiện sai lệch?]
       |
   +---+---+
   |       |
  Có      Không
   |       |
   v       v
[Yêu cầu  [Xác nhận
 bổ sung]  thanh toán]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận yêu cầu đổi trả, hoàn tiền hoặc tra cứu đơn hàng, tôi muốn xác định chính xác nội dung và mức độ ưu tiên của từng yêu cầu, để chuyển đến đúng bộ phận và xử lý kịp thời. |
| Actor |Nhân viên chăm sóc khách hàng |
| Thời điểm / bối cảnh |Khi tiếp nhận ticket mới qua email, live chat hoặc các kênh CSKH. |
| Quy trình hiện tại (3–7 bước) |1. Tiếp nhận yêu cầu. 2. Đọc và xác định vấn đề của khách hàng. 3. Tra cứu thông tin đơn hàng. 4. Xác định nhóm vấn đề và mức độ ưu tiên. 5. Chuyển bộ phận phụ trách hoặc phản hồi khách hàng. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2–3 – Hiểu nội dung yêu cầu và tra cứu thông tin liên quan, ước tính 3–6 phút/ticket. |
| Impact (nếu không giải thì sao) |Với 30–80 ticket/ngày, tổng thời gian xử lý có thể đạt 2,5–13,3 giờ/ngày. Khách hàng phải chờ lâu, tăng khả năng khiếu nại hoặc liên hệ lại. |
| Success metric (baseline → target) |Thời gian tiếp nhận ban đầu từ 5-10 phút/ ticket giảm xuống còn 3-5 phút/ ticket. Độ chính xác phân loại và chuyển đúng bộ phận: mục tiêu ≥ 90%. |
| Phương án không dùng AI |Sử dụng checklist đối chiếu và bảng tính Excel với các công thức, quy tắc kiểm tra cố định.  |
| Giả thuyết về AI (nếu có) |AI có thể hiểu nội dung khách hàng bằng ngôn ngữ tự nhiên, xác định loại yêu cầu, trích xuất thông tin quan trọng và đề xuất bộ phận xử lý. |
| Cảm nhận nhanh |  Workflow |

Quy trình nháp hiện tại:

```text
[Tiếp nhận ticket]
       |
       v
[Đọc nội dung yêu cầu]
       |
       v
[Tra cứu đơn hàng / lịch sử]
       |
       |  BOTTLENECK: 3–6 phút
       v
[Phân loại vấn đề và ưu tiên]
       |
       v
[Chuyển bộ phận phụ trách]
       |
       v
[Phản hồi khách hàng]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận được nhiều CV cho một vị trí tuyển dụng, tôi muốn đánh giá mức độ phù hợp của từng ứng viên với yêu cầu công việc, để rút ngắn thời gian sàng lọc và không bỏ sót ứng viên tiềm năng. |
| Actor |Nhân viên tuyển dụng |
| Thời điểm / bối cảnh |Khi tiếp nhận hồ sơ ứng tuyển và thực hiện vòng sàng lọc CV ban đầu. |
| Quy trình hiện tại (3–7 bước) |1. Tiếp nhận CV. 2. Đọc thông tin ứng viên. 3. Đối chiếu kỹ năng, kinh nghiệm với JD. 4. Đánh giá mức độ phù hợp. 5. Ghi nhận kết quả và lập danh sách ứng viên tiềm năng. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2–3 – Đọc CV và đối chiếu với yêu cầu tuyển dụng, khoảng 3–5 phút/CV (ước tính). |
| Impact (nếu không giải thì sao) |Với 100–300 CV/vị trí, có thể tiêu tốn 5–25 giờ công sàng lọc/vị trí. Quá trình tuyển dụng kéo dài và có nguy cơ bỏ sót ứng viên phù hợp. |
| Success metric (baseline → target) |Thời gian sàng lọc: 3–5 phút → ≤ 2 phút/CV. Tỷ lệ nhận diện đúng ứng viên phù hợp trên bộ CV đã được chuyên gia đánh giá: mục tiêu ≥ 90%. |
| Phương án không dùng AI |Sử dụng bảng tiêu chí tuyển dụng (Scorecard), checklist kỹ năng và kinh nghiệm để đánh giá CV thủ công. |
| Giả thuyết về AI (nếu có) |AI có thể đọc CV, trích xuất kỹ năng, kinh nghiệm, dự án và đối chiếu với JD để đưa ra nhận xét về mức độ phù hợp kèm bằng chứng. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[Tiếp nhận CV]
       |
       v
[Đọc thông tin ứng viên]
       |
       v
[Đối chiếu CV với JD]
       |
       |  BOTTLENECK: 3–5 phút
       v
[Đánh giá mức độ phù hợp]
       |
       v
[Phân loại ứng viên]
       |
       v
[Lập danh sách ứng viên tiềm năng]
```

### Card muốn pitch nhất

- Card số: 3
- Vì sao: Đã có bảng tiêu chí cụ thể có thể chuyển hóa với rule để hỗ trợ công việc lặp đi lặp lại để đạt được hiệu quả công việc tốt hơn


### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Actor còn quá rộng |Có |Xác định cụ thể: Recruiter phụ trách tuyển dụng IT. |
|Quy trình chưa được xác thực|Có| Bổ sung yêu cầu khảo sát Recruiter để xác minh quy trình thực tế.|
|Bottleneck chưa cụ thể| Có | Tách riêng bước đọc CV và đối chiếu CV với JD.|

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
