# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Dương Thanh Bình
- MSSV: 2A202603531
- Email trường (không bắt buộc, repo có thể để public): 26ai.binhdt2@vinuni.edu.vn
- Tên nhóm: TenNhom
- Link repo nhóm: https://github.com/trinhcongduc112/K5-L3A-DAY02-TenNhom-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi vừa sửa xong một phần giao diện Vue và cần chạy thử trên WAMP, tôi muốn thay đổi hiện ra đúng chỗ ngay, để không mất công build, copy file và restart Apache mỗi lần | Tôi (dev solo) | Mỗi lần sửa phải chạy 3 bước thủ công; ~5–10 phút/lần, ~10 lần/tuần (cần bấm giờ lại) |
| 2 | Lặp lại | Khi vừa seed dữ liệu xong và chuẩn bị demo đồ án, tôi muốn hệ thống ở trạng thái sẵn sàng, để không quên các bước thủ công làm demo trống hoặc chậm | Tôi, hội đồng chấm | ≥2 bước thủ công dễ quên (`recommendation:build-similarity`, `optimize`); từng có lần tải trang 1,2s do cấu hình trùng, sau sửa còn ~149ms |
| 3 | Tốn thời gian | Khi viết lại các chương báo cáo đồ án, tôi muốn trình bày quyết định kiến trúc và lý do, để báo cáo đọc như phân tích chứ không như hướng dẫn từng bước | Tôi, giảng viên hướng dẫn, hội đồng | 4 chương phải rà lại; ~2–3 giờ/chương (cần đo) |
| 4 | Tốn thời gian | Khi review bộ sơ đồ sequence PlantUML, tôi muốn biết sơ đồ nào sai logic hoặc lỗi mã hóa, để không nộp sơ đồ mâu thuẫn với code | Tôi, người đọc báo cáo | ≥10 nhóm chức năng có sơ đồ; 2 đợt review tìm ra ≥4 loại lỗi (UTF-8, thiếu bước query DB, thiếu trạng thái Refunded, luồng auth không nhất quán) |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi viết phần quy trình Agile Scrum cho báo cáo, tôi muốn thấy mỗi sprint đã làm gì, để mô tả đúng thực tế thay vì nhớ mơ hồ | Tôi | Phải dựng 6 sprint (Sprint 0–5, tháng 4 đến cuối tháng 7) từ lịch sử commit git, đọc lại hàng trăm commit |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi ứng tuyển các vai trò khác nhau (Fullstack, QA/Tester, BA), tôi muốn CV nhấn đúng dự án liên quan từng vai trò, để nhà tuyển dụng thấy mình phù hợp | Tôi | 3 vai trò = 3 bản CV; 5 repo GitHub và các project Java chưa được đưa vào CV; ~1–2 giờ/bản (cần đo) |
| 7 | Tốn thời gian | Khi có lịch phỏng vấn cho vị trí mới (vd. Intern Tester), tôi muốn biết cần ôn gì theo mô tả công việc, để không ôn lan man | Tôi | Mỗi buổi phải tự soạn một tài liệu ôn riêng; ~3–4 giờ/buổi (cần đo) |
| 8 | Tốn thời gian | Khi chạy phần LLM trong lab, tôi muốn có một model gọi được ngay, để không mất thời gian thử từng provider/model | Tôi, bạn cùng lớp | Gemini nhiều model không chạy → đổi sang Groq (gpt-oss-20b/120b); ≥2 provider phải thử, ~30–60 phút (cần đo) |
| 9 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị bài kiểm tra đầu vào AI (90 phút, 4 module A–D, 100 điểm), tôi muốn biết module nào mình yếu và cần ôn gì, để dồn thời gian đúng chỗ | Tôi | 4 module, tài liệu ôn từ nhiều nguồn rời rạc; chưa có bảng điểm yếu theo module |
| 10 | Pain từ người khác | Khi khách hỏi chatbot về cấu hình và giá bằng nhiều cách viết khác nhau ("16GB RAM" / "RAM 16", "15 triệu" / "15tr"), khách muốn nhận đúng sản phẩm, để không phải hỏi lại hoặc bỏ đi | Khách hàng, chủ shop | ≥4 lỗi phải sửa trong parser và hội thoại (`recentHistory`, `detectRam`, `extractOrderId`, thứ tự FAQ); 25 test case viết thêm để kiểm |
| 11 | Lặp lại | Khi nộp báo cáo lab (.md) lúc gần deadline, tôi muốn biết mình còn thiếu mục nào so với yêu cầu, để không bị trừ điểm vì sai cấu trúc | Tôi, bạn cùng lớp | 2 báo cáo cá nhân đã làm (Day 01, Day 02), mỗi bài có cấu trúc bắt buộc; ~20 phút/bài tự đối chiếu (cần đo) |

