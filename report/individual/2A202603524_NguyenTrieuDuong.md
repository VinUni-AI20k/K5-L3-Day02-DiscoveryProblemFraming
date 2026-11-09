# Báo cáo cá nhân — 2A202603524_NguyenTrieuDuong

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Triều Dương
- MSSV: 2A202603524
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:
- Link repo nhóm: https://github.com/olivercuongnguyen-ca/K5-L3A-DAY02-NguyenHoangCuong-2A202603568-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Pain từ người khác | Khi gửi Pull Request (PR) để Senior/Tech Lead review, tôi muốn đáp ứng các yêu cầu về convention và type ngay từ lần gửi đầu, để giảm số vòng sửa và thời gian chờ merge. | Fresher Dev, Tech Lead | PR thường kéo dài 2–3 vòng review, mất 1–2 ngày mới được merge do lỗi convention hoặc thiếu type. |
| 2 | Tốn thời gian | Khi tích hợp một API mới từ Backend vào component React, tôi muốn hiểu rõ cấu trúc payload và response, để triển khai đúng mà không phải hỏi lại nhiều lần qua Slack. | Frontend Dev, Backend Dev | Tốn trung bình 15–20 phút nhắn hỏi/trao đổi lại mỗi endpoint mới, khoảng 3–4 lần/tuần. |
| 3 | Lặp lại | Khi triển khai giao diện mới theo thiết kế Figma, tôi muốn xác định đúng màu sắc, spacing và typography tương ứng trong dự án, để giảm thời gian tra cứu và đối chiếu thủ công từng thông số. | Frontend Dev, Designer | Mất 20 phút/màn hình mới: 10 phút tra thông số và 10 phút đối chiếu token/class. |
| 4 | Tốn thời gian | Khi tự kiểm tra tính năng trên các kích thước màn hình khác nhau trước khi bàn giao QA, tôi muốn phát hiện các lỗi vỡ layout hoặc lỗi hiển thị khó thấy, để giảm số lần bị trả task để sửa giao diện. | Frontend Dev, QA | QA thường trả về 3–5 bug liên quan đến UI/responsive ở mỗi task hoàn thành. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi gặp lỗi TypeScript phức tạp hoặc lỗi build cho môi trường production, tôi muốn xác định nhanh nguyên nhân gốc rễ từ thông báo lỗi và các tài liệu liên quan, để tránh bị nghẽn tiến độ sprint. | Frontend Dev | Mất 30–60 phút cho mỗi lỗi build/type phức tạp chưa từng gặp. |
| 6 | Lặp lại | Khi viết unit test cho component React phức tạp, tôi muốn chuẩn bị dữ liệu mock và môi trường kiểm thử nhất quán với ít thao tác lặp lại, để dành nhiều thời gian hơn cho các tình huống kiểm thử của component. | Frontend Dev | Mất 25 phút setup/component phức tạp, gồm 10 phút chạy và sửa lỗi setup; viết test nghiệp vụ mất thêm 20 phút, tổng 45 phút. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Sáu problem và số liệu ban đầu do tôi cung cấp. AI hỗ trợ rà soát và đề xuất chỉnh cách diễn đạt Job Story, không bổ sung ý mới.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

CP1 và CP2 dùng số liệu thời gian đã được học viên cập nhật. Target là mục tiêu cải thiện.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | #2 — Làm rõ payload/response khi tích hợp API | Actor rõ; có thời gian 15–20 phút/endpoint và tần suất 3–4 lần/tuần; kiểm chứng được trên phạm vi vài endpoint. | Thời gian đã gồm chờ Backend hay chỉ trao đổi chủ động? Tài liệu hiện tại thiếu gì? |
| 2 | #3 — Đối chiếu Figma với style trong dự án | Actor rõ; đã có thời gian từng bước; so sánh được với giải pháp tài liệu và quy ước dùng chung. | Chuẩn hóa token có giảm được cả thời gian đối chiếu và kiểm tra giao diện không? |
| 3 | #6 — Chuẩn bị môi trường và mock cho unit test | Thao tác lặp lại; tách được setup khỏi viết test logic; có thể thử template/helper trên phạm vi nhỏ. | Template/helper dùng chung được cho những nhóm component nào? |

