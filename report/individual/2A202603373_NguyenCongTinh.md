# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Công Tĩnh
- MSSV: 2A202603373
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: hhuydaugg
- Link repo nhóm: https://github.com/hhuydaugg/K5-L3-Day02-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)
**Nhân vật:** Nam là một Junior Product Manager phụ trách tham gia kiểm thử, đánh giá và cải tiến các chức năng thuộc hệ thống chăm sóc khách hàng và xử lý sự cố của Xanh SM. Trong công việc hằng ngày, Nam thường xuyên tiếp nhận thông tin phản hồi từ nhân viên chăm sóc khách hàng, bộ phận vận hành, tài xế và người dùng. Nam có nhiệm vụ tổng hợp các lỗi phát sinh trong quá trình sử dụng hệ thống, ghi nhận những bất cập trong quy trình xử lý, phân tích phản hồi của các bên liên quan và phối hợp với đội ngũ kỹ thuật để đề xuất cải tiến sản phẩm. 

**Vì sao đây là ví dụ tốt:** actor cụ thể; quy trình lặp lại hằng tuần; bottleneck rõ; có baseline thời gian; so sánh được No AI / Rule / Workflow / Agent; và quan trọng nhất, **research làm nhóm đổi kết luận**.


| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Khi kết thúc mỗi đợt kiểm thử, tôi muốn tổng hợp toàn bộ lỗi phát sinh vào một danh sách, để không bỏ sót lỗi cần xử lý |Nam, QA, Developer |Mỗi đợt kiểm thử phải tổng hợp từ 30–50 lỗi, mất khoảng 60–90 phút |
| 2 |Lặp lại |Khi nhận phản hồi khách hàng, tôi muốn phân loại theo từng nhóm vấn đề, để dễ theo dõi và chuyển đúng bộ phận xử lý |Nam, CSKH |Mỗi ngày tiếp nhận khoảng 50–100 phản hồi cần phân loại |
| 3 |Cần đọc, tổng hợp nhiều thông tin |Khi có nhiều phản hồi từ khách hàng và nhân viên CSKH, tôi muốn phát hiện những vấn đề giống nhau, để xác định lỗi phổ biến và ưu tiên cải tiến |Nam, CSKH, Product Manager |Một vấn đề có thể xuất hiện trong nhiều phản hồi khác nhau, khó nhận diện thủ công |
| 4 |Pain từ người khác |Khi nhân viên CSKH gặp lỗi trên hệ thống, họ muốn có hướng dẫn xử lý rõ ràng, để không phải liên hệ bộ phận kỹ thuật nhiều lần |Nhân viên CSKH, Developer |Nhân viên CSKH thường xuyên phải hỏi lại cách xử lý lỗi qua Slack |
| 5 |Pain từ người khác |Khi Developer nhận yêu cầu xử lý lỗi, họ muốn nhận được mô tả đầy đủ và chính xác, để không phải hỏi lại Nam hoặc CSKH |Developer, Nam, CSKH |Developer phải yêu cầu bổ sung thông tin nhiều lần trước khi tái hiện được lỗi |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Phân loại phản hồi khách hàng theo nhóm vấn đề |Công việc lặp lại hằng ngày, số lượng phản hồi lớn, dễ mất thời gian và phân loại sai |Có thể dùng Rule thay vì AI hay không? |
| 2 |Phát hiện vấn đề trùng lặp từ phản hồi khách hàng và CSKH |Cần đọc, đối chiếu nhiều nguồn, khó nhận diện lỗi phổ biến và nguyên nhân chung |AI có phát hiện chính xác các phản hồi cùng bản chất nhưng khác cách diễn đạt không? |
| 3 |Xây dựng hướng dẫn xử lý lỗi cho nhân viên CSKH |Giảm việc hỏi lại bộ phận kỹ thuật, giúp nhân viên xử lý nhanh và nhất quán |Có đủ tài liệu hướng dẫn đáng tin cậy và cập nhật không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story |Khi nhận phản hồi khách hàng, tôi muốn phân loại theo từng nhóm vấn đề, để dễ theo dõi và chuyển đúng bộ phận xử lý.|
| Actor |Nam – Junior Product Manager; nhân viên CSKH |
| Thời điểm / bối cảnh |Hằng ngày, khi tiếp nhận phản hồi từ khách hàng qua các kênh chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |1. Tiếp nhận phản hồi. 2. Đọc nội dung. 3. Xác định nhóm vấn đề. 4. Ghi nhận vào bảng theo dõi. 5. Chuyển bộ phận phụ trách. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Đọc và phân loại thủ công từng phản hồi; giả định mất 1–2 phút/phản hồi. |
| Impact (nếu không giải thì sao) |Tốn thời gian, phân loại không nhất quán, chuyển sai bộ phận và chậm xử lý phản hồi. |
| Success metric (baseline → target) |Baseline giả định: 50–100 phản hồi/ngày. Target: giảm ít nhất 50% thời gian phân loại, độ chính xác từ 90% trở lên. |
| Phương án không dùng AI |Xây dựng danh mục nhóm lỗi, biểu mẫu nhập liệu và quy tắc phân loại cố định. |
| Giả thuyết về AI (nếu có) |AI có thể đọc hiểu nội dung phản hồi và tự động đề xuất nhóm vấn đề phù hợp. |
| Cảm nhận nhanh | Workflow kết hợp AI |

Quy trình nháp hiện tại:


Nhận phản hồi khách hàng
          ↓
Đọc nội dung phản hồi
          ↓
Xác định nhóm vấn đề
          ↓
Ghi nhận vào bảng theo dõi
          ↓
Chuyển bộ phận phụ trách
          ↓
