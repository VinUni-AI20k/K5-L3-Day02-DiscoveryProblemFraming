# Báo cáo cá nhân — 2A202603624_DamTuanLinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Đàm Tuấn Linh
- MSSV:2A202603624
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:TEAMLAGI
- Link repo nhóm:https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/tree/main

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Sau khi kết thúc cuộc họp cần textnote lại các task quan trọng trong cuộc họp để không phải tổng hợp thủ công |Thư ký, PM, nhân viên văn phòng |Một cuộc họp dài vài tiếng cần textnote lại những điểm key quan trọng |
| 2 |Lặp lại |Khi xem các nội dung nước ngoài cần dịch thuật real_time, cần tua đến đoạn mà nhân vật thoại một keyword nào đó |Người dùng thông thường|Xem các nội dung giảng dạy về AI bằng tiếng anh trên youtube mà không có sub,Cần tua lại đoạn thầy nói về embedding |
| 3 |Cần đọc tổng hợp thông tin |Khi tham gia nhiều cuộc họp trong tuần các quyết định của các cuộc họp liên quan chồng chéo lên nhau, có những quyết định hôm trước dc đề xuất, nhưng hôm nay lại dc bác bỏ,vv|PM, thư ký, quản lý,trưởng bộ phận, giám đốc. |Giả định một công ty bán hàng họp 3 lần trong tuần để quyết định có mua một sản phẩm từ nhà sản xuất a,b hoặc c, cần tổng hợp lại lý do chọn nsx nào, ưu điểm nhược điểm ra sao|
| 4 |Cần đọc tổng hợp thông tin |Khi phỏng vấn tuyển nhân sự, có nhiều ứng viên, và nhiều cuộc phỏng vấn với nội dung câu hỏi khác nhau, cần tổng hợp lại thông tin để lựa chọn ứng viên|Trưởng các phòng ban HR|Cần tổng hợp dữ liệu của 1000 ứng viên, tìm ra người phù hợp với vị trí trống real time, dễ dc can thiệp bởi các trưởng phòng để đóng góp ý kiến cho bộ phận HR |
| 5 |Cần đọc tổng hợp thông tin |Khi có nhiều cuộc gọi tư vấn, CSKH cần AI tóm tắt nhu cầu và vấn đề của từng khách hàng để cập nhật CRM nhanh và chăm sóc đúng nhu cầu |Sales, CSKH, quản lý kinh doanh|Một ngân hàng có hàng nghìn cuộc gọi CSKH hàng ngày nhu cầu về đánh giá tiềm năng khách hàng rất lớn, về khả năng vay,khoản vay, người vay có khả năng trả không có nguy cơ nợ xấu hay không,...  |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)


### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |CSKH mất thời gian nghe lại cuộc gọi và cập nhật thông tin lên CRM |Đội ngũ CSKH không chăm sóc đúng đối tượng, khó ghi chép, tổng hợp và mất thời gian để cập nhật vào dữ liệu hệ thống |CRM hiện có tự động ghi chú chưa? Có được phép xử lý bản ghi âm và dữ liệu cá nhân không? |
| 2 |Người xem video tiếng nước ngoài khó tìm lại đúng đoạn có thuật ngữ cần học |Nhiều người đau, impact rộng |Tần suất gặp video không có phụ đề là bao nhiêu? Công cụ phụ đề/tìm transcript sẵn có đã đáp ứng đến đâu? |
| 3 |HR khó tổng hợp, đối chiếu thông tin ứng viên từ nhiều hồ sơ và vòng phỏng vấn |Có nhiều nguồn thông tin không đồng nhất; mất thời gian chuẩn bị shortlist và trao đổi với trưởng bộ phận. |Quy mô tuyển dụng thực tế có đủ lớn? Có bộ tiêu chí đánh giá thống nhất và dữ liệu được phép dùng không? |

