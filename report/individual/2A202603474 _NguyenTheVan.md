# Báo cáo cá nhân — 2A202603474 _NguyenTheVan

## 1. Thông tin học viên

- Họ tên: Nguyễn Thế Văn
- MSSV: 2A202603474
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:
- Link repo nhóm: https://github.com/zannngyn/K5-L3-Day02-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi mỗi ngày có hơn 50 sản phẩm mới cần đăng lên các fanpage, tôi muốn biến thông tin sản phẩm thành bài đăng hoàn chỉnh mà không phải copy qua lại giữa nhiều nơi, để kịp lịch đăng trong ngày | Nhân viên content, quản lý fanpage | Mỗi người >10 bài/ngày, 10–15 phút thao tác/bài (copy sản phẩm → soạn → dán lên FB → đăng), tức 100–150 phút/ngày/người |
| 2 | Pain từ người khác | Khi một bài trên fanpage bị sai giá hoặc sai thông tin, tôi muốn biết ai đã đăng và ai đã duyệt, để sửa nhanh và nhắc đúng người | Quản lý, nhân viên content, khách hàng | 5–10 lần/tháng phải hỏi trong group "ai đăng bài này"; mỗi lần 10–15 phút mới tìm ra người |
| 3 | Tốn thời gian | Khi bài viết xong phải chờ quản lý duyệt, tôi muốn biết bài đang kẹt ở đâu, để không lỡ khung giờ đăng đã định | Nhân viên content, quản lý | Chờ duyệt trung bình 15 phút/bài; 4–5 bài/tuần đăng trễ giờ |
| 4 | Lặp lại | Khi có nhiều bài cần lên trong tuần, tôi muốn thấy bài nào đăng giờ nào trên trang nào, để không bị trùng giờ hoặc bỏ trống ngày | Nhân viên content, quản lý | Hơn 10 fanpage, 50–60 bài/tuần/trang; tuần trước bị trùng hoặc trống lịch 10 lần |
| 5 | Pain từ người khác *(ý từ AI)* | Khi khách nhắn fanpage hỏi giá, size, còn hàng, tôi muốn trả lời đúng và nhanh, để khách không bỏ đi | Nhân viên trực inbox, khách hàng | Khoảng 10 tin/ngày, 70% là câu hỏi lặp lại; phản hồi trung bình 5 phút |
| 6 | Cần đọc, tổng hợp nhiều thông tin *(ý từ AI)* | Khi cuối tuần cần báo cáo hiệu quả fanpage, tôi muốn biết bài nào có tương tác tốt và vì sao, để lên kế hoạch content tuần sau | Nhân viên content, quản lý marketing | 120 phút/tuần xem từng bài trong Insights rồi chép ra Sheets |
| 7 | Cần đọc, tổng hợp nhiều thông tin *(ý từ AI)* | Khi nhận yêu cầu sửa giao diện từ nhiều kênh (chat, email, comment Figma), tôi muốn có một danh sách đầy đủ và mới nhất, để không làm sót hoặc làm theo bản cũ | Lập trình viên FE, designer, PM | Tuần trước sót 3 yêu cầu; 2 lần làm lại vì theo bản cũ |
| 8 | Tốn thời gian *(ý từ AI)* | Khi review pull request của đồng đội, tôi muốn nắm nhanh thay đổi nào ảnh hưởng UI, để review kỹ đúng chỗ trước khi merge | Lập trình viên FE, reviewer | 10 PR/tuần, khoảng 2 phút/PR |
| 9 | Lặp lại *(ý từ AI)* | Khi có thông báo đổi hạn nộp bài trên Discord lớp, tôi muốn biết ngay deadline mới, để không nộp trễ | Sinh viên, coach | Trễ hoặc suýt trễ 1 lần/tháng; 10 phút/tuần lướt lại các kênh |
| 10 | Pain từ người khác *(ý từ AI)* | Khi nhóm đi chơi chung và nhiều người cùng trả tiền, tôi muốn biết mỗi người còn nợ ai bao nhiêu, để chia sòng phẳng mà không phải hỏi lại | Bạn bè trong nhóm | Chuyến gần nhất 8 người, 5 khoản chi, mất 60 phút tính lại |