**Phân bố lăng kính:** Lặp lại (#1, #2, #11), Tốn thời gian (#3, #4, #7, #8), Cần đọc/tổng hợp (#5, #6, #9), Pain từ người khác (#10).

**AI gợi ý thêm:** *(điền sau khi dùng prompt)*
- Ý AI gợi ý và giữ lại: ...
- Ý AI gợi ý nhưng bỏ (quá rộng / không có quy trình thật / chứa giải pháp): ...

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | CV theo vai trò (#6) | Lặp lại mỗi lần ứng tuyển, quy trình rõ, bottleneck là một bước, đo được bằng phút | Thế nào là bản CV "đủ tốt"? |
| 2 | Review sơ đồ PlantUML (#4) | Đã có bằng chứng thật (2 đợt review, ≥4 loại lỗi), có phần kiểm tra bằng rule được | Đối chiếu sơ đồ với code có ngoài sức một buổi lab không? |
| 3 | Kiểm báo cáo lab trước khi nộp (#11) | Quy trình ngắn, rõ, kiểm được bằng checklist; làm nhanh trong lab | Impact nhỏ (~20 phút/bài), có thể No AI là đủ |

**Vì sao chưa chọn các ý khác:**
- **#3 Viết lại chương báo cáo:** thời gian lớn nhưng "viết hay" khó đo, và sắp tới hạn bảo vệ nên khó thử quy trình mới.
- **#5 Dựng sprint từ git:** làm một lần rồi xong, không lặp lại.
- **#1, #2 Deploy và seed:** là việc dev, giải bằng script rule là đủ, chưa có chỗ nào cần AI.
- **#7, #9 Ôn phỏng vấn / ôn đầu vào:** dữ liệu và baseline còn mỏng.
- **#8, #10:** #8 là sự cố một lần của lab, #10 là bài toán xây chatbot, không phải một quy trình có bottleneck rõ.

### Problem Card #1 — CV theo vai trò

| Trường | Nội dung |
|---|---|
| Job Story | Khi ứng tuyển các vai trò khác nhau (Fullstack, QA/Tester, BA), tôi muốn CV nhấn đúng dự án liên quan từng vai trò, để nhà tuyển dụng thấy mình phù hợp |
| Actor | Sinh viên CS năm cuối, đang ứng tuyển nhiều vai trò cùng lúc |
| Thời điểm / bối cảnh | Mỗi khi có JD mới, thường vào buổi tối trước hạn nộp |
| Quy trình hiện tại | 1. Đọc JD · 2. Chọn dự án liên quan trong 5+ repo · 3. Đọc lại repo/README để nhớ điểm nổi bật và số liệu · 4. Viết lại bullet theo vai trò · 5. Sắp xếp và format · 6. Tự review rồi gửi |
| Bottleneck | Bước 3, đọc lại repo để rút kết quả và số liệu: ~30 phút/bản, dự án cũ nên quên chi tiết |
| Impact | ~95 phút/bản CV; 3 vai trò nên ≥3 bản/đợt ứng tuyển; nhiều project Java/Python chưa lên CV |
| Success metric | Tổng thời gian từ ~95 phút xuống dưới 40 phút; mọi con số trong CV truy được về repo |
| Phương án không dùng AI | Một "CV gốc" liệt kê mọi dự án kèm số liệu, mỗi lần chỉ chọn và cắt. Giảm bước 3 nhưng không giúp viết bullet theo từng JD |
| Giả thuyết về AI | AI soạn nháp bullet từ README/số liệu đã gom sẵn + JD; mình chọn, sửa và duyệt |
| Cảm nhận nhanh | Workflow |

```text
HIỆN TẠI — ~95 phút/bản CV (ước lượng)

[1 Đọc JD: 10'] → [2 Chọn project: 15'] → [3 Đọc lại repo, rút số liệu: 30'] ← BOTTLENECK
→ [4 Viết bullet: 20'] → [5 Format: 10'] → [6 Review + gửi: 10']
```

### Problem Card #2 — Review sơ đồ PlantUML

| Trường | Nội dung |
|---|---|
| Job Story | Khi review bộ sơ đồ sequence PlantUML, tôi muốn biết sơ đồ nào sai logic hoặc lỗi mã hóa, để không nộp sơ đồ mâu thuẫn với code |
| Actor | Sinh viên làm đồ án cá nhân, tự viết và tự review sơ đồ |
| Thời điểm / bối cảnh | Sau mỗi đợt thêm hoặc sửa tính năng, trước khi chốt báo cáo |
| Quy trình hiện tại | 1. Mở sơ đồ và code tương ứng · 2. Đối chiếu từng message với controller/service · 3. Kiểm lỗi UTF-8 và render · 4. Ghi danh sách lỗi · 5. Sửa file .puml · 6. Render lại để kiểm |
| Bottleneck | Bước 2, đối chiếu từng bước trong sơ đồ với code: ~25 phút/đợt, dễ sót bước truy vấn DB hoặc trạng thái |
| Impact | ~60 phút/đợt; 2 đợt đã làm; mỗi đợt tìm ra ≥4 loại lỗi |
| Success metric | 60 → dưới 25 phút/đợt; lỗi còn sót sau review = 0 ở lần kiểm cuối; số cảnh báo sai không làm mất thêm thời gian |
| Phương án không dùng AI | Checklist lỗi hay gặp + script quét lỗi UTF-8. Giải quyết lỗi mã hóa, không giải quyết lỗi logic |
| Giả thuyết về AI | Script rule bắt lỗi mã hóa; AI đối chiếu .puml với code và liệt kê chỗ không khớp; mình duyệt |
| Cảm nhận nhanh | Rule cho lỗi mã hóa, Workflow cho lỗi logic |

```text
HIỆN TẠI — ~60 phút/đợt review (ước lượng)

[1 Mở sơ đồ + code: 10'] → [2 Đối chiếu với code: 25'] ← BOTTLENECK
→ [3 Kiểm UTF-8/render: 5'] → [4 Ghi lỗi: 5'] → [5 Sửa .puml: 10'] → [6 Render lại: 5']
```

### Problem Card #3 — Kiểm báo cáo lab trước khi nộp

| Trường | Nội dung |
|---|---|
| Job Story | Khi nộp báo cáo lab (.md) lúc gần deadline, tôi muốn biết mình còn thiếu mục nào so với yêu cầu, để không bị trừ điểm vì sai cấu trúc |
| Actor | Sinh viên làm lab cá nhân, nộp báo cáo .md theo mẫu |
| Thời điểm / bối cảnh | Buổi tối cuối ngày, trước hạn nộp |
| Quy trình hiện tại | 1. Đọc lại yêu cầu của đề · 2. Lập checklist mục cần có · 3. Đối chiếu từng mục với báo cáo · 4. Đối chiếu số liệu và tham số với output notebook · 5. Sửa chỗ thiếu rồi nộp |
| Bottleneck | Bước 4, đối chiếu số liệu (SEED, kết quả, tham số của challenge) trong báo cáo với output notebook: ~7 phút/bài, dễ nhầm khi chạy lại notebook |
| Impact | ~20 phút/bài; 2 bài đã làm, các lab sau còn lặp lại |
| Success metric | 20 → dưới 5 phút/bài; số mục thiếu phát hiện sau khi nộp = 0 |
| Phương án không dùng AI | Checklist cố định theo đề, tự tick. Có thể đã đủ |
| Giả thuyết về AI | Chưa thấy chỗ nào bắt buộc phải dùng AI; script kiểm tiêu đề mục và số liệu có thể đủ |
| Cảm nhận nhanh | No AI hoặc Rule |

```text
HIỆN TẠI — ~20 phút/bài (ước lượng)

[1 Đọc yêu cầu: 3'] → [2 Lập checklist: 3'] → [3 Đối chiếu mục: 4']
→ [4 Đối chiếu số liệu với notebook: 7'] ← BOTTLENECK → [5 Sửa + nộp: 3']
```

### Bản pitch nhanh (trình bày với nhóm)

```text
┌──────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #1                                              │
│ Khi ứng tuyển vai trò khác nhau, tôi muốn CV nhấn đúng dự án │
│ liên quan, để nhà tuyển dụng thấy mình phù hợp               │
│ Ai chịu ảnh hưởng? Sinh viên CS năm cuối đang tìm việc       │
│ Quy trình: 1.Đọc JD → 2.Chọn project → 3.Đọc lại repo →      │
│            4.Viết bullet → 5.Format → 6.Review               │
│ Bước nghẽn: Đọc lại repo rút số liệu (~30 phút/lần)          │
│ Đo thành công: từ ~95 phút xuống dưới 40 phút                │
│ Cảm nhận nhanh: □ No AI □ Rule ■ Workflow                    │
│                 □ Agent □ Chưa biết                          │
└──────────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #2                                              │
│ Khi review sơ đồ PlantUML, tôi muốn biết sơ đồ nào sai       │
│ logic hoặc lỗi mã hóa, để không nộp sơ đồ lệch với code      │
│ Ai chịu ảnh hưởng? Người làm đồ án, người đọc báo cáo        │
│ Quy trình: 1.Mở sơ đồ+code → 2.Đối chiếu → 3.Kiểm UTF-8 →   │
│            4.Ghi lỗi → 5.Sửa → 6.Render lại                 │
│ Bước nghẽn: Đối chiếu sơ đồ với code (~25 phút/đợt)          │
│ Đo thành công: từ ~60 phút xuống dưới 25 phút/đợt            │
│ Cảm nhận nhanh: □ No AI ■ Rule ■ Workflow                    │
│                 □ Agent □ Chưa biết                          │
└──────────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #3                                              │
│ Khi nộp báo cáo lab lúc gần deadline, tôi muốn biết còn      │
│ thiếu mục nào, để không bị trừ điểm vì sai cấu trúc          │
│ Ai chịu ảnh hưởng? Sinh viên làm lab cá nhân                 │
│ Quy trình: 1.Đọc đề → 2.Lập checklist → 3.Đối chiếu mục →    │
│            4.Đối chiếu số liệu → 5.Sửa + nộp                 │
│ Bước nghẽn: Đối chiếu số liệu với notebook (~7 phút/bài)     │
│ Đo thành công: từ ~20 phút xuống dưới 5 phút/bài             │
│ Cảm nhận nhanh: ■ No AI ■ Rule □ Workflow                    │
│                 □ Agent □ Chưa biết                          │
└──────────────────────────────────────────────────────────────┘
```

### AI phản biện Card #1

Prompt đã điền sẵn, bạn dán vào AI và dán card #1 ở trên:

```text
Đây là Problem Card của tôi:
[dán card #1]

Đóng vai một product manager hoài nghi và phản biện:
1. Actor có đủ cụ thể không?
2. Quy trình có thật không, hay là quy trình tôi tưởng tượng?
3. Bottleneck có phải một bước cụ thể không?
4. Metric có đo được không?
5. Sửa quy trình hoặc dùng rule đã đủ chưa?
6. Tôi có đang nhảy sang AI quá sớm không?
Trả lời ngắn, chỉ nói điểm yếu.
```

Điểm yếu mình tự thấy ở card #1 (thay bằng câu trả lời thật của AI khi bạn chạy):

| Điểm yếu | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline ~95 phút là ước lượng, chưa bấm giờ | *(điền)* | *(vd. bấm giờ 2 lần làm CV tới, ghi lại)* |
| Có thể một "CV gốc" kèm số liệu đã đủ, không cần AI | *(điền)* | *(vd. giữ làm phương án No AI, so sánh ở CP6)* |
| Chưa rõ thế nào là CV "đủ tốt" ngoài việc nhanh hơn | *(điền)* | *(vd. thêm metric: không số liệu bịa, bullet khớp JD)* |
| Thiếu bằng chứng nhà tuyển dụng đọc CV kỹ đến mức này | *(điền)* | *(đưa vào giả định cần kiểm ở CP4)* |

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
