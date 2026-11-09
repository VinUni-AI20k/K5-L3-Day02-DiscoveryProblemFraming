# Báo cáo cá nhân — 2A202603563_NguyenDucMinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Đức Minh
- MSSV: 2A202603563
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: 3AE
- Link repo nhóm: https://github.com/hoangtukhoi/K5-L3A-Day02-Nhom3AE-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)|
|---:|---|---|---|---|
| 1 | Pain từ người khác | Khi nhận ca, tôi muốn biết ngay ca trước để lại việc gì dở và tiền két có khớp không, để không sót việc hay gánh khoản lệch không phải của mình | Nhân viên ca sau, quản lý cửa hàng | ~10 phút/lần giao ca; ~2–3 lần/tháng sót việc hoặc lệch tiền (ước lượng, chưa phỏng vấn) |
| 2 | Tốn thời gian | Khi hết ca, tôi muốn báo cáo doanh thu, hàng bán và sự cố trong ca cho quản lý, để quản lý nắm tình hình mà không phải gọi hỏi | Trưởng ca, quản lý | ~15 phút/báo cáo; ~2 lần/tuần quản lý nhắn hỏi lại (ước lượng) |
| 3 | Pain từ người khác | Khi có nhân viên mới vào làm, tôi muốn họ tự tra được quy trình (pha chế, thu ngân, đóng cửa), để không phải hỏi lại người cũ nhiều lần | Nhân viên mới, nhân viên kèm | ~10 câu hỏi lặp lại/ngày trong tuần đầu; ~7–10 ngày đến khi làm được một mình (ước lượng) |
| 4 | Lặp lại | Khi đầu ca có người báo nghỉ đột xuất, tôi muốn tìm nhanh người làm thay, để ca không bị thiếu người | Quản lý, nhân viên trong ca | ~2–4 lần/tháng; ~20 phút nhắn gọi tìm người (ước lượng) |
| 5 | Lặp lại | Khi khách hỏi cùng một câu (giờ mở cửa, khuyến mãi, đổi trả), tôi muốn trả lời nhanh và đúng, để không làm chậm hàng đợi | Nhân viên thu ngân, khách | ~10–15 lần/ca bị hỏi câu giống nhau (ước lượng) |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi cuối tháng tính lương, tôi muốn đối chiếu giờ làm thực tế với lịch ca và đơn xin nghỉ, để trả lương đúng và không bị khiếu nại | Quản lý, nhân viên | ~4–6 giờ/tháng đối chiếu; ~1–2 lần/tháng nhân viên khiếu nại sai giờ (ước lượng) |


**Dùng AI:** để thảo luận các bối cảnh để lựa chọnt. Bỏ bối cảnh ở xưởng sản xuất vì hôm nay chưa có người để kiểm chứng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Giao ca | Lặp mỗi ngày, quy trình rõ, dễ hỏi người thật | Pain là sót việc hay lệch tiền? |
| 2 | Báo cáo cuối ca | Lặp mỗi ca, đo được thời gian | Quản lý có đọc kỹ báo cáo không? |
| 3 | Nhân viên mới hỏi lại quy trình | Pain từ cả người mới và người kèm | Chỉ nặng ở tuần đầu |

### Problem Card #1 — Giao ca

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận ca, tôi muốn biết ngay ca trước để lại việc gì dở và tiền két có khớp không, để không sót việc hay gánh khoản lệch không phải của mình |
| Actor | Nhân viên bán thời gian ca sau |
| Thời điểm / bối cảnh | Lúc đổi ca, cửa hàng vẫn có khách |
| Quy trình hiện tại | 1. Ca trước đếm két · 2. Kiểm hàng · 3. Ghi sổ / nhắn nhóm chat · 4. Ca sau đọc lại · 5. Đếm lại két · 6. Hỏi lại chỗ chưa rõ |
| Bottleneck | Bước 4–6 (dự đoán): tin quan trọng trôi trong nhóm chat, ~8 phút (ước lượng) |
| Impact | Sót đơn đặt trước, khách phàn nàn; lệch tiền không rõ ca nào |
| Success metric | Số lần hỏi lại: ~5/tuần → tối đa 1; lệch tiền không rõ nguyên nhân: ~2/tháng → 0 |
| Phương án không dùng AI | Mẫu sổ giao ca cố định, ca sau ký xác nhận |
| Giả thuyết về AI | Chưa cần |
| Cảm nhận nhanh | Rule |

