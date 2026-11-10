# Báo cáo cá nhân — 2A202603531_DuongThanhBinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Dương Thanh Bình
- MSSV: 2A202603531
- Email trường (không bắt buộc, repo có thể để public): 26ai.binhdt2@vinuni.edu.vn
- Tên nhóm: BDHH
- Link repo nhóm: https://github.com/trinhcongduc112/K5-L3A-DAY02-BDHH-DiscoveryProblemFraming
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

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | CV theo vai trò (#6) | Lặp lại mỗi lần ứng tuyển, quy trình rõ, bottleneck là một bước, đo được bằng phút | Thế nào là bản CV "đủ tốt"? |
| 2 | Review sơ đồ PlantUML (#4) | Đã có bằng chứng thật (2 đợt review, ≥4 loại lỗi), có phần kiểm tra bằng rule được | Đối chiếu sơ đồ với code có ngoài sức một buổi lab không? |
| 3 | Kiểm báo cáo lab trước khi nộp (#11) | Quy trình ngắn, rõ, kiểm được bằng checklist; làm nhanh trong lab | Impact nhỏ (~20 phút/bài), có thể No AI là đủ |

### Problem Card #1 — CV theo vai trò

| Trường | Nội dung |
|---|---|
| Job Story | Khi ứng tuyển các vai trò khác nhau (Fullstack, QA/Tester, BA), tôi muốn CV nhấn đúng dự án liên quan từng vai trò, để nhà tuyển dụng thấy mình phù hợp |
| Actor | Sinh viên CS năm cuối ứng tuyển đồng thời 2–3 vai trò (Fullstack, QA/Tester, BA), có 5+ repo đồ án cũ chưa đưa lên CV |
| Thời điểm / bối cảnh | Mỗi khi có JD mới, thường vào buổi tối trước hạn nộp |
| Quy trình hiện tại | 1. Đọc JD · 2. Chọn dự án liên quan trong 5+ repo · 3. Lục lại code/commit/README của repo cũ chưa tổng hợp để tìm bằng chứng kỹ thuật & số liệu · 4. Viết lại bullet theo góc nhìn của vai trò · 5. Sắp xếp và format · 6. Tự review rồi gửi |
| Bottleneck | Bước 3, lục lại code/commit/test của đồ án cũ để tìm bằng chứng kỹ thuật có thật (số API, số test case, cấu hình, benchmark): ~30 phút/bản vì đồ án cũ quên chi tiết và thiếu production metric sẵn có |
| Impact | ~95 phút/bản CV (ước lượng, cần bấm giờ 2 lần tới); 3 vai trò nên ≥3 bản/đợt ứng tuyển; nhiều project Java/Python chưa lên CV |
| Success metric | Thời gian từ ~95 phút xuống dưới 40 phút (đo bằng bấm giờ thực tế); 100% con số trong bullet truy được về repo (không bịa số) và khớp từ khóa kỹ năng của JD |
| Phương án không dùng AI | File Markdown **"Master Project Log"** ghi sẵn 5 bullet + số liệu ngay khi xong môn học (giải quyết dứt điểm bước 3 cho dự án mới, chỉ mất ~2 phút copy; nhưng chưa tự đổi góc nhìn bullet theo từng JD Dev/QA/BA) |
| Giả thuyết về AI | AI soạn nháp bullet theo góc nhìn từng JD từ "Master Project Log"/README đã gom sẵn; mình chọn, kiểm chứng số liệu và duyệt |
| Cảm nhận nhanh | No AI (Master Project Log) + Workflow nháp |

```text
HIỆN TẠI — ~95 phút/bản CV (ước lượng)

[1 Đọc JD: 10'] → [2 Chọn project: 15'] → [3 Đọc lại repo, rút số liệu: 30'] ← BOTTLENECK
→ [4 Viết bullet: 20'] → [5 Format: 10'] → [6 Review + gửi: 10']
```

### Problem Card #2 — Review sơ đồ PlantUML

| Trường | Nội dung |
|---|---|
| Job Story | Khi review bộ sơ đồ sequence PlantUML trước khi chốt báo cáo, tôi muốn biết sơ đồ nào sai mã hóa hoặc lệch luồng xử lý so với code, để không nộp sơ đồ mâu thuẫn với hệ thống thật |
| Actor | Sinh viên làm đồ án cá nhân (6 sprint), viết báo cáo dùng PlantUML (`.puml`) cho ≥10 nhóm chức năng và sửa code backend nhiều đợt trước khi nộp |
| Thời điểm / bối cảnh | Cuối mỗi đợt sửa lớn hoặc trước khi chốt báo cáo đồ án (2–3 đợt/học kỳ) |
| Quy trình hiện tại | 1. Mở file `.puml` và cặp Controller/Service tương ứng · 2. Đối chiếu từng message, truy vấn DB và trạng thái trả về với code · 3. Kiểm lỗi mã hóa UTF-8 và render thử · 4. Ghi danh sách lỗi · 5. Sửa file `.puml` · 6. Render lại để kiểm |
| Bottleneck | Bước 2, đối chiếu luồng gọi hàm, truy vấn DB và trạng thái giữa file `.puml` với Controller/Service: ~25 phút/đợt (~2.5 phút/sơ đồ × 10 sơ đồ), dễ sót khi phải mở 3–4 file code cho mỗi sơ đồ |
| Impact | ~60 phút/đợt (~6 phút/sơ đồ × 10 sơ đồ); 2 đợt đã làm tìm ra ≥4 loại lỗi (UTF-8, thiếu bước query DB, thiếu trạng thái `Refunded`, luồng auth không nhất quán); tần suất 2–3 đợt/kỳ |
| Success metric | Thời gian từ ~6 phút/sơ đồ (~60 phút/đợt) xuống dưới 2.5 phút/sơ đồ (<25 phút/đợt); 100% sơ đồ vượt qua checklist 4 lỗi cố định; số cảnh báo giả của công cụ không làm mất thêm thời gian kiểm lại |
| Phương án không dùng AI | Checklist cố định 4 loại lỗi hay gặp + script/linter quét lỗi UTF-8 và cú pháp `.puml` (Rule). Giải quyết triệt để lỗi mã hóa và nhắc đúng chỗ cần dò trong code |
| Giả thuyết về AI | Rule bắt lỗi UTF-8/cú pháp; nếu dùng AI thì chỉ đưa từng cặp (1 file `.puml` + 1 hàm Controller) vào Workflow để liệt kê bước lệch, người làm tự duyệt (nhưng cần cân nhắc ROI vì chỉ làm 2–3 đợt/kỳ) |
| Cảm nhận nhanh | Rule (cho lỗi UTF-8/cú pháp) + Checklist No AI (hoặc Workflow nhỏ cho từng cặp file) |

```text
HIỆN TẠI — ~60 phút/đợt review (10 sơ đồ, ước lượng)

[1 Mở sơ đồ + code: 10'] → [2 Đối chiếu với Controller/Service: 25'] ← BOTTLENECK
→ [3 Kiểm UTF-8/render: 5'] → [4 Ghi lỗi: 5'] → [5 Sửa .puml: 10'] → [6 Render lại: 5']
```

### Problem Card #3 — Kiểm báo cáo lab trước khi nộp

| Trường | Nội dung |
|---|---|
| Job Story | Khi nộp báo cáo lab (`.md`) lúc gần deadline, tôi muốn biết mình còn bỏ trống mục nào hoặc ghi lệch số liệu nào so với lần chạy notebook cuối, để không bị trừ điểm vì sai sót hình thức |
| Actor | Sinh viên học môn AI/ML làm báo cáo `.md` tách rời khỏi file `.ipynb`, hay chạy lại thực nghiệm sát giờ nộp làm thay đổi tham số/kết quả |
| Thời điểm / bối cảnh | Buổi tối cuối ngày, 15–30 phút trước hạn nộp bài lab |
| Quy trình hiện tại | 1. Đọc lại yêu cầu đề và cấu trúc mẫu `.md` · 2. Rà các mục/bảng trong file `.md` xem còn ô nào trống · 3. Mở file `.ipynb` đối chiếu từng số liệu (`SEED`, tham số, kết quả) với con số đã gõ trong `.md` · 4. Sửa chỗ thiếu/lệch rồi commit nộp |
| Bottleneck | Bước 3, đối chiếu thủ công số liệu (`SEED`, kết quả, tham số challenge) giữa báo cáo `.md` và output cell của `.ipynb`: ~7 phút/bài (micro-pain), dễ sót khi chạy lại cell notebook vào phút chót mà quên copy lại sang `.md` |
| Impact | ~20 phút/bài; 2 bài đã làm (Day 01, Day 02), lặp lại ở các lab sau; tổng thời gian mất mỗi lần không lớn nhưng dễ mất điểm đáng tiếc |
| Success metric | Thời gian rà soát từ ~20 phút xuống dưới 5 phút/bài; 0 ô placeholder (`*(điền)*`) bị bỏ trống và 0 số liệu trong `.md` lệch với output `.ipynb` khi nộp |
| Phương án không dùng AI | Sửa quy trình: chốt chạy xong toàn bộ `.ipynb` rồi mới điền `.md` + dùng checklist cố định trước khi `git commit`. Đủ giải quyết phần lớn vấn đề mà không tốn công xây tool |
| Giả thuyết về AI | **Không dùng AI** (bài toán kiểm tra đúng/sai tường minh, dùng LLM vừa chậm vừa có rủi ro đọc sót số). Nếu tự động hóa chỉ cần 1 script Rule nhỏ quét các mục trống hoặc regex kiểm placeholder |
| Cảm nhận nhanh | No AI hoặc Rule (không cần AI) |

```text
HIỆN TẠI — ~20 phút/bài (ước lượng)

[1 Đọc lại yêu cầu đề: 3'] → [2 Rà mục trống trong .md: 7']
→ [3 Đối chiếu số liệu với output .ipynb: 7'] ← BOTTLENECK → [4 Sửa + nộp: 3']
```


#### Card muốn pitch nhất

- **Card số:** Card #2 — Review bộ sơ đồ sequence PlantUML (`.puml`) đối chiếu với code backend.
- **Vì sao:**
  1. **Có bằng chứng thật đã xảy ra (hơn hẳn Card #1):** Sau khi AI phản biện, mình nhận ra Card #1 (CV theo vai trò) chưa bấm giờ thực tế và có thể giải quyết phần lớn bằng 1 file *"Master Project Log"* (No AI). Ngược lại, Card #2 đã trải qua **2 đợt review thật** trên ≥10 nhóm chức năng của đồ án (6 sprint), bắt được **≥4 loại lỗi cụ thể** (lỗi mã hóa UTF-8, thiếu bước query DB, thiếu trạng thái `Refunded`, luồng auth không nhất quán).
  2. **Tách bạch rõ ranh giới No AI / Rule / Workflow:** Lỗi mã hóa UTF-8 và cú pháp xử lý dứt điểm bằng **Rule (script)**; các lỗi thường gặp chặn bằng **No AI (Checklist 4 mục)**; còn phần đối chiếu luồng gọi hàm giữa 1 file `.puml` và 1 cặp `Controller/Service` là bài toán vừa sức một buổi lab để so sánh với **Workflow**.
- **Câu hỏi muốn nhóm phản biện:**
  1. *"Với tần suất chỉ 2–3 đợt review lớn trong một học kỳ, liệu kết hợp **Checklist 4 lỗi thường gặp (No AI) + script quét UTF-8 (Rule)** đã đủ giải quyết 80% vấn đề chưa, hay có thực sự đáng để đưa AI vào đối chiếu `.puml` với code?"*
  2. *"Nếu dùng AI đối chiếu `.puml` với Controller/Service, làm sao tránh việc AI báo lỗi giả (hallucination) khiến người làm mất thời gian kiểm tra lại còn lâu hơn 25 phút tự đọc?"*

### AI phản biện 3 Problem Cards

Prompt đã dùng để phản biện:

```text
Đây là Problem Card của tôi:

Đóng vai một product manager hoài nghi và phản biện:
1. Actor có đủ cụ thể không?
2. Quy trình có thật không, hay là quy trình tôi tưởng tượng?
3. Bottleneck có phải một bước cụ thể không?
4. Metric có đo được không?
5. Sửa quy trình hoặc dùng rule đã đủ chưa?
6. Tôi có đang nhảy sang AI quá sớm không?
Trả lời ngắn, chỉ nói điểm yếu.
```

Kết quả AI phản biện và cách tôi xử lý:
### AI phản biện Card #1

| Điểm yếu | Đồng ý? | Đã sửa gì |
|---|---|---|
| **1. Actor chưa đủ cụ thể:** "Sinh viên CS năm cuối" quá rộng (người rải 100 CV không đọc lại repo; người nhắm Big Tech chỉ cần 1–2 CV hoàn thiện kỹ) | Đồng ý một phần | Thu hẹp Actor thành: *Sinh viên CS năm cuối ứng tuyển đồng thời 2–3 vai trò (Fullstack, QA/Tester, BA), có 5+ repo đồ án cũ chưa đưa lên CV* |
| **2. Quy trình bị lý tưởng hóa:** Thực tế sinh viên ít khi mở repo đọc lại mỗi lần nộp mà thường copy từ Master CV có sẵn | Đồng ý một phần | Tách rõ: bước "đọc lại repo" chỉ xảy ra với các đồ án cũ chưa được tổng hợp lần nào; đưa vào giả định cần hỏi bạn cùng lớp ở CP4 xem họ làm thật thế nào |
| **3. Bottleneck xác định sai bản chất:** Nghẽn không phải vì thiếu công cụ tóm tắt, mà vì đồ án sinh viên thiếu production metric thật, phải vắt óc nhớ lại mình đã làm gì | Đồng ý | Sửa lại bản chất bottleneck: không phải "tóm tắt README", mà là *lục lại code/commit/test để tìm bằng chứng kỹ thuật có thật* (số API, số test case, cấu hình, benchmark) thay vì bịa số liệu |
| **4. Metric ~95 phút là tự ước lượng, thiếu tiêu chí chất lượng:** Làm ngắt quãng khó đo; viết nhanh hơn nhưng bullet tệ hoặc không đậu CV screening thì vô nghĩa | Đồng ý | Sẽ bấm giờ thực tế 2 lần sửa CV tới để lấy baseline thật; thêm quality metric: *100% con số trong bullet truy được về repo (không bịa số) và khớp từ khóa kỹ năng của JD* |
| **5. Sửa quy trình (No AI) là đủ:** Chỉ cần 1 file Markdown/Notion "Master Project Log" ghi sẵn 5 bullet + số liệu ngay khi xong môn học, mất 2 phút copy | Đồng ý một phần | Cập nhật phương án No AI thành **"Master Project Log"** để so sánh công bằng ở CP6. Giữ giả thuyết AI hỗ trợ viết lại góc nhìn của cùng 1 dự án theo từng JD (Dev vs QA vs BA) |
| **6. Nhảy sang giải pháp (Workflow) quá sớm:** Bẫy solution-first khi chưa kiểm chứng xem nỗi đau thật là "đọc lại repo" hay "không biết JD cần từ khóa gì" | Đồng ý | Chưa chốt cứng xây tool đọc repo; đưa câu hỏi *"Khó nhất khi chỉnh CV theo JD là lục lại dự án cũ hay chọn góc viết khớp từ khóa JD?"* vào kiểm chứng ở CP4 |

### AI phản biện Card #2
| Điểm yếu | Đồng ý? | Đã sửa gì |
|---|---|---|
| **1. Actor chưa đủ cụ thể:** "Người làm đồ án, người đọc báo cáo" gộp 2 vai trò khác nhau; đa số sinh viên kéo thả trên draw.io chứ không viết code `.puml` cho ≥10 chức năng | Đồng ý | Thu hẹp Actor thành: *Sinh viên làm đồ án cá nhân (6 sprint), viết báo cáo dùng PlantUML (`.puml`) cho ≥10 nhóm chức năng và sửa code backend nhiều đợt trước khi nộp* |
| **2. Quy trình có tần suất thấp:** Sinh viên thường chỉ vẽ/sửa sơ đồ 1–2 lần trước khi in báo cáo cuối kỳ, không phải công việc lặp lại hằng tuần | Đồng ý một phần | Ghi rõ tần suất thực tế là **2–3 đợt lớn/học kỳ** (do đồ án làm 6 sprint nên sơ đồ vẽ giữa kỳ bị lệch khi thêm bước refund, cache, auth ở cuối kỳ) |
| **3. Bottleneck gộp 2 vấn đề khác bản chất:** "Lỗi mã hóa UTF-8" và "lệch logic với code" hoàn toàn khác nhau; nghẽn thật sự là phải mở 3–4 file (Route, Controller, Service, Model) để nhớ luồng gọi hàm | Đồng ý | Tách hẳn lỗi UTF-8/cú pháp sang bước Rule; định nghĩa lại bottleneck chỉ còn là *đối chiếu luồng gọi hàm, truy vấn DB và trạng thái giữa `.puml` với cặp Controller/Service (~25 phút/đợt cho 10 sơ đồ)* |
| **4. Metric "lỗi còn sót = 0" không tự kiểm chứng được:** Tự mình review lần cuối thì không biết còn sót lỗi nào; "60 phút/đợt" chưa chuẩn hóa theo số lượng sơ đồ | Đồng ý | Chuẩn hóa metric theo sơ đồ: *từ ~6 phút/sơ đồ (~60 phút/10 sơ đồ) xuống dưới 2.5 phút/sơ đồ*; thay "lỗi sót = 0" bằng *100% sơ đồ vượt qua checklist 4 loại lỗi cố định* |
| **5. Rule + Checklist (No AI) đã giải quyết được phần lớn:** Lỗi UTF-8 chỉ cần 1 script/linter; lệch logic có thể rà nhanh bằng checklist 4 lỗi từng gặp (thiếu query DB, thiếu trạng thái trả về, lệch actor, lỗi mã hóa) | Đồng ý một phần | Đưa **Checklist 4 loại lỗi + script quét UTF-8** làm phương án chính (No AI + Rule); chỉ cân nhắc AI khi cần đối chiếu nhanh 1 file `.puml` viết bằng tiếng Việt với 1 hàm Controller dài |
| **6. Nhảy sang Workflow AI dễ âm ROI:** Chỉ làm 2–3 đợt/kỳ mà xây pipeline đưa cả codebase + `.puml` vào LLM sẽ tốn công hơn tự dò, chưa kể LLM báo lỗi giả (hallucination) làm mất thêm giờ kiểm lại | Đồng ý | Hạ kỳ vọng với AI: không xây tool quét cả repo; nếu dùng AI chỉ dán đúng 1 cặp (1 file `.puml` + 1 file Controller) với prompt cố định để gợi ý điểm lệch |

### AI phản biện Card #3
| Điểm yếu | Đồng ý? | Đã sửa gì |
|---|---|---|
| **1. Actor chưa phân biệt rõ nhóm gặp lỗi:** Người điền báo cáo sau khi đã chốt notebook không bị lệch số; chỉ người vừa viết `.md` vừa chạy lại `.ipynb` sát giờ nộp mới hay nhầm | Đồng ý | Cụ thể hóa Actor: *Sinh viên học môn AI/ML làm báo cáo `.md` tách rời khỏi file `.ipynb`, hay chạy lại thực nghiệm sát giờ nộp làm thay đổi tham số/kết quả* |
| **2. Bước "Lập checklist (3 phút)" là tưởng tượng:** File template `.md` của bài lab đã có sẵn toàn bộ đề mục, thực tế không ai ngồi lập lại checklist mới mỗi tuần | Đồng ý | Bỏ bước "Lập checklist" khỏi quy trình; sửa thành bước thực tế: *rà các ô còn trống `*(điền)*` trong template `.md` và đối chiếu số liệu với output cell của `.ipynb`* |
| **3. Bottleneck (~7 phút/bài) chỉ là micro-pain:** 7 phút/tuần quá nhỏ; nguyên nhân gốc không phải thiếu công cụ kiểm tra mà là thói quen copy-paste thủ công khi chưa khóa kết quả chạy notebook | Đồng ý | Ghi nhận thẳng đây là **micro-pain (~7 phút/bài)** do thao tác copy-paste rời rạc giữa `.ipynb` và `.md` khi chạy lại cell vào phút chót |
| **4. Metric tiết kiệm 15 phút/bài có ROI thấp:** Nếu mất vài tiếng viết script đọc `.ipynb` đối chiếu `.md` để tiết kiệm 15 phút/bài thì không bõ công trong phạm vi môn học | Đồng ý | Giữ nguyên cảnh báo *Impact nhỏ (~20 phút/bài)* ở bảng Top 3; bổ sung metric chất lượng đơn giản: *0 ô placeholder `*(điền)*` bị bỏ trống và 0 số liệu (`SEED`, kết quả) lệch với `.ipynb`* |
| **5. Sửa quy trình (No AI) hoặc 1 lệnh grep (Rule) là đủ 100%:** Chỉ cần chốt chạy xong `.ipynb` rồi mới điền `.md`, cộng 1 lệnh tìm chuỗi `*(điền)*` là giải quyết triệt để | Đồng ý hoàn toàn | Chốt phương án **No AI (sửa quy trình: khóa output `.ipynb` trước khi điền `.md`) + Rule đơn giản (tìm các ô chưa điền)** |
| **6. Tuyệt đối không nên dùng AI:** Kiểm tra thiếu mục và khớp con số là bài toán đúng/sai tường minh (deterministic); đưa vào LLM vừa tốn thời gian vừa dễ bị AI đọc lướt bỏ sót số lệch | Đồng ý hoàn toàn | Khẳng định **Không dùng AI** ở Card #3; giữ Card #3 làm ví dụ đối chứng (counter-example) cho thấy bài toán chỉ cần No AI / Rule |

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày và so sánh 3 Problem Cards cá nhân: Problem #1 (CV theo vai trò); Problem #3 (Kiểm báo cáo Lab); Problem #2 (Review sơ đồ sequence PlantUML). Đề xuất Card #2 làm card pitch ưu tiên | Giúp nhóm có tiêu chí rõ ràng để loại nhanh các bài toán chỉ cần No AI / Rule (như Card #3) hoặc đã bão hòa công cụ (Card #1), đồng thời đóng góp góc nhìn "kết hợp Rule tiền xử lý + AI đối chiếu mã nguồn kèm chỉ số đánh giá định lượng" cho bài toán chung của nhóm |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: *"Khi gặp lỗi backend/CSDL, có thật là dev mất 20–30 phút chỉ để đọc chữ trong file log không, hay mất thời gian ở bước mở qua lại nhiều file code để tìm nguyên nhân gốc? Và nếu chỉ dùng script/regex lọc log thì đã giải quyết được bao nhiêu %?"* | Buộc nhóm không kết luận vội "đọc log là bottleneck duy nhất", dẫn tới việc đưa vào Assumption Map (Giả định #3, #4) để kiểm chứng ở CP4 |
| Nhận phản biện | Câu hỏi tôi nhận được: *"Với tần suất chỉ 2–3 đợt review sơ đồ PlantUML trong một học kỳ, liệu Checklist 4 lỗi thường gặp (No AI) + script quét UTF-8 (Rule) đã đủ giải quyết 80% vấn đề chưa? Và nếu AI báo lỗi giả khiến người làm mất hơn 25 phút kiểm tra lại thì có đáng làm bài toán chung cho cả nhóm không?"* | Tôi đã sửa gì: Thừa nhận tần suất của Card #2 thấp (2–3 đợt/kỳ) nên ROI của việc xây pipeline AI thấp hơn phương án No AI + Rule; đồng thuận rút Card #2 để cùng nhóm chọn bài toán **Debug lỗi từ file log hệ thống** (thuộc Cluster 3, xảy ra thường xuyên hơn với mọi thành viên code backend) |
| Gom cluster | Trực tiếp phân tích và gom toàn bộ candidate của nhóm thành 3 Cluster theo bản chất pattern:<br>1. Cluster 1 — Báo cáo & Tổng hợp thông tin đa nguồn: dữ liệu rải rác, tốn thời gian đọc lướt, trích lọc và viết lại văn bản .<br>2. Cluster 2 — Đối chiếu chéo & Kiểm tra tính nhất quán : so sánh thủ công giữa 2+ nguồn để tìm sai lệch .<br>3. Cluster 3 — Thu thập, Sàng lọc & Gỡ lỗi kỹ thuật : đối mặt khối lượng dữ liệu lớn/nhiễu cần khoanh vùng nhanh root cause hoặc nội dung phù hợp  | Giúp nhóm nhìn thấy bức tranh tổng thể từ 10+ candidate rời rạc về 3 nhóm nhu cầu cốt lõi, làm cơ sở dựng cây OST không bị lẫn tên công cụ/giải pháp vào tầng Opportunity |
| Chọn candidate problem | Cùng nhóm đối chiếu 3 Cluster và chấm điểm shortlist theo 7 tiêu chí, đồng thuận chọn **Debug lỗi từ file log hệ thống** (đại diện từ Cluster 3 kết hợp kỹ thuật đối chiếu code của Cluster 2) | Chốt được bài toán có tần suất cao, cả nhóm đều hiểu domain và có sẵn nguồn tài liệu thực nghiệm để kiểm chứng ở CP4 |
| Kiểm chứng / research | Phụ trách chính toàn bộ **Mục 3 — Kiểm chứng + research (CP4)**:<br>- Thiết lập **Assumption Map** (6 giả định Value, Feasibility, Viability).<br>- Đọc, trích xuất số liệu và phân tích giới hạn của **5 Evidence Snapshots** từ tài liệu thứ cấp (`[1]` Alaboudi & LaToza 2021 trên 89 phiên debug, `[2]` LogGPT, `[3]` khảo sát Stripe, `[4]` Cambridge RDB, `[5]` Fahim et al. 2025 trên 492 crash report Java).<br>- Thực hiện **Research giải pháp đã có** (`Sentry Seer [6]`, `GitHub Copilot Chat [7]`, `LogGPT [2]`, `RDB [4]`, `Aggregator tools [1]`) và viết phần điều chỉnh bài toán + kết luận research | Làm nhóm **thay đổi kết luận cốt lõi sau CP4**:<br>1. **Thu hẹp phạm vi:** bỏ qua lỗi nhỏ (~6 phút), chỉ tập trung vào lỗi khó liên tầng (nơi 25/89 phiên chiếm 80% thời gian debug `[1]`).<br>2. **Sửa bottleneck:** từ "đọc chữ trong log" sang **chuyển qua lại giữa log, nhiều file code và lần chạy thử** (`[1, §4.3, §7]`; *"The stack trace shows the location but not why it failed"* `[5]`).<br>3. **Chốt hướng Hybrid nhẹ:** bác bỏ việc xây mô hình/agent mới vì đã có `Sentry Seer` `[6]` và `Copilot Chat` `[7]`; đề xuất dùng script lọc nhiễu log (`[2]`) + trích code các hàm trong stack trace (`Direct-LLM` `[5]` đạt 40.24% gần bằng 43.09% của `Agentic-LLM` với nửa chi phí) → đưa vào AI kèm bước dev duyệt (vì 57–60% ca vẫn chưa định vị đúng hàm `[5]`) |
| Quy trình nhóm | Đưa kết quả từ CP4 (`LogGPT [2]` + `Direct-LLM [5]` + `Aggregator [1]`) vào thiết kế quy trình tương lai của nhóm: tách rõ bước **Rule** (parser lọc timestamp/ID + regex trích hàm trong stack trace), bước **AI** (chẩn đoán trên log sạch + code hàm liên quan) và bước **Con người** (dev kiểm tra bằng chứng code trước khi sửa) | Giúp quy trình tương lai của nhóm bám sát bằng chứng thực nghiệm thay vì giao cả file log thô cho AI đoán mò |
| Mức can thiệp AI | Dùng AI để hệ thống hóa khung phân tích mức can thiệp (so sánh No AI / Rule / Workflow / Agent dựa trên số liệu `Direct-LLM` vs `Agentic-LLM` của `[5]`), trực tiếp thiết kế cấu trúc prompt chuẩn (ép đầu ra JSON có cấu trúc gồm `Root Cause`, `Problem Location`, `Repair Suggestion` kèm đoạn code bằng chứng theo `[2], [5]`) và chạy thử prompt để kiểm nghiệm | Cung cấp bộ khung phân tích mức can thiệp AI và mẫu prompt chạy thử thực tế cho bài nhóm, chứng minh **Workflow nhẹ (Rule + 1 lượt LLM)** là mức phù hợp thay vì nhảy lên Agent phức tạp |


---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Hệ thống lại các problem từng gặp trong quá trình làm dự án tốt nghiệp bao gồm code và báo cáo hay là một số vấn đề khi học và làm bài tập cá nhân | Giúp nhớ lại các việc hay làm theo quán tính mà quên tính thời gian (như bước chạy lại lệnh khi sửa Vue trên WAMP ) | Có xu hướng gợi ý các ý quá chung kiểu "trợ lý AI học tập toàn năng" hoặc viết sẵn tên giải pháp vào trong Job Story | Loại bỏ các ý rộng; viết lại toàn bộ 11 problem theo đúng cấu trúc|
| CP2 Problem Card | Đóng vai PM hoài nghi phản biện cả 3 Problem Cards theo 6 câu hỏi | Chỉ đúng bản chất bottleneck ở Card #1, vạch rõ ROI thấp ở Card #2 và chỉ ra bước "Lập checklist" ở Card #3 | Ở Card #1 bỏ qua việc phải đổi góc nhìn Dev/Tester/BA; ở Card #2 giả định sinh viên chỉ vẽ sơ đồ 1 lần | Thu hẹp Actor cả 3 card |
| CP4 Research | Hỗ trợ tóm tắt nhanh cấu trúc các bài báo và hệ thống kiến thức | Giúp định vị nhanh các bảng số liệu quan trọng | Dễ trích dẫn gộp số liệu tự khai  | Kiểm tra trích dẫn có đúng không và nguồn tài liệu có tồn tại không |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi nghe phần trình bày Top 3 Problems của các bạn khác, tôi nhận ra rằng nhiều vấn đề tưởng chừng đơn giản trong công việc hằng ngày như phản hồi sinh viên, tổng hợp báo cáo tiến độ hàng tuần hay xử lý các câu hỏi lặp đi lặp lại đều có thể được cải thiện bằng cách ứng dụng AI.

Điều tôi học được là không nhất thiết phải lựa chọn những vấn đề quá phức tạp hoặc xây dựng một hệ thống AI lớn mới tạo ra giá trị. Đôi khi, chỉ cần xác định đúng điểm gây mất thời gian, thao tác thủ công hoặc công việc lặp lại là đã có thể tìm ra cơ hội ứng dụng AI phù hợp.

Bên cạnh đó, tôi nhận thấy mỗi người có góc nhìn khác nhau về cùng một vấn đề. Việc lắng nghe các ý tưởng giúp tôi học cách xác định nguyên nhân gốc rễ, đánh giá mức độ ảnh hưởng và suy nghĩ về tính khả thi của giải pháp thay vì chỉ tập trung vào việc đưa AI vào sản phẩm.

Từ đó, tôi rút ra rằng giá trị của AI không nằm ở mức độ phức tạp của công nghệ mà nằm ở khả năng giải quyết vấn đề thực tế và mang lại hiệu quả có thể đo lường được.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có. Ban đầu, nhóm nghĩ ngay đến việc xây dựng một công cụ AI có khả năng đọc log backend/CSDL, phân tích lỗi và gợi ý nguyên nhân để hỗ trợ developer debug nhanh hơn. Tuy nhiên, nhóm nhận ra mình đang giả định rằng việc đọc log chính là nguyên nhân khiến developer mất nhiều thời gian.

Để kiểm tra lại, nhóm đặt ra các câu hỏi: Developer thực sự mất 20–30 phút để đọc log hay chủ yếu mất thời gian tìm kiếm nguyên nhân bằng cách mở qua lại nhiều file code? Nếu chỉ sử dụng script hoặc regex để lọc log thì đã giải quyết được bao nhiêu phần trăm vấn đề?

Từ đó, nhóm chuyển hướng sang tìm hiểu quy trình debug thực tế, xác định điểm nghẽn và kiểm chứng các giả định trước khi lựa chọn giải pháp. Nhóm cũng cân nhắc những phương án đơn giản hơn thay vì mặc định phải sử dụng AI.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Trong quá trình thảo luận, ban đầu tôi khá nghiêng về phương án sử dụng AI để tự động đọc log backend/CSDL, phân tích lỗi và đưa ra gợi ý nguyên nhân nhằm giúp developer tiết kiệm thời gian debug.

Tuy nhiên, khi được các thành viên trong nhóm phản biện, tôi nhận ra rằng chưa chắc AI là giải pháp cần thiết. Một ý kiến đặt ra là liệu vấn đề thực sự nằm ở việc đọc log hay ở quá trình truy tìm nguyên nhân gốc rễ trong nhiều file code. Nếu chỉ cần sử dụng script hoặc regex để lọc log thì liệu có thể giải quyết phần lớn khó khăn mà không cần đến AI hay không?

Sau khi suy nghĩ lại, tôi thay đổi quan điểm từ việc tập trung xây dựng một công cụ AI sang việc cần xác định chính xác vấn đề và nhu cầu thực tế của developer trước. Tôi nhận ra rằng một giải pháp tốt không nhất thiết phải sử dụng công nghệ phức tạp nhất, mà phải giải quyết đúng khó khăn của người dùng.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Có. Điều khiến tôi bất ngờ là dù nhóm đã tìm được 5 tài liệu nghiên cứu và báo cáo có liên quan để củng cố một số giả định ban đầu, nhưng vẫn chưa có đủ bằng chứng để khẳng định giải pháp thực sự phù hợp với đối tượng người dùng mục tiêu.

Đặc biệt, tài liệu [5] là nguồn duy nhất kiểm tra trực tiếp việc đưa stack trace và code vào LLM, nhưng chỉ đánh giá trên benchmark Java mã nguồn mở và không đo thời gian debug thực tế. Điều này khiến tôi nhận ra rằng kết quả nghiên cứu về khả năng kỹ thuật của AI chưa đồng nghĩa với việc AI chắc chắn giúp developer tiết kiệm thời gian trong công việc thực tế.

Ngoài ra, nhóm chưa phỏng vấn trực tiếp developer nên vẫn chưa xác nhận được nhu cầu và mức độ sẵn sàng sử dụng giải pháp. Qua đó, tôi hiểu rằng research có thể hỗ trợ kiểm chứng giả định, nhưng không thể thay thế hoàn toàn phản hồi từ người dùng thực tế.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất đối với tôi là xác định chính xác vấn đề cốt lõi mà developer đang gặp phải, thay vì chỉ mô tả những khó khăn bề mặt hoặc vội vàng đưa giải pháp AI vào Problem Statement.

Ban đầu, nhóm tập trung vào việc developer mất nhiều thời gian khi đọc log và tìm nguyên nhân lỗi backend/CSDL. Tuy nhiên, khi phân tích sâu hơn, chúng tôi nhận ra chưa có đủ bằng chứng để khẳng định thời gian bị lãng phí chủ yếu nằm ở việc đọc log hay quá trình truy tìm nguyên nhân gốc rễ trong nhiều file code.

Qua quá trình này, tôi nhận ra một Problem Statement tốt không chỉ cần mô tả rõ ai đang gặp vấn đề gì, mà còn phải có bằng chứng đủ tin cậy để chứng minh vấn đề đó thực sự tồn tại và đáng được giải quyết.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu được làm lại, tôi sẽ dành nhiều thời gian hơn để tìm hiểu quy trình debug thực tế trước khi đề xuất giải pháp. Thay vì nhanh chóng đồng ý với ý tưởng sử dụng AI để phân tích log, tôi sẽ chủ động đặt câu hỏi về nguyên nhân thực sự khiến developer mất thời gian và mức độ ảnh hưởng của vấn đề.

Tôi cũng sẽ phản biện nhóm mạnh hơn ở việc kiểm chứng các giả định. Cụ thể, tôi muốn làm rõ liệu AI có thực sự cần thiết hay các công cụ đơn giản như script, regex đã đủ đáp ứng nhu cầu. Đồng thời, tôi sẽ đề xuất nhóm tìm cách tiếp cận developer để thu thập dữ liệu thực tế thay vì chỉ dựa vào các tài liệu nghiên cứu thứ cấp.

Qua đó, tôi muốn cải thiện khả năng tư duy phản biện, không ngại đặt câu hỏi với những ý tưởng ban đầu và tập trung vào giá trị thực tế của giải pháp hơn là sự hấp dẫn của công nghệ.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Problem: Developer backend gặp khó khăn và mất thời gian khi điều tra các lỗi liên quan đến backend/CSDL, đặc biệt khi phải phân tích log và truy tìm nguyên nhân gốc rễ.

Quy trình: Khi xảy ra lỗi, developer thường phải kiểm tra log, xác định vị trí lỗi, đối chiếu stack trace với code và tìm nguyên nhân trước khi đưa ra hướng xử lý.

Metric: Nhóm cần quan tâm đến thời gian trung bình để xác định nguyên nhân lỗi, tỷ lệ xác định đúng nguyên nhân và thời gian tiết kiệm được khi sử dụng công cụ hỗ trợ.

Boundary: Giải pháp tập trung hỗ trợ developer debug lỗi backend/CSDL, không thay thế developer sửa code hoặc tự động triển khai thay đổi lên hệ thống.

Mức can thiệp AI: AI có thể hỗ trợ phân tích log, stack trace, đối chiếu code và đề xuất nguyên nhân tiềm năng, nhưng kết quả cần được developer kiểm tra lại.

Quyết định: Nhóm cần kiểm chứng thêm với developer để xác định AI có thực sự cần thiết hay các công cụ đơn giản như script và regex đã đủ giải quyết vấn đề.

---

## 7. Tài liệu tham khảo

- **[1]** Abdulaziz Alaboudi and Thomas D. LaToza. 2021. *An Exploratory Study of Debugging Episodes*. https://arxiv.org/pdf/2105.02162.
- **[2]** Jiaxing Qi, Shaohan Huang, Zhongzhi Luan, Carol Fung, Hailong Yang, and Depei Qian. 2023. *LogGPT: Exploring ChatGPT for Log-Based Anomaly Detection*. https://arxiv.org/pdf/2309.01189.
- **[3]** Stripe (in partnership with Harris Poll). 2018. *The Developer Coefficient: Software engineering efficiency and its $3 trillion impact on global GDP*. Corporate Report (Sep 2018)
https://stripe.com/files/reports/the-developer-coefficient.pdf.
- **[4]** Tom Britton, Lisa Jeng, Graham Carver, Paul Cheak, and Tomer Katzenellenbogen. 2013. *Reversible Debugging Software: "Quantify the time and cost saved using reversible debuggers"*. Cambridge MBA Venture Project, University of Cambridge Judge Business School https://www.researchgate.net/publication/345843594_Reversible_Debugging_Software_Quantify_the_time_and_cost_saved_using_reversible_debuggers.
- **[5]** S M Farah Al Fahim, Md Nakhla Rafi, Zeyang Ma, Dong Jae Kim, and Tse-Hsun (Peter) Chen. 2025. *Crash Report Enhancement with Large Language Models: An Empirical Study*. https://arxiv.org/pdf/2509.13535.
- **[6]** Sentry Documentation. *Seer (AI Debugging Agent)*. https://docs.sentry.io/product/ai-in-sentry/seer/
- **[7]** GitHub Copilot Documentation. *Prompt engineering for GitHub Copilot Chat*. https://docs.github.com/en/copilot/concepts/prompting-and-context/prompt-engineering
