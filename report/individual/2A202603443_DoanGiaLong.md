# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đoàn Gia Long
- MSSV: 2A202603443
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Ban3
- Link repo nhóm: https://github.com/LysLama/K5-L3A-DAY02-Ban3-DiscoveryProblemFraming/tree/main

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi đến siêu thị mua đồ sau khi đi làm về tôi muốn mua đồ để nấu bữa cơm tối cho cả gia đình | Bố, mẹ | mua đồ trong khoảng 20 phút, tần suất hàng ngày |
| 2 | Lặp lại |Khi tôi đến siêu thị thì tôi phải suy nghĩ là hôm nay nấu món gì để phù hợp với khẩu vị ăn của cả gia đình và khác món bữa trước | cả gia đình | Thời gian suy nghĩ trên đường từ công ty đến siêu thị |
| 3 | Tốn thời gian|Khi tôi đến siêu thị thì tôi chỉ muốn mua đúng những đồ để nấu những món ăn tôi đã nghĩ đến trên đường từ công ty đến siêu thị | Tôi, Bố, Mẹ | Mất 10 phút để đi loanh quanh tìm đúng đồ theo ý muốn, và hỏi 2-3 bạn nhân viên siêu thị để tìm được đúng đồ mình muốn |
| 4 |Cần đọc, tổng hợp nhiều thông tin |Khi tôi tìm được đồ mình muốn mua thì tôi phải đọc thông tin sản phẩm để so sánh các thông tin và chọn xem sản phẩm nào phù hợp | Tôi, Bố, Mẹ |trung bình mất 2 phút/sản phẩm để đọc |
| 5 |Pain từ người khác |Khi đã chọn được sản phẩm phù hợp về nấu ăn thì tôi phải xem xét bố mẹ tôi có bị dị ứng gì với sản phẩm đó không để tránh bố mẹ tôi bị dị ứng với một số chất trong sản phẩm đó | Bố, Mẹ |Cần 1 phút/sản phẩm để check lại thông tin dị ứng của bố mẹ tôi |
| 6 | Lặp lại |Khi tôi đã biết bố mẹ dị ứng với gì thì tôi phải kiểm tra từng sản phẩm để không bỏ sót sản phẩm nào không phù hợp mà có thể đảm bảo độ ngon của món ăn đó | Tôi |2 phút cuối khi đã mau đủ đồ và checklist lại trước khi thanh toán, tần suất là 1 lần trên 1 lượt đi siêu thị |
| 7 |Tốn thời gian |Khi đã chọn đủ đồ thì nếu còn thời gian thì tôi có thể đi xem 1 số sản phảm khác trong siêu thị mà tôi có thể thích và định mua để đỡ phải mất thời gian đi mua | Tôi, Bố, Mẹ| 10-15 phút cuối/1 lần đi siêu thị, nếu như bố mẹ tôi không dục về sớm |

**AI gợi ý thêm**: sau khi tự scan 7 ý, Minh hỏi AI và giữ lại ý #2, #4, #6. Bỏ các ý còn lại vì khó đo lường data thật

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Nghĩ món ăn |Lặp lại hàng ngày, nhiều người chịu ảnh hưởng (cả nhà), có nhiều gợi ý món ăn |Chưa có baseline (nghĩ mất bao nhiêu phút?). Đây có phải pain thật hay chỉ là việc quen thuộc? |
| 2 | đọc, so sánh thông tin sản phẩm |Có sẵn thông tin trên sản phẩm; Có baseline đo được (~2 phút/sản phẩm), lặp lại mỗi lần đi siêu thị | Thông tin trên nhãn có đủ rõ, đủ ảnh chụp để AI đọc chính xác không? “Sản phẩm phù hợp” tiêu chí là gì? |
| 3 |Checklist lại trước khi thanh toán |Pain từ người khác, có rủi ro sức khỏe nếu bỏ sót, lặp lại mỗi lượt đi siêu thị |Mới có 2 phút/lượt, chưa có bằng chứng từng xảy ra sự cố. Sợ bỏ sót thì có thật không, hay chỉ là lo xa? |

