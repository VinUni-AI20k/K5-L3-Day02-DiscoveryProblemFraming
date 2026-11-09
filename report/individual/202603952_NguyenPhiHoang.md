# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Phi Hoàng
- MSSV: 2A202603952
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Titanic
- Link repo nhóm: https://github.com/phihoang1709/K5-L3B-DAY02-Titanic-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Cần đọc, tổng hợp nhiều thông tin |Mỗi 7h hằng ngày tôi muốn tổng hợp các tin tức mới nhất về công nghệ để bắt kịp xu hướng |Bản thân | 1-2h mỗi ngày |
| 2 |Tăng hiệu suất |Khi bắt đầu chạy một dự án mới, tôi muốn xác định đúng môi trường và các thư viện cần thiết, tài liệu nội bộ để tham gia vào dự án |Dev, tester | 2h|
| 3 |Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị cho kỳ thi cuối kỳ để có thể ôn tập nằm ở nhiều tài liệu, tôi muốn xác định đầy đủ các mục phải ôn tập, các bài tập điều kiện để không bỏ sót nội dung, bị trừ điểm hoặc bị cấm thi. |Học sinh, sinh viên | 1 tuần |
| 4 |Sự tập trung |Khi học buổi tối thường dễ mất tập trung hơn sau 20p, tôi muốn tập trung hơn dể đạt kết quả tốt |Học sinh, sinh viên | Mỗi tối |
| 5 |Lặp lại, tốn thời gian| Khi công ty có thêm nhân sự mới, cần tạo tài nguyên(tài khoản, vé xe ...), hướng dẫn với các tài liệu dự án công ty, nội quy để có thể bắt nhịp với công việc  | Nhân viên mới| 1 tuần |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

