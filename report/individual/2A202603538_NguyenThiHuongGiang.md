# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Nguyễn Thị Hương Giang
- MSSV:2A202603538
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:
- Link repo nhóm:

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
## Education – Problem Statements

| STT | Loại problem | Problem statement | Người liên quan | Tần suất / Thời gian / Tác động |
|---|---|---|---|---|
| 1 | Lặp lại | Khi kết thúc mỗi buổi học, tôi muốn tự động tổng hợp nội dung bài giảng, bài tập về nhà và gửi thông báo cho phụ huynh, để không phải soạn và gửi thông tin thủ công. | Giáo viên, phụ huynh | 2–3 lớp/ngày, khoảng 15 phút/lớp |
| 2 | Tốn thời gian | Khi cần xây dựng thời khóa biểu cho học kỳ mới, tôi muốn tự động đề xuất lịch học dựa trên lịch rảnh của giáo viên, phòng học và số tiết của từng môn, để hạn chế trùng lịch và không phải điều chỉnh thủ công nhiều lần. | Nhân viên giáo vụ, giáo viên, ban giám hiệu | Mỗi học kỳ 1 lần, khoảng 2–3 ngày để hoàn thiện và điều chỉnh thời khóa biểu |
| 3 | Cần đọc, tổng hợp nhiều thông tin, lặp lại | Khi kết thúc một học kỳ, tôi muốn tổng hợp điểm số, mức độ chuyên cần và kết quả học tập của từng học sinh, để xác định những em cần được hỗ trợ thêm, những em được khen thưởng và trả về báo cáo cho từng phụ huynh. | Giáo viên chủ nhiệm, ban giám hiệu | 30–40 học sinh/lớp, khoảng 2–3 giờ/lớp |
| 4 | Đọc và tổng hợp thông tin | Quản lý việc đưa đón học sinh: Nhà trường phải tổng hợp danh sách học sinh đi xe buýt, lịch nghỉ học, tuyến xe, điểm đón/trả và thông tin người được phép đón. Khi phụ huynh thay đổi người đón, học sinh nghỉ đột xuất hoặc thay đổi điểm đón, thông tin cần được cập nhật và thông báo kịp thời để tránh nhầm lẫn hoặc bàn giao sai người. | Nhân viên phụ trách xe, giáo viên chủ nhiệm, tài xế, phụ huynh | 5–10 tuyến xe/ngày; khoảng 30–45 phút/ngày để tổng hợp, kiểm tra và cập nhật thông tin |
| 5 | Pain từ người khác | Khi phụ huynh muốn tìm hiểu lịch học, học phí, quy định hoặc chương trình đào tạo, họ muốn nhận được câu trả lời nhanh và chính xác, để không phải liên hệ trực tiếp với nhà trường cho từng câu hỏi. | Phụ huynh, nhân viên tư vấn tuyển sinh | 20–30 câu hỏi/ngày, khoảng 5–10 phút/câu |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Giải đáp thắc mắc của phụ huynh (#5) | Nhiều câu hỏi lặp lại, quy trình dễ xác định, có thể xây dựng Knowledge Base để trả lời tự động và đo tỷ lệ trả lời đúng. | Tài liệu nhà trường có đầy đủ, cập nhật và thống nhất không? |
| 2 | Quản lý đưa đón học sinh (#4) | Liên quan trực tiếp đến an toàn học sinh, cần phối hợp thông tin giữa phụ huynh, giáo viên và nhân viên phụ trách xe. | Thông tin người đón, học sinh nghỉ và thay đổi lịch được cập nhật theo thời gian thực như thế nào? |
| 3 | Lập thời khóa biểu (#2) | Tốn thời gian, có nhiều ràng buộc về giáo viên, phòng học và tiết học; có tiềm năng tự động hóa. | Các ràng buộc có thể biểu diễn đầy đủ thành quy tắc không? Có cần thuật toán tối ưu hóa thay vì AI Agent không? |

### Problem Card #1 — Giải đáp thắc mắc của phụ huynh

| Trường | Nội dung |
|---|---|
| Job Story | Khi có thắc mắc về lịch học, học phí, chương trình học hoặc quy định nhà trường, tôi muốn nhận được câu trả lời nhanh và chính xác, để không phải liên hệ trực tiếp với nhân viên nhà trường cho từng vấn đề. |
| Actor | Phụ huynh học sinh; nhân viên tư vấn hoặc bộ phận chăm sóc phụ huynh |
| Thời điểm / bối cảnh | Trong ngày, đặc biệt vào đầu năm học, thời điểm đóng học phí, đăng ký hoạt động và khi có thay đổi lịch học. |
| Quy trình hiện tại (3–7 bước) | 1. Phụ huynh gửi câu hỏi qua điện thoại, Zalo hoặc email. 2. Nhân viên tiếp nhận và phân loại câu hỏi. 3. Tìm thông tin trong tài liệu hoặc hỏi bộ phận liên quan. 4. Soạn câu trả lời. 5. Gửi lại phụ huynh. 6. Nếu chưa giải quyết được, chuyển câu hỏi đến bộ phận phụ trách. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Tìm kiếm và xác minh thông tin trong nhiều tài liệu hoặc hỏi các bộ phận khác, khoảng 3–5 phút/câu hỏi. |
| Impact (nếu không giải thì sao) | Nhân viên mất nhiều thời gian xử lý câu hỏi lặp lại; phụ huynh phải chờ phản hồi; thông tin có nguy cơ thiếu nhất quán giữa các nhân viên. |
| Success metric (baseline → target) | Thời gian phản hồi trung bình: 5–10 phút xuống dưới 2 phút đối với câu hỏi thông thường; tỷ lệ câu trả lời chính xác đạt ít nhất 95% trên bộ câu hỏi kiểm thử. |
| Phương án không dùng AI | Xây dựng trang FAQ, phân loại câu hỏi và chuẩn hóa câu trả lời theo từng chủ đề. |
| Giả thuyết về AI (nếu có) | Chatbot sử dụng RAG để truy xuất thông tin từ tài liệu chính thức của nhà trường, sau đó tạo câu trả lời bằng ngôn ngữ tự nhiên. Nếu không tìm thấy thông tin đáng tin cậy, chatbot chuyển câu hỏi cho nhân viên phụ trách. |
| Cảm nhận nhanh | Workflow + AI (RAG) |

#### Quy trình nháp hiện tại

```text
PHỤ HUYNH CÓ THẮC MẮC
          |
          v
[1. Gửi câu hỏi qua Zalo / Email / Điện thoại]
          |
          v
[2. Nhân viên tiếp nhận và phân loại câu hỏi]
          |
          v
[3. Tìm kiếm thông tin trong tài liệu]
          |
          v
[4. Xác minh thông tin với bộ phận liên quan]
          |                 BOTTLENECK
          v
[5. Soạn câu trả lời]
          |
          v
[6. Gửi phản hồi cho phụ huynh]
          |
          v
[7. Kết thúc / Chuyển cấp xử lý nếu chưa giải quyết được]
```

### Problem Card #2 — Quản lý đưa đón học sinh

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu ngày học, tôi muốn nắm được danh sách học sinh đi xe, học sinh nghỉ, người đón và các thay đổi về điểm đón/trả, để đảm bảo mỗi học sinh được đưa đón đúng lịch và bàn giao đúng người. |
| Actor | Nhân viên phụ trách xe, tài xế, giáo viên chủ nhiệm và phụ huynh |
| Thời điểm / bối cảnh | Đầu giờ sáng và cuối giờ chiều; đặc biệt khi phụ huynh thông báo học sinh nghỉ, thay đổi người đón hoặc thay đổi điểm đón/trả. |
| Quy trình hiện tại (3–7 bước) | 1. Phụ huynh đăng ký dịch vụ xe đưa đón và cung cấp thông tin người được phép đón. 2. Phụ huynh thông báo học sinh nghỉ hoặc thay đổi lịch qua điện thoại/Zalo. 3. Nhân viên tiếp nhận và cập nhật thông tin. 4. Tổng hợp danh sách học sinh theo tuyến và điểm đón/trả. 5. Gửi danh sách cập nhật cho tài xế và giáo viên. 6. Tài xế đón/trả học sinh và xác nhận tình trạng bàn giao. 7. Xử lý các trường hợp thiếu thông tin hoặc thay đổi đột xuất. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: Đối chiếu thông tin từ nhiều nguồn và cập nhật danh sách cho các bên liên quan, khoảng 30–45 phút/ngày. |
| Impact (nếu không giải thì sao) | Tài xế có thể sử dụng danh sách cũ; học sinh có thể bị đón sai điểm hoặc bỏ sót; giáo viên và phụ huynh khó nắm được tình trạng đưa đón; nguy cơ bàn giao học sinh không đúng người. |
| Success metric (baseline → target) | Thời gian tổng hợp danh sách: 30–45 phút xuống dưới 10 phút/ngày; 100% thay đổi người đón phải được xác minh trước khi bàn giao; giảm các trường hợp sai lệch thông tin so với quy trình hiện tại. |
| Phương án không dùng AI | Sử dụng biểu mẫu đăng ký và biểu mẫu thông báo nghỉ/thay đổi người đón; lưu dữ liệu tập trung và tự động cập nhật danh sách theo tuyến bằng các quy tắc cố định. |
| Giả thuyết về AI (nếu có) | AI Agent có thể tiếp nhận và phân loại thông báo bằng ngôn ngữ tự nhiên, ví dụ: học sinh nghỉ hôm nay, đổi người đón hoặc đổi điểm đón. Workflow cập nhật dữ liệu, kiểm tra các điều kiện và gửi thông báo đến những người liên quan. |
| Cảm nhận nhanh | Workflow + Database + AI Agent |

#### Quy trình nháp hiện tại

```text
PHỤ HUYNH ĐĂNG KÝ ĐƯA ĐÓN
          |
          v
[1. Cung cấp thông tin học sinh, tuyến xe và người được phép đón]
          |
          v
[2. Thông báo nghỉ học / thay đổi người đón / điểm đón]
          |
          v
[3. Nhân viên tiếp nhận và cập nhật thông tin]
          |                 BOTTLENECK
          v
[4. Tổng hợp danh sách học sinh theo tuyến]
          |
          v
[5. Gửi danh sách cho tài xế và giáo viên]
          |
          v
[6. Đón / trả học sinh và xác nhận bàn giao]
          |
          v
[7. Xử lý trường hợp bất thường hoặc thiếu xác nhận]
```

**Lưu ý:** AI không tự xác định người có quyền đón học sinh. Danh sách người được phép đón phải dựa trên thông tin phụ huynh đăng ký; các thay đổi bất thường cần nhân viên xác minh trước khi bàn giao.

### Problem Card #3 — Lập thời khóa biểu

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu học kỳ mới, tôi muốn xây dựng thời khóa biểu phù hợp với lịch dạy của giáo viên, số lượng phòng học và số tiết của từng môn, để hạn chế trùng lịch và giảm thời gian điều chỉnh thủ công. |
| Actor | Nhân viên phòng đào tạo, ban giám hiệu và giáo viên |
| Thời điểm / bối cảnh | Trước khi bắt đầu học kỳ hoặc khi có thay đổi về giáo viên, lớp học, phòng học và kế hoạch giảng dạy. |
| Quy trình hiện tại (3–7 bước) | 1. Thu thập kế hoạch giảng dạy và số tiết của từng môn. 2. Thu thập lịch rảnh/bận của giáo viên. 3. Kiểm tra số lượng phòng học và điều kiện sử dụng phòng. 4. Sắp xếp tiết học cho từng lớp. 5. Kiểm tra các trường hợp trùng giáo viên, phòng học hoặc lịch lớp. 6. Điều chỉnh thời khóa biểu. 7. Công bố thời khóa biểu cho giáo viên và học sinh. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4–6: Sắp xếp và điều chỉnh lịch để thỏa mãn nhiều ràng buộc cùng lúc, ước tính 2–3 ngày làm việc cho một đợt lập thời khóa biểu. |
| Impact (nếu không giải thì sao) | Thời khóa biểu có thể bị trùng giáo viên hoặc phòng học; giáo viên và học sinh phải thay đổi lịch; phòng đào tạo mất nhiều thời gian xử lý các yêu cầu điều chỉnh. |
| Success metric (baseline → target) | Thời gian lập và điều chỉnh thời khóa biểu: 2–3 ngày xuống dưới 1 ngày; không có xung đột về giáo viên, phòng học và thời gian học trong thời khóa biểu được công bố. |
| Phương án không dùng AI | Sử dụng bảng dữ liệu tập trung và thuật toán lập lịch dựa trên các ràng buộc cố định; tự động cảnh báo khi có trùng lịch. |
| Giả thuyết về AI (nếu có) | AI hỗ trợ đọc và chuẩn hóa yêu cầu lập lịch từ nhiều nguồn, nhận diện các ràng buộc và đề xuất phương án sắp xếp. Thuật toán tối ưu hóa có thể được sử dụng để tìm thời khóa biểu thỏa mãn các ràng buộc cứng và tối ưu các tiêu chí mềm. |
| Cảm nhận nhanh | Rule + Workflow + Optimization Algorithm |

#### Quy trình nháp hiện tại

```text
BẮT ĐẦU HỌC KỲ MỚI
          |
          v
[1. Thu thập kế hoạch giảng dạy và số tiết từng môn]
          |
          v
[2. Thu thập lịch rảnh/bận của giáo viên]
          |
          v
[3. Kiểm tra số lượng và điều kiện phòng học]
          |
          v
[4. Sắp xếp thời khóa biểu cho từng lớp]
          |                 BOTTLENECK
          v
[5. Kiểm tra trùng lịch giáo viên / phòng học / lớp]
          |
          v
[6. Điều chỉnh các lịch bị xung đột]
          |
          v
[7. Công bố thời khóa biểu]
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: dễ triển khai và giá thành thấp nhất nhóm. Card này sử dụng dữ liệu riêng của nhà trường (rule, lịch học, tư vấn...) nên sẽ cần hệ thống riêng để đảm bảo trả lời chính xác. Card này cũng có thể giải quyết một số vấn đề của card khác như lịch đưa đón, phụ huynh đăng kí đưa đón, thành tích học tập...
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

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