### Problem Card #1 Đọc, so sánh thông tin sản phẩm

| Trường | Nội dung |
|---|---|
| Job Story | Khi tìm được đồ cần mua ở siêu thị, tôi muốn đọc và so sánh nhanh thông tin các sản phẩm, để chọn được sản phẩm phù hợp mà không mất nhiều thời gian |
| Actor |Người đi chợ nấu cơm tối cho cả nhà (tôi) |
| Thời điểm / bối cảnh |Chiều tối sau giờ làm, đứng trước kệ hàng ở siêu thị, đang vội về nấu cơm |
| Quy trình hiện tại (3–7 bước) |. Cầm 2-3 sản phẩm cùng loại · 2. Tìm và đọc nhãn thành phần · 3. Đọc hạn dùng, trọng lượng, giá · 4. So sánh trong đầu · 5. Chọn và bỏ vào giỏ |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2-4: nhãn chữ nhỏ, nhiều thông tin, phải tự so sánh |
| Impact (nếu không giải thì sao) |2 phút/sản phẩm. Nếu mua khoảng 5 sản phẩm/lượt thì ~10 phút/lượt, ~70 phút/tuần (giả định, cần đo lại) |
| Success metric (baseline → target) |Thời gian chọn sản phẩm giảm từ 2 phút xuống dưới 30 giây, chọn xong không phải đổi ý |
| Phương án không dùng AI |Ghi sẵn tiêu chí chọn (loại, hãng quen mua) vào ghi chú điện thoại. Giảm được việc phải nghĩ, nhưng vẫn phải đọc nhãn |
| Giả thuyết về AI (nếu có) |Chụp nhãn, AI đọc và tóm tắt thành phần, hạn dùng, rồi gợi ý sản phẩm hợp nhất |
| Cảm nhận nhanh |  Workflow  |

Quy trình nháp hiện tại: 

```HIỆN TẠI: ~2 phút/sản phẩm

[1 Cầm 2-3 sản phẩm: 15s] → [2 Tìm, đọc nhãn thành phần: 50s]
→ [3 Đọc hạn dùng, giá, trọng lượng: 25s] → [4 So sánh trong đầu: 25s] ← BOTTLENECK
→ [5 Chọn, bỏ vào giỏ: 5s]

```

### Problem Card #2 Kiểm tra dị ứng cho bố mẹ

| Trường | Nội dung |
|---|---|
| Job Story | Khi đã chọn sản phẩm để nấu ăn, tôi muốn biết chắc sản phẩm không có chất bố mẹ bị dị ứng, để cả nhà ăn an toàn | |
| Thời điểm / bối cảnh |Ở siêu thị, ngay sau khi chọn sản phẩm, và rà lại lần cuối trước khi thanh toán |
| Quy trình hiện tại (3–7 bước) |1. Nhớ lại bố mẹ dị ứng gì · 2. Đọc thành phần sản phẩm · 3. Đối chiếu từng chất · 4. Không chắc thì tra Google hoặc gọi hỏi bố mẹ · 5. Bỏ vào giỏ · 6. Rà lại cả giỏ trước khi thanh toán |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2-3: thành phần dài, tên chất lạ, dễ bỏ sót |
| Impact (nếu không giải thì sao) |1 phút/sản phẩm + 2 phút rà cuối. Nếu bỏ sót, bố mẹ có thể bị dị ứng (chưa có bằng chứng từng xảy ra, cần xác nhận) |
| Success metric (baseline → target) |Mỗi sản phẩm kiểm tra dưới 15 giây, 0 sản phẩm không phù hợp lọt vào giỏ |
| Phương án không dùng AI |Ghi danh sách chất dị ứng của bố mẹ vào ghi chú điện thoại, dán sẵn trong giỏ. Đỡ phải nhớ, nhưng vẫn phải tự đọc và đối chiếu |
| Giả thuyết về AI (nếu có) |Lưu sẵn hồ sơ dị ứng của bố mẹ. Chụp nhãn, AI báo ngay “an toàn” hoặc “có chất cần tránh” |
| Cảm nhận nhanh |  Rule / Workflow / Agent  |