### Problem Card #1 :

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc một cuộc gọi tư vấn và cần chuyển sang khách hàng tiếp theo, tôi muốn lưu nhanh nhu cầu, vấn đề, cam kết và bước chăm sóc tiếp theo vào CRM, để đồng nghiệp có thể tiếp nhận đúng ngữ cảnh mà không phải nghe lại toàn bộ cuộc gọi. |
| Actor |	Nhân viên CSKH/tư vấn bán hàng, ngân hàng (người trực tiếp thao tác); trưởng nhóm CSKH và nhân viên tiếp nhận ca sau (người chịu ảnh hưởng). |
| Thời điểm / bối cảnh |	Ngay sau cuộc gọi, nhất là khi lượng cuộc gọi liên tiếp cao và một khách hàng có thể được nhiều nhân viên chăm sóc. Giới hạn vào ghi chú và cập nhật CRM, không tự động đánh giá khả năng trả nợ hay quyết định cấp tín dụng. |
| Quy trình hiện tại (3–7 bước) |	(1) Nhận cuộc gọi và tra hồ sơ khách trên CRM; (2) trao đổi, ghi chú rời các thông tin quan trọng; (3) kết thúc cuộc gọi; (4) nhớ lại hoặc nghe lại phần cần thiết; (5) phân loại nhu cầu và nhập tóm tắt, trạng thái, lịch hẹn vào CRM; (6) kiểm tra và chuyển việc cho người phụ trách tiếp theo. Đây là quy trình nháp cần phỏng vấn xác nhận. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 4–5: nghe lại, lọc thông tin và nhập liệu. Giả định 5–8 phút/cuộc gọi; chưa đo thực tế. Đặc biệt dễ bỏ sót cam kết, thời hạn hoặc nhu cầu thay đổi. |
| Impact (nếu không giải thì sao) |Tăng thời gian xử lý sau cuộc gọi; CRM thiếu/không nhất quán; khách phải nhắc lại nhu cầu; bỏ lỡ lịch chăm sóc. Chưa có bằng chứng để quy đổi thành doanh thu mất đi. |
| Success metric (baseline → target) |Thời gian hoàn tất ghi chú CRM: baseline giả định 6 phút → mục tiêu ≤3 phút/cuộc gọi; tỷ lệ bản ghi đủ 4 trường (nhu cầu, vấn đề, cam kết, bước tiếp theo): baseline cần đo → mục tiêu ≥95%; tỷ lệ thông tin sai nghiêm trọng: baseline cần đo → mục tiêu ≤2%. Đo thử 30–50 cuộc gọi có sự đồng ý và đối chiếu với người phụ trách. |
| Phương án không dùng AI |Chuẩn hóa biểu mẫu CRM với trường bắt buộc, menu chọn loại nhu cầu, checklist cuối cuộc gọi và mẫu ghi chú; phân công kiểm tra ngẫu nhiên. Đây là phương án đối chứng cần thử trước. |
| Giả thuyết về AI (nếu có) |	Với bản ghi âm được phép xử lý, speech-to-text kết hợp trích xuất thông tin có thể tạo bản nháp ghi chú và gợi ý trường CRM; nhân viên kiểm tra, sửa và xác nhận trước khi lưu. Không tự gửi tin nhắn, không tự quyết định nghiệp vụ nhạy cảm. |
| Cảm nhận nhanh | 	Workflow + AI hỗ trợ (chưa cần Agent tự chủ): quy trình có bước cố định, điểm cần AI là hiểu hội thoại không cấu trúc|

Quy trình nháp hiện tại:

```text
Khách gọi đến
  → Nhân viên tra cứu hồ sơ CRM
  → Trao đổi và ghi chú rời
  → Kết thúc cuộc gọi
  → [NGHẼN: nhớ/nghe lại + lọc nhu cầu, cam kết]
  → Nhập tay các trường CRM
  → Kiểm tra và chuyển ca / đặt lịch chăm sóc
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | 	Khi xem một bài giảng AI bằng tiếng Anh không có phụ đề hoặc phụ đề khó tra cứu, tôi muốn tìm đúng mốc thời gian giảng viên nhắc tới một thuật ngữ (ví dụ “embedding”) và hiểu nội dung đoạn đó bằng tiếng Việt, để ôn tập mà không phải tua đi tua lại toàn bộ video.|
| Actor |	Sinh viên/người tự học bằng video tiếng nước ngoài; người học cần tra cứu thuật ngữ chuyên ngành|
| Thời điểm / bối cảnh |Trong lúc học hoặc ôn lại video dài; người học nhớ từ khóa nhưng không nhớ vị trí. Phạm vi ưu tiên: video bài giảng tiếng Anh, không mở rộng ngay sang mọi nền tảng và mọi ngôn ngữ.|
| Quy trình hiện tại (3–7 bước) |	(1) Mở video; (2) kiểm tra có phụ đề/transcript không; (3) nếu có thì tìm từ khóa trong transcript; (4) nếu không có thì tua và nghe thử nhiều đoạn; (5) ghi lại timestamp; (6) tự dịch/tra thuật ngữ và xem lại ngữ cảnh.|
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 4–5 khi không có transcript tìm kiếm được. Giả định mất 5–15 phút để tìm một đoạn trong video dài 45–90 phút; cần đo bằng bài kiểm tra tìm từ khóa. |
| Impact (nếu không giải thì sao) |	Gián đoạn việc học, tốn thời gian ôn tập, có thể bỏ lỡ phần giải thích quan trọng hoặc hiểu sai thuật ngữ do nghe không rõ. |
| Success metric (baseline → target) |Thời gian tìm đúng timestamp: baseline giả định 10 phút → mục tiêu ≤2 phút/từ khóa; tỷ lệ tìm đúng đoạn (người học xác nhận): baseline cần đo → mục tiêu ≥90%; tỷ lệ bản dịch thuật ngữ đúng ngữ cảnh: baseline cần đo → mục tiêu ≥90% trên tập kiểm tra nhỏ. |
| Phương án không dùng AI |	Dùng transcript/phụ đề có sẵn của YouTube, Ctrl+F tìm từ, tự tạo mục lục timestamp hoặc ghi chú theo chương; nếu video đã có transcript tốt thì chưa cần xây hệ thống mới. |
| Giả thuyết về AI (nếu có) |Nếu video thiếu transcript, nhận dạng tiếng nói tạo transcript có timestamp; tìm kiếm từ khóa (có thể dùng tìm kiếm văn bản thông thường), dịch đoạn liên quan sang tiếng Việt. Hiển thị đoạn gốc để người học tự đối chiếu, đặc biệt với thuật ngữ AI. |
| Cảm nhận nhanh | 	Workflow + Rule + AI theo điều kiện: tìm từ khóa và nhảy timestamp là rule; AI chỉ cần khi phải phiên âm/dịch. Không cần Agent. |

Quy trình nháp hiện tại:

```text
Mở video bài giảng
  → Kiểm tra transcript/phụ đề
  → Có transcript? ─ Có → Tìm từ khóa → Nhảy đến timestamp
                    └ Không → [NGHẼN: tua thủ công, nghe thử]
                               → Xác định đoạn cần tìm
  → Tra nghĩa/diễn giải tiếng Việt → Ghi chú để ôn tập
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần chuẩn bị danh sách ứng viên cho một vị trí sau nhiều vòng đánh giá, tôi muốn tổng hợp bằng chứng về kỹ năng, kinh nghiệm và nhận xét phỏng vấn theo cùng bộ tiêu chí, để trưởng bộ phận so sánh và quyết định ai cần được xem xét tiếp mà không phải đọc lại từng tài liệu rời rạc.|
| Actor |Chuyên viên tuyển dụng HR (thực hiện tổng hợp); trưởng bộ phận và người phỏng vấn (đánh giá/ra quyết định). |
| Thời điểm / bối cảnh |Trước buổi họp chọn shortlist, khi CV, phiếu phỏng vấn và nhận xét nằm ở nhiều tệp/kênh. Chỉ hỗ trợ tổ chức thông tin, không tự chấm điểm con người bằng tiêu chí thiếu minh bạch hoặc tự động loại ứng viên. |
| Quy trình hiện tại (3–7 bước) |	(1) Nhận mô tả công việc và tiêu chí tuyển; (2) thu thập CV/hồ sơ; (3) nhận phiếu và nhận xét từ các vòng phỏng vấn; (4) đọc, chuẩn hóa thông tin theo tiêu chí; (5) đối chiếu bằng chứng và phát hiện thông tin thiếu/mâu thuẫn; (6) lập bảng shortlist cho trưởng bộ phận rà soát; (7) thống nhất bước tiếp theo. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 4–6: đối chiếu nhiều định dạng và nhận xét không thống nhất. Giả định 10–20 phút/ứng viên khi tổng hợp thủ công; số lượng 1.000 ứng viên trong CP1 chỉ là tình huống giả định, không phải số liệu đã xác minh. |
| Impact (nếu không giải thì sao) |	HR mất nhiều giờ chuẩn bị, chậm phản hồi ứng viên; bằng chứng quan trọng bị bỏ sót; đánh giá thiếu nhất quán giữa các người phỏng vấn. |
| Success metric (baseline → target) |Thời gian tổng hợp hồ sơ: baseline giả định 15 phút → mục tiêu ≤7 phút/ứng viên; tỷ lệ thông tin trích dẫn truy ngược được về nguồn: baseline cần đo → mục tiêu 100%; tỷ lệ lỗi trích xuất trường quan trọng: baseline cần đo → mục tiêu ≤3%. Thử trên bộ hồ sơ đã được cho phép sử dụng và có người đánh giá độc lập. |
| Phương án không dùng AI |	Dùng biểu mẫu phỏng vấn chung, bảng tính/ATS với trường dữ liệu bắt buộc, rubric đánh giá theo vị trí và quy tắc lọc điều kiện rõ ràng; HR kiểm tra trước buổi họp. |
| Giả thuyết về AI (nếu có) |	AI hỗ trợ đọc CV/nhận xét, chuẩn hóa thành các trường có dẫn nguồn và đánh dấu thông tin còn thiếu hoặc mâu thuẫn; người tuyển dụng kiểm chứng, không dùng AI để suy đoán phẩm chất cá nhân hay tự ra quyết định tuyển/loại. |
| Cảm nhận nhanh |	Workflow + AI hỗ trợ: dữ liệu phi cấu trúc có thể cần trích xuất, nhưng quyết định tuyển dụng phải do con người phụ trách. |