*Số liệu là ước lượng từ trải nghiệm của tôi, chưa bấm giờ chính xác.*

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Dòng 1–4 là ý của tôi; AI giúp viết lại thành Job Story và tách ý gốc thành nhiều problem.
- Giữ lại dòng 5–10 (ý từ AI) vì tôi đã gặp những việc này và tự ước lượng được số liệu.
- Bỏ: ý "công cụ tự viết và đăng bài tự động", vì đây là giải pháp chứ không phải problem, và không có bước người duyệt.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Soạn và đăng bài sản phẩm hàng loạt lên fanpage (CP1 #1, #3) | Lặp lại mỗi ngày, 100–150 phút/ngày/người, 4–5 bài/tuần đăng trễ | Phút từng bước chưa đo; chưa chắc bước soạn bài hay chờ duyệt là nghẽn chính |
| 2 | Không biết ai đã đăng, ai đã duyệt một bài (CP1 #2) | 5–10 lần/tháng, bài sai đến tay khách | Facebook có thể đã lưu thông tin này, chỉ là team không biết xem ở đâu |
| 3 | Lên lịch đăng bài cho nhiều fanpage (CP1 #4) | Hơn 10 trang, 10 lần trùng hoặc trống lịch tuần trước | Có thể chỉ cần dùng lịch có sẵn của Facebook |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi mỗi ngày có hơn 50 sản phẩm mới cần đăng lên các fanpage, tôi muốn biến thông tin sản phẩm thành bài đăng hoàn chỉnh mà không phải copy qua lại giữa nhiều nơi, để kịp lịch đăng trong ngày |
| Actor | Nhân viên content phụ trách fanpage bán hàng (mỗi người >10 bài/ngày); quản lý duyệt bài |
| Thời điểm / bối cảnh | Hằng ngày, khi có sản phẩm mới hoặc chương trình khuyến mãi |
| Quy trình hiện tại (3–7 bước) | 1. Copy thông tin sản phẩm (tên, giá, mô tả, ảnh) · 2. Dán vào công cụ AI để viết bài · 3. Sửa lại bài · 4. Dán lên Facebook · 5. Gửi quản lý duyệt và chờ · 6. Đăng |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5, chờ duyệt: trung bình 15 phút/bài, lâu hơn toàn bộ phần thao tác (10–15 phút/bài) và là nguyên nhân của 4–5 bài/tuần đăng trễ |
| Impact (nếu không giải thì sao) | 1 người: >10 bài × 10–15 phút = 100–150 phút/ngày thao tác tay, chưa tính thời gian chờ. Cả team: hơn 10 trang × 50–60 bài/tuần ≈ 500–600 bài/tuần ≈ 83–150 giờ công/tuần. 4–5 bài/tuần lỡ khung giờ đăng |
| Success metric (baseline → target) | (1) Thời gian từ lúc có sản phẩm đến lúc bài lên: 28 phút/bài (13 thao tác + 15 chờ) → dưới 10 phút/bài; (2) bài đăng trễ: 4–5/tuần → ≤1/tuần. Đo bằng bấm giờ 20 bài trong 1 tuần |
| Phương án không dùng AI | Template bài cố định theo loại sản phẩm + một file sản phẩm chuẩn (tên, giá, ảnh) để copy 1 lần; quy định khung giờ duyệt cố định trong ngày |
| Giả thuyết về AI (nếu có) | AI soạn nháp bài từ file sản phẩm; người sửa, quản lý duyệt trước khi đăng |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 28 phút/bài (13' thao tác + 15' chờ)

[1 Copy thông tin SP: 3'] → [2 Dán vào AI viết: 2'] → [3 Sửa bài: 5'] → [4 Dán lên FB: 2']
→ [5 Chờ duyệt: 15'] ← BOTTLENECK → [6 Đăng: 1']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi một bài trên fanpage bị sai giá hoặc sai thông tin, tôi muốn biết ai đã đăng và ai đã duyệt, để sửa nhanh và nhắc đúng người |
| Actor | Quản lý fanpage; nhân viên content |
| Thời điểm / bối cảnh | Khi khách comment hoặc inbox báo bài sai |
| Quy trình hiện tại (3–7 bước) | 1. Phát hiện bài sai (qua khách hoặc tự thấy) · 2. Hỏi trong group chat "ai đăng bài này" · 3. Chờ người nhận · 4. Người đó sửa bài · 5. Trả lời khách |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3, hỏi và chờ người nhận: 10–15 phút/lần |
| Impact (nếu không giải thì sao) | 5–10 lần/tháng × 10–15 phút = 50–150 phút/tháng chỉ để tìm người; trong thời gian đó bài sai vẫn hiển thị với khách |
| Success metric (baseline → target) | Thời gian tìm ra người đăng: 10–15 phút → dưới 2 phút, đếm từ group chat trong 1 tháng |
| Phương án không dùng AI | Quy ước ghi tên người soạn và người duyệt vào file theo dõi bài; xem lịch sử hoạt động của Trang |
| Giả thuyết về AI (nếu có) | Không thấy cần AI |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 20–25 phút/lần xử lý, 5–10 lần/tháng

[1 Phát hiện bài sai: không tính, phụ thuộc lúc khách báo]
→ [2–3 Hỏi group "ai đăng" + chờ người nhận: 10–15'] ← BOTTLENECK
→ [4 Sửa bài: 5'] → [5 Trả lời khách: 5']

Ghi chú: "Sửa bài 5'" lấy theo bước sửa bài ở card #1; "Trả lời khách 5'" lấy theo thời gian phản hồi inbox ở CP1 #5.
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhiều bài cần lên trong tuần, tôi muốn thấy bài nào đăng giờ nào trên trang nào, để không bị trùng giờ hoặc bỏ trống ngày |
| Actor | Nhân viên content quản lý hơn 10 fanpage |
| Thời điểm / bối cảnh | Đầu tuần lên kế hoạch; trong tuần khi có bài phát sinh |
| Quy trình hiện tại (3–7 bước) | 1. Gom danh sách bài cần đăng · 2. Ghi giờ đăng vào [Sheets/ghi chú] · 3. Đến giờ thì vào từng trang đăng tay · 4. Đánh dấu đã đăng |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: phải nhớ giờ và vào từng trang trong hơn 10 trang, 3 phút/bài (dán 2' + đăng 1', theo card #1) × >10 bài/ngày = hơn 30 phút/ngày/người |
| Impact (nếu không giải thì sao) | 50–60 bài/tuần/trang; tuần trước 10 lần trùng giờ hoặc bỏ trống |
| Success metric (baseline → target) | Số lần trùng/trống lịch: 10/tuần → ≤1/tuần, đếm trong 2 tuần |
| Phương án không dùng AI | Dùng tính năng lên lịch có sẵn của Facebook và một lịch chung cho cả team |
| Giả thuyết về AI (nếu có) | Không thấy cần AI |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — hơn 30 phút/ngày/người ở bước 3, 10 lần trùng/trống tuần trước

[1 Gom danh sách bài: ~20'/tuần*] → [2 Ghi giờ vào sheet: ~30'/tuần*]
→ [3 Đến giờ vào từng trang đăng: 3'/bài × >10 bài = >30'/ngày (>150'/tuần)] ← BOTTLENECK
→ [4 Đánh dấu đã đăng: ~5'/ngày*]

* Ước lượng thô, chưa bấm giờ.
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: tốn nhiều giờ công nhất (83–150 giờ/tuần cả team), lặp lại mỗi ngày, và là card duy nhất trong 3 card so sánh được đủ 4 mức No AI / Rule / Workflow / Agent
- Câu hỏi muốn nhóm phản biện: Chờ duyệt (15 phút) đang lâu hơn soạn bài. Nếu vậy thì giúp soạn bài nhanh hơn có giảm được thời gian đến lúc bài lên không, hay phải sửa khâu duyệt trước?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Ý ban đầu "cần tự động hóa đăng bài bằng AI" là giải pháp, không phải problem | Đồng ý | Viết lại Job Story chỉ tả cái khó, bỏ chữ AI và tự động hóa |
| Ý gốc gộp 3 vấn đề khác nhau (soạn bài, duyệt, không biết ai đăng) vào một | Đồng ý | Tách thành card #1 và card #2 riêng |
| Card #1: bottleneck ghi "cả quy trình đều cần tự động" là mơ hồ và lại là giải pháp | Đồng ý | Chỉ ra 1 bước cụ thể: chờ duyệt 15 phút/bài |
| Card #1: impact "50 bài × 10 trang × 5 phút = 2500 phút/ngày cho 1 người" vô lý (hơn 41 giờ/ngày) và mâu thuẫn với số 10–15 phút/bài ở CP1 | Đồng ý | Tách số theo 1 người (100–150 phút/ngày) và theo cả team (83–150 giờ/tuần) |
| Card #1: nếu bottleneck là chờ duyệt thì AI viết bài nhanh hơn cũng không giảm tổng thời gian | Đồng ý | Thêm phương án không dùng AI cho khâu duyệt (khung giờ duyệt cố định); đưa thành câu hỏi khi pitch |
| Card #2, #3: Facebook đã có lên lịch và lịch sử hoạt động của Trang, có thể chỉ cần biết dùng | Đồng ý một phần | Đưa vào research ở CP4; cảm nhận nhanh ghi No AI / Rule |

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