> Bản nháp phát triển từ CP1 #5, #2 và #1. Dữ kiện hiện có do người viết ghi ở CP1: onboarding khoảng 1 tuần; thiết lập dự án 2 giờ; đọc tin 1–2 giờ/ngày. Chưa có log hoặc phỏng vấn đối chiếu. Thời gian từng bước bên dưới là **giả định minh họa để kiểm chứng**, không phải kết quả đo. Các target là đề xuất, chưa phải cam kết của nhóm.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Onboarding nhân viên mới (#5) | Có nhiều bên bàn giao; liên quan tài khoản, tài liệu và người hướng dẫn; phù hợp hướng muốn đào sâu | 1 tuần gồm bao nhiêu thời gian chờ, tìm tài liệu và học việc bình thường? |
| 2 | Thiết lập dự án cho dev/tester (#2) | Có đầu ra kiểm tra được: chạy ứng dụng hoặc bộ test; CP1 ghi 2 giờ | Nghẽn ở tài liệu, phiên bản thư viện hay quyền truy cập? |
| 3 | Tổng hợp tin công nghệ mỗi sáng (#1) | Lặp lại hằng ngày; CP1 ghi 1–2 giờ/ngày | Cần cập nhật chủ đề nào, và tin nào thực sự giúp công việc? |

Không chọn #3 ôn thi và #4 tập trung buổi tối vào top 3 vì bối cảnh còn rộng, chưa tách được bước nghẽn và cách đo kết quả. Đây là lựa chọn cá nhân để chuẩn bị pitch, chưa phải kết luận CP3 của nhóm.

### Problem Card #1 — Onboarding nhân viên mới

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu tuần làm việc đầu tiên ở công ty, tôi muốn biết các việc cần hoàn thành, tài liệu đúng với vai trò và người chịu trách nhiệm hỗ trợ, để hoàn tất điều kiện bắt đầu công việc mà không phải hỏi vòng qua nhiều người. |
| Actor | Nhân viên mới; phạm vi khảo sát ban đầu đề xuất là dev/tester. HR, IT và buddy/mentor là bên phối hợp. |
| Thời điểm / bối cảnh | Từ lúc nhận hướng dẫn ngày đầu tới khi có đủ tài khoản, đọc nội quy cần thiết và bắt đầu nhiệm vụ đầu tiên. |
| Quy trình hiện tại (3–7 bước) | Nhận hướng dẫn → xác định tài nguyên cần có → gửi yêu cầu → chờ cấp/duyệt → tìm và đọc tài liệu → hỏi lại và xác nhận hoàn tất. Đây là quy trình giả thuyết cần đối chiếu người thật. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết chính: bước 5 tìm đúng tài liệu và người phụ trách, giả định 60 phút chủ động/lượt. Giả thuyết cạnh tranh: bước 4 chờ cấp quyền mới là phần kéo dài lịch. Chưa có dữ liệu để chốt. |
| Impact (nếu không giải thì sao) | CP1 ghi mất khoảng 1 tuần; chưa rõ mốc bắt đầu/kết thúc. Có nguy cơ trì hoãn nhiệm vụ đầu tiên và làm HR/IT/buddy trả lời lặp lại; chưa định lượng được số lần hỏi hay thời gian hỗ trợ. |
| Success metric (baseline → target) | Baseline hiện có: khoảng 1 tuần theo CP1, cần xác minh. Đề xuất đo trung vị phút tìm được tài liệu đúng và số lần chuyển người hỗ trợ/lượt; target giảm ít nhất 30% so với baseline đo thật, không tăng lỗi hướng dẫn. Theo dõi riêng thời gian chờ cấp quyền và thời gian tới nhiệm vụ đầu tiên. |
| Phương án không dùng AI | Checklist theo vai trò, một trang bắt đầu, danh bạ HR/IT/buddy, người sở hữu từng tài liệu và ngày cập nhật; yêu cầu cấp quyền theo mẫu có trạng thái. |
| Giả thuyết về AI (nếu có) | Chỉ khi tài liệu đã có nhưng vẫn khó tra cứu: hỗ trợ tìm câu trả lời kèm nguồn trong phạm vi được phép đọc; thiếu nguồn thì chuyển đúng người. Không tự cấp tài khoản, phê duyệt quyền hay quyết định chính sách. |
| Cảm nhận nhanh | Chưa biết. Ưu tiên kiểm tra No AI/Rule; chỉ cân nhắc Workflow nếu khó khăn đọc hiểu vẫn còn sau khi chuẩn hóa tài liệu. |

Quy trình nháp hiện tại — **thời gian minh họa, cần đo lại**:

```text
[1 Nhận hướng dẫn HR: 15 phút]
→ [2 Xác định tài khoản/tài nguyên cần có: 20 phút]
→ [3 Gửi yêu cầu tới đầu mối: 15 phút]
→ [4 Chờ cấp/duyệt: __ phút theo thời gian thực tế]
→ [5 Tìm tài liệu đúng vai trò/phiên bản: 60 phút] ← NGHẼN GIẢ THUYẾT
→ [6 Đọc, hỏi buddy và xác nhận checklist: 40 phút]

Tổng giả định: 150 phút làm chủ động + thời gian chờ chưa đo.
Mốc khoảng 1 tuần ở CP1 là thời gian theo lịch, không phải 150 phút.
Nếu các bước chạy song song, đo thời gian toàn trình bằng mốc đầu/cuối,
không cộng thời gian chờ của nhiều yêu cầu chồng nhau.
```

### Problem Card #2 — Thiết lập môi trường dự án

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu tham gia một dự án mới, tôi muốn xác định đúng môi trường, thư viện và hướng dẫn nội bộ cần thiết, để chạy được dự án và bắt đầu nhiệm vụ được giao. |
| Actor | Dev/tester mới tham gia dự án, kể cả nhân viên cũ chuyển dự án. |
| Thời điểm / bối cảnh | Sau khi đã được nhận vào dự án; trước lần chạy ứng dụng hoặc bộ test đầu tiên. |
| Quy trình hiện tại (3–7 bước) | Lấy mã nguồn → đọc tài liệu → cấu hình môi trường → cài thư viện → xử lý lỗi → chạy xác nhận. Quy trình cần đối chiếu thực tế. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 5 đối chiếu lỗi với hướng dẫn/phiên bản, 40 phút minh họa. |
| Impact (nếu không giải thì sao) | CP1 ghi 2 giờ/lần; chưa xác nhận đã gồm thời gian chờ mentor hay chưa. Chậm bắt đầu nhiệm vụ và có thể ngắt việc người hỗ trợ. |
| Success metric (baseline → target) | Baseline tự ghi 120 phút → target đề xuất ≤60 phút tới lần chạy thành công, không bỏ qua kiểm tra bắt buộc. Ghi thời gian từng bước ở các lượt setup tiếp theo và lưu kết quả chạy. |
| Phương án không dùng AI | README đã kiểm thử, chốt phiên bản, file dependency và script setup; người mới làm thử trên máy sạch. |
| Giả thuyết về AI (nếu có) | Giải thích log và trỏ tới hướng dẫn đã duyệt; dev kiểm tra trước khi thực hiện lệnh. Không đưa bí mật vào công cụ hỗ trợ. |
| Cảm nhận nhanh | Rule trước; chưa có căn cứ cần Agent. |

```text
GIẢ ĐỊNH PHÂN BỔ 120 PHÚT — chưa bấm giờ từng bước
[1 Lấy mã nguồn: 10'] → [2 Đọc hướng dẫn: 20']
→ [3 Cấu hình môi trường: 20'] → [4 Cài thư viện: 20']
→ [5 Đối chiếu và xử lý lỗi: 40'] ← NGHẼN GIẢ THUYẾT
→ [6 Chạy ứng dụng/test xác nhận: 10']
```

Card #2 chỉ xét kỹ thuật sau khi có quyền truy cập; card #1 xét hành trình bàn giao HR–IT–buddy. Không cộng tác động của hai card khi cùng một lượt onboarding.

### Problem Card #3 — Tổng hợp tin công nghệ buổi sáng

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu cập nhật tin công nghệ lúc 7 giờ mỗi ngày, tôi muốn xác định những thay đổi liên quan đến việc học và công việc, để theo kịp thông tin cần thiết mà vẫn dành thời gian cho nhiệm vụ chính. |
| Actor | Bản thân người viết báo cáo. |
| Thời điểm / bối cảnh | Khoảng 7 giờ hằng ngày, trước các nhiệm vụ chính. |
| Quy trình hiện tại (3–7 bước) | Mở nguồn → lướt tiêu đề → đọc bài → đối chiếu tin trùng → ghi chú. Cần xác minh nguồn thường đọc. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 3 đọc nhiều bài trước khi biết có liên quan hay không, 40 phút minh họa. |
| Impact (nếu không giải thì sao) | CP1 ghi 1–2 giờ mỗi ngày; chưa đo phần đọc trùng hoặc không liên quan. |
| Success metric (baseline → target) | Baseline tự ghi 60–120 phút/ngày → target đề xuất ≤30 phút/ngày. Ghi giờ trong 5 buổi; cuối mỗi buổi đối chiếu danh sách tin được giữ với chủ đề đã chọn, tránh giảm giờ bằng cách bỏ hết tin cần thiết. |
| Phương án không dùng AI | Giới hạn chủ đề, chọn ít nguồn đáng tin, dùng RSS và khung giờ đọc cố định. |
| Giả thuyết về AI (nếu có) | Gom tin trùng và tóm tắt kèm link gốc; người đọc kiểm nguồn trước khi sử dụng. |
| Cảm nhận nhanh | No AI trước; Workflow là giả thuyết nếu vẫn mất nhiều thời gian tổng hợp. |

```text
MINH HỌA MỘT BUỔI 90 PHÚT — không phải baseline đo thật
[1 Mở nguồn: 5'] → [2 Lướt và chọn bài: 20']
→ [3 Đọc nội dung: 40'] ← NGHẼN GIẢ THUYẾT
→ [4 Đối chiếu tin trùng: 15'] → [5 Ghi chú: 10']
```

### Card muốn pitch nhất

- Card số: **1 — Onboarding nhân viên mới**.
- Vì sao: phù hợp hướng đào sâu; có thể khảo sát cả nhân viên mới và bên hỗ trợ; có phương án cải thiện quy trình đơn giản để so sánh.
- Câu hỏi muốn nhóm phản biện: “Trong khoảng 1 tuần onboarding, phần chậm nhất là chờ cấp quyền, tìm đúng tài liệu hay học nghiệp vụ; dữ liệu nào giúp phân biệt ba nguyên nhân này?”

### AI đã phản biện card thế nào

> Đây là phản biện của AI trong lần hỗ trợ soạn bản nháp này. Cột đồng ý để người viết tự đánh giá; không ghi nhận thay quyết định cá nhân.

| Điểm yếu AI chỉ ra | Đồng ý? | Thay đổi trong bản nháp sau phản biện |
|---|---|---|
| “Onboarding mất 1 tuần” chưa xác định thế nào là hoàn tất | Chờ người viết xác nhận | Đề xuất mốc có đủ điều kiện và bắt đầu nhiệm vụ đầu tiên; tách thời gian theo lịch và làm chủ động. |
| Đang gom cấp tài khoản, vé xe và học dự án thành một bottleneck | Chờ người viết xác nhận | Tách bước chờ cấp quyền và tìm tài liệu; để hai giả thuyết cạnh tranh ở CP4. |
| Có thể chỉ thiếu checklist, không cần AI | Chờ người viết xác nhận | Bổ sung phương án trang bắt đầu, owner tài liệu và phân công hỗ trợ trước khi thử AI. |
| Thời gian từng bước chưa có nguồn đo | Chờ người viết xác nhận | Đánh dấu toàn bộ số phân bổ là minh họa; không dùng làm bằng chứng CP4. |

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
| CP2 Problem Card | Hỗ trợ phát triển 3 card từ CP1 và phản biện onboarding | Tách phạm vi, metric và giả thuyết nghẽn | Phân bổ thời gian từng bước chưa có dữ liệu thật | Chờ tôi đối chiếu quy trình, sửa số và tự đánh giá phản biện |
| CP4 Research | Tìm tài liệu chính thức và chuẩn bị kế hoạch kiểm chứng onboarding | So sánh checklist, wiki và quản trị tri thức | Tài liệu sản phẩm không chứng minh pain tại công ty | Chờ tôi kiểm link, phỏng vấn người thật và cập nhật kết luận |
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