Quy trình nháp hiện tại:

```text
Nhận yêu cầu tuyển dụng và tiêu chí
  → Thu CV + phiếu phỏng vấn + nhận xét
  → [NGHẼN: đọc và chuẩn hóa từng nguồn]
  → Đối chiếu bằng chứng, phát hiện thiếu/mâu thuẫn
  → Lập bảng shortlist có dẫn nguồn
  → HR và trưởng bộ phận rà soát
  → Quyết định bước tuyển dụng tiếp theo (con người)
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Có actor và thời điểm phát sinh công việc rõ ràng, thao tác lặp lại thường xuyên, kết quả có thể kiểm chứng trực tiếp bằng thời gian hoàn tất CRM và độ đầy đủ/chính xác của thông tin. Phạm vi MVP có thể giới hạn ở tạo bản nháp để nhân viên duyệt, tránh đề xuất AI thay con người quyết định.
- Câu hỏi muốn nhóm phản biện:Đa số các cuộc gọi dạng spam để tư vấn khoản vay đều không được bắt máy hoặc có thì làm sao để đảm bảo được mô hình dự đoán đúng nhu cầu và khả năng trả của đối tượng.

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Mô tả “tệp khách hàng lớn, nhu cầu thực” chưa chứng minh pain cụ thể của người trực tiếp làm.|Đồng ý |Thu hẹp Card #1 vào thời gian nghe lại và nhập CRM sau từng cuộc gọi; xác định actor, điểm nghẽn và cách đo. |
| Đề xuất AI ngay có thể rơi vào solution-first; một số phần chỉ cần rule hoặc cải tiến quy trình.|Đồng ý |Bổ sung phương án không AI cho cả ba card; chỉ dùng AI ở phần dữ liệu phi cấu trúc, không mặc định dùng Agent. |
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
