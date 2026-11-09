# Báo cáo cá nhân — 2A202603914_TranGiaBao

> Đổi tên file theo quy tắc `2A202603914_TranGiaBao.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Gia Bảo
- MSSV: 2A202603914
- Email trường: 26ai.baotg@vinuni.edu.vn
- Tên nhóm: HEHEHE
- Link repo nhóm: https://github.com/hoangvu1806/K5-L3B-DAY02-HEHEHE-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

**Bối cảnh:** Tôi từng tham gia dự án kết nối AI chạy local với cơ sở dữ liệu khách hàng. Mục tiêu của hệ thống là cho phép người dùng đặt câu hỏi bằng ngôn ngữ tự nhiên, hệ thống chuyển thành truy vấn SQL và trả lại dữ liệu phục vụ phân tích. Trong phần này, tôi tách bài toán người dùng khỏi giải pháp Text-to-SQL: điều cần tìm hiểu trước là những bước nào trong việc tra cứu và phân tích dữ liệu hiện tại đang gây khó khăn.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi cần xem doanh thu theo tháng hoặc theo nhóm sản phẩm, tôi muốn lấy được số liệu từ cơ sở dữ liệu mà không phải nhờ developer viết từng câu SQL, để chủ động kiểm tra tình hình kinh doanh. | Quản lý, nhân viên kinh doanh, người phụ trách dữ liệu | Cần xác minh khách đã từng nhờ kỹ thuật xuất báo cáo bao nhiêu lần và mất bao lâu. |
| 2 | Đọc, tổng hợp nhiều thông tin | Khi một chỉ số kinh doanh thay đổi, tôi muốn đối chiếu dữ liệu từ nhiều bảng liên quan, để hiểu chỉ số đó đến từ nhóm khách hàng, đơn hàng hoặc sản phẩm nào. | Người phân tích kinh doanh, quản lý | Cần kiểm tra những báo cáo thực tế có phép JOIN/tổng hợp nhiều bảng và thời gian xử lý. |
| 3 | Pain từ người khác | Khi yêu cầu một báo cáo dữ liệu, tôi muốn hai người cùng hiểu đúng ý nghĩa các trường như doanh thu, đơn hủy và khách hàng mới, để tránh nhận kết quả không đúng câu hỏi ban đầu. | Người yêu cầu báo cáo, developer, data analyst | Cần đối chiếu các lần làm rõ yêu cầu, sửa câu truy vấn hoặc sửa báo cáo trong dự án. |
| 4 | Lặp lại | Khi cần theo dõi cùng một chỉ số theo ngày hoặc theo tuần, tôi muốn có kết quả cập nhật mà không phải nhờ tạo lại báo cáo từ đầu. | Quản lý, vận hành | Cần xác minh tần suất yêu cầu số liệu lặp lại và có dashboard/báo cáo tự động hay chưa. |
| 5 | Tốn thời gian | Khi người dùng hỏi dữ liệu bằng câu thông thường, tôi muốn hệ thống hiểu đúng tên bảng, cột và quan hệ dữ liệu, để không phải sửa truy vấn nhiều lần. | Developer triển khai Text-to-SQL, người sử dụng | Quan sát trực tiếp từ dự án tích hợp AI local; cần bổ sung test case thực tế và tỷ lệ truy vấn sinh đúng. |
| 6 | Lặp lại | Khi kết nối một mô hình AI local với cơ sở dữ liệu của khách, tôi muốn kiểm soát truy vấn được phép chạy, để tránh thao tác sai hoặc lộ dữ liệu nhạy cảm. | Developer, quản trị hệ thống, khách hàng | Cần kiểm tra cấu hình quyền của tài khoản DB, log truy vấn và các tình huống bị chặn. |
| 7 | Đọc, tổng hợp nhiều thông tin | Khi một câu hỏi được diễn đạt theo nhiều cách, tôi muốn nhận kết quả nhất quán và có thể kiểm tra nguồn dữ liệu, để tin tưởng số liệu dùng ra quyết định. | Người dùng nghiệp vụ, người kiểm tra dữ liệu | Cần thử các cách diễn đạt tương đương và so sánh SQL/kết quả với truy vấn chuẩn. |
| 8 | Pain từ người khác | Khi khách hàng muốn chạy AI trên hạ tầng nội bộ, tôi muốn biết rõ giới hạn phần cứng, tốc độ phản hồi và cách phân quyền, để triển khai được mà không phụ thuộc gửi dữ liệu lên dịch vụ ngoài. | IT khách hàng, developer, quản trị bảo mật | Cần bổ sung thông số máy local, thời gian phản hồi và yêu cầu bảo mật thực tế nếu được phép công khai. |

**Phân biệt phạm vi trải nghiệm:** Tôi có trải nghiệm triển khai bài toán Text-to-SQL và cấu hình AI local. Các tình huống liên quan đến việc nhân viên kinh doanh phải chờ báo cáo, cách họ xem doanh thu hoặc việc báo cáo bị hiểu sai là **giả thuyết về người dùng**, cần xác nhận qua trao đổi hoặc dữ liệu công việc; không xem đây là bằng chứng khách đã gặp.

**Ý tưởng cần loại:** “Xây chatbot AI phân tích mọi dữ liệu doanh nghiệp” là một mô tả giải pháp quá rộng. Tôi giới hạn từng vấn đề vào một tác vụ, một người sử dụng và một đầu ra có thể đo được.

---

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tự lấy số liệu kinh doanh mà không phụ thuộc viết SQL (#1) | Liên quan trực tiếp tới mục tiêu của dự án Text-to-SQL, có thể kiểm tra thời gian và độ chính xác | Khách đã có BI/dashboard hoặc truy vấn mẫu đáp ứng đủ nhu cầu chưa? |
| 2 | Hiểu đúng cấu trúc CSDL khi chuyển câu hỏi thành SQL (#5) | Có thể xây bộ test từ schema và truy vấn đúng để đo | Lỗi chủ yếu đến từ schema, prompt hay mô hình local? |
| 3 | Kết quả phân tích nhất quán và có thể kiểm chứng (#7) | Có ảnh hưởng trực tiếp tới độ tin cậy của công cụ | Mức sai lệch hiện tại là bao nhiêu, người dùng kiểm bằng cách nào? |

### Problem Card #1 — Truy xuất số liệu bằng ngôn ngữ tự nhiên

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần biết doanh thu, số đơn hoặc hiệu quả theo giai đoạn, tôi muốn tự hỏi và lấy dữ liệu từ hệ thống, để không phải chờ người biết SQL xuất báo cáo. |
| Actor | Quản lý hoặc nhân viên nghiệp vụ có quyền xem dữ liệu nhưng không sử dụng SQL |
| Thời điểm / bối cảnh | Khi cần câu trả lời ngoài những báo cáo cố định đã có |
| Quy trình hiện tại cần xác minh | 1. Người dùng xác định chỉ số cần xem · 2. Gửi yêu cầu cho người có quyền truy vấn · 3. Làm rõ điều kiện lọc · 4. Viết và chạy SQL · 5. Kiểm tra số liệu · 6. Trả kết quả |
| Bottleneck | Có thể nằm ở bước 2–4: chờ xử lý và làm rõ yêu cầu; **chưa đo trên quy trình khách hàng** |
| Impact | Người dùng phụ thuộc vào người kỹ thuật để lấy câu trả lời ngoài báo cáo có sẵn |
| Success metric | Baseline: [phút từ lúc yêu cầu đến khi có số liệu, số lần phải hỏi lại]; target đề xuất: giảm 50% thời gian với câu hỏi phù hợp, độ chính xác kết quả không thấp hơn truy vấn chuẩn; thử tối thiểu 20 câu hỏi |
| Phương án không dùng AI | Dashboard BI, báo cáo SQL định sẵn, bộ lọc và trình tạo báo cáo trực quan |
| Giả thuyết về AI | Mô hình local hiểu câu hỏi, lập truy vấn SQL chỉ đọc, giải thích kết quả và cho người dùng kiểm tra trước khi dùng ra quyết định |
| Cảm nhận nhanh | Workflow có bước AI; chưa chứng minh cần Agent |

```text
QUY TRÌNH HIỆN TẠI — cần xác nhận với khách
[1 Đặt câu hỏi: ?'] → [2 Gửi yêu cầu: ?']
→ [3 Làm rõ bộ lọc: ?'] → [4 Viết/chạy SQL: ?'] ← CẦN ĐO
→ [5 Kiểm tra số liệu: ?'] → [6 Trả kết quả: ?']
```

### Problem Card #2 — Chuyển câu hỏi thành SQL đúng với schema của khách

| Trường | Nội dung |
|---|---|
| Job Story | Khi người dùng hỏi bằng ngôn ngữ tự nhiên, tôi muốn hệ thống chọn đúng bảng, cột và quan hệ dữ liệu, để truy vấn trả đúng chỉ số mà họ hỏi. |
| Actor | Developer triển khai hệ thống Text-to-SQL và người dùng nghiệp vụ |
| Thời điểm / bối cảnh | Khi đưa một cơ sở dữ liệu mới vào hệ thống AI local hoặc khi người dùng đặt câu hỏi phức tạp |
| Quy trình hiện tại | 1. Kết nối schema · 2. Xác định bảng/cột liên quan · 3. Diễn giải câu hỏi · 4. Tạo SQL · 5. Kiểm tra quyền/cú pháp · 6. Chạy và đối chiếu kết quả |
| Bottleneck | Bước 2–4: ánh xạ ngôn ngữ nghiệp vụ sang cấu trúc bảng và điều kiện truy vấn; **cần đo bằng test case** |
| Impact | SQL có thể chạy thành công nhưng trả sai ý nghĩa, làm người dùng hiểu sai dữ liệu |
| Success metric | Baseline: [tỷ lệ kết quả đúng trên bộ test]; target đề xuất: tối thiểu 90% câu hỏi trong phạm vi demo khớp kết quả chuẩn; kiểm trên tối thiểu 30 câu hỏi có đáp án SQL tham chiếu |
| Phương án không dùng AI | Từ điển dữ liệu, các truy vấn SQL mẫu, giao diện chọn trường/điều kiện |
| Giả thuyết về AI | Chọn schema liên quan, sinh SQL và mô tả cách hiểu câu hỏi; validator và tài khoản DB chỉ đọc chặn truy vấn không hợp lệ |
| Cảm nhận nhanh | Workflow có AI kết hợp Rule kiểm tra cú pháp/quyền |

```text
LUỒNG XỬ LÝ TEXT-TO-SQL — bước cần đo chất lượng
[1 Nhận câu hỏi] → [2 Lấy schema liên quan]
→ [3 Xác định ý định/bộ lọc]  ← CẦN KIỂM THỬ
→ [4 Sinh SQL]  ← CẦN KIỂM THỬ
→ [5 Validate & giới hạn quyền] → [6 Thực thi/đối chiếu]
```

### Problem Card #3 — Kiểm chứng độ tin cậy của kết quả phân tích

| Trường | Nội dung |
|---|---|
| Job Story | Khi hỏi cùng một chỉ số theo các cách diễn đạt khác nhau, tôi muốn kết quả nhất quán và có căn cứ đối chiếu, để không quyết định dựa trên số liệu sai. |
| Actor | Người sử dụng báo cáo, developer và người kiểm tra số liệu |
| Thời điểm / bối cảnh | Khi nghiệm thu hoặc sử dụng Text-to-SQL cho các câu hỏi có điều kiện lọc và phép tổng hợp |
| Quy trình hiện tại | 1. Đặt câu hỏi · 2. Sinh SQL · 3. Xem câu SQL/điều kiện · 4. Chạy truy vấn · 5. Đối chiếu báo cáo chuẩn · 6. Ghi nhận câu hỏi sai |
| Bottleneck | Bước 3–5: kiểm tra tính đúng nghĩa của SQL và kết quả; **chưa có baseline** |
| Impact | Người dùng có thể nhận số liệu khác nhau hoặc thiếu căn cứ để tin tưởng kết quả |
| Success metric | Baseline: [tỷ lệ câu trả lời đúng, tỷ lệ nhất quán giữa các cách hỏi]; target đề xuất: 100% truy vấn được kiểm quyền, ít nhất 90% test case đúng và không có kết quả sai âm thầm trong tập kiểm thử |
| Phương án không dùng AI | Báo cáo chuẩn, bộ SQL đã kiểm thử, đối chiếu thủ công |
| Giả thuyết về AI | Hỗ trợ diễn đạt kết quả và cách hiểu câu hỏi; không tự khẳng định đúng khi không kiểm chứng được |
| Cảm nhận nhanh | Rule kiểm định kết quả + Workflow cho việc sinh SQL và xác nhận |

```text
KIỂM CHỨNG KẾT QUẢ — cần đo thời gian và độ chính xác
[1 Câu hỏi] → [2 Sinh SQL] → [3 Kiểm điều kiện]
→ [4 Chạy SQL] → [5 Đối chiếu truy vấn chuẩn] ← BƯỚC CẦN ĐO
→ [6 Ghi lỗi/cập nhật test case]
```

### Card muốn pitch nhất

- **Card số:** 1 — Người dùng nghiệp vụ tự truy xuất số liệu từ cơ sở dữ liệu mà không cần viết SQL.
- **Vì sao:** Đây là mục tiêu có liên hệ rõ với dự án đã tham gia. Có thể kiểm chứng bằng câu hỏi thực tế của người dùng, thời gian chờ báo cáo và so sánh kết quả với SQL đúng.
- **Câu hỏi muốn nhóm phản biện:** Nếu một dashboard và vài bộ lọc đã đủ để người dùng lấy phần lớn số liệu, những loại câu hỏi nào vẫn buộc họ phải nhờ người biết SQL?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Text-to-SQL là giải pháp, chưa phải bản thân problem | Đồng ý | Đặt problem ở nhu cầu tự tra cứu và phân tích dữ liệu của người nghiệp vụ |
| Chưa có bằng chứng người dùng phải chờ developer trả số liệu | Đồng ý | Giữ baseline cần xác minh, đề xuất hỏi về yêu cầu báo cáo gần nhất |
| SQL chạy được chưa chắc trả kết quả đúng | Đồng ý | Bổ sung metric độ chính xác so với truy vấn chuẩn và bước kiểm quyền |
| Dashboard có thể đủ dùng cho các chỉ số lặp lại | Đồng ý | Nêu phương án không AI, chỉ cân nhắc Text-to-SQL cho câu hỏi linh hoạt |

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

- [Đề bài CHECKPOINTS](../../CHECKPOINTS.md)
- [Quy định sử dụng AI](../../RULES.md)
- [Rubric](../../RUBRIC.md)
- [Bổ sung nguồn tài liệu hoặc hồ sơ QC được phép sử dụng sau khi xác minh]