### Problem Card #1 — Làm rõ payload/response khi tích hợp API (CP1 #2)

| Trường | Nội dung |
|---|---|
| Job Story | Khi tích hợp một API mới từ Backend vào component React, tôi muốn hiểu rõ cấu trúc payload và response, để triển khai đúng mà không phải hỏi lại nhiều lần qua Slack. |
| Actor | Frontend Dev tích hợp endpoint; Backend Dev giải đáp cấu trúc dữ liệu. |
| Thời điểm / bối cảnh | Nhận endpoint mới và chuẩn bị nối dữ liệu vào component React. |
| Quy trình hiện tại (3–7 bước) | Nhận endpoint → đọc tài liệu → trao đổi làm rõ với Backend → khai báo type và tích hợp → kiểm tra response. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: trao đổi làm rõ payload/response, 15 phút theo quy trình chi tiết; CP1 ghi khoảng 15–20 phút. Bước 4 tích hợp cũng mất 15 phút; chọn bước 3 làm điểm tập trung vì có thao tác hỏi lại. Khi đo, ghi riêng thời gian chờ và thời gian trao đổi chủ động. |
| Impact (nếu không giải thì sao) | Hỏi lại mỗi endpoint, ngắt quãng công việc hai bên. Riêng trao đổi khoảng 45–80 phút/tuần, tính từ số liệu CP1: 15–20 phút × 3–4 lần; không phải tổng thời gian tích hợp. |
| Success metric (baseline → target) | Baseline chi tiết: 15 phút làm rõ/endpoint → target ≤10 phút/endpoint, số lỗi do hiểu sai payload không tăng trên cùng số endpoint so sánh. Đo trên 5 endpoint mới, ghi riêng thời gian chờ và thời gian trao đổi chủ động, dùng cùng cách đo trước/sau. |
| Phương án không dùng AI | Thống nhất tài liệu API có ví dụ request/response, type, trường bắt buộc/nullable và mã lỗi; cập nhật khi endpoint thay đổi. |
| Giả thuyết về AI (nếu có) | Nếu tài liệu đã có nhưng khó tra cứu, có thể thử hỗ trợ trích cấu trúc từ tài liệu được phép sử dụng. Dev phải đối chiếu với API thực tế, không chấp nhận trường dữ liệu do AI suy đoán. Chưa có bằng chứng cần AI. |
| Cảm nhận nhanh | No AI — ưu tiên làm rõ hợp đồng dữ liệu và cách cập nhật tài liệu; chưa chốt mức can thiệp. |

Quy trình nháp hiện tại:

```text
[1. Nhận endpoint: 5 phút]
 → [2. Đọc tài liệu và ví dụ: 5 phút]
 → [3. Trao đổi làm rõ với Backend: 15 phút] ← BOTTLENECK
 → [4. Khai báo type và tích hợp: 15 phút]
 → [5. Kiểm tra response: 10 phút]
Tổng: 50 phút/endpoint, theo các bước đã điền.
Phần làm rõ API: 15 phút; chưa tách thời gian chờ và trao đổi chủ động.
```

### Problem Card #2 — Đối chiếu Figma với style trong dự án (CP1 #3)

