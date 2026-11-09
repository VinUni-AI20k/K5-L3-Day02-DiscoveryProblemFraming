# Báo cáo cá nhân — 2A202603527_TrinhCongDuc

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trịnh Công Đức
- MSSV: 2A202603527
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: BDHH
- Link repo nhóm: https://github.com/trinhcongduc112/K5-L3A-DAY02-BDHH-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi đưa bản cập nhật lên môi trường chạy thử vào cuối ngày, tôi muốn bản mới chạy đúng mà không sót hay sai bước cấu hình, để cuối ngày không phải ở lại sửa lỗi thao tác. | Developer trong nhóm | Thời gian thao tác deploy: 10–15 phút/lần; tần suất 3–4 lần/tuần. Riêng lỗi thao tác cấu hình phải mất thêm 20–30 phút sửa lại, xảy ra khoảng 1 lần/tuần (dựa trên lịch sử Git commit). |
| 2 | Tốn thời gian | Khi gặp lỗi logic lúc viết backend, tôi muốn truy ra đúng dòng gây lỗi từ file log, để không phải thử sửa mò nhiều lần. | Backend developer | Mất 30–60 phút cho mỗi lần debug lỗi logic, tần suất 3–4 lần/tuần (dựa trên file log hệ thống và commit sửa lỗi). |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận tài liệu API dài hoặc schema cơ sở dữ liệu mới, tôi muốn nắm đủ trường đầu vào và đầu ra, để viết code tích hợp đúng ngay từ đầu. | Backend developer | Mất 2–3 tiếng nghiên cứu tài liệu mỗi module, khoảng 2 module/tháng (dựa trên tài liệu module dự án). |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi cần dùng lại cấu hình Docker/Nginx hoặc đoạn xử lý đã viết ở dự án trước, tôi muốn tìm thấy đúng bản đó ngay, để dùng lại mà không viết lại từ đầu. | Developer | Mất 15–20 phút mỗi lần tìm kiếm lại mã nguồn cũ, tần suất 3–5 lần/tuần (dựa trên lịch sử tìm kiếm code). |
| 5 | Pain từ người khác | Khi nhận mô tả API từ tôi, thành viên nhóm muốn nắm rõ định dạng và điều kiện ràng buộc ngay lần đầu, để không phải nhắn tin hỏi lại nhiều lần. | Thành viên nhóm (Frontend/Tester) | Bị hỏi lại 3–5 lần/tuần, mỗi lần giải thích lại tốn khoảng 5–10 phút chuyển đổi bối cảnh (context-switching) (dựa trên lịch sử chat nhóm dự án). |
| 6 | Tốn thời gian | Khi triển khai dịch vụ backend lên môi trường mới, tôi muốn biết ngay bản thân còn thiếu biến cấu hình nào, để ứng dụng khởi động thành công mà không bị crash ngầm. | Backend developer | Tần suất dựng môi trường mới khoảng 2 lần/tháng; mỗi lần thiếu biến cấu hình phải mất 15–20 phút rà soát lại file cấu hình (dựa trên lịch sử commit file config). |
| 7 | Pain từ người khác | Khi gặp sự cố hệ thống và cần thông báo cho tôi, thành viên nhóm muốn cung cấp đầy đủ thông tin log tại thời điểm lỗi, để vấn đề được khoanh vùng xử lý ngay thay vì mất thời gian trao đổi bổ sung. | Thành viên nhóm / Tester | Trong 10 báo lỗi gần nhất trên nhóm chat, có 7/10 trường hợp thiếu log chi tiết, khiến tôi mất thêm 5–10 phút mỗi lần để yêu cầu gửi lại thông tin (có log tin nhắn nhóm chứng minh). |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Không dùng AI để gợi ý thêm. Cả 7 problem đều tự scan từ trải nghiệm thật.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Debug lỗi runtime (ngoại lệ) từ file log (CP1 #2) | Tốn nhiều thời gian nhất cho cá nhân dev, xảy ra thường xuyên, có baseline rõ ràng. | Ranh giới tối ưu giữa việc dùng rule lọc log tự động và việc cần đến LLM phân tích nguyên nhân. |
| 2 | Lỗi thao tác cấu hình khi deploy lên môi trường chạy thử (CP1 #1) | Quy trình lặp lại hằng tuần, rủi ro cao nếu thao tác sót file cấu hình môi trường. | Liệu việc dùng Bash script hoặc CI/CD thuần túy đã giải quyết triệt để mà chưa cần đến AI không? |
| 3 | Báo lỗi thiếu log từ thành viên nhóm (CP1 #7) | Phản ánh trực tiếp pain point từ người khác (đồng đội/tester), có bằng chứng log chat thực tế. | Khó khăn trong việc ép đồng đội thay đổi thói quen cung cấp thông tin ban đầu. |

### Problem Card #1 — Debug lỗi runtime (ngoại lệ) từ file log

| Trường | Nội dung |
|---|---|
| Job Story | Khi gặp lỗi runtime (ngoại lệ) lúc chạy backend, tôi muốn truy ra đúng dòng gây lỗi từ file log, để không phải thử sửa mò nhiều lần. |
| Actor | Backend developer |
| Thời điểm / bối cảnh | Khi gặp lỗi runtime (ngoại lệ) lúc chạy backend, khoảng 3–4 lần/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Phát sinh ngoại lệ (1 ph) → 2. Mở terminal và file log hệ thống (2 ph) → 3. Dùng lệnh grep hoặc search tìm kiếm thủ công (10 ph) → 4. Đọc dải stack trace dài và nhiều thông tin nhiễu (20 ph) → 5. Khoanh vùng dòng code và sửa lỗi (10 ph). Tổng khoảng 43 phút/lần |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, đọc stack trace: 20 phút/lần, vì phải dò dải stack trace dài, chứa nhiều thông tin nhiễu để tìm ra nguyên nhân gốc rễ (root cause) |
| Impact (nếu không giải thì sao) | 30–60 phút/lần × 3–4 lần/tuần ≈ 1,5–4 giờ/tuần cho debug (số liệu CP1). Ngoài ra làm gián đoạn nặng nề mạch tư duy viết code, gây căng thẳng mệt mỏi cuối ngày |
| Success metric (baseline → target) | Baseline: bước 3–4 (tìm ra nguyên nhân) mất khoảng 30 phút/lần → target: dưới 10 phút/lần. Chỉ số phụ: số lần sửa thử trước khi sửa đúng (ghi trong tuần đầu làm baseline). Cách đo: tự ghi thời gian bước 3–4 và số lần sửa thử mỗi lần debug, trong 2 tuần pilot |
| Phương án không dùng AI | Dùng công cụ lọc log chuẩn hóa màu sắc hoặc câu lệnh tìm kiếm nâng cao (grep, awk) |
| Giả thuyết về AI (nếu có) | Workflow: Rule lọc bỏ frame thư viện và dòng log nhiễu trước, sau đó LLM tóm tắt stack trace và chỉ ra vị trí file/dòng code nghi gây lỗi dựa trên ngữ cảnh code hiện tại |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 43 phút/lần, 3–4 lần/tuần

[1 Phát sinh ngoại lệ: 1'] → [2 Mở terminal + file log: 2']
→ [3 grep / search thủ công: 10']
→ [4 Đọc stack trace dài, nhiều nhiễu: 20'] ← BOTTLENECK
→ [5 Khoanh vùng dòng code + sửa lỗi: 10']
```

### Problem Card #2 — Lỗi thao tác cấu hình khi deploy

| Trường | Nội dung |
|---|---|
| Job Story | Khi đưa bản cập nhật lên môi trường chạy thử vào cuối ngày, tôi muốn bản mới chạy đúng mà không sót hay sai bước cấu hình, để cuối ngày không phải ở lại sửa lỗi thao tác. |
| Actor | Developer trong nhóm |
| Thời điểm / bối cảnh | Cuối ngày, khi đưa bản cập nhật lên môi trường chạy thử, 3–4 lần/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Kiểm tra trạng thái Git và branch (2 ph) → 2. Chạy lệnh build source code (5 ph, máy tự chạy) → 3. Cập nhật file cấu hình môi trường .env thủ công (5 ph) → 4. Thực hiện lệnh deploy lên server qua SSH (5 ph) → 5. Kiểm tra log khởi động service (3 ph). Tổng khoảng 20 phút/lần, trong đó thao tác tay khoảng 15 phút. Khi sót biến cấu hình (khoảng 1 lần/tuần): thêm 20–30 phút dò lỗi và sửa lại |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, cập nhật .env thủ công: 5 phút/lần, nhưng thao tác thủ công dễ dẫn đến sót biến môi trường, gây chết service ngầm; mỗi lần sót (khoảng 1 lần/tuần) mất thêm 20–30 phút sửa lại |
| Impact (nếu không giải thì sao) | Deploy 10–15 phút/lần × 3–4 lần/tuần ≈ 30–60 phút/tuần, cộng 20–30 phút sửa lỗi cấu hình khoảng 1 lần/tuần → khoảng 50–90 phút/tuần (số liệu CP1). Ngoài ra có rủi ro hệ thống staging/production sập ngoài giờ làm việc, gây áp lực phải ở lại fix gấp |
| Success metric (baseline → target) | Baseline: lỗi thao tác cấu hình khoảng 1 lần/tuần, mỗi lần 20–30 phút sửa; thao tác tay 10–15 phút/lần (CP1) → target: 0 lỗi cấu hình trong 4 tuần, thời gian thao tác tay dưới 5 phút/lần. Cách đo: mỗi lần deploy ghi 1 dòng vào sổ deploy (mất bao lâu, có lỗi cấu hình không) trong 4 tuần |
| Phương án không dùng AI | Viết Bash script tự động hóa chuỗi lệnh deploy và kiểm tra file .env mẫu |
| Giả thuyết về AI (nếu có) | Không cần AI: script tự động thực hiện quy trình, kết hợp kiểm tra tự động xem file cấu hình hiện tại có khớp với các biến môi trường bắt buộc hay không trước khi chạy lệnh (Rule) |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 20 phút/lần (thao tác tay ~15 phút), 3–4 lần/tuần

[1 Kiểm tra Git + branch: 2'] → [2 Build source (máy tự chạy): 5']
→ [3 Cập nhật .env thủ công: 5'] ← BOTTLENECK
→ [4 Deploy lên server qua SSH: 5']
→ [5 Kiểm tra log khởi động service: 3']

Khi sót biến .env (~1 lần/tuần): service chết ngầm → dò lỗi + sửa: +20–30'
```

### Problem Card #3 — Báo lỗi thiếu log

| Trường | Nội dung |
|---|---|
| Job Story | Khi gặp sự cố, thành viên nhóm muốn báo lỗi thật nhanh mà vẫn đủ thông tin, để không phải quay lại gửi bổ sung. |
| Actor | Thành viên nhóm / Tester |
| Thời điểm / bối cảnh | Khi gặp sự cố hệ thống và báo lỗi qua nhóm chat |
| Quy trình hiện tại (3–7 bước) | 1. Phát sinh lỗi trên hệ thống (1 ph) → 2. Gửi thông báo ngắn gọn "Hệ thống lỗi rồi" lên chat (1 ph) → 3. Developer nhận tin và vào hỏi xin thông tin log chi tiết (2 ph) → 4. Tester/Thành viên đi tìm log và gửi lại (5 ph thao tác, nhưng phải chờ 10–30 ph mới nhận được) → 5. Developer mới bắt đầu tiến hành debug (15 ph). Tổng khoảng 24 phút thao tác, cộng 10–30 phút chờ |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, tester/thành viên đi tìm log và gửi lại: 5 phút thao tác nhưng phải chờ 10–30 phút, vì thông báo ban đầu không đính kèm sẵn thông tin kỹ thuật nên phải trao đổi vòng vo |
| Impact (nếu không giải thì sao) | 7–10 báo lỗi/tuần, 7/10 thiếu log → khoảng 5–7 báo lỗi thiếu log/tuần. Mỗi lần dev mất thêm 5–10 phút trao đổi (≈ 25–70 phút/tuần) và lỗi bị chậm xử lý thêm 10–30 phút chờ log (số liệu CP1). Ngoài ra gây bực dọc, giao tiếp kém hiệu quả giữa dev và tester/thành viên trong nhóm |
| Success metric (baseline → target) | Baseline: 7/10 báo lỗi thiếu log (CP1) → target: 0/10 báo lỗi thiếu log. "Đủ log" = có thời điểm, môi trường, thao tác gây lỗi và đoạn log. Cách đo: đếm trên log tin nhắn nhóm chat dự án |
| Phương án không dùng AI | Quy định template báo lỗi bắt buộc kèm theo khung nhập log trên kênh chat nhóm |
| Giả thuyết về AI (nếu có) | Không cần AI: thử template báo lỗi trước (No AI); nếu vẫn thiếu log thì chuyển sang giao diện báo lỗi tự động thu thập log hệ thống tại thời điểm bấm nút "Báo lỗi" và gửi kèm thông báo (Rule) |
| Cảm nhận nhanh | No AI |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 24 phút thao tác + 10–30 phút chờ/lần, 7–10 báo lỗi/tuần (7/10 thiếu log)

[1 Phát sinh lỗi: 1'] → [2 Gửi "Hệ thống lỗi rồi" lên chat: 1']
→ [3 Dev hỏi xin log chi tiết: 2']
→ [4 Tester/thành viên đi tìm log + gửi lại: 5', chờ 10–30'] ← BOTTLENECK
→ [5 Dev bắt đầu debug: 15']
```

### Card muốn pitch nhất

- Card số: 1 — Debug lỗi runtime (ngoại lệ) từ file log
- Vì sao: Impact lớn nhất trong 3 card (1,5–4 giờ/tuần), và so sánh được đủ 4 mức No AI / Rule / Workflow / Agent.
- Câu hỏi muốn nhóm phản biện: Lọc stack trace bằng rule đã đủ chưa, hay thật sự cần AI phân tích nguyên nhân?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card 1: Job Story ghi "lỗi logic" nhưng quy trình lại xoay quanh ngoại lệ và stack trace; lỗi logic thường không sinh stack trace | Đồng ý | Đổi Job Story thành "lỗi runtime (ngoại lệ)", giữ nguyên quy trình vì lỗi tôi hay phải dò thực tế là ngoại lệ có stack trace |
| Card 1: Target "dưới 10 phút/lần" không khớp quy trình (riêng bước 1, 2, 5 đã 13 phút); metric chỉ đo tốc độ, chưa đo số lần "sửa mò" mà Job Story muốn tránh | Đồng ý | Đổi metric sang đo riêng bước tìm nguyên nhân (bước 3–4: 30 phút → dưới 10 phút/lần), thêm chỉ số số lần sửa thử trước khi đúng |
| Card 2: Các bước cộng lại 20 phút nhưng CP1 ghi 10–15 phút/lần; bottleneck ghi bước 4 (SSH) nhưng lý do lại là cập nhật .env (bước 3); quy trình thiếu nhánh lỗi 20–30 phút sửa | Đồng ý | Ghi rõ build 5 phút là máy tự chạy, thao tác tay khoảng 15 phút (khớp CP1); chuyển bottleneck sang bước 3; thêm nhánh "sót biến: +20–30 phút sửa" |
| Card 2: Git không ghi thời gian deploy hay lỗi cấu hình nên chưa đo được; target "deploy dưới 5 phút" trong khi riêng build đã 5 phút | Đồng ý | Đổi cách đo sang sổ ghi deploy trong 4 tuần; target là thời gian thao tác tay dưới 5 phút và 0 lỗi cấu hình trong 4 tuần |
| Cả 3 card ghi "Workflow": card 2 (script kiểm tra .env) và card 3 (nút tự gom log) không có bước AI nào nên là Rule; card 1 chưa cho thấy Rule (lọc bỏ frame thư viện) là không đủ | Đồng ý | Card 2 đổi sang Rule; card 3 đổi sang No AI (thử template trước, chuyển sang Rule nếu không đủ); card 1 giữ Workflow nhưng ghi rõ Rule lọc nhiễu trước, LLM chỉ phân tích nguyên nhân |
| Card 3: Job Story nói đồng đội "muốn cung cấp đầy đủ log" nhưng phần còn chưa chắc lại nói khó ép họ đổi thói quen | Đồng ý | Viết lại Job Story theo pain thật: đồng đội thấy mất công, muốn báo lỗi nhanh mà vẫn đủ thông tin |
| Card 3: "5 phút" ở bước 4 là thời gian thao tác hay thời gian chờ; target 0/10 chưa định nghĩa thế nào là "đủ log" | Đồng ý | Bước 4 ghi thêm thời gian chờ thực tế 10–30 phút; định nghĩa "đủ log" = có thời điểm, môi trường, thao tác gây lỗi và đoạn log |

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
| CP1 Scan | Rà bảng scan theo rubric C1 và chuyển sang bảng Markdown, sau khi đã tự scan xong (không dùng để nghĩ ra problem) | Giúp định dạng bảng Markdown nhanh chóng, rà cấu trúc Job Story và chỉ ra các dòng thiếu số liệu (dòng 1 chưa rõ 10–15 phút đo gì, dòng 6 thiếu tần suất, dòng 7 thiếu mẫu số cho 70%). | AI khuyên dòng 2 chỉ giữ một tình huống nhưng không lưu ý tình huống nào khớp với quy trình đọc stack trace của tôi; tôi chọn "lỗi logic" và chỗ lệch này đến CP2 mới lộ ra. | Tự tay điều chỉnh lại các con số, bổ sung nguồn chứng cứ thực tế (Git commit, log chat) và sửa lại dòng 5, 7 theo góc nhìn của đồng đội. |
| CP2 Problem Card | Nội dung 3 card tôi tự làm; dùng AI đóng vai PM hoài nghi để phản biện card (yêu cầu của CP2) và chuyển nội dung sang bảng Markdown | Đóng vai PM hoài nghi rất sắc bén, chỉ ra được các điểm mù về logic giữa "lỗi logic" và "stack trace", vạch ra lỗi mâu thuẫn số phút giữa CP1 và CP2, và chỉ ra card 2, 3 bị ghi nhầm "Workflow" dù không có bước AI nào. | AI khuyên card 3 chọn No AI (template báo lỗi) trước khi biết pain thật là đồng đội thấy mất công; template bắt điền thêm thông tin có thể làm họ ngại hơn. | Sửa lại hoàn toàn nhãn mức AI (Card 2 thành Rule, Card 3 thành No AI), điều chỉnh lại quy trình đo lường thời gian debug bước 3-4 và bổ sung các nhánh phụ cho Card 2; card 3 giữ template nhưng ghi phương án dự phòng chuyển sang nút tự gom log (Rule) nếu template không đủ. |
| CP4 Research | | | | |
| CP5 Quy trình | Chuyển quy trình hiện tại và tương lai (theo nguyên tắc thiết kế nhóm rút ra ở CP4) sang sơ đồ Mermaid và tính bảng before/after | | | |
| CP5–6 Problem Statement | Nhờ AI phản biện Problem Statement v0: AI chỉ ra 4 lỗ hổng (Actor, baseline/target, Boundary, phương án quay về) kèm phương án sửa, nhóm tự chọn cách sửa | | | |
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