```text
[Đếm két 5'] → [Kiểm hàng 3'] → [Ghi sổ 2'] → [Ca sau đọc 3'] ← BOTTLENECK → [Đếm lại 5'] → [Hỏi lại 5']   (tổng ~23', ước lượng)
```

### Problem Card #2 — Báo cáo cuối ca

| Trường | Nội dung |
|---|---|
| Job Story | Khi hết ca, tôi muốn báo cáo doanh thu, hàng bán và sự cố trong ca cho quản lý, để quản lý nắm tình hình mà không phải gọi hỏi |
| Actor | Trưởng ca |
| Thời điểm / bối cảnh | 10–15 phút cuối ca |
| Quy trình hiện tại | 1. Xem số trên máy bán hàng · 2. Đếm hàng tồn · 3. Nhớ lại sự cố trong ca · 4. Viết tin nhắn báo cáo · 5. Gửi quản lý · 6. Trả lời câu hỏi lại |
| Bottleneck | Bước 3–4: nhớ và viết lại sự cố, ~7 phút (ước lượng) |
| Impact | Quản lý thiếu thông tin, phải gọi hỏi; sự cố lặp lại không ai ghi nhận |
| Success metric | ~15 phút/báo cáo → dưới 5 phút; số lần quản lý hỏi lại: ~2/tuần → 0 |
| Phương án không dùng AI | Mẫu báo cáo cố định; số liệu lấy thẳng từ máy bán hàng |
| Giả thuyết về AI | Nếu phần sự cố dài, có thể tóm tắt từ ghi chú trong ca |
| Cảm nhận nhanh | Rule / Workflow |

```text
[Xem số 2'] → [Đếm tồn 5'] → [Nhớ sự cố 3'] → [Viết báo cáo 4'] ← BOTTLENECK → [Gửi 1'] → [Trả lời hỏi lại 3']   (tổng ~18', ước lượng)
```

### Problem Card #3 — Nhân viên mới hỏi lại quy trình

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhân viên mới vào làm, tôi muốn họ tự tra được quy trình (pha chế, thu ngân, đóng cửa), để không phải hỏi lại người cũ nhiều lần |
| Actor | Nhân viên mới và người kèm |
| Thời điểm / bối cảnh | 1–2 tuần đầu đi làm |
| Quy trình hiện tại | 1. Người cũ chỉ miệng · 2. Người mới làm thử · 3. Quên thì hỏi lại · 4. Người cũ dừng việc để chỉ · 5. Lặp lại đến khi thuộc |
| Bottleneck | Bước 3–4: hỏi lại và người cũ phải dừng việc, ~10 lần/ngày (ước lượng) |
| Impact | Chậm phục vụ giờ đông khách; người cũ mệt; người mới làm sai |
| Success metric | Số câu hỏi lại/ngày: ~10 → 3; số ngày đến khi làm một mình: ~10 → 5 |
| Phương án không dùng AI | Sổ tay quy trình ngắn có ảnh, dán tại quầy |
| Giả thuyết về AI | Chưa cần |
| Cảm nhận nhanh | No AI |

