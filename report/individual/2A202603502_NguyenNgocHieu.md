# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyen Ngoc Hieu
- MSSV: 2A202603502
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhom01Ban02
- Link repo nhóm: https://github.com/VuTriDung1123/K5-L3A-DAY02-Nhom01Ban02-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Lặp lại, tốn thời gian| Mỗi sáng hàng ngày trước 10h, GĐ sàn, Trưởng phòng cần 1 bảng tổng hợp thông tin vĩ mô có khả năng tác động tới thị trường bất động sản | Quản lý sàn, trưởng phòng, NVKD | Thường bị trễ, ảnh hưởng tới những công việc khác |
| 2 | Lặp lại, tốn thời gian, nỗi đau người khác| Mỗi sáng hàng ngày trước 10h, toàn bộ sàn cần nắm rõ tình hình biến động của tất cả bảng hàng về tồn kho, biến động giá, thay đổi chính sách..| Toàn bộ Sàn | Thường bị trễ, ảnh hưởng tới những công việc khác, khó nắm được toàn bộ bảng hàng, NV hay tư vấn sai chính sách |
| 3 | Lặp lại, tốn thời gian, nỗi đau người khác| Mỗi sáng hàng ngày trước 10h, nhân viên cần rà soát lại tình hình chăm sóc khách hàng của cá nhân | Nhân viên kinh doanh | Nhân viên ko nắm chắc tình hình chăm sóc của mình, dễ bị sót khách 
| 4 | Lặp lại, tốn thời gian| Hàng ngày vào lúc 3h chiều, quản lý sàn cần báo cáo tình hình marketing| Quản lý sàn | Thường bị trễ, thiếu thông tin cập nhật, ảnh hưởng tới độ chính xác củ quyết định|
| 5 | Tổng hợp thông tin| Hàng ngày tôi muốn biết những thông tin cập nhật về lớp học aithucchien| Cá nhân | Khó theo kịp được tiến độ lớp, ko tối ưu được thời gian |
-
---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |1  | Có baseline rõ ràng, tốn thời gian, tạo ảnh hưởng toàn bộ kinh doanh| | Tiêu chí sàng lọc tin ảnh hưởng tới sản phẩm công ty đang bán
| 2 |4 | Ảnh hưởng trực tiếp tới thu chi | Bảo mật thông tin  |
| 3 | 3 | Tài nguyên quan trọng nhất của doanh nghiệp, tốn thời gian, dễ nhầm lẫn | Bảo mật thông tin, quyền truy cập dữ liệu |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu công việc hàng ngày, tôi muốn có 1 bảng tổng hợp thông tin vĩ mô ngành, để giám đôc sàn đọc trước 10h |
| Actor | Trợ lý hoặc sales admin |
| Thời điểm / bối cảnh | Trước 10h sáng hàng ngày |
| Quy trình hiện tại (3–7 bước) | 1. Assistant tự lọc hoặc nhờ AI tổng hợp 2. Assistant tự xác định thông tin cần thiết tổng hợp vào google docs 3. Assistant viết đánh giá theo góc nhìn cá nhân 4. Review và format 5. Gửi email| 
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 viêt narrative hoặc để trắng|
| Impact (nếu không giải thì sao) | Quản lý mất nhiều thời gian tổng hợp thông tin, ảnh hưởng tiến độ công việc khác|
| Success metric (baseline → target) | Có báo cáo ngày trước 10h, nội dung được tổng hợp khoa học, có narrative|
| Phương án không dùng AI | Mua sẵn từ 1 đơn vị chuyên nghiệp ; tạo template cố định + checklist |
| Giả thuyết về AI (nếu có) | AI soạn nháp, trợ lý duyệt  |
| Cảm nhận nhanh |  Workflow |
Quy trình nháp hiện tại:

[1 Tổng hợp tin: 30'] → [2 Phân loại: 10'] → [3 Đánh giá: 15']
→ [4 Tổng hợp Docs: 15']  ← BOTTLENECK
→ [5 Review + format: 10'] → [6 Gửi: 5']

### Problem Card #2 — Báo cáo tình hình marketing hàng ngày lúc 3h chiều (Problem #4)

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến 3h chiều, tôi muốn có bảng tổng hợp tình hình marketing trong ngày (chi phí, số lead, hiệu quả từng kênh), để quản lý sàn điều chỉnh ngân sách kịp thời trước khi kết thúc ca làm việc |
| Actor | Nhân viên marketing / sales admin |
| Thời điểm / bối cảnh | 3h chiều hàng ngày |
| Quy trình hiện tại (3–7 bước) | 1. Mở Facebook Ads Manager, Google Ads lấy số liệu từng chiến dịch 2. Hỏi NV qua Zalo lấy số lead buổi sáng 3. Tổng hợp thủ công vào Google Sheets 4. Viết nhận xét đánh giá hiệu quả từng kênh 5. Gửi báo cáo cho BGĐ |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 1 & 3 — pull số liệu thủ công từng nền tảng rồi tổng hợp vào bảng tính, mất 25–30' |
| Impact (nếu không giải thì sao) | Quyết định điều chỉnh ngân sách bị muộn, dễ bỏ lỡ khung giờ hiệu quả cao; NV marketing bị ngắt việc để trả lời hỏi thăm số liệu |
| Success metric (baseline → target) | Báo cáo có trước 3h15 đủ 3 kênh và nhận định điều chỉnh; đúng giờ 5/5 ngày/tuần (baseline: ~2–3/5 ngày) |
| Phương án không dùng AI | Looker Studio kết nối API tự cập nhật mỗi 30'; tạo template điền tay cố định, quản lý tự mở dashboard |
| Giả thuyết về AI (nếu có) | Script pull số liệu từ Ads về một bảng; AI so sánh hiệu quả với trung bình 7 ngày trước và soạn nháp nhận định điều chỉnh; quản lý duyệt |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[1 Mở từng nền tảng Ads lấy số: 15'] → [2 Hỏi NV Zalo lấy lead: 5']
→ [3 Tổng hợp vào Sheets: 15']  ← BOTTLENECK
→ [4 Viết nhận xét hiệu quả: 10'] → [5 Gửi báo cáo BGĐ: 5']
```

### Problem Card #3 — Rà soát tình hình chăm sóc khách hàng cá nhân mỗi sáng (Problem #3)

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu ngày làm việc mỗi sáng, tôi muốn rà soát nhanh danh sách khách hàng đang chăm sóc, để không bỏ sót khách tiềm năng và ưu tiên đúng việc từ đầu buổi |
| Actor | Nhân viên kinh doanh bất động sản |
| Thời điểm / bối cảnh | Trước 10h sáng hàng ngày |
| Quy trình hiện tại (3–7 bước) | 1. Mở CRM hoặc Excel dò danh sách khách 2. Nhớ lại trạng thái chăm sóc từng người 3. Mở lại Zalo/Facebook từng khách kiểm tra lần liên hệ gần nhất 4. Ghi chú tay khách cần gọi trong ngày 5. Bắt đầu liên hệ theo thứ tự ưu tiên |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 mở riêng từng chat Zalo/Facebook kiểm tra lần liên hệ cuối, mất 20–25' |
| Impact (nếu không giải thì sao) | Dễ bỏ sót khách đang ở bước quan trọng, mất cơ hội chốt hợp đồng vì liên hệ muộn |
| Success metric (baseline → target) | Rà soát và lên danh sách gọi xong trước 9h30, không bỏ sót khách cần liên hệ trong ngày |
| Phương án không dùng AI | Bắt buộc điền "ngày liên hệ tiếp theo" trong CRM sau mỗi lần trao đổi ; Google Sheets có cột ngày sort tự động |
| Giả thuyết về AI (nếu có) | AI tóm tắt trạng thái từng khách ưu tiên thành checklist buổi sáng, NV xác nhận và gọi |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[1 Mở CRM/Excel dò danh sách: 5'] → [2 Nhớ lại trạng thái từng KH: 10']
→ [3 Mở từng chat Zalo/FB kiểm tra lần liên hệ cuối: 20']  ← BOTTLENECK
→ [4 Ghi chú tay KH cần gọi hôm nay: 5'] → [5 Bắt đầu gọi: —]
```

### Card muốn pitch nhất

- **Card số:** Card #1 — Tổng hợp thông tin vĩ mô ngành BĐS mỗi sáng (Problem #1).
- **Vì sao:** Đây là vấn đề xảy ra **hàng ngày** ảnh hưởng trực tiếp đến toàn bộ sàn từ GĐ đến NVKD; có baseline rõ (thường bị trễ, ảnh hưởng công việc khác); actor rõ (trợ lý/sales admin); và có thể so sánh rõ ràng các mức No AI → Rule → Workflow trong quy trình tổng hợp thông tin.
- **Câu hỏi muốn nhóm phản biện:**
  1. _"Tiêu chí để lọc tin tức vĩ mô nào thực sự ảnh hưởng đến sản phẩm sàn đang bán là gì? Ai định nghĩa được 'ảnh hưởng' một cách đo được?"_
  2. _"Nếu Assistant dùng công cụ tổng hợp tin tức tự động (Rule/script) mà không có AI phân tích, bảng tổng hợp có đủ dùng cho GĐ sàn ra quyết định không?"_

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| **Card #1:** Actor "trợ lý hoặc sales admin" còn rộng — cần chỉ rõ hơn ai là người thực sự thực hiện quy trình (1 người hay nhiều người thay nhau?), để xác định đúng người dùng thật sự của giải pháp. | Đồng ý | Bổ sung rõ hơn vào trường Actor: "Trợ lý hoặc sales admin — người được phân công trực tiếp chuẩn bị bảng tổng hợp trước 10h sáng mỗi ngày". |
| **Card #1:** Success metric ban đầu chỉ ghi "thường bị trễ" mà không có con số baseline cụ thể; cần số liệu đo được để đánh giá cải thiện sau khi triển khai giải pháp. | Đồng ý | Bổ sung thêm vào Impact và Success Metric: trễ bình quân **30–45 phút** so với giờ quy định; target là giao đúng giờ **5/5 ngày/tuần**. |
| **Card #2:** Báo cáo marketing lúc 3h chiều có thể giải quyết hoàn toàn bằng dashboard tự động (Rule/Looker Studio) mà không cần AI — cần giải thích rõ hơn vì sao Rule không đủ trước khi đề xuất Workflow có AI. | Đồng ý | Ghi rõ trong Card #2: dashboard Rule giải quyết được phần số liệu thô, nhưng phần **phân tích xu hướng và đề xuất điều chỉnh ngân sách** (so sánh với lịch sử, nhận định ngữ cảnh) vẫn cần AI hỗ trợ trong Workflow. |

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

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?** Không kịp nghe 

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?** Không

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.** Không

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?** Thực sự hiểu vấn đề

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?** Trưởng nhóm chưa biết điều phối nên hầu như ko thực hiện được hoạt động nhóm

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
 Xác định vấn đề thông qua việc làm rõ quy trình, xác định được metric đo thành công thất bại, xác định ranh giới AI và con người từ đó đưa ra quyết định mức độ áp dụng AI để giải quyết vấn đề
 
---

## 7. Tài liệu tham khảo

-