| Trường | Nội dung |
|---|---|
| Job Story | Khi triển khai giao diện mới theo thiết kế Figma, tôi muốn xác định đúng màu sắc, spacing và typography tương ứng trong dự án, để giảm thời gian tra cứu và đối chiếu thủ công từng thông số. |
| Actor | Frontend Dev triển khai giao diện; Designer giải thích thông số chưa rõ. |
| Thời điểm / bối cảnh | Bắt đầu một màn hình mới từ thiết kế Figma, cần xác định style trước khi triển khai. |
| Quy trình hiện tại (3–7 bước) | Mở màn hình Figma → tra thông số → đối chiếu token/class → áp dụng style → kiểm tra với thiết kế. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước dài nhất theo quy trình: kiểm tra với thiết kế (bước 5), 15 phút/màn hình. Đối chiếu token/class (bước 3) mất 10 phút, là điểm tập trung của problem nhưng chưa có bằng chứng đây là nguyên nhân khiến bước kiểm tra kéo dài. |
| Impact (nếu không giải thì sao) | Quy trình mất 50 phút/màn hình; riêng tra cứu + đối chiếu là 20 phút (10 + 10), kiểm tra với thiết kế là 15 phút. |
| Success metric (baseline → target) | Baseline theo thời gian chi tiết: tra cứu + đối chiếu 20 phút/màn hình → target đề xuất ≤10 phút; kiểm tra với thiết kế 15 phút → target đề xuất ≤10 phút. Đo riêng hai phần trên 5 màn hình tương đương, ghi số sai lệch màu/spacing/typography để tránh tăng tốc nhưng tăng lỗi. |
| Phương án không dùng AI | Thống nhất tên token giữa thiết kế và code; tạo bảng đối chiếu token/class dùng chung và ví dụ; làm rõ cách xử lý giá trị chưa có token. |
| Giả thuyết về AI (nếu có) | Chỉ cân nhắc gợi ý token nếu tên gọi khó khớp. Nếu ánh xạ cố định, bảng tra hoặc rule có thể đủ. |
| Cảm nhận nhanh | No AI / Rule — cần kiểm tra tính nhất quán của token trước khi chọn. |

Quy trình nháp hiện tại:

```text
[1. Mở màn hình Figma: 5 phút]
 → [2. Tra màu, spacing, typography: 10 phút]
 → [3. Đối chiếu token/class: 10 phút] ← Điểm tập trung của problem
 → [4. Áp dụng style: 10 phút]
 → [5. Kiểm tra với thiết kế: 15 phút] ← BOTTLENECK
Tổng: 50 phút/màn hình. Riêng bước 2 + 3: 20 phút.

```

### Problem Card #3 — Chuẩn bị môi trường và mock cho unit test (CP1 #6)

| Trường | Nội dung |
|---|---|
| Job Story | Khi viết unit test cho component React phức tạp, tôi muốn chuẩn bị dữ liệu mock và môi trường kiểm thử nhất quán với ít thao tác lặp lại, để dành nhiều thời gian hơn cho các tình huống kiểm thử của component. |
| Actor | Frontend Dev viết unit test cho component React. |
| Thời điểm / bối cảnh | Bắt đầu file test cho component phức tạp có dữ liệu hoặc phụ thuộc cần mock. |
| Quy trình hiện tại (3–7 bước) | Xác định phụ thuộc → tạo file test/import → chuẩn bị wrapper/mock → chạy và sửa lỗi setup → viết test case nghiệp vụ. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: chạy và sửa lỗi setup, 10 phút/component; đây là bước khiến học viên phải dừng lại hoặc làm lại nhiều nhất trong phần setup. Viết test nghiệp vụ (20 phút) nằm ngoài metric setup. |
| Impact (nếu không giải thì sao) | Setup bước 1–4 mất 25 phút/component, trong đó chạy và sửa lỗi setup chiếm 10 phút; toàn quy trình gồm viết test là 45 phút. Thời gian chuẩn bị lặp lại làm giảm thời gian dành cho test nghiệp vụ. |
| Success metric (baseline → target) | Setup 25 phút/component → target đề xuất ≤15 phút; riêng chạy và sửa lỗi setup 10 phút → ≤5 phút. Đo trên 5 component cùng nhóm phụ thuộc, từ bắt đầu chuẩn bị đến khi kiểm tra setup tối thiểu chạy được; loại thời gian viết test nghiệp vụ khỏi cả hai lần đo. |
| Phương án không dùng AI | Tạo template file test, helper render với provider và fixture/mock dùng chung theo nhóm component; cho phép tùy chỉnh phụ thuộc riêng. |
| Giả thuyết về AI (nếu có) | Chỉ thử hỗ trợ phác thảo mock cho trường hợp chưa có helper nếu template không đủ. Dev kiểm tra mock phản ánh đúng hành vi; test chạy được chưa chứng minh mock đúng. |
| Cảm nhận nhanh | Rule — thử template/helper trước; chưa có bằng chứng cần Workflow hoặc Agent. |