Theo dõi kết quả xử lý
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story |Khi có nhiều phản hồi từ khách hàng và nhân viên CSKH, tôi muốn phát hiện những vấn đề giống nhau, để xác định lỗi phổ biến và ưu tiên cải tiến.|
| Actor |Nam – Junior Product Manager; nhân viên CSKH; Product Manager; Developer. |
| Thời điểm / bối cảnh |Khi tổng hợp phản hồi khách hàng, kết quả kiểm thử và báo cáo sự cố định kỳ. |
| Quy trình hiện tại (3–7 bước) |1. Thu thập phản hồi từ các nguồn. 2. Đọc nội dung từng phản hồi. 3. Đối chiếu các nội dung tương tự. 4. Nhóm các vấn đề trùng lặp. 5. Xác định lỗi phổ biến. 6. Báo cáo và đề xuất ưu tiên cải tiến. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Phải đọc và đối chiếu nhiều nội dung khác nhau; giả định mất 60–90 phút cho mỗi lần tổng hợp. |
| Impact (nếu không giải thì sao) |Bỏ sót lỗi có cùng nguyên nhân, thống kê sai số lượng sự cố, chậm phát hiện vấn đề nghiêm trọng và ưu tiên cải tiến chưa chính xác. |
| Success metric (baseline → target) |Baseline giả định: 60–90 phút/lần tổng hợp. Target: giảm ít nhất 50% thời gian; độ chính xác phát hiện nhóm vấn đề trùng lặp đạt từ 90% trở lên. |
| Phương án không dùng AI |Dùng từ khóa, mã lỗi, danh mục sự cố và bộ lọc trong Google Sheets để nhóm dữ liệu. |
| Giả thuyết về AI (nếu có) |AI có thể đọc hiểu ngữ nghĩa, nhận diện các phản hồi khác cách diễn đạt nhưng cùng bản chất, tự động nhóm và gợi ý vấn đề cần ưu tiên. |
| Cảm nhận nhanh | Agent kết hợp Workflow (cần kiểm chứng với Rule và Workflow đơn giản hơn). |

Quy trình nháp hiện tại:

```
Thu thập phản hồi từ nhiều nguồn
                ↓
Đọc từng phản hồi
                ↓
Đối chiếu nội dung tương tự
                ↓
Nhóm các vấn đề trùng lặp
                ↓
Thống kê lỗi phổ biến
                ↓
Xác định mức độ ưu tiên
                ↓
Báo cáo và đề xuất cải tiến
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhân viên CSKH gặp lỗi trên hệ thống, họ muốn có hướng dẫn xử lý rõ ràng, để không phải liên hệ bộ phận kỹ thuật nhiều lần. |
| Actor |Nhân viên CSKH; Developer; Nam – Junior Product Manager. |
| Thời điểm / bối cảnh |Khi nhân viên CSKH gặp lỗi trong quá trình sử dụng hệ thống chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |1. Nhân viên phát hiện lỗi. 2. Tìm hướng dẫn xử lý. 3. Không tìm được thì liên hệ kỹ thuật. 4. Mô tả tình trạng lỗi. 5. Nhận hướng dẫn. 6. Thực hiện và phản hồi kết quả. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Nhân viên phải tìm kiếm tài liệu hoặc chờ Developer phản hồi; giả định mất 10–20 phút cho mỗi trường hợp cần hỗ trợ. |
| Impact (nếu không giải thì sao) |Tăng thời gian xử lý, gây quá tải cho Developer, ảnh hưởng trải nghiệm khách hàng và hiệu suất CSKH. |
| Success metric (baseline → target) |Baseline giả định: 10–20 phút/lần hỗ trợ. Target: giảm ít nhất 40% thời gian tìm kiếm hướng dẫn và giảm số lượt hỏi lại kỹ thuật. |
| Phương án không dùng AI |Xây dựng thư viện FAQ, tài liệu hướng dẫn và quy trình xử lý lỗi theo từng tình huống. |
| Giả thuyết về AI (nếu có) |AI có thể tìm kiếm tài liệu, hiểu tình huống nhân viên mô tả và đưa ra hướng dẫn xử lý phù hợp. |
| Cảm nhận nhanh |Workflow kết hợp AI hoặc Agent tra cứu tài liệu. |

Quy trình nháp hiện tại:

```
Nhân viên CSKH gặp lỗi
          ↓
Tìm kiếm tài liệu hướng dẫn
          ↓
Không tìm thấy hướng xử lý
          ↓
Liên hệ bộ phận kỹ thuật
          ↓
Chờ phản hồi hướng dẫn
          ↓
Thực hiện xử lý lỗi
          ↓
Phản hồi kết quả

```

### Card muốn pitch nhất

- Card số:2
- Vì sao:
 +Phải đọc và tổng hợp lượng lớn phản hồi từ nhiều nguồn.
 +Các phản hồi có thể khác cách diễn đạt nhưng cùng một nguyên nhân.
 +Khó phát hiện lỗi phổ biến nếu chỉ kiểm tra thủ công.
 +Có thể đo thời gian, độ chính xác và tỷ lệ phát hiện lỗi trùng lặp.
 +Có cơ hội so sánh rõ ràng giữa Rule, Workflow và Agent.
- Câu hỏi muốn nhóm phản biện:
Liệu AI Agent có thực sự cần thiết để phát hiện và nhóm các vấn đề trùng lặp, hay một Workflow kết hợp AI phân loại ngữ nghĩa đã đủ giải quyết bài toán với chi phí thấp và dễ kiểm soát hơn?
### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Chưa chứng minh được các phản hồi khác nhau thực sự có cùng nguyên nhân. |Đồng ý |Bổ sung bước đối chiếu, xác minh nhóm lỗi và kiểm chứng bằng dữ liệu thực tế. |

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