Quy trình nháp hiện tại:

```HIỆN TẠI: ~1 phút/sản phẩm + 2 phút rà cuối

[1 Nhớ bố mẹ dị ứng gì: 10s] → [2 Đọc thành phần: 25s]
→ [3 Đối chiếu từng chất: 15s] ← BOTTLENECK → [4 Không chắc: tra Google / gọi hỏi: 10s]
→ [5 Bỏ vào giỏ] → [6 Rà lại cả giỏ trước thanh toán: 2 phút]

```

### Problem Card #3 Nghĩ món ăn hôm nay

| Trường | Nội dung |
|---|---|
| Job Story | Khi đang trên đường từ công ty đến siêu thị, tôi muốn nhanh chóng có món ăn phù hợp khẩu vị cả nhà và khác bữa trước, để mua đúng nguyên liệu |
| Actor |Người nấu cơm tối (tôi), người chịu ảnh hưởng là cả gia đình |
| Thời điểm / bối cảnh |Chiều tối hàng ngày, trên đường từ công ty đến siêu thị |
| Quy trình hiện tại (3–7 bước) |1. Nhớ lại hôm qua ăn gì · 2. Nghĩ món mới · 3. Cân nhắc khẩu vị bố, mẹ, cả nhà · 4. Nghĩ trong nhà còn gì · 5. Liệt kê nguyên liệu trong đầu · 6. Đến siêu thị mới nhớ ra thiếu hoặc quên |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2-3: nghĩ món vừa mới vừa hợp khẩu vị |
| Impact (nếu không giải thì sao) |Hàng ngày, cả nhà ảnh hưởng. Thời gian nghĩ: ? phút/ngày (chưa đo, cần đo trong vài ngày) |
| Success metric (baseline → target) |Có món và danh sách nguyên liệu trong dưới 2 phút, không lặp món 3 ngày liền |
| Phương án không dùng AI |Lập sẵn thực đơn cả tuần vào cuối tuần. Hiệu quả, nhưng tốn công và không linh hoạt khi thay đổi |
| Giả thuyết về AI (nếu có) |AI nhớ khẩu vị cả nhà và các món đã ăn, gợi ý 2-3 món và xuất ngay danh sách nguyên liệu |
| Cảm nhận nhanh | No AI  |

Quy trình nháp hiện tại:

```HIỆN TẠI: ? phút (chưa đo)

[1 Nhớ hôm qua ăn gì: ?'] → [2 Nghĩ món mới: ?'] ← BOTTLENECK
→ [3 Cân nhắc khẩu vị cả nhà: ?'] → [4 Nghĩ trong nhà còn gì: ?']
→ [5 Liệt kê nguyên liệu trong đầu: ?'] → [6 Đến siêu thị, quên hoặc thiếu đồ]

```

### Card muốn pitch nhất

- Card số: #2 Kiểm tra dị ứng cho bố mẹ
- Vì sao: Vì khâu này vừa cần đọc thông tin vừa cần kiểm tra so sánh với các chất dị ứng của bố mẹ vừa phải đảm bảo độ ngon của món ăn
- Câu hỏi muốn nhóm phản biện: Tại sao card này quan trọng và cần thiết nhất

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Lý do pitch bị lệch trọng tâm. “Đảm bảo độ ngon của món ăn” không liên quan đến dị ứng | Đồng ý |Bỏ ý “độ ngon”, viết lại lý do chỉ xoay quanh an toàn sức khỏe |
| Chưa có bằng chứng thật. Mới có “2 phút/lượt”, chưa nói bố mẹ dị ứng gì, chưa rõ đã từng gặp sự cố hay suýt gặp chưa | Đồng ý | Bổ sung nhóm chất dị ứng cụ thể và hỏi bố mẹ xem đã từng có sự cố chưa
| Giá trị không nằm ở thời gian. Tiết kiệm 2-3 phút/lượt thì nhỏ, dễ bị hỏi “có đáng làm không?” | Đồng ý |y


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
