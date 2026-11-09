# Báo cáo cá nhân — 2A202603694_HoangHaiNam

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Hoàng Hải Nam
- MSSV: 2A202603694
- Email trường (không bắt buộc, repo có thể để public): 26ai.namhh2@vinuni.edu.vn
- Tên nhóm: C204T1
- Link repo nhóm: https://github.com/nashtran001/K5-L3A-DAY02-C204T1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại| Khi đến cuối ngày làm việc, tôi muốn nắm được danh sách các commit, PR và tiến độ phần việc đã làm trong ngày, để gửi báo cáo cuối ngày cho Tech Lead| Dev, Tech Lead| 10–15 phút/ngày, 6 ngày/tuần (phải xem lại task, commit, task trên jira để nhớ hôm nay đã làm được những gì và mai mình sẽ làm gì)|
| 2 | Lặp lại | Khi đã code xong một task và tạo Pull Request vào nhánh `main`, tôi muốn tóm tắt đầy đủ các thay đổi và đồng bộ trạng thái sang ticket Jira, để Tech Lead nắm rõ ngữ cảnh khi review mà không bị sót bước cập nhật | Dev, Tech Lead | 10–15 phút/task, khoảng 4–6 task/tuần (đếm từ lịch sử PR và log chuyển trạng thái Jira) |
| 3 | Tốn thời gian | Khi vừa hoàn thành logic của một task, tôi muốn chuẩn bị nhanh dữ liệu mẫu (mock data) và các kịch bản kiểm thử biên, để viết xong unit test trước khi đẩy PR cho Tech Lead | Dev | 30–45 phút/task, 4–6 lần/tuần (xem thời gian giữa commit code logic và commit unit test) |
| 4 | Tốn thời gian | Khi nhận một ticket báo bug từ Tester, tôi muốn dựng lại đúng trạng thái dữ liệu và các bước thao tác gây lỗi trên máy local, để tái hiện được bug trước khi bắt đầu sửa | Dev, Tester | 20–30 phút/bug để tái hiện, trung bình 3–5 bug/tuần (đếm từ các ticket bug trên Jira) |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi đã tái hiện được bug, tôi muốn khoanh vùng nhanh dòng lỗi trong file log hệ thống và đối chiếu với dữ liệu đầu vào của Tester, để tìm ra nguyên nhân gốc thay vì mò từng dòng log | Dev | 30–40 phút/bug, 3–5 lần/tuần; mỗi lần phải lọc đọc hàng trăm dòng log hệ thống |
| 6 | Pain từ người khác | Khi Tech Lead mở một Pull Request mới để review trước khi merge vào `main`, Tech Lead muốn biết ngay mục đích thay đổi, các file trọng tâm và phạm vi ảnh hưởng, để không phải đọc mò toàn bộ code diff hoặc hỏi lại dev | Tech Lead, Dev | PR thường phải chờ 2–4 tiếng mới được merge; 2–3 lần/tuần Tech Lead phải nhắn hỏi lại ngữ cảnh |
| 7 | Pain từ người khác | Khi Tester báo bug lên Jira hoặc nhận lại bản fix từ dev, Tester muốn biết rõ dữ liệu liên quan và phạm vi các tính năng bị ảnh hưởng khi sửa code, để không phải nhắn hỏi qua lại và không bỏ sót lỗi hồi quy | Tester, Dev | 2–3 ticket/tuần phải comment hỏi lại thông tin thao tác hoặc phạm vi test trên Jira |
| 8 | Cần đọc, tổng hợp nhiều thông tin | Khi bắt đầu sửa bug ở một module cũ ít đụng tới, tôi muốn biết hàm này đang được gọi ở những luồng nghiệp vụ nào, để sửa lỗi mà không làm hỏng các tính năng khác | Dev, Tester | 25–35 phút đọc code cũ mỗi lần gặp bug ở module lạ, khoảng 1–2 lần/tuần |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Sau khi tự nêu 3 luồng công việc hàng ngày (báo cáo cuối ngày, viết unit test/tạo PR/cập nhật Jira, tái hiện bug/đọc log) và tách thành 6 ý đầu, tôi dùng AI hỏi thêm góc nhìn và giữ lại ý 7 và 8 vì đúng với thực tế làm việc. Bỏ gợi ý "xây dựng hệ thống AI tự động tìm và tự sửa mọi bug từ log" vì đây là giải pháp không quá tốt, phạm vi quá rộng và rủi ro làm hỏng nhánh `main` rất cao.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Khoanh vùng dòng lỗi trong log hệ thống tìm nguyên nhân gốc (#5) | Tốn nhiều thời gian nhất mỗi khi xử lý bug (30–40 phút/bug), quy trình rõ ràng, bottleneck cụ thể | Log hệ thống hiện tại đã đủ thông tin ngữ cảnh hay phải chuẩn hóa lại format log trước? |
| 2 | Chuẩn bị mock data và kịch bản biên để viết Unit Test (#3) | Lặp lại ở mọi task (30–45 phút/task, 4–6 lần/tuần), có thể đo thời gian rất dễ qua lịch sử commit | Làm sao đảm bảo các kịch bản kiểm thử biên không bị bỏ sót nếu nhờ công cụ sinh nháp? |
| 3 | Tổng hợp commit, PR và tiến độ Jira để gửi báo cáo cuối ngày (#1) | Làm đều đặn 6 ngày/tuần (10–15 phút/ngày), dữ liệu đầu vào đã có sẵn trên Git và Jira| Chỉ dùng script lấy danh sách commit/Jira (Rule) đã đủ chưa hay cần bước tóm tắt bằng AI? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi đã tái hiện được bug, tôi muốn khoanh vùng nhanh dòng lỗi trong file log hệ thống và đối chiếu với dữ liệu đầu vào của Tester, để tìm ra nguyên nhân gốc thay vì mò từng dòng log |
| Actor | Developer trực tiếp xử lý bug |
| Thời điểm / bối cảnh | Ngay sau khi Dev vừa tái hiện được bug trên máy/môi trường test theo ticket của Tester |
| Quy trình hiện tại (3–7 bước) | 1. Lấy thông tin thời điểm lỗi và dữ liệu đầu vào (payload/tham số) từ bước tái hiện bug · 2. Mở file log hệ thống và tìm kiếm thủ công theo từ khóa hoặc khoảng thời gian · 3. Đọc dò qua hàng trăm dòng log để lọc ra đúng khối stack trace và dữ liệu liên quan · 4. Đối chiếu dòng log lỗi với dữ liệu đầu vào của Tester và luồng code trong IDE · 5. Xác định chính xác hàm/điều kiện gây ra lỗi để bắt đầu sửa |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (đọc dò trong hàng trăm dòng log hệ thống để tách đúng chuỗi log lỗi: 15 phút) và Bước 4 (đối chiếu thủ công log với dữ liệu đầu vào và luồng code: 12 phút) |
| Impact (nếu không giải thì sao) | Mất 30–40 phút/bug chỉ riêng cho khâu đọc log tìm nguyên nhân; đọc log thủ công dễ nhìn nhầm dòng lỗi phụ thành nguyên nhân chính, làm kéo dài thời gian fix bug |
| Success metric (baseline → target) | Giảm thời gian đọc log và đối chiếu tìm nguyên nhân gốc từ 35 phút xuống dưới 12 phút/bug; xác định đúng hàm gây lỗi ngay từ lần khoanh vùng đầu tiên |
| Phương án không dùng AI | Gắn mã định danh (`request_id`) cố định cho mỗi thao tác test + dùng script CLI tự động cắt riêng các dòng log thuộc đúng `request_id` đó ra một file ngắn |
| Giả thuyết về AI (nếu có) | Sau khi script lọc ra đoạn log của phiên lỗi, AI đọc đoạn log + payload đầu vào của Tester để tóm tắt luồng chạy, chỉ ra biến bị sai giá trị và gợi ý vị trí hàm gây lỗi cho Dev kiểm tra |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 35 phút/bug

[1 Lấy thời điểm & dữ liệu đầu vào: 3'] → [2 Mở file log & tìm theo từ khóa/giờ: 5']
→ [3 Đọc dò hàng trăm dòng log để lọc stack trace: 15'] ← BOTTLENECK
→ [4 Đối chiếu log với dữ liệu Tester & luồng code: 10'] ← BOTTLENECK
→ [5 Chốt nguyên nhân gốc (root cause): 2']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa hoàn thành logic của một task, tôi muốn chuẩn bị nhanh dữ liệu mẫu (mock data) và các kịch bản kiểm thử biên, để viết xong unit test trước khi đẩy PR cho Tech Lead |
| Actor | Developer phụ trách phát triển tính năng/task|
| Thời điểm / bối cảnh | Sau khi đã code xong logic chính của task trên nhánh hiện tại, trước khi commit và mở Pull Request vào nhánh `main` (4–6 lần/tuần) |
| Quy trình hiện tại (3–7 bước) | 1. Đọc lại hàm logic vừa viết và các model/kiểu dữ liệu đầu vào — đầu ra · 2. Liệt kê các kịch bản cần kiểm thử (happy case, null/empty, dữ liệu biên, ngoại lệ) · 3. Tự gõ thủ công dữ liệu mẫu (mock data) cho từng object/bảng liên quan · 4. Viết code cho từng hàm unit test và các lệnh `assert` · 5. Chạy test trên máy local và sửa lại nếu mock data chưa khớp kiểu dữ liệu |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (tự tạo thủ công dữ liệu mẫu mock data khớp với nhiều trường của model: 15 phút) và Bước 4 (viết lặp đi lặp lại các hàm unit test cho từng kịch bản biên: 12 phút) |
| Impact (nếu không giải thì sao) | Tốn 30–45 phút/task (khoảng 2,5–4 tiếng/tuần/Dev); vì việc tạo mock data nhàm chán nên Dev dễ bỏ qua các kịch bản biên (edge cases), dẫn tới lọt lỗi khi Tester kiểm thử |
| Success metric (baseline → target) | Giảm thời gian chuẩn bị mock data và viết unit test từ 35–40 phút xuống dưới 15 phút/task; mỗi hàm logic có tối thiểu 3 kịch bản kiểm thử biên được bao phủ |
| Phương án không dùng AI | Xây dựng bộ hàm tạo dữ liệu mẫu dùng chung (Test Data Builder / Fixture có sẵn) + dùng snippet template tạo nhanh khung hàm unit test trong IDE |
| Giả thuyết về AI (nếu có) | Đưa hàm logic và cấu trúc model vào để AI sinh nháp bộ mock data hợp lệ kèm danh sách các unit test cho trường hợp biên; Dev rà soát lại các điều kiện `assert` và chạy test thật |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 38 phút/task

[1 Đọc lại hàm logic & model: 4'] → [2 Liệt kê kịch bản chuẩn & biên: 4']
→ [3 Tự gõ thủ công bộ mock data: 15'] ← BOTTLENECK
→ [4 Viết code unit test & assert: 10'] ← BOTTLENECK
→ [5 Chạy test local & chỉnh sửa: 5']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến cuối ngày làm việc, tôi muốn nắm được danh sách các commit, PR và tiến độ phần việc đã làm trong ngày, để gửi báo cáo cuối ngày cho Tech Lead |
| Actor | Developer trong team phát triển (báo cáo cho Tech Lead mỗi cuối ngày) |
| Thời điểm / bối cảnh | Cuối mỗi ngày làm việc (khoảng 17h30–18h00), lặp lại 6 ngày/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Mở terminal/Git xem lại danh sách các commit mình đã đẩy trong ngày · 2. Mở GitHub kiểm tra các Pull Request đã tạo hoặc đang đợi review · 3. Mở Jira xem lại trạng thái các task và bug mình đã xử lý trong ngày · 4. Ngồi nhớ lại và đối chiếu xem hôm nay đã xong được gì, còn vướng gì và ngày mai sẽ làm gì · 5. Gõ nội dung báo cáo cuối ngày theo mẫu và gửi cho Tech Lead |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 (phải tự nhớ lại và ghép nối thông tin rời rạc từ commit, PR và task Jira để tổng hợp tiến độ hôm nay + kế hoạch ngày mai: 5 phút) |
| Impact (nếu không giải thì sao) | Mất 10–15 phút mỗi cuối ngày (60–90 phút/tuần/Dev); cuối ngày mệt mỏi dễ quên liệt kê các đầu việc nhỏ hoặc cập nhật thiếu tiến độ khiến Tech Lead phải hỏi lại |
| Success metric (baseline → target) | Giảm thời gian tổng hợp và viết báo cáo cuối ngày từ 13 phút xuống dưới 3 phút/ngày; không bỏ sót task hay PR nào đã làm trong ngày |
| Phương án không dùng AI | Viết 1 script ngắn chạy lệnh `git log --since="today"` kết hợp lấy danh sách task Jira xuất thẳng ra khung văn bản Markdown để Dev chỉ việc điền thêm dòng kế hoạch ngày mai |
| Giả thuyết về AI (nếu có) | Script tự gom danh sách commit, PR và Jira trong ngày → AI tóm tắt gọn thành 3 mục (Đã hoàn thành hôm nay / Đang xử lý & vướng mắc / Kế hoạch ngày mai) → Dev đọc kiểm tra 1 phút rồi gửi Tech Lead |
| Cảm nhận nhanh | Rule / Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 13 phút/ngày (6 ngày/tuần)

[1 Xem lại commit trên Git: 2'] → [2 Kiểm tra PR đã tạo: 2'] → [3 Xem lại task trên Jira: 2']
→ [4 Nhớ lại & ghép nối tiến độ hôm nay + việc ngày mai: 4'] ← BOTTLENECK
→ [5 Viết nội dung báo cáo & gửi Tech Lead: 3']
```

### Card muốn pitch nhất

- Card số: **Card #1** — Khoanh vùng dòng lỗi trong log hệ thống tìm nguyên nhân gốc (#5) *(dự phòng **Card #3** — Báo cáo cuối ngày (#1) nếu nhóm muốn chọn bài toán quy trình gọn, dễ làm pilot ngay trong buổi lab)*.
- Vì sao: Đây là việc ngốn nhiều thời gian và gây mệt mỏi nhất mỗi khi xử lý bug (30–40 phút/bug), quy trình từng bước rất rõ ràng và dễ phân tách giữa phần việc của Rule (lọc cắt log theo ID/thời gian) với phần việc của AI (đối chiếu log với dữ liệu đầu vào của Tester).
- Câu hỏi muốn nhóm phản biện: *"Theo các bạn, nếu chỉ dùng script lọc log theo `request_id` và khoảng thời gian lỗi (Rule) mà không dùng AI thì đã giảm được quá nửa thời gian mò log của Dev chưa?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Ở bản nháp đầu, tôi gộp nhiều problem ở CP1 vào chung một Problem Card làm quy trình bị dàn trải và có quá nhiều bottleneck | Đồng ý | Tách lại đúng chuẩn 1-1: mỗi Problem Card chỉ lấy đúng 1 problem từ bảng Scan ở CP1 (#5, #3, #1) và giữ nguyên câu Job Story tương ứng |
| Ở Card 1, AI chỉ ra nếu đưa nguyên cả file log hàng nghìn dòng vào AI thì vừa tốn chi phí vừa dễ bị nhiễu | Đồng ý | Bổ sung rõ ở "Phương án không dùng AI" và "Giả thuyết về AI": dùng script (Rule) cắt đoạn log quanh thời điểm lỗi trước, sau đó mới đối chiếu với dữ liệu của Tester |
| Ở Card 3, AI gợi ý cho hệ thống tự động gửi báo cáo thẳng cho Tech Lead vào cuối ngày | Không đồng ý | Giữ boundary là Dev luôn phải đọc duyệt lại bản nháp trước khi gửi, vì phần kế hoạch ngày mai và vướng mắc thực tế cần con người xác nhận |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Đưa ra problem card để các thành viên trong nhóm cùng thảo luận và phản biện ý tưởng của thành viên khác trong nhóm| Giúp nhóm biết thêm được vấn đề mà lập trình viên thường gặp phải và nhận được ý kiến cải thiện. Đồng thời phản biện với ý kiến của thành viên khác để họ nhận ra vấn đề về sự thiếu chính xác khi xử dụng AI để xử lý các context lớn|
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Nếu dùng AI để đọc tin nhắn qua các nền tảng mạng xã hội thì context sẽ quá lớn vì có hàng trăm tin nhắn, vậy thì làm thế nào để đảm bảo AI đã trả lời đúng và không bị halucinate| Giúp cả nhóm cùng thảo luận và tìm ra giải pháp là chia nhỏ các đoạn tin nhắn ra và gửi cho AI nhiều lần, đồng thời các đoạn hội thoại được overlap lên nhau để tránh trường hợp context không liền mạch|
| Nhận phản biện | Câu hỏi tôi nhận được: Hiện tại các hệ thống tracing log đã có các nền tảng đã làm như firebase, nó có thể tái hiện thao tác của người dùng trên production và đưa ra gợi ý sửa lỗi. Vậy thì ý tưởng này triển khai có khả thi không?| Tôi đã sửa gì: Tiếp tục xem xét vì trong thực tế đi làm không phải lúc nào cũng dùng firebase mà thường là các hệ thống tracing log khác không có hệ thống AI sẵn như firebase|
| Gom cluster / cây OST | Trực tiếp gom các candidate có chung pattern tổng hợp tin nhắn vào Cluster A và dựng cây OST (1 Outcome, 3 Opportunity) | Hoàn thành cây OST của nhóm và gạch bỏ các ý mang tính giải pháp đội lốt (#5, #7) |
| Chọn candidate problem | Lập bảng chấm điểm shortlist 3 candidate theo 7 tiêu chí và đề xuất chốt chọn Candidate #1 (Tổng hợp hơn 10 nhóm Zalo cho CEO) | Chốt được bài toán trọng tâm của nhóm (#1 đạt 27 điểm, tốn ~120 phút/ngày đọc và lọc tin) |
| Kiểm chứng / research | Xây dựng Assumption Map (6 giả định) và trực tiếp research 3 giải pháp có sẵn: Zalo OA / GMF, Slack AI, n8n Information Extractor | Chỉ ra giới hạn kỹ thuật của Zalo OA/GMF (chỉ quản lý nhóm do OA tạo) để nhóm điều chỉnh hướng tiếp cận |
| Quy trình nhóm | Thiết kế sơ đồ quy trình trước/sau (5 bước hiện tại → 6 bước tương lai thử trên 3 nhóm) và lập bảng so sánh Before/After | Đưa giải pháp cắt nhỏ hội thoại có overlap (Rule) + người duyệt bản nháp vào quy trình, kỳ vọng giảm từ 120' xuống ≤20'/ngày |
| Problem Statement | Trực tiếp viết Problem Statement v0, nâng cấp lên v1 và xây dựng bộ 3 tiêu chí đánh giá (eval) đầu ra của AI | Chuẩn hóa metric cả về thời gian lẫn chất lượng (độ phủ ≥85%, tỉ lệ sai/bịa ≤5%, bắt buộc gắn nguồn tin nhắn) |
| Mức can thiệp AI | Phân tích ma trận độ mơ hồ × độ phức tạp, lập bảng so sánh 4 mức, điền AI Canvas và trả lời 2 câu hỏi Google PAIR | Chốt mức **Workflow có điều kiện kết hợp Rule** (hướng Augment hỗ trợ CEO, không dùng Agent tự hành) |
| Quyết định | Đánh giá chi tiết 4 rủi ro (Value, Usability, Feasibility, Viability), viết kết luận quyết định và đặt ngưỡng dừng | Chốt quyết định **Not Yet** kèm lộ trình kiểm chứng Tuần 0–2 và ngưỡng dừng định lượng (độ phủ <70% hoặc sai/bịa >10% thì quay về thủ công) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Dùng để gợi ý viết problem sao cho chuẩn trong khi tôi chỉ nêu các vấn để ở mức độ rất sơ khai và chưa mô tả quá chi tiết| Giúp tôi có cái nhìn sâu sắc hơn vào vấn đề| Có 1 số case bị lặp lại hoặc đưa ra 1 số ý tưởng không khả thi| Khi AI đưa ra các giải pháp hoặc đề xuất không hợp lý thì tôi bảo AI đề xuất lại hoặc tự sửa ngôn từ bằng tay|
| CP2 Problem Card | Bảo AI đóng vai PM để phản biện 3 Problem Cards và kiểm tra cách vẽ quy trình nháp| Chỉ ra việc cần tách bước lọc cắt log bằng script trước khi dùng AI ở Card 1 để tránh nhiễu| Ở bản nháp đầu, AI gộp nhiều problem ở CP1 vào chung 1 Card làm quy trình bị dàn trải; ở Card 3 lại gợi ý cho bot tự động gửi báo cáo thẳng cho Tech Lead | Sửa lại đúng chuẩn 1-1 và giữ boundary là Dev luôn phải đọc duyệt lại bản nháp trước khi gửi Tech Lead|
| CP4 Research | Tìm các công cụ có sẵn trên thị trường đang giải bài toán tổng hợp báo cáo qua tin nhắn qua nền tảng mạng xã hội như Zalo OA đã có sẵn công cụ này | Gợi ý nhanh tên các công cụ/tính năng có sẵn | Đưa ra một số thông tin tính năng ở gói miễn phí/trả phí chưa chính xác | Tự mở kiểm tra link chính thức để ghi đúng bước nào công cụ giải được và bước nào còn bỏ trống |
| CP5 Quy trình | Nhờ AI chuyển mô tả các bước quy trình xử lý tin nhắn và tổng hợp báo cáo sang sơ đồ và bảng so sánh trước/sau | Tạo khung sơ đồ nhanh và gợi ý cách trình bày bảng Before/After rõ ràng | AI gộp bước tiền xử lý tin nhắn với bước tóm tắt thành 1 bước, đồng thời bỏ qua bước xử lý context dài và bước con người kiểm tra lại | Tự tách rõ bước dùng Rule (chia nhỏ đoạn hội thoại có overlap để không đứt mạch ngữ cảnh), bước AI tóm tắt và bước con người kiểm duyệt kèm phương án quay về |
| CP5–6 Problem Statement | Nhờ AI phản biện và chỉ ra lỗ hổng trong 6 trường của Problem Statement | Chỉ ra Success Metric ở bản v0 mới chỉ đo thời gian tổng hợp mà chưa đo độ chính xác và tỉ lệ bỏ sót thông tin trong tin nhắn | Khi phản biện xong, AI tự ý viết lại câu Problem Statement theo hướng tính năng giải pháp | Không dùng câu viết lại của AI; tự giữ cấu trúc của nhóm |
| CP6 Mức can thiệp / quyết định | Kiểm tra bảng so sánh 4 mức (No AI / Rule / Workflow / Agent) và gợi ý cách viết các tiêu chí đánh giá (eval) | Giúp rà soát các thành phần trong AI Canvas và cách đặt ngưỡng dừng (kill criteria) cụ thể | Đề xuất dùng tới mức Agent tự động đọc và tự gửi báo cáo, chưa tính đến rủi ro AI bị hallucinate khi có hàng trăm tin nhắn | Chốt ở mức kết hợp Rule (cắt nhỏ tin nhắn có overlap) + Workflow (AI tóm tắt từng phần, con người duyệt cuối) vì kiểm soát được chất lượng và tránh hallucinate |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi đã học được thêm về ý tưởng tư duy sản phẩm của các bạn khác, các bạn có ý tưởng rất hay và thú vị, giải quyết được nhiều bài toán thực tế 

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Lúc mới thảo luận bài toán nhóm Zalo và cả lúc làm cây OST, nhóm từng nghĩ ngay đến việc "dùng AI đọc toàn bộ tin nhắn các nhóm Zalo để tự tạo báo cáo và giao việc". Khi rà lại quy tắc OST và đặt câu hỏi phản biện về việc context hàng trăm tin nhắn quá dài sẽ khiến AI bị hallucinate cũng như chưa rõ Zalo có cho phép đọc tin nhắn không, nhóm đã gạch bỏ các ý mang tính giải pháp ở tầng Opportunity và lùi lại xác định đúng từng bước nghẽn trong quy trình đọc.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Khi tôi pitch Problem Card #1 về việc khoanh vùng dòng lỗi trong log hệ thống để tìm nguyên nhân gốc, Việt Anh và Minh Nhật đã phản biện rằng hiện nay các nền tảng như Firebase hay Sentry đã hỗ trợ tracing log, tái hiện thao tác trên production với chi phí thấp, hoặc nếu Tester ghi rõ bước tái hiện kèm `request_id` thì chỉ cần lọc bằng script là đủ. Dù ở một số dự án tự host log nội bộ chưa có sẵn các dịch vụ đó, tôi đồng ý rằng bài toán của tôi hẹp hơn và phần lớn giải quyết được bằng chuẩn hóa quy trình báo bug, nên tôi đã đồng thuận cùng nhóm chọn bài toán tổng hợp báo cáo từ tin nhắn trong nhóm Zalo để đào sâu.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất ở bước research là tài liệu chính thức của Zalo OA chỉ hỗ trợ quản lý các nhóm do chính Official Account tạo ra, chứ chưa có cơ chế rõ ràng để lấy lịch sử tin nhắn từ các nhóm Zalo cá nhân sẵn có của CEO với nhân viên. Phát hiện này thay đổi hoàn toàn góc nhìn của nhóm: rào cản lớn nhất không chỉ nằm ở việc AI tóm tắt có hay không, mà nằm ngay ở tính khả thi của dữ liệu đầu vào và rào cản bảo mật.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là đặt ra Success Metric và Boundary sao cho đo đếm được trong thực tế mà không lồng giải pháp sẵn vào câu mô tả vấn đề. Với bài toán đọc tin nhắn Zalo, hiện chưa có số liệu đếm số lần sót việc thực tế, nên nhóm phải thiết kế lại là thu hẹp thử nghiệm trên 3 nhóm Zalo trong 2 tuần để đo cả thời gian lẫn độ phủ và tỉ lệ sai/bịa.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, ngay từ đầu tôi sẽ đo đếm số liệu thật trên một nhóm chat cụ thể thay vì để nhiều chỉ số ở mức ước lượng. Tôi cũng sẽ phản biện nhóm mạnh hơn ở phương án No AI vì số lượng nhân sự ít và hoàn toàn có thể tự kiểm soát được.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Problem của nhóm xuất phát từ việc CEO một công ty (~5 người) phải theo dõi nhiều nhóm Zalo, mất nhiều thời gian mỗi ngày để đọc các báo cáo. Quy trình hiện tại gồm 5 bước thủ công hoàn toàn, trong đó phần mất thời gian nhất nằm ở khâu đọc lại hàng trăm tin nhắn chưa đọc và lọc ra các thông tin quan trọng. Để cải thiện, nhóm thiết kế quy trình thử nghiệm trên 3 nhóm Zalo với Success Metric là giảm thời gian CEO đọc và kiểm tra từ 120 phút xuống tối đa 20 phút/ngày, giảm ít nhất 80% sự cố sót việc, đạt độ phủ tối thiểu 85% việc quan trọng và tỉ lệ thông tin sai/bịa không quá 5%. Về Boundary, hệ thống chỉ được đọc các nhóm được cấp phép, mỗi ý tóm tắt bắt buộc phải gắn kèm nguồn tin nhắn gốc để đối chiếu, tuyệt đối không tự ý nhắn tin cho người khác, và có người kiểm tra bản nháp trong tuần đầu. Nhóm chọn mức can thiệp là Workflow có điều kiện kết hợp với Rule (Rule gom tin nhắn, chia nhỏ đoạn hội thoại có overlap để giữ ngữ cảnh và gửi báo cáo đúng 7h sáng; AI chỉ làm một bước là trích xuất quyết định, cam kết ai–việc–hạn và câu hỏi còn chờ) vì chat tự do không thể bắt hết bằng Rule thuần túy nhưng cũng chưa cần tới Agent tự hành. Cuối cùng, sau khi đánh giá 4 rủi ro, nhóm đưa ra quyết định cần kiểm chứng kết nối dữ liệu và đo baseline ở Tuần 0–2 trước, kèm ngưỡng dừng là nếu không lấy được đầu vào hợp lệ hoặc sau 2 vòng chỉnh mà độ phủ dưới 70% / tỉ lệ bịa trên 10% thì dừng và quay về phương án nhân viên tóm tắt thủ công theo mẫu.

---

## 7. Tài liệu tham khảo

- Tài liệu hướng dẫn Zalo Official Account — Quản lý nhóm (GMF): https://oa.zalo.me/home/documents/vie/guides/quan-ly-nhom-gmf_1954166378348758227
- Tài liệu tính năng Slack AI (Tóm tắt hội thoại & recap): https://slack.com/help/articles/25076892548883-Guide-to-AI-features-in-Slack
- Tài liệu n8n Information Extractor Node: https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.information-extractor/