```text
[Chỉ miệng 15'] → [Làm thử] → [Quên, hỏi lại 2'/lần] ← BOTTLENECK → [Người cũ dừng việc chỉ 3'/lần] → [Lặp lại ~10 lần/ngày]
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: ai cũng hiểu, dễ phỏng vấn người thật, quy trình giống giao ca ở xưởng sản xuất.
- Câu hỏi muốn nhóm phản biện: mẫu sổ giao ca cố định đã đủ chưa?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: quy trình và số phút đang là đoán, chưa hỏi người làm ca thật | Đồng ý | Ghi rõ "ước lượng" cạnh mọi con số; đưa vào việc cần phỏng vấn |
| Card #1: bottleneck có thể là "quên ghi" ở bước 3, không phải "đọc lại" | Đồng ý một phần | Giữ bước 4–6 nhưng ghi là "dự đoán", cần hỏi người làm ca để chốt |
| Card #2: chưa chắc quản lý đọc phần sự cố hay chỉ xem doanh thu | Đồng ý | Ghi vào cột "Điều còn chưa chắc" của bảng top 3 |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch 3 card: giao ca, báo cáo cuối ca, nhân viên mới hỏi lại quy trình | Card giao ca được xếp vào cụm A "thông tin bàn giao", cụm nhóm chọn |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Thông tin hay thiếu nhất là gì? Thêm ô bắt buộc vào form đặt lịch đã đủ chưa?" (candidate làm rõ mô tả nhu cầu của Nguyễn Minh Quân) | Nhóm giữ Rule (form bắt buộc) làm phương án quay về và làm giả định #2 |
| Nhận phản biện | Câu hỏi tôi nhận được: "Lần gần nhất bàn giao chỉ bằng hỏi lại ca trước khiến bạn bỏ sót việc là khi nào, hậu quả là gì?" (Nguyễn Minh Quân) | Tôi đã sửa gì: thừa nhận chưa có chuyện cụ thể, ghi số liệu card #1 là ước lượng |
| Gom cluster / cây OST | Hỗ trợ Nguyễn Minh Quân gom 12 candidate thành 3 cụm | Cụm A, B, C và cây OST ở mục 2.2–2.3 |
| Chọn candidate problem | Hỗ trợ chấm điểm shortlist | Chọn candidate "làm rõ mô tả nhu cầu" (26 điểm) |
| Kiểm chứng / research | Người chính toàn bộ CP4 (Nguyễn Minh Quân, Phan Gia Bảo, Vũ Lê Hoàng hỗ trợ): assumption map 4 giả định, 3 snapshot từ tư liệu công khai, bảng research 3 giải pháp có link | Nhóm thu hẹp problem thành "cố vấn thiếu bộ câu hỏi bổ sung"; tìm ra myKaarma đã làm gần đúng bài này |
| Quy trình nhóm | Hỗ trợ Phan Gia Bảo vẽ quy trình trước/sau | Mục 4 báo cáo nhóm |
| Problem Statement | Hỗ trợ viết v0, góp ý thêm metric chất lượng ở v1 | v1 có thêm số lần kỹ thuật viên hỏi lại |
| Mức can thiệp AI | Hỗ trợ Vũ Lê Hoàng so sánh 4 mức | Chọn Workflow, Rule làm phương án quay về |
| Quyết định | Hỗ trợ chấm 4 rủi ro | Not Yet, vì Value chỉ có bằng chứng từ Mỹ và Viability ở mức Cao |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Hỏi Claude gợi ý bối cảnh | Đưa nhiều bối cảnh để chọn | Gợi ý lệch hướng: lúc đầu toàn chuyện học tập, lab, đời sống sinh viên, không phải bối cảnh đi làm | Yêu cầu đổi sang bối cảnh đi làm, chọn vận hành cửa hàng/quán |
| CP2 Problem Card | Nhờ soạn nháp 3 card và phản biện card | Giữ đúng khuôn bài mẫu, chỉ ra số liệu đang là đoán | Card đầu tiên dài, lẫn chuyện cá nhân không liên quan | Bắt viết ngắn lại, bỏ phần không liên quan, ghi rõ "ước lượng" |
| CP4 Research | Tìm tư liệu công khai và công cụ đã có | Tìm được 3 nguồn người trong nghề kể chuyện thật và công cụ myKaarma | Cả 3 nguồn đều ở Mỹ; một số trang không mở được | Ghi rõ đây là tư liệu công khai, không phải nhóm tự phỏng vấn; ghi giới hạn vào tín hiệu phản bác |
| CP5 Quy trình | Nhờ dựng quy trình hiện tại và tương lai | Có ngay khung 6 bước, boundary, phương án quay về | Số phút từng bước là ước lượng, không có nguồn | Ghi chú "ước lượng, chưa bấm giờ" trong báo cáo |
| CP5–6 Problem Statement | Nhờ soạn v0, v1 | Chỉ ra metric v0 chỉ đo tốc độ | Viết dài, nhiều thuật ngữ | Rút gọn, giữ metric chất lượng ở v1 |
| CP6 Mức can thiệp / quyết định | Nhờ so sánh 4 mức và chấm rủi ro | Lập luận rõ vì sao không dừng ở Rule | Dễ nghiêng về chọn AI dù bằng chứng còn yếu | Chọn Not Yet, đặt ngưỡng dừng: thông tin thiếu chỉ vài mục cố định thì dừng ở Rule |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Mình nhận ra nhiều card thực chất là cùng một vấn đề, thông tin bị thiếu khi chuyển từ người này sang người khác, giống hệt card giao ca của mình dù bối cảnh khác hẳn.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có. Một số candidate viết thẳng giải pháp: "có bảng báo giá sơ bộ", "đồng bộ booking thành lệnh sửa chữa", "từ điển mã lỗi chung". Khi vẽ cây OST, nhóm hỏi lại "nỗi khó thật ở đây là gì" và chuyển các ý này xuống mục giải pháp đội lốt, không đưa vào nhánh.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có đổi ý sau khi bị phản biện. Thành viên nhóm hỏi mình lần gần nhất việc giao ca bị sót là khi nào, hậu quả ra sao. Mình không kể được chuyện cụ thể nào, nên đã thừa nhận số liệu card giao ca chỉ là ước lượng và ghi rõ như vậy trong báo cáo.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Có hai điều. Thứ nhất, ở Mỹ đã có công cụ (myKaarma) gửi bảng hỏi cho khách trước khi xe tới, gần đúng bài của nhóm. Thứ hai, một diễn đàn quản lý xưởng cho rằng lỗi nằm ở thói quen hỏi của cố vấn, không chỉ ở khách mô tả kém.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Đặt success metric có baseline thật. Nhóm không bấm giờ được ở xưởng nên phải để đo và ghi rõ số phút là ước lượng.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Mình sẽ phỏng vấn người thật ngay từ đầu (thành viên nhóm khác), hoặc là đổi bối cảnh chủ đề, vì cả ba nguồn trên mạng đều ở Mỹ. Mình cũng sẽ phản biện mạnh hơn việc chọn Workflow: nếu thông tin thiếu chỉ là vài mục cố định thì form bắt buộc đã đủ.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Problem: cố vấn dịch vụ phải gọi lại khách nhiều đợt vì mô tả nhu cầu lúc đặt lịch thiếu. Quy trình hiện tại có 6 bước, nghẽn ở bước gọi lại khách hỏi thêm. Metric là số lần gọi lại mỗi lịch, thời gian tiếp nhận mỗi lượt và số lần kỹ thuật viên hỏi lại cố vấn. Boundary: AI không chẩn đoán, không báo giá, không tự liên hệ khách, cố vấn duyệt mọi thứ. Mức can thiệp là Workflow: form bắt buộc (Rule) rồi AI gợi ý câu hỏi còn thiếu, cố vấn duyệt. Quyết định là Not Yet vì bằng chứng chỉ có từ Mỹ và chưa biết quy định dữ liệu của xưởng. Nếu khảo sát cho thấy thông tin thiếu chỉ là vài mục cố định thì dừng ở Rule.

---

## 7. Tài liệu tham khảo

- [KTAR — Ever have your auto shop fix the wrong noise](https://ktar.com/uncategorized/ever-have-your-auto-shop-fix-the-wrong-noise)
- [DealersEdge forum — Terminology](https://forums.dealersedge.com/viewtopic.php?p=48481)
- [DealerELITE — The 3 C's: Customer concern](https://www.dealerelite.net/profiles/blogs/the-3c-s-customer-concern)
- [myKaarma — Service Pre-Diag AI Overview](https://support.mykaarma.com/hc/en-us/articles/45647747400211-Service-Pre-Diag-AI-Overview-Smarter-Service-Conversations-Before-Check-In)
- [Brake & Front End — ASE C1 Test Prep, Customer Interview and Write Up](https://www.brakeandfrontend.com/ase-c1-test-prep-customer-interview-and-write-up/)
- [Motor Magazine — Make Your Initial Assessment Count (2012)](https://www.motor.com/wp-content/uploads/MakeYourInitialAssessmentCount-Feb-2012.pdf)