Quy trình nháp hiện tại:

```text
[1. Xác định phụ thuộc: 5 phút]
 → [2. Tạo file test/import: 5 phút]
 → [3. Chuẩn bị wrapper/mock: 5 phút]
 → [4. Chạy và sửa lỗi setup: 10 phút] ← BOTTLENECK
 → [5. Viết test case nghiệp vụ: 20 phút; ngoài metric setup]
Tổng: 45 phút/component; setup bước 1–4: 25 phút; viết test: 20 phút.

```

### Card muốn pitch nhất

- Card số: #1 — Tích hợp API.
- Vì sao: Có thời gian và tần suất từ CP1, actor rõ, phạm vi kiểm chứng nhỏ. Cần phân biệt vấn đề tài liệu với thời gian chờ phản hồi.
- Câu hỏi muốn nhóm phản biện: Nếu chuẩn hóa tài liệu API và ví dụ request/response thì đã đủ giảm trao đổi chưa, hay bottleneck thật sự nằm ở việc chờ Backend phản hồi?

### AI đã phản biện card thế nào

**AI phản biện card #1 — Làm rõ payload/response khi tích hợp API:**

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 15–20 phút/endpoint chưa phân biệt thời gian chờ Backend với thời gian chủ động trao đổi, nên chưa xác định đúng phần có thể cải thiện. | Đồng ý | Trong bottleneck và success metric, tách hai loại thời gian cần đo; dùng 15 phút từ quy trình chi tiết làm baseline và theo dõi hai loại thời gian riêng khi đo trước/sau. |
| Target ≤10 phút/endpoint chưa có dữ liệu chứng minh khả thi hoặc kiểm soát việc hiểu sai payload. | Đồng ý  | Card đã ghi rõ target đề xuất và cách theo dõi lỗi hiểu sai payload trên 5 endpoint mới. Chưa có kết quả đo để khẳng định đạt target. |
| Chưa chứng minh cần AI: nếu nguyên nhân là tài liệu API thiếu hoặc không được cập nhật, AI có thể tiếp tục đưa thông tin sai. | Không đồng ý | Giữ giả thuyết AI hỗ trợ tra cứu khi tài liệu đã có, kèm bước đối chiếu API thực tế. Giữ No AI là phương án thử trước; AI vẫn là giả thuyết so sánh, không phải lựa chọn đã chốt. |

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
| CP1 Scan | Nhờ AI rà soát 6 problem tự liệt kê và đề xuất chỉnh Job Story. | Chỉ ra dòng 3 và 6 đang gắn với cách giải; đề xuất diễn đạt theo nhu cầu. | AI chưa kiểm chứng được số liệu hoặc nguồn bằng chứng thực tế. | Cần tự kiểm tra bản chỉnh và bổ sung nguồn, thời gian quan sát cho số liệu. |
| CP2 Problem Card | Nhờ AI đề xuất top 3, hỗ trợ dựng card/quy trình và phản biện; đã chọn #2, #3, #6. | Tính tổng từ thời gian đã điền; phân biệt setup với viết test; chỉ ra baseline CP1/CP2 chưa khớp. | Bản nháp ban đầu gán bottleneck khi chưa có thời gian từng bước; target vẫn là đề xuất chưa kiểm chứng. | Đã bổ sung thời gian và mức đồng ý với phản biện; dùng thời gian chi tiết cho metric CP2, tách setup khỏi viết test và giữ phương án đơn giản để so sánh. |
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
