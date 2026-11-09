# Báo cáo cá nhân — 2A202603405_NguyenNgocToan

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Ngọc Toàn
- MSSV: 2A202603405
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: tido
- Link repo nhóm: https://github.com/datnguyen101004/K5-L3A-DAY02-tido-DiscoveryProblemFraming/tree/main

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

> Số liệu là ước lượng của tôi theo trí nhớ (chưa bấm giờ). Sẽ đo lại khi kiểm chứng ở CP4.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Pain từ người khác · Tốn thời gian | Khi tôi hoặc một thành viên mới bắt đầu làm một project mới, tôi muốn chạy được project ở máy local ngay trong ngày đầu, để bắt tay vào task sớm mà không phải hỏi đi hỏi lại người cũ | SWE mới vào team hoặc đổi project; người cũ bị hỏi | Lần vào project gần nhất: khoảng nửa ngày (~4 giờ) từ lúc clone tới khi chạy được; kẹt nhiều nhất ở cấu hình biến môi trường/config (~2 giờ), phải hỏi người cũ giá trị config |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi cần biết vì sao team chọn thiết kế hoặc cấu hình hiện tại, hoặc cần đúng bản tài liệu mới nhất, tôi muốn tìm ra nhanh trong chat, Drive và Jira, để không phải hỏi lại hoặc làm theo bản cũ | SWE; đồng nghiệp bị hỏi lại | 5–15 phút/lần, 1–2 lần/tuần (khoảng 5–30 phút/tuần); phải tìm ở 3 nơi: chat (Slack/Teams/Zalo), Google Drive/OneDrive, Jira/email |
| 3 | Lặp lại · Cần đọc, tổng hợp nhiều thông tin | Khi deadline bài tập và lab được thông báo rải rác trên LMS, email và Discord/Zalo, tôi muốn thấy mọi hạn nộp của tuần ở một chỗ, để không trễ hạn hoặc phải làm gấp sát giờ | Tôi và các bạn cùng lớp | Phải dò 3 nguồn; 0 lần trễ hoặc suýt trễ trong 1 tháng qua (**tín hiệu phản bác**: pain hiện tại nhỏ) |
| 4 | Lặp lại · Pain từ người khác | Khi đồng nghiệp mới, tester, PO hoặc khách hàng hỏi về cách dùng, cấu hình hay quy trình của phần hệ thống tôi phụ trách, tôi muốn họ tự tìm được câu trả lời đúng, để tôi không bị cắt ngang khi đang code | Tôi; người hỏi phải chờ câu trả lời | 6–10 câu/tuần, nhiều nhất từ Tester/QA; 25–50% là câu tôi đã từng trả lời; 5–15 phút/câu (khoảng 30–150 phút/tuần) |
| 5 | Lặp lại · Tốn thời gian | Khi tôi mở PR cho một task đã xong, tôi muốn có người review sớm, để merge kịp sprint và không phải chuyển qua lại giữa task cũ và task mới | Tôi, reviewer, tiến độ sprint | Thường có review đầu tiên trong vòng 4 giờ (**tín hiệu phản bác**: team review nhanh, pain nhỏ) |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Cả 5 ý trên được chọn từ danh sách khoảng 15 vấn đề do tôi và AI (Claude) gợi ý theo 3 bối cảnh: học tập, văn phòng và Software Engineer. Tôi chỉ giữ những ý tôi đã trực tiếp gặp; số liệu ở cột "Dấu hiệu thật" là ước lượng của tôi.
- Bỏ ý "Tìm lại thông báo hoặc link cũ trong kênh chat lớp" vì trùng pattern với #2 (tìm lại thông tin cũ trong kênh chat). Thay bằng #5 "PR chờ review".
- Sau khi ước lượng số liệu, #3 (0 lần trễ) và #5 (review dưới 4 giờ) cho thấy pain nhỏ, nên không đưa vào top 3.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tester hỏi lặp lại (#4) | Pain lớn nhất trong 5 ý (30–150 phút/tuần), lặp lại hằng tuần, 25–50% câu là câu cũ; có độ mơ hồ nên so sánh được cả 4 mức can thiệp | Tỉ lệ câu trùng mới là ước lượng; câu hỏi mới (50–75%) FAQ không giải được |
| 2 | Tìm tài liệu hoặc quyết định cũ (#2) | Phải tìm ở 3 nơi (chat, Drive, Jira); nhiều người trong ngành gặp nên dễ kiểm chứng | Impact nhỏ (5–30 phút/tuần); có thể chỉ cần quy ước lưu tài liệu |
| 3 | Setup môi trường project mới (#1) | Bottleneck rất cụ thể (config ~2 giờ); quy trình vẽ được ngay | Tần suất thấp (chỉ khi vào project mới), nên tổng impact phụ thuộc số người mới mỗi năm |

### Problem Card #1 — Tester hỏi lặp lại

| Trường | Nội dung |
|---|---|
| Job Story | Khi Tester/QA hỏi về luồng nghiệp vụ, dữ liệu test hoặc cấu hình của phần hệ thống tôi phụ trách, tôi muốn họ tự tìm được câu trả lời đúng cho những câu đã từng được hỏi, để tôi không bị cắt ngang khi đang code |
| Actor | Software Engineer phụ trách một module, người hay được Tester/QA hỏi (đã thu hẹp từ 4 nhóm người hỏi xuống nhóm hỏi nhiều nhất) |
| Thời điểm / bối cảnh | Trong giờ làm, câu hỏi đến qua chat vào bất kỳ lúc nào, thường khi tester đang test tính năng của tôi |
| Quy trình hiện tại (3–7 bước) | 1. Nhận câu hỏi qua chat · 2. Dừng việc đang code, đọc câu hỏi · 3. Nhớ lại hoặc tra lại code/tài liệu · 4. Soạn câu trả lời · 5. Quay lại task, lấy lại mạch làm việc |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, tra lại code/tài liệu để trả lời đúng: khoảng 5 phút/câu (trên tổng khoảng 12 phút/câu) |
| Impact (nếu không giải thì sao) | 6–10 câu/tuần × khoảng 12 phút ≈ 70–120 phút/tuần bị cắt ngang; trong đó 25–50% là câu cũ (khoảng 2–5 câu, 25–60 phút/tuần) |
| Success metric (baseline → target) | Số câu hỏi lặp lại từ 2–5 câu/tuần xuống còn tối đa 1 câu/tuần. Đo bằng đếm tin nhắn và đánh dấu câu trùng trong 2 tuần trước và 2 tuần sau thay đổi |
| Phương án không dùng AI | Viết FAQ cho các câu tester hay hỏi lại, ghim trong kênh team; quy ước tester hỏi trong kênh chung thay vì nhắn riêng, để câu trả lời cũ tìm lại được |
| Giả thuyết về AI (nếu có) | Trả lời câu hỏi của tester dựa trên FAQ và tài liệu, có dẫn nguồn; câu nào không có trong tài liệu thì chuyển cho tôi |
| Cảm nhận nhanh | Rule (FAQ) trước; Workflow nếu câu hỏi quá đa dạng |

Quy trình nháp hiện tại (khoảng 12 phút/câu):

```text
[1 Nhận câu hỏi: 1'] → [2 Dừng việc, đọc câu hỏi: 1'] → [3 Tra code/tài liệu: 5'] ← BOTTLENECK
→ [4 Soạn trả lời: 2'] → [5 Quay lại task, lấy lại mạch: 3']
```

### Problem Card #2 — Tìm tài liệu hoặc quyết định cũ

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần biết vì sao team chọn thiết kế hoặc cấu hình hiện tại, hoặc cần đúng bản tài liệu mới nhất, tôi muốn tìm ra nhanh trong chat, Drive và Jira, để không phải hỏi lại hoặc làm theo bản cũ |
| Actor | Software Engineer cần tra lại quyết định thiết kế, cấu hình hoặc bản spec mới nhất |
| Thời điểm / bối cảnh | Khi bắt đầu task chạm vào phần code cũ, hoặc khi người khác hỏi "vì sao hệ thống làm vậy" |
| Quy trình hiện tại (3–7 bước) | 1. Nhớ mơ hồ, đoán nơi lưu · 2. Tìm từ khóa trong chat · 3. Lục Drive/Jira, so phiên bản · 4. Hỏi đồng nghiệp nếu không thấy · 5. Xác nhận đúng bản mới nhất |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, lục Drive/Jira và so phiên bản: khoảng 5 phút/lần (trên tổng khoảng 12 phút/lần) |
| Impact (nếu không giải thì sao) | 1–2 lần/tuần × khoảng 12 phút ≈ 12–24 phút/tuần; rủi ro làm theo spec hoặc cấu hình cũ |
| Success metric (baseline → target) | Thời gian tìm từ 5–15 phút/lần xuống dưới 5 phút/lần. Đo bằng ghi lại mỗi lần tìm trong 2 tuần |
| Phương án không dùng AI | Quy ước gắn link tài liệu chính vào ticket Jira; ghi quyết định thiết kế ngắn (ADR) ngay trong repo; ghim link spec mới nhất trong kênh team |
| Giả thuyết về AI (nếu có) | Tìm chung trên chat, Drive và Jira rồi tóm tắt kèm link nguồn. Chưa chắc cần, vì tần suất thấp |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại (khoảng 12 phút/lần):

```text
[1 Nhớ mơ hồ, đoán nơi lưu: 1'] → [2 Tìm từ khóa trong chat: 3'] → [3 Lục Drive/Jira, so phiên bản: 5'] ← BOTTLENECK
→ [4 Hỏi đồng nghiệp nếu không thấy: 2'] → [5 Xác nhận đúng bản mới nhất: 1']
```

### Problem Card #3 — Setup môi trường project mới

| Trường | Nội dung |
|---|---|
| Job Story | Khi tôi hoặc một thành viên mới bắt đầu làm một project mới, tôi muốn chạy được project ở máy local ngay trong ngày đầu, để bắt tay vào task sớm mà không phải hỏi đi hỏi lại người cũ |
| Actor | Software Engineer mới vào team hoặc chuyển sang repo khác |
| Thời điểm / bối cảnh | Ngày đầu vào project; lần gần nhất mất khoảng nửa ngày |
| Quy trình hiện tại (3–7 bước) | 1. Clone repo · 2. Đọc README · 3. Cài runtime và dependency · 4. Cấu hình biến môi trường/config · 5. Hỏi người cũ giá trị config · 6. Chạy được app và test |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, cấu hình biến môi trường/config: khoảng 120 phút, vì không có sẵn giá trị config đúng |
| Impact (nếu không giải thì sao) | Khoảng 240 phút (nửa ngày) cho mỗi lần vào project mới; người cũ mất khoảng 40 phút hỗ trợ |
| Success metric (baseline → target) | Thời gian từ lúc clone tới khi chạy được: từ khoảng 240 phút xuống dưới 60 phút. Đo bằng bấm giờ ở lần setup tiếp theo |
| Phương án không dùng AI | File `.env.example` có giá trị mặc định; script setup một lệnh hoặc docker-compose/devcontainer; cập nhật README mỗi khi đổi config |
| Giả thuyết về AI (nếu có) | Không cần AI: các bước có đúng/sai rõ ràng, script và tài liệu đã đủ |
| Cảm nhận nhanh | No AI |

Quy trình nháp hiện tại (khoảng 240 phút):

```text
[1 Clone: 5'] → [2 Đọc README: 15'] → [3 Cài runtime + dependency: 40']
→ [4 Cấu hình env/config: 120'] ← BOTTLENECK → [5 Hỏi người cũ giá trị config: 40'] → [6 Chạy được app + test: 20']
```

### Card muốn pitch nhất

- Card số: 1 (Tester hỏi lặp lại)
- Vì sao: Pain lớn nhất trong 5 ý (30–150 phút/tuần), lặp lại hằng tuần, và đủ mơ hồ để nhóm so sánh No AI / Rule / Workflow / Agent.
- Câu hỏi muốn nhóm phản biện: Chỉ 25–50% câu hỏi là câu cũ. Một trang FAQ có đủ không, hay phần câu hỏi mới mới là phần tốn thời gian thật?

### AI đã phản biện card thế nào

AI (Claude) đóng vai "PM hoài nghi" theo prompt trong worksheet.

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card câu hỏi lặp lại: người hỏi gộp 4 nhóm (dev mới, tester, PO, khách hàng) có loại câu hỏi khác nhau; actor quá rộng | Đồng ý | Thu hẹp người hỏi xuống Tester/QA, nhóm hỏi nhiều nhất |
| Card câu hỏi lặp lại: bottleneck thật có thể là bước 5 (mất mạch sau khi bị cắt ngang), không phải bước 3 tra cứu | Không đồng ý | Giữ bước 3: theo ước lượng của tôi, tra cứu khoảng 5 phút, lấy lại mạch khoảng 3 phút |
| Card câu hỏi lặp lại: chưa biết bao nhiêu % câu hỏi là trùng lặp; nếu tỉ lệ thấp thì FAQ không giúp nhiều | Đồng ý | Ước lượng 25–50% câu trùng; đổi success metric sang đo số câu trùng, và đưa câu này thành câu hỏi phản biện cho nhóm |
| Card PR chờ review: bottleneck là thời gian chờ, nên giả thuyết "AI review sơ bộ" không đánh vào đúng bước nghẽn | Đồng ý | Khi ước lượng thấy PR thường được review dưới 4 giờ, pain nhỏ, nên bỏ card khỏi top 3 và thay bằng "Tìm tài liệu cũ" |
| Card setup: tần suất thấp, cần nhân với số lần vào project mới mới thấy impact thật | Đồng ý | Ghi rõ ở cột "Điều còn chưa chắc" của top 3; impact tính theo mỗi lần vào project |

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
| CP1 Scan | Gợi ý khoảng 15 vấn đề theo 3 bối cảnh (học tập, văn phòng, Software Engineer) và tìm số liệu ngành (Stack Overflow 2024, Atlassian DevEx 2025, Microsoft Work Trend Index 2023) | Gợi ý được vấn đề sát công việc SWE, kèm link nguồn | Có 1 số liệu (16% flaky test ở Google) AI không kiểm được nguồn gốc; 2 ý gợi ý (tìm tài liệu cũ, tìm thông báo lớp) trùng pattern | Thay ý "tìm thông báo lớp" bằng "PR chờ review"; không dùng số liệu chưa kiểm được |
| CP2 Problem Card | Soạn khung Problem Card và quy trình nháp; hỏi trắc nghiệm để tôi ước lượng số liệu; đề xuất cách chia số phút cho từng bước dựa trên tổng thời gian tôi ước lượng (tôi xác nhận khớp); đóng vai "PM hoài nghi" | Chỉ ra actor card #1 quá rộng; nhận ra PR được review dưới 4 giờ là tín hiệu phản bác | Ban đầu xếp "PR chờ review" vào top 3 trước khi có số liệu; khi có số liệu thì pain nhỏ | Thu hẹp actor card #1 xuống Tester/QA; thay card PR bằng "Tìm tài liệu cũ"; không đồng ý đổi bottleneck card #1 sang bước 5 |
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
