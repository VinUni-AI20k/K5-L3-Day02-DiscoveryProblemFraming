# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: TamCa
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Sinh viên IT năm cuối/mới ra trường mất nhiều thời gian (khoảng 16/30 phút mỗi CV) để đối chiếu và viết lại mô tả dự án trong CV cho khớp với từ khóa yêu cầu trong JD khi ứng tuyển Intern/Fresher.
- Quyết định cuối: **Go (pilot nhỏ, có điều kiện)** — mức can thiệp **Workflow** (Rule + AI gợi ý + người duyệt từng dòng)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Trần Thị Nhài | Khi apply một vị trí mới, tôi muốn chỉnh CV cho khớp yêu cầu trong JD, để không bị loại ngay ở vòng lọc hồ sơ | Sinh viên năm cuối / mới ra trường ngành IT | Viết lại mô tả dự án/kinh nghiệm cho khớp từng yêu cầu JD (~16'/CV, hơn nửa tổng thời gian) | "Chuẩn bị sẵn CV master có 2–3 phiên bản mô tả (No AI) đã đủ chưa?" (Ngô Ngọc Hải) |
| 2 | Trần Thị Nhài | Khi lướt các trang tuyển dụng mỗi ngày, tôi muốn thấy nhanh tin Intern/Fresher đúng tech stack và khu vực, để không mất thời gian đọc tin không hợp | Sinh viên năm cuối / mới ra trường IT, theo dõi 4 nguồn (TopCV, ITviec, LinkedIn, group FB) | Đọc từng tin để kiểm stack/cấp độ/khu vực (~30'/ngày; 7/10 tin đọc xong mới biết không hợp) | "Bộ lọc / job alert có sẵn của TopCV/ITviec/LinkedIn đã đủ chưa?" (Trần Hữu Tài) |
| 3 | Trần Thị Nhài | Khi nhận đề lab mới gồm nhiều file hướng dẫn, tôi muốn nắm cần làm gì, nộp gì và phần nào bị giới hạn, để bắt tay làm ngay mà không sót/vi phạm | Học viên khóa học có lab mỗi buổi (6 lab/tuần) | Đọc chéo RULES/RUBRIC/SUBMISSION/template (~20'/lab; yêu cầu 1 checkpoint nằm rải ở 3–4 file) | "Bottleneck thật là do phải đọc chéo file hay do đề lab viết chưa rõ?" (Ngô Ngọc Hải) |
| 4 | Ngô Ngọc Hải | Khi bắt đầu ngày làm việc hoặc tìm hiểu công nghệ mới, tôi muốn nhanh chóng cập nhật thông tin & xu hướng mới nhất, để không tụt hậu và không dùng phương pháp lỗi thời | Bản thân, thành viên phụ trách công nghệ / R&D | Đọc chi tiết 2–3 bài viết dài để lọc nội dung thực chất (~25'/lần) | "Dùng RSS feed + newsletter (No AI) đã đủ lọc tin rác chưa?" (Trần Thị Nhài) |
| 5 | Ngô Ngọc Hải | Khi nhóm trưởng/đồng đội cần nắm tình hình các việc dở dang, tôi muốn có danh sách việc tồn và blocker, để cả nhóm phối hợp kịp thời mà không phải hỏi dồn dập | Thành viên nhóm đồ án, nhóm trưởng | Nhắn tin và chờ từng người trả lời nguyên nhân nghẽn (~25') | "Pain là do thiếu công cụ hay do thành viên không chịu tự cập nhật?" (Trần Thị Nhài) |
| 6 | Ngô Ngọc Hải | Khi chuẩn bị nộp lab AI20K trước 23h59, tôi muốn đối chiếu cấu trúc thư mục, tên file và link repo theo đúng barem, để không bị trừ điểm oan | Học viên AI20K, người nộp đại diện nhóm | Rà soát thủ công từng file báo cáo (~15'/lần) | "Một shell script kiểm rule đã đủ 95% chưa? Bõ công cả buổi lab?" (Trần Hữu Tài) |
| 7 | Trần Hữu Tài | Khi luyện trả lời xong, tôi muốn biết câu trả lời của mình tốt/dở ở điểm nào, để biết phải sửa gì trước buổi phỏng vấn thật | Ứng viên (sinh viên năm cuối / người mới đi làm) | Tự đánh giá câu trả lời, không tiêu chí, không người chuyên môn (~15–30') | "Ứng viên cần điểm số hay cần gợi ý sửa cụ thể?" (Trần Thị Nhài) |
| 8 | Trần Hữu Tài | Khi sắp có buổi phỏng vấn, tôi muốn luyện tập trong tình huống giống thật (có người hỏi, áp lực thời gian), để không bị run và bí ý | Ứng viên; người đóng vai (bạn bè, mentor) | Tìm và hẹn được người đóng vai phỏng vấn (chờ 1–3 ngày) | "Mock interview với bạn bè / Pramp đã đủ chưa?" (Ngô Ngọc Hải) |
| 9 | Trần Hữu Tài | Khi ứng tuyển một vị trí cụ thể, tôi muốn biết phỏng vấn mấy vòng và câu hỏi có khả năng được hỏi, để chuẩn bị đúng trọng tâm | Ứng viên | Tìm và đọc thông tin rời rạc từ nhiều nguồn (60–120'/công ty) | "Glassdoor/group cộng đồng đã đủ? Thông tin tổng hợp có đáng tin?" (Ngô Ngọc Hải) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung (Nỗi đau chung) |
|---|---|---|
| **A — Lọc tin từ nhiều nguồn** | • #2 (Nhài — Lọc tin tuyển dụng)<br>• #4 (Hải — Lọc tin công nghệ)<br>• #9 (Tài — Lọc review & câu hỏi phỏng vấn) | Phải mở nhiều trang, đọc lướt hàng chục bài viết/tin tức để nhặt ra vài thông tin đúng nhu cầu; tốn 30–60 phút mỗi ngày và dễ đọc phải tin rác/không hợp. |
| **B — So khớp & sửa theo barem** | • #1 (Nhài — Chỉnh CV theo JD)<br>• #6 (Hải — Soát bài nộp theo barem lab)<br>• #7 (Tài — Tự chấm câu trả lời PV theo rubric) | Đã có tiêu chuẩn sẵn (JD, barem lab, rubric), nhưng phải tự căng mắt đối chiếu từng dòng và sửa thủ công; rất dễ sót lỗi khiến hồ sơ bị loại hoặc bài thi bị trừ điểm. |
| **C — Chuẩn bị trước khi bắt tay vào làm** | • #3 (Nhài — Đọc chéo file đề lab để nắm việc)<br>• #5 (Hải — Hỏi từng người để nắm việc tồn & blocker)<br>• #8 (Tài — Chờ hẹn người để luyện phỏng vấn thử) | Trước khi bắt đầu việc chính (làm lab, họp nhóm, đi phỏng vấn), bị nghẽn ở khâu chuẩn bị vì thông tin bị xé nhỏ ở nhiều nơi hoặc phải phụ thuộc, chờ đợi người khác. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Sinh viên IT năm cuối/mới ra trường giảm thời gian chuẩn bị cho một lần ứng tuyển Intern/Fresher IT (từ lúc lọc tin đến lúc nộp CV), mà tỷ lệ hồ sơ vượt qua vòng lọc CV không giảm (baseline: 1/4 hồ sơ có phản hồi).
├── Opportunity A (từ Cluster A): Mất nhiều thời gian đọc lướt hàng chục tin tuyển dụng rải rác trên nhiều trang để nhặt ra tin đúng stack và khu vực.
├── Opportunity B (từ Cluster B - Trọng tâm nhóm chọn): Mất hơn một nửa thời gian để so từng yêu cầu trong JD và viết lại mô tả dự án trong CV cho khớp từ khóa.
└── Opportunity C (từ Cluster C): Mất nhiều thời gian tự chuẩn bị câu trả lời phỏng vấn mà không có tiêu chuẩn rõ ràng để tự đánh giá câu trả lời đã đạt hay chưa.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ "Website/Tool tự động cào tin tuyển dụng và nộp CV hàng loạt" — Solution kỹ thuật, vi phạm boundary đạo đức (spam ứng tuyển), làm tăng tỷ lệ bị từ chối.
- ✗ "AI tự động viết lại toàn bộ CV từ đầu" — Solution trá hình, có nguy cơ nghiêm trọng về việc AI phóng đại hoặc bịa đặt kỹ năng không có thật.
- ✗ "Chatbot tư vấn phỏng vấn có AI chấm điểm" — Solution mơ hồ, chưa làm rõ tiêu chí chấm và giải quyết sai mắt xích (nghẽn chính nằm ở khâu chuẩn bị CV để qua vòng hồ sơ).

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **1. Chỉnh CV theo JD (#1 — Nhài, Cluster B)** | 5 | 5 | 5 | 5 | 4 | 5 | 5 | **34** |
| **2. Barem & quy cách nộp lab AI20K (#6 — Hải, Cluster B)** | 5 | 5 | 5 | 5 | 5 | 3 | 5 | **33** |
| **3. Lọc tin tuyển dụng Intern/Fresher (#2 — Nhài, Cluster A)** | 4 | 4 | 4 | 4 | 4 | 4 | 4 | **28** |

**Candidate được chọn:**
Candidate #1 — Chỉnh CV theo JD khi ứng tuyển vị trí Intern/Fresher IT.

**Vì sao chọn:**
1. **Điểm đánh giá cao nhất (34/35):** Đạt điểm tối đa ở hầu hết các tiêu chí quan trọng.
2. **Bottleneck cực kỳ sắc nét:** Bước viết lại mô tả dự án/kinh nghiệm theo từ khóa của JD chiếm tới 16/30 phút của mỗi CV (hơn 50% thời gian) và lặp lại với mỗi JD mới.
3. **So sánh 4 mức can thiệp rất tự nhiên:**
   - *No AI:* Chuẩn bị sẵn "CV master" với nhiều phiên bản mô tả dự án theo các hướng (Backend, Frontend, Fullstack...) để copy-paste sửa nhẹ.
   - *Rule:* Trích xuất từ khóa bằng regex / text matching giữa CV và JD.
   - *Workflow:* Hệ thống trích xuất yêu cầu JD, map với dự án thật trong CV master, gợi ý viết lại mô tả theo keyword của JD và **bắt buộc người dùng duyệt từng dòng** (Human-in-the-loop).
   - *Agent:* Tự động viết lại và tự nộp CV (đây là rủi ro và nhóm đặt boundary cấm).
4. **Domain gần gũi, thuận lợi cho CP4:** Cả 3 thành viên và bạn học trong lớp đều đang là sinh viên năm cuối chuẩn bị xin việc, có thể phỏng vấn người thật (The Mom Test) để thu thập dữ liệu kiểm chứng ngay trong buổi học mà không phải phỏng vấn giả định.

**Vì sao loại các candidate còn lại:**
- **Loại Candidate #6 (Barem & quy cách nộp lab AI20K):** Dù đây là nỗi đau thật (đã từng bị trừ 5 điểm) và quy trình rất rõ, nhưng bản chất bài toán là logic cố định (deterministic rule) — chỉ cần một shell script bash hoặc checklist cố định là giải quyết được 95% vấn đề. Không có bài toán về ngôn ngữ hay độ mơ hồ để cần đến mức can thiệp Workflow/AI. Nếu chọn bài này, ở CP5–CP6 sẽ bị gượng ép khi đưa AI vào một bài toán mà Rule làm tốt hơn.
- **Loại Candidate #2 (Lọc tin tuyển dụng Intern/Fresher):** Các nền tảng tuyển dụng lớn (TopCV, ITviec, LinkedIn) đều đã có sẵn bộ lọc theo cấp độ/địa điểm và tính năng Job Alert gửi email hằng ngày (No AI). Điểm nghẽn nằm ở các bài đăng không cấu trúc trên Facebook group, nhưng việc thu thập dữ liệu này vướng rào cản kỹ thuật và pháp lý (scraping, API hạn chế), khó triển khai kiểm chứng thực tế trong thời gian lab.

**Xử lý bất đồng (nếu có):**
- Hải ban đầu muốn chọn bài Barem nộp lab (#6) vì bài học bị trừ 5 điểm ở bài lab trước còn rất mới và muốn có giải pháp dứt điểm. Tuy nhiên, sau khi cả nhóm thảo luận tiêu chí "So sánh được 4 mức", Hải nhận thấy một script bash chạy local đã đủ giải quyết bài này và nhóm không nên "dùng dao mổ trâu để giết gà". Hải đồng ý chuyển sang chọn bài Chỉnh CV (#1) và đề xuất viết script kiểm barem lab như một công cụ nội bộ riêng của nhóm.
- Tài muốn giải bài toán Luyện phỏng vấn (#7, #8) vì thấy nhiều bạn gặp khó khăn khi trả lời câu hỏi hành vi. Nhưng Nhài và Hải phân tích: phỏng vấn cần xử lý âm thanh/video hoặc ngữ cảnh giao tiếp phức tạp, tiêu chí "câu trả lời hay" có độ mơ hồ quá cao để đánh giá trong phạm vi lab. Cả nhóm thống nhất: vượt qua vòng lọc hồ sơ (CV) là điều kiện tiên quyết trước khi đến vòng phỏng vấn, do đó giải quyết khâu CV (#1) là bước đi cấp thiết và vừa sức hơn. Tài hoàn toàn nhất trí.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên IT khác (không chỉ mình Nhài) cũng mất trên 20 phút/CV để viết lại mô tả cho khớp JD | Value | 5 | 2 | ✅ |
| 2 | Bước tốn thời gian nhất là viết lại mô tả dự án cho khớp từ khóa JD, không phải khâu tìm việc hay lọc tin | Value | 5 | 2 | ✅ |
| 3 | Người dùng đã thử workaround (CV master / copy từ khóa JD / tool có sẵn) và vẫn thấy chưa đủ | Value / Feasibility | 4 | 1 | ✅ |
| 4 | AI gợi ý viết lại tiết kiệm thời gian nhiều hơn thời gian người dùng phải duyệt lại | Value / Usability | 4 | 1 | ✅ |
| 5 | Trích xuất yêu cầu/từ khóa từ JD đủ đáng tin (text/regex/AI) | Feasibility | 4 | 3 | — |
| 6 | Thị trường đã có công cụ làm việc này (Jobscan, Teal) nên không nên tự xây từ đầu | Feasibility / Viability | 4 | 4 | — |

Giả định nhóm kiểm chứng trong buổi này: **#1, #2, #3, #4** (quan trọng cao nhưng ít bằng chứng).

### 3.2. Kiểm chứng

> ⚠️ Các ô `_(điền)_` **phải lấy từ phỏng vấn/survey người thật**. Không được bịa (rubric: bịa kết quả phỏng vấn/survey → C7 = 0 cho cả nhóm). Mục này do **Nhài phụ trách**, Tài hỗ trợ tổng hợp.

Cách đã dùng: **Phỏng vấn nhanh 3 người (The Mom Test) + micro survey/poll 5–10 người trong lớp.**

> File hỗ trợ: bộ câu hỏi `report/assets/cp4-poll-cau-hoi.md` · mẫu snapshot `report/assets/cp4-interview-snapshot-template.md` · tin nhắn mời + poll `report/assets/cp4-tin-nhan-va-poll.md`.

- Đối tượng phỏng vấn: 2 bạn cùng lớp đang tìm Intern/Fresher IT + 1 anh/chị khóa trên đã đi làm. **Không phỏng vấn thành viên nhóm mình.**
- Nguyên tắc: hỏi về **chuyện đã xảy ra** và **cách họ đang xử lý**, tuyệt đối không hỏi dạng "Bạn có muốn…".

**Bộ câu hỏi phỏng vấn (The Mom Test):**

1. Lần gần nhất bạn chỉnh CV để ứng tuyển một vị trí là khi nào? Kể lại từng bước bạn đã làm.
2. Bước nào mất nhiều thời gian nhất? Khoảng bao lâu?
3. Bạn đã thử cách nào để CV khớp JD chưa (CV master, copy từ khóa, dùng tool)? Kết quả thế nào?
4. Bạn có đối chiếu CV với JD trước khi nộp không? Bằng cách nào?
5. Sau khi nộp, bạn có nhận được phản hồi nào không?

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

**Snapshot 1 — P1**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | P1 — Sinh viên năm 4 cùng lớp, đang tìm Intern Backend (Java/Spring) |
| Câu nói đáng nhớ nhất (nguyên văn) | "Mình có 3 project thôi mà mỗi JD lại gọi tên một kiểu, ngồi đổi chữ 'xây dựng API' thành 'thiết kế RESTful service' mà mất cả buổi." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước nộp 4 công ty trong 1 tối. Mở JD, bôi đen các yêu cầu, rồi sửa phần mô tả 2 project trong file Word cho trùng chữ với JD. Nộp được 3/4 vì hết giờ. |
| Hiện đang xử lý bằng cách nào (workaround)? | Giữ 1 file CV gốc, mỗi JD "Save as" một bản rồi sửa tay; thỉnh thoảng dán JD vào ChatGPT hỏi "từ khóa quan trọng là gì". |
| Mất bao lâu, bao lần? | ~25 phút/CV, trong đó ~15 phút là viết lại mô tả dự án; 3–5 CV/tuần. |
| Insight / opportunity rút ra | Nghẽn không phải ở *tìm* từ khóa mà ở *diễn đạt lại* kinh nghiệm thật bằng ngôn ngữ của JD. Đã dùng ChatGPT nhưng chỉ để lấy từ khóa, không tin để viết lại vì "nó hay chém thêm". |

**Snapshot 2 — P2**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | P2 — Sinh viên năm cuối cùng lớp, apply Fresher Frontend (React) |
| Câu nói đáng nhớ nhất (nguyên văn) | "Mình làm CV master rồi, có sẵn bản Frontend với Fullstack, nhưng gặp JD nào đòi kiểu 'có kinh nghiệm tối ưu performance' là lại phải ngồi nghĩ project nào của mình dính tới cái đó." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | 5 ngày trước apply một công ty product; JD có 8 gạch đầu dòng yêu cầu. CV master khớp được khoảng một nửa, phần còn lại phải lục lại repo GitHub để nhớ mình đã làm gì rồi viết bullet mới. |
| Hiện đang xử lý bằng cách nào (workaround)? | CV master 2 phiên bản (Frontend / Fullstack) + copy-paste bullet; dùng bản free của Jobscan 1 lần nhưng bỏ vì "hết lượt scan free". |
| Mất bao lâu, bao lần? | ~10 phút với JD "quen", ~30 phút với JD "lạ"; khoảng 2/3 JD là "lạ". |
| Insight / opportunity rút ra | CV master (No AI) giải quyết tốt JD quen, nhưng **không đủ** cho JD lạ. Phần đau là map yêu cầu JD ↔ dự án thật đã làm. |

**Snapshot 3 — P3**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | P3 — Anh khóa trên, đã đi làm Backend 1.5 năm, từng tham gia sàng lọc CV intern ở công ty |
| Câu nói đáng nhớ nhất (nguyên văn) | "Bên anh lọc CV intern chủ yếu nhìn xem project có đúng stack không, chứ nhồi từ khóa mà phỏng vấn hỏi không trả lời được thì loại luôn." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Hồi đi xin intern (2 năm trước) nộp ~20 chỗ, chỉ sửa câu Objective cho từng công ty, mô tả dự án giữ nguyên → 3 phản hồi. Lúc lọc CV ở công ty, anh gặp nhiều CV "khớp từ khóa 100% nhưng mô tả chung chung". |
| Hiện đang xử lý bằng cách nào (workaround)? | Khi còn đi apply: không tailor nhiều. Khi lọc CV: đọc nhanh mục dự án, check stack + vai trò thật. |
| Mất bao lâu, bao lần? | Người lọc: ~1–2 phút/CV. Hồi apply: ~5 phút/CV (chỉ sửa Objective). |
| Insight / opportunity rút ra | **Tín hiệu phản bác/điều chỉnh:** khớp từ khóa không phải là tất cả — mô tả phải *đúng sự thật và cụ thể* (stack, vai trò, kết quả). Củng cố boundary: AI không được thêm kỹ năng không có thật. |

**Poll nhanh trong lớp (8 người, không tính thành viên nhóm; Google Form ẩn danh, ~5 phút):**

| Câu hỏi | Kết quả |
|---|---|
| Q1. 30 ngày qua bạn có nộp CV Intern/Fresher IT không? | 7/8 có (1 người chưa apply → loại khỏi các câu sau, n = 7) |
| Q2. Lần nộp gần nhất, bạn có chỉnh CV theo JD không? | 6/7 có chỉnh; 1/7 nộp nguyên bản |
| Q3. Thời gian trung bình chỉnh 1 CV (n = 6) | < 10': 1 · 10–20': 2 · 20–30': 2 · > 30': 1 |
| Q4. Bước tốn thời gian nhất (n = 6) | Viết lại mô tả dự án/kinh nghiệm: 4 · Đọc/hiểu JD: 1 · Chỉnh format/layout: 1 |
| Q5. Bạn đang dùng cách nào? (chọn nhiều, n = 6) | CV master nhiều phiên bản: 3 · Copy từ khóa JD thủ công: 5 · ChatGPT/AI chat: 4 · Jobscan/Teal: 1 |
| Q6. Lần gần nhất dùng AI để viết lại CV, bạn có phải sửa lại nội dung AI viết không? (n = 4) | Sửa nhiều / viết lại: 3 · Sửa ít: 1 · Dùng nguyên: 0 |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn | 3 | P1, P2 mất 15–30'/CV, phần lớn ở bước viết lại mô tả dự án (xác nhận GĐ #1, #2). P2 đã dùng CV master nhưng không đủ cho JD "lạ" (xác nhận GĐ #3). P1 dùng ChatGPT nhưng không tin để viết lại vì "chém thêm" (liên quan GĐ #4). | P3 (người lọc CV): nhồi từ khóa không giúp qua vòng nếu mô tả không thật/không cụ thể → metric "khớp từ khóa" một mình là sai hướng. P3 khi còn đi apply gần như không tailor mà vẫn có phản hồi. |
| Poll trong lớp | 8 (n = 7 đã apply) | 6/7 có chỉnh CV theo JD; 3/6 mất ≥ 20'/CV; 4/6 nói bước viết lại mô tả dự án tốn nhất (xác nhận GĐ #1, #2). 4/6 đã thử AI chat → nhu cầu hỗ trợ có thật. | 3/6 mất < 20'/CV → GĐ #1 ("> 20'") chỉ đúng với khoảng một nửa. 3/4 người đã dùng AI phải sửa nhiều → GĐ #4 (AI tiết kiệm hơn thời gian duyệt) **chưa được chứng minh**, là rủi ro chính. |

**Kết quả từng giả định:**

| # | Giả định | Kết quả |
|---:|---|---|
| 1 | Người khác cũng mất > 20'/CV | **Xác nhận một phần** — ~một nửa mẫu; nặng nhất với JD "lạ" (~30'). |
| 2 | Bước viết lại mô tả dự án tốn nhất | **Xác nhận** — 4/6 poll + 2/2 ứng viên phỏng vấn. |
| 3 | Workaround hiện tại chưa đủ | **Xác nhận** — CV master ổn với JD quen, không đủ với JD lạ; Jobscan free bị giới hạn lượt. |
| 4 | AI gợi ý tiết kiệm hơn thời gian duyệt | **Chưa xác nhận / có tín hiệu ngược** — người dùng phải sửa nhiều vì AI bịa thêm. Cần thiết kế để AI chỉ diễn đạt lại *dựa trên dữ liệu dự án thật*. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
1. **Thu hẹp phạm vi:** tập trung vào **JD "lạ"** (JD có yêu cầu chưa có sẵn bullet tương ứng trong CV master) — đây là nơi workaround No AI hết tác dụng và thời gian tăng gấp ~3 lần.
2. **Đổi metric:** không chỉ đo "thời gian/CV" mà thêm **tỉ lệ bullet gợi ý được chấp nhận mà không phải viết lại** và **0 kỹ năng bịa** — vì P3 và poll Q6 cho thấy nội dung sai sự thật mới là rủi ro lớn nhất, không phải thiếu từ khóa.
3. **Đổi cách AI tham gia:** AI không viết CV tự do; đầu vào bắt buộc là **"hồ sơ dự án thật"** (stack, vai trò, việc đã làm) do người dùng khai báo, AI chỉ **map yêu cầu JD → dự án thật** và **diễn đạt lại**; yêu cầu không có dự án tương ứng thì đánh dấu "thiếu", không được bù.
4. **Giữ CV master (No AI) là bước nền** — không thay thế, vì nó đã đủ cho JD quen.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Jobscan** — ATS Resume Matcher | https://www.jobscan.co/resume-matcher | Bước 1+2: đọc JD, đối chiếu CV với JD, chỉ ra hard/soft skills còn thiếu | Có Match Score theo từng vị trí; quét 30+ tiêu chí; bản scan miễn phí; có AI Optimize | "AI Optimize"/"Predicted Skills" có thể thêm từ khóa không có thật trong kinh nghiệm; optimize là tính năng trả phí; chỉ tối ưu cho ATS, không đảm bảo nội dung đúng | Phần đối chiếu từ khóa đã có tool làm tốt → dùng để **gợi ý**, con người phải **duyệt từng từ khóa** |
| **Teal** — Resume Job Description Match | https://www.tealhq.com/tool/resume-job-description-match | Bước 2+3: so CV với JD ra Match Score, đánh dấu từ khóa Xanh/Vàng/Đỏ, gợi ý bullet | Trực quan (green/yellow/red); AI gợi ý bullet theo hành động; có bản free | AI bullet "có thể chứa số liệu giả định" (Teal tự cảnh báo); nhiều tính năng cần Teal+; chỉ xuất PDF | Đúng hướng **Workflow + người duyệt**: AI gợi ý, người sửa và xác nhận |
| **Pattern "CV master + bật/tắt bullet theo JD"** (No AI) | https://help.tealhq.com/en/articles/14435726-how-to-tailor-your-resume-for-a-specific-job | Bước 3: thay vì viết lại từ đầu, dựng 1 CV master rồi bật/tắt bullet phù hợp cho từng JD | Không cần AI; nhanh nếu CV master đủ; kiểm soát hoàn toàn nội dung | Mỗi JD "lạ" vẫn phải viết mới; CV master tốn công dựng ban đầu | Đây là **phương án No AI** cần kiểm chứng trước khi kết luận cần AI |

**Kết luận research:** bài toán "đối chiếu CV ↔ JD" đã có tool làm sẵn, **không nên tự xây từ đầu**. Hướng hợp lý: **Rule** trích từ khóa JD → **AI gợi ý** viết lại mô tả → **con người duyệt** → nộp. Điểm khác biệt so với tool có sẵn là nhấn mạnh bước người duyệt để tránh AI bịa kinh nghiệm.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
[JD mới]
   │
   ▼
(1) Đọc JD, bôi đen yêu cầu ──► (2) Mở CV master, chọn phiên bản gần nhất (Save as)
                                        │
                                        ▼
                     (3) So từng yêu cầu JD ↔ dự án đã làm  ◄── lục lại repo/ghi chú
                                        │
                                        ▼
                     (4) Viết lại mô tả dự án cho khớp từ khóa JD   ◄═══ BOTTLENECK
                                        │      (đôi khi dán vào ChatGPT rồi sửa lại)
                                        ▼
                     (5) Đọc soát, chỉnh format, xuất PDF ──► (6) Nộp
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Ứng viên | JD (TopCV/ITviec/LinkedIn) | Danh sách yêu cầu được bôi đen | ~3' / mỗi JD | Làm trong đầu hoặc highlight trên trình duyệt |
| 2 | Ứng viên | CV master (1–3 phiên bản) | Bản CV nháp cho JD này | ~2' | Chọn bản Backend/Frontend/Fullstack gần nhất |
| 3 | Ứng viên | Yêu cầu JD + dự án đã làm | Biết yêu cầu nào đã có/chưa có bullet | ~5' (JD lạ ~8') | Phải lục repo GitHub để nhớ việc đã làm (P2) |
| 4 | Ứng viên (± ChatGPT) | Bullet cũ + từ khóa JD | Mô tả dự án mới | ~16' (JD lạ 20–25') | Nếu dùng ChatGPT: phải sửa lại vì AI thêm kỹ năng không có (P1, poll Q6 3/4) |
| 5 | Ứng viên | CV đã sửa | File PDF hoàn chỉnh | ~4' | Kiểm tra lỗi chính tả, căn lề |
| 6 | Ứng viên | PDF + form ứng tuyển | Hồ sơ đã nộp | ~2' | 3–5 lần/tuần |

**Tổng:** ~30'/CV (JD quen ~15', JD lạ ~40'). **Bottleneck chính:** bước 3 + 4 — map yêu cầu JD với dự án thật rồi diễn đạt lại bằng ngôn ngữ JD, chiếm ~21/30 phút (~70%), nặng nhất với JD "lạ".

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
[Một lần duy nhất] [NGƯỜI] Khai báo "hồ sơ dự án thật": mỗi dự án = stack, vai trò, việc đã làm, kết quả
                                        │
[JD mới]                                ▼
   │
   ▼
(1) [RULE]  Tách JD thành danh sách yêu cầu (gạch đầu dòng) + từ khóa stack (từ điển kỹ năng IT)
   │
   ▼
(2) [RULE]  Đối chiếu với CV master: yêu cầu nào đã có bullet khớp → dùng lại luôn (JD quen dừng ở đây → bước 5)
   │
   ▼
(3) [AI]    Với yêu cầu còn lại: map sang dự án thật trong hồ sơ + gợi ý 1–2 bullet diễn đạt lại
   │        • Mỗi bullet ghi rõ NGUỒN (dự án nào, dòng nào trong hồ sơ)
   │        • Yêu cầu không có dự án tương ứng → đánh dấu "THIẾU", KHÔNG viết bù
   ▼
(4) [NGƯỜI] Duyệt TỪNG bullet: Chấp nhận / Sửa / Loại  ◄═══ HITL bắt buộc, không có nút "chấp nhận tất cả"
   │        [RULE] chặn: bullet chứa kỹ năng/công nghệ không có trong hồ sơ dự án → cảnh báo đỏ
   ▼
(5) [NGƯỜI] Đọc soát, xuất PDF ──► (6) [NGƯỜI] Tự nộp

BOUNDARY: AI không thêm kỹ năng/số liệu không có trong hồ sơ; AI không tự nộp CV; không gửi CV lên dịch vụ ngoài khi chưa xóa SĐT/email.
QUAY VỀ khi AI sai: bỏ gợi ý AI → dùng bullet CV master (bước 2) và tự viết như hiện tại.
  Nếu ≥ 2/5 bullet bị loại trong 1 JD → tự động gợi ý chuyển sang tự viết cho JD đó.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 | 6 (+1 bước khai báo hồ sơ dự án, làm 1 lần) | Số bước không giảm; thay đổi nằm ở ai làm bước 1–3 |
| Tổng thời gian | ~30'/CV (JD lạ ~40') | ~15'/CV (JD lạ ~20') | Khai báo hồ sơ dự án ~30' một lần, hòa vốn sau ~2 CV |
| Số bước thủ công | 6/6 | 3/6 (duyệt, soát, nộp) | Bước 1–2 là Rule, bước 3 là AI |
| Bottleneck chính | Map JD ↔ dự án + viết lại (~21') | Duyệt từng bullet AI gợi ý (~7') | Bottleneck chuyển sang khâu duyệt — đúng chủ đích (con người giữ quyền quyết định) |
| Rủi ro mới phát sinh | — | AI bịa kỹ năng/số liệu; người dùng duyệt qua loa; lộ thông tin cá nhân khi gửi CV cho AI | Giảm bằng: AI chỉ dùng hồ sơ dự án, Rule chặn kỹ năng lạ, buộc duyệt từng dòng, xóa thông tin liên hệ trước khi gửi |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên IT năm cuối / mới ra trường ứng tuyển Intern/Fresher, đã có CV master nhưng thường gặp JD "lạ" (yêu cầu chưa có sẵn bullet tương ứng). |
| **Quy trình** | Đọc JD → chọn bản CV master → map từng yêu cầu JD với dự án thật đã làm → viết lại mô tả dự án theo ngôn ngữ JD → soát, xuất PDF → nộp. Tần suất 3–5 CV/tuần trong mùa tìm việc. |
| **Bottleneck** | Bước map yêu cầu JD ↔ dự án thật và diễn đạt lại mô tả: ~21/30 phút mỗi CV (~70%), JD lạ lên 20–25'; khi dùng ChatGPT thì phải sửa lại vì AI thêm kỹ năng không có thật (3/4 người trong poll). |
| **Impact** | Mỗi người mất 1.5–2.5 giờ/tuần chỉ để chỉnh CV; nộp được ít hồ sơ hơn dự định (P1: 3/4 vì hết giờ); hoặc bỏ qua tailor → CV chung chung; hoặc dùng AI chat → rủi ro CV sai sự thật, bị loại ở vòng phỏng vấn (P3). |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian chỉnh 1 CV cho JD lạ: **~40' → ≤ 20'** (tự bấm giờ trên 5 JD thật/người, 3 người). (2) Tỉ lệ bullet AI gợi ý được chấp nhận hoặc chỉ sửa nhẹ: **≥ 60%**. (3) Số kỹ năng/số liệu không có trong hồ sơ dự án xuất hiện trong CV cuối: **0** (người kiểm tra đối chiếu chéo). Theo dõi phụ: tỉ lệ phản hồi giữ ≥ baseline 1/4. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI **không** thêm kỹ năng, công nghệ, số liệu, vai trò không có trong hồ sơ dự án; **không** tự nộp CV; **không** viết lại toàn bộ CV. Con người **bắt buộc duyệt từng bullet** trước khi đưa vào CV; mọi bullet bị Rule gắn cờ "kỹ năng lạ" phải được người dùng xác nhận hoặc xóa. Thông tin liên hệ được xóa trước khi gửi nội dung cho AI. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **"Jobscan/Teal đã làm việc này, nhóm làm thêm để làm gì?"** (nhóm bạn) — **Đồng ý một phần.** Phần chấm điểm khớp từ khóa đã có tool làm tốt, nhóm không xây lại. Khác biệt nhóm nhắm tới là: gợi ý chỉ dựa trên hồ sơ dự án thật + có nguồn cho từng bullet + chặn kỹ năng lạ; và bản free của Jobscan bị giới hạn lượt (P2). Nếu ở CP6 thấy dùng Teal + checklist duyệt đã đủ, nhóm sẵn sàng hạ mức can thiệp.

- **"Metric 'thời gian' có thể đạt được bằng cách duyệt qua loa — tiết kiệm thời gian nhưng CV tệ hơn."** (AI phản biện) — **Đồng ý.** Đã thêm metric (2) tỉ lệ chấp nhận và (3) 0 kỹ năng bịa, và không có nút "chấp nhận tất cả".
- **"Mục tiêu cuối là được gọi phỏng vấn, sao không đo tỉ lệ phản hồi?"** (nhóm bạn) — **Đồng ý về mặt ý nghĩa nhưng không dùng làm metric chính:** tỉ lệ phản hồi phụ thuộc thị trường, thời điểm và mất 1–3 tuần mới có, không đo được trong phạm vi lab. Nhóm giữ nó làm chỉ số theo dõi phụ (không được giảm so với 1/4).
- **"Bước khai báo hồ sơ dự án có thể khiến người dùng bỏ cuộc ngay từ đầu."** (AI phản biện) — **Ghi nhận, chưa có bằng chứng.** Sẽ kiểm chứng ở pilot: đo thời gian khai báo và số người hoàn thành; nếu > 45' hoặc < 2/3 người hoàn thành thì cho phép nhập trực tiếp từ CV master thay vì form riêng.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ CAO × Độ phức tạp THẤP–TRUNG BÌNH** → vùng phù hợp với **Workflow** (các bước cố định, AI xử lý đúng một bước cần hiểu ngôn ngữ).

Vì sao:
- **Mơ hồ cao:** cùng một kinh nghiệm có nhiều cách gọi ("xây dựng API" / "thiết kế RESTful service" — P1); yêu cầu JD viết tự do, không có cấu trúc chuẩn; quyết định "dự án này có đáp ứng yêu cầu kia không" cần hiểu ngữ nghĩa → Rule thuần (regex, so khớp từ khóa) không xử lý được phần map và diễn đạt lại.
- **Phức tạp thấp–TB:** quy trình tuyến tính, 6 bước cố định, không cần ra quyết định nhiều nhánh, không cần gọi hệ thống ngoài, không cần tự lập kế hoạch → **không cần Agent**.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | CV master 2–3 phiên bản (Backend/Frontend/Fullstack) + thư viện bullet có sẵn, bật/tắt theo JD | JD "quen" — yêu cầu đã có bullet tương ứng (P2: ~10'/CV) | Không giải được JD "lạ" (~2/3 JD theo P2), vẫn ~30–40'/CV | Giữ làm **bước nền** |
| **Rule** | Tách JD thành gạch đầu dòng; so từ khóa với từ điển kỹ năng IT và với CV master; chặn bullet có kỹ năng không có trong hồ sơ | Kiểm tra thiếu/đủ từ khóa stack (Java, React, Docker…) | Chỉ khớp chữ, không hiểu nghĩa; khuyến khích nhồi từ khóa — điều P3 nói là bị loại | Dùng cho bước 1, 2 và **lớp kiểm tra** ở bước 4 |
| **Workflow** | Rule tách JD → AI map yêu cầu ↔ dự án thật + gợi ý bullet có ghi nguồn → **người duyệt từng dòng** → người tự nộp | JD lạ, cần diễn đạt lại kinh nghiệm thật theo ngôn ngữ JD | AI bịa kỹ năng/số liệu; người duyệt qua loa | **CHỌN** |
| **Agent** | AI tự tìm JD, tự viết lại CV, tự nộp hàng loạt | — | Bịa kinh nghiệm không ai kiểm tra; spam ứng tuyển; vi phạm boundary nhóm đã đặt ở CP3 | Cấm |

**Mức chọn:** **Workflow** — Rule (bước 1, 2, chặn kỹ năng lạ) + AI (chỉ bước 3: map & gợi ý) + Con người (duyệt, soát, nộp).

**Vì sao không chọn mức đơn giản hơn:**
- **No AI không đủ:** P2 đã dùng CV master nhưng vẫn mất ~30' với JD lạ; poll: 3/6 vẫn ≥ 20'/CV dù 3/6 có CV master.
- **Rule không đủ:** phần nghẽn (~21') là *diễn đạt lại theo nghĩa*, không phải *tìm từ khóa* — P1 tìm từ khóa bằng ChatGPT rất nhanh nhưng vẫn mất 15' viết lại. Rule thuần còn đẩy người dùng về hướng nhồi từ khóa (P3 phản bác).
- Ngược lại, **không lên Agent** vì quy trình không có nhánh phức tạp và rủi ro sai sự thật đòi hỏi con người ở mọi bullet.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Với mỗi yêu cầu JD chưa có bullet khớp: (a) dự án thật nào trong hồ sơ liên quan nhất (hoặc "THIẾU"); (b) 1–2 bullet diễn đạt lại kèm trích nguồn từ hồ sơ dự án. |
| **Judgment** — con người cân nhắc, quyết định gì? | Bullet có đúng sự thật không, có nói quá vai trò không, có tự tin trả lời khi bị hỏi phỏng vấn không; chấp nhận / sửa / loại; yêu cầu "THIẾU" thì bỏ qua hay cân nhắc không apply. |
| **Action** — hành động cuối cùng là gì, ai làm? | Người dùng đưa bullet đã duyệt vào CV, soát, xuất PDF và **tự nộp**. AI không có quyền nộp. |
| **Outcome** — đo kết quả bằng gì? | Thời gian chỉnh 1 CV JD lạ (bấm giờ); tỉ lệ bullet được chấp nhận/sửa nhẹ; số kỹ năng bịa trong CV cuối (= 0); theo dõi phụ: tỉ lệ phản hồi ≥ 1/4. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | (1) Văn bản JD — **có sẵn** (copy từ trang tuyển dụng). (2) Hồ sơ dự án thật (stack, vai trò, việc làm, kết quả) — **chưa có**, người dùng khai báo 1 lần ~30', có thể lấy từ CV master + README repo. (3) Danh sách yêu cầu đã tách bởi Rule — **tự sinh**. Đã xóa SĐT/email trước khi gửi. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Hành động duyệt của người dùng (chấp nhận / sửa / loại + lý do loại: "bịa", "sai dự án", "văn phong"); các bullet người dùng sửa lại được lưu làm ví dụ mẫu cho lần sau; phản hồi từ nhà tuyển dụng (có/không gọi) theo dõi dài hạn. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: **Augment.** P1 dùng ChatGPT để lấy từ khóa nhưng "không tin để viết lại vì nó hay chém thêm"; poll Q6: 0/4 người dùng nguyên văn AI viết, 3/4 sửa nhiều; P3 nhấn mạnh người viết CV phải trả lời được khi bị hỏi về từng dòng → người dùng cần giữ quyền quyết định nội dung, chỉ muốn bớt phần "nghĩ cách diễn đạt".
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: **Báo nhầm tệ hơn** — tức AI khẳng định một dự án đáp ứng yêu cầu khi thực tế không (hoặc thêm kỹ năng không có). Hậu quả: CV sai sự thật, lộ ở vòng phỏng vấn, mất uy tín với công ty (P3). Bỏ sót (không tìm ra dự án khớp) chỉ khiến người dùng tự viết như hiện tại — tệ nhất là quay về baseline. Thiết kế xử lý: AI được hướng dẫn **thà đánh dấu "THIẾU" còn hơn đoán**; mỗi bullet phải trích nguồn từ hồ sơ dự án; Rule gắn cờ đỏ bất kỳ kỹ năng/công nghệ/số liệu nào không có trong hồ sơ; người duyệt từng dòng, không có "chấp nhận tất cả".

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên IT năm cuối / mới ra trường ứng tuyển Intern/Fresher, **đã có CV master**, đang gặp JD "lạ" (yêu cầu chưa có bullet tương ứng); 3–5 CV/tuần. |
| **Quy trình** | (Một lần) khai báo hồ sơ dự án thật → Với mỗi JD: tách yêu cầu → đối chiếu CV master → map yêu cầu còn thiếu với dự án thật & diễn đạt lại → duyệt → soát, xuất PDF → tự nộp. |
| **Bottleneck** | Map yêu cầu JD lạ ↔ dự án thật và diễn đạt lại: ~21/30' mỗi CV, 20–25' với JD lạ; dùng AI chat tự do thì phải sửa nhiều vì AI bịa thêm. |
| **Impact** | 1.5–2.5 giờ/tuần/người; nộp ít hơn dự định hoặc nộp CV chung chung; rủi ro CV sai sự thật khi dùng AI chat không kiểm soát. |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian/CV JD lạ: **~40' → ≤ 20'** (bấm giờ, 3 người × 5 JD thật). (2) Bullet AI được chấp nhận/sửa nhẹ: **≥ 60%**. (3) Kỹ năng/số liệu không có trong hồ sơ trong CV cuối: **0** (thành viên nhóm đối chiếu chéo từng CV pilot). (4) Phụ: tỉ lệ phản hồi **≥ 1/4** (theo dõi 3 tuần). |
| **Boundary** | AI không thêm kỹ năng, công nghệ, số liệu, vai trò ngoài hồ sơ dự án; không viết lại toàn bộ CV; không tự nộp. Người dùng duyệt từng bullet; bullet bị cờ đỏ phải xác nhận hoặc xóa. Xóa thông tin liên hệ trước khi gửi cho AI. |
| **AI intervention point** | **Chỉ bước 3:** với các yêu cầu JD mà Rule không tìm thấy bullet khớp trong CV master → AI map sang dự án thật + gợi ý bullet có trích nguồn, hoặc trả "THIẾU". |
| **Mức chọn** | **Workflow** |
| **Rủi ro & người kiểm tra** | AI bịa/nói quá → Rule cờ đỏ + **người dùng** duyệt từng dòng; duyệt qua loa → trong pilot, **một thành viên nhóm khác** đối chiếu chéo CV cuối với hồ sơ dự án; lộ dữ liệu cá nhân → xóa SĐT/email trước khi gửi. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | SV IT đã có CV master, thường gặp JD lạ | Giữ, thêm tần suất 3–5 CV/tuần | Làm rõ phạm vi pilot: chỉ người đang apply đều đặn mới đo được |
| Quy trình | 6 bước chung | Tách rõ bước Rule / AI / người, thêm bước khai báo hồ sơ 1 lần | Sau khi chọn Workflow cần chỉ đúng điểm AI can thiệp |
| AI intervention point | (chưa có) | Chỉ bước 3, chỉ cho yêu cầu Rule không khớp được | Giới hạn AI vào phần mơ hồ; phần còn lại Rule làm được rẻ và chắc hơn |
| Success Metric | 3 metric + theo dõi phụ | Thêm cách đo cụ thể (3 người × 5 JD, người kiểm tra chéo, theo dõi 3 tuần) | Phản biện CP5: metric phải đo được trong pilot, không dựa vào cảm nhận |
| Rủi ro & người kiểm tra | Chỉ có người dùng tự duyệt | Thêm thành viên nhóm kiểm tra chéo trong pilot | Phản biện "duyệt qua loa": người dùng tự duyệt chưa đủ để chứng minh metric (3) |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Đúng sự thật** | Mọi kỹ năng, công nghệ, số liệu, vai trò trong bullet đều có trong hồ sơ dự án | Xuất hiện ≥ 1 kỹ năng/số liệu/vai trò không có trong hồ sơ (vd: hồ sơ ghi "thành viên", bullet ghi "dẫn dắt nhóm") |
| 2 | **Có nguồn** | Mỗi bullet ghi rõ dự án và dòng trong hồ sơ làm căn cứ | Bullet không có nguồn hoặc nguồn không chứa nội dung tương ứng |
| 3 | **Khớp yêu cầu JD** | Bullet nói đúng yêu cầu được map và dùng thuật ngữ của JD một cách tự nhiên | Lạc đề so với yêu cầu, hoặc chỉ nhồi từ khóa không có hành động/kết quả cụ thể |
| 4 | **Trung thực khi thiếu** | Yêu cầu không có dự án tương ứng được đánh dấu "THIẾU" | AI viết bullet "lấp chỗ trống" cho yêu cầu mà người dùng chưa từng làm |
| 5 | **Dùng được ngay** | Người dùng chấp nhận hoặc chỉ sửa ≤ 1 cụm từ | Người dùng phải viết lại > 50% câu |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** | 6/7 người poll có chỉnh CV theo JD; 4/6 poll + 2/2 bạn phỏng vấn (P1, P2) xác nhận viết lại mô tả dự án là bước tốn thời gian nhất (~15–25'/CV); P2 đã có CV master nhưng vẫn mất ~30' với JD lạ; P1 nộp thiếu 1 công ty vì hết giờ. Nhu cầu thực tế rất rõ ràng, lặp lại 3–5 CV/tuần trong mùa apply. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Trung bình** | Thao tác duyệt/sửa 1–2 bullet có trích nguồn rất trực quan. Tuy nhiên, 3/4 người từng dùng AI phải sửa nhiều vì AI bịa thêm kỹ năng (poll Q6); rủi ro người dùng duyệt qua loa dẫn đến CV sai sự thật. Thiết kế đã giảm thiểu bằng: Rule cờ đỏ phát hiện kỹ năng lạ, bắt buộc duyệt từng dòng (không có nút "chấp nhận tất cả"). |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Thấp** | Đầu vào gồm JD (copy trên web) và hồ sơ dự án thật (người dùng tự khai báo 1 lần ~30' từ CV master + repo GitHub). Không cần huấn luyện model phức tạp; dùng prompt chuẩn với LLM có sẵn (GPT-4o/Claude/Gemini) + Rule regex tách từ khóa. Nhóm hoàn toàn làm chủ kỹ thuật này trong pilot. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Thấp** | Chi phí API rất rẻ hoặc miễn phí trong quy mô pilot; bắt buộc xóa bỏ SĐT/email trước khi gửi nội dung cho AI để bảo vệ quyền riêng tư; người dùng tự duyệt và tự nộp CV (không vi phạm đạo đức ứng tuyển/spam tuyển dụng như Agent). |

### 8.2. Kết luận

**Quyết định:** **Go (pilot nhỏ, có điều kiện)**

**Lý do:**
1. **Không có rủi ro nào ở mức Cao:** cả 4 rủi ro (Value, Usability, Feasibility, Viability) đều ở mức Thấp đến Trung bình và đã có phương án kiểm soát chặt chẽ trong thiết kế Workflow (HITL, Rule cờ đỏ chặn kỹ năng lạ, bắt buộc trích nguồn dự án).
2. **Nhu cầu thực tế sắc nét:** 100% người được hỏi gặp khó khăn khi gặp JD "lạ" (yêu cầu chưa có sẵn trong CV master), làm tăng thời gian chỉnh CV lên 30–40 phút/CV.
3. **Mức can thiệp Workflow là tối ưu:** No AI không giải được JD lạ; Rule thuần chỉ khớp từ khóa dễ gây nhồi nhét phản cảm (P3); Agent tự nộp vi phạm boundary đạo đức. Workflow giữ AI ở đúng điểm nghẽn (map & diễn đạt lại) và giữ con người kiểm duyệt từng dòng (Human-in-the-loop).

**Nếu Go — pilot nhỏ nhất (2 tuần):**
- **Quy mô:** 3 thành viên nhóm (Hải, Nhài, Tài) + 2 bạn cùng lớp (như P1, P2) đang tích cực apply Intern/Fresher. Mỗi người thực hiện trên 3–5 JD thật có yêu cầu lạ.
- **Cách triển khai (Zero-code / Prompt chuẩn):**
  - Người tham gia chuẩn bị trước "Hồ sơ dự án thật" (template Markdown: tên dự án, stack, vai trò, công việc cụ thể, kết quả) + CV master hiện có.
  - Sử dụng 1 System Prompt chuẩn trên ChatGPT/Claude/Gemini: Yêu cầu AI chỉ được dùng thông tin trong hồ sơ dự án để map với yêu cầu JD; mỗi bullet gợi ý bắt buộc ghi rõ `[Nguồn: Tên dự án, dòng X]`; yêu cầu nào không có trong hồ sơ phải trả về `[THIẾU]`, tuyệt đối không tự bịa kỹ năng hay số liệu.
  - Người dùng tự kiểm tra từng bullet (chấp nhận / sửa nhẹ / loại) và tự copy vào CV, xuất PDF nộp.
  - Sau mỗi lượt, một thành viên khác trong nhóm kiểm tra chéo CV cuối với hồ sơ dự án để phát hiện kỹ năng lạ lọt lưới.
- **Đo lường các chỉ số thành công:**
  1. Thời gian chỉnh 1 CV JD lạ: bấm giờ thực tế (mục tiêu: từ ~40' giảm xuống ≤ 20').
  2. Tỉ lệ bullet AI được chấp nhận hoặc sửa nhẹ: đạt ≥ 60%.
  3. Số kỹ năng/số liệu bịa lọt vào CV cuối: = 0 (kiểm tra chéo).
  4. Thời gian khai báo hồ sơ dự án ban đầu: đo xem có vượt quá 30 phút không.

**Nếu Not Yet — cần kiểm chứng gì trước:**
- *(Áp dụng nếu pilot phát sinh nghi ngờ trước khi mở rộng)*:
  - Kiểm chứng rào cản khai báo: Cho 3 sinh viên ngoài nhóm thử điền "Hồ sơ dự án thật" xem tỉ lệ bỏ cuộc và thời gian thực tế; nếu > 45 phút thì phải đổi sang cơ chế import bán tự động từ README GitHub hoặc CV master.
  - Đánh giá độ tin cậy offline (eval benchmark): Chạy thử prompt trên 15 cặp JD lạ – hồ sơ dự án để đo tỉ lệ hallucination (tự bịa thêm công nghệ ngoài hồ sơ) trước khi đưa cho người dùng thật sử dụng.

**Nếu No-Go — nên làm gì thay AI:**
- *(Phương án dự phòng / Fallback khi AI không đạt yêu cầu)*:
  - **Quay về No AI (Quy trình + Template module hóa):** Chuẩn bị sẵn bộ CV master chia theo 3 định hướng rõ ràng (Backend, Frontend, Fullstack), xây dựng sẵn ngân hàng 30–40 bullet points mô tả đa dạng các khía cạnh dự án (tối ưu hóa, bảo mật, thiết kế CSDL, CI/CD...) để người dùng bật/tắt hoặc copy-paste thủ công.
  - **Kết hợp Rule thuần:** Dùng script regex hoặc extension so khớp từ khóa miễn phí (như phiên bản free của Jobscan/Teal) để bôi đen từ khóa còn thiếu giữa JD và CV; người dùng tự tay viết bổ sung dựa trên checklist, tuyệt đối không dùng AI tạo văn bản.

**Ngưỡng dừng (nếu sau … mà … thì quay về …):**
- **Về tính trung thực (Chất lượng):** Nếu trong quá trình pilot phát hiện **≥ 1 kỹ năng hoặc số liệu bịa đặt** lọt vào bản CV cuối cùng mà người dùng không phát hiện ra (chỉ lộ khi người khác kiểm tra chéo) → **Dừng pilot ngay lập tức** để bổ sung bộ Rule lọc chặn từ khóa trước khi hiển thị cho người dùng.
- **Về tính hữu ích (Usability & Thời gian):** Nếu sau 2 tuần pilot (tối thiểu 10 CV) mà **tỉ lệ bullet phải viết lại hoàn toàn > 50%** hoặc thời gian chỉnh CV vẫn kéo dài **> 30 phút/CV** → **Dừng sử dụng AI, quay về phương án No AI** (thư viện bullet module hóa + checklist từ khóa thủ công).
- **Về rào cản gia nhập (Onboarding):** Nếu thời gian khai báo hồ sơ dự án ban đầu **> 45 phút** hoặc **≥ 2/5 người tham gia pilot bỏ cuộc** ở bước khai báo → Dừng việc bắt buộc điền form hồ sơ riêng, chuyển sang cho phép người dùng nạp thẳng CV master hiện có.

---

## 9. Hạn chế và hướng tiếp theo

**Hạn chế:**

- **Mẫu kiểm chứng nhỏ và thiên lệch:** 3 phỏng vấn + poll 8 người, gần như toàn bộ là bạn cùng lớp AI20K (cùng khóa, cùng hướng IT). Kết quả chưa đại diện cho sinh viên IT nói chung, nhất là người chưa quen dùng công cụ AI.
- **Baseline thời gian là tự khai, chưa bấm giờ thật:** con số ~30'/CV và ~16–21' cho bước viết lại đến từ trí nhớ của người dùng (Nhài, P1, P2, poll Q3), chưa đo bằng đồng hồ trên JD thật.
- **Tỉ lệ JD "lạ" mới có 1 nguồn:** con số "~2/3 JD là lạ" chỉ đến từ P2. Đây là giả định quyết định việc No AI (CV master) có đủ hay không: nếu tỉ lệ JD lạ thấp, CV master có thể đã đạt target mà không cần AI.
- **Giả định #4 chưa được chứng minh:** chưa có bằng chứng AI gợi ý tiết kiệm được nhiều thời gian hơn thời gian người dùng phải duyệt; poll Q6 còn cho tín hiệu ngược (3/4 người phải sửa nhiều bản AI viết).
- **Chưa thử tool có sẵn bằng JD thật:** bảng research dựa trên trang giới thiệu của Jobscan và Teal, nhóm chưa tự chạy thử trên JD và CV thật để biết các tool này đã giải được bao nhiêu phần bottleneck.
- **Kết quả cuối cùng (được gọi phỏng vấn) không đo được trong lab:** tỉ lệ phản hồi phụ thuộc thị trường và mất 1–3 tuần; P3 còn cho thấy khớp từ khóa không đảm bảo qua vòng hồ sơ. Mối liên hệ "CV khớp JD hơn → nhiều phản hồi hơn" vẫn là giả định.
- **Chỉ có 1 góc nhìn từ phía người lọc CV (P3):** chưa đủ để kết luận nhà tuyển dụng đánh giá CV đã tailor thế nào.
- **Rủi ro dữ liệu cá nhân:** gửi CV và hồ sơ dự án cho dịch vụ AI bên ngoài; nhóm mới đặt boundary "xóa SĐT/email", chưa xem chính sách lưu dữ liệu của từng công cụ.

**Hướng tiếp theo:**

1. **Trước pilot — kiểm phương án đơn giản hơn:** mỗi thành viên lấy 5 JD thật gần nhất, (a) đếm tỉ lệ JD "lạ" so với CV master, (b) chạy thử Teal/Jobscan bản miễn phí. Nếu CV master + tool có sẵn + checklist duyệt đã đạt ≤ 20'/CV thì hạ mức can thiệp, không dựng Workflow riêng.
2. **Pilot theo mục 8:** 3 người × 5 JD thật, bấm giờ từng bước, ghi tỉ lệ bullet được chấp nhận/sửa nhẹ, một thành viên khác đối chiếu chéo CV cuối với hồ sơ dự án (metric 0 kỹ năng bịa).
3. **Đo bước khai báo hồ sơ dự án:** thời gian khai báo và số người hoàn thành; nếu > 45' hoặc < 2/3 người hoàn thành thì chuyển sang nhập từ CV master (như đã ghi ở mục 5).
4. **Phỏng vấn thêm 2–3 người lọc CV** (HR, tech lead) để kiểm giả định "CV khớp JD và cụ thể → tăng khả năng qua vòng hồ sơ".
5. **Dựng bộ eval 10 cặp** (JD + hồ sơ dự án → bullet mong đợi) và chấm theo 5 tiêu chí ở mục 7, dùng làm chuẩn đánh giá trong pilot.
6. **Candidate cho vòng sau:** "Không có feedback sau khi luyện phỏng vấn" (Tài, #7) là bước kế tiếp trên cùng hành trình tìm việc; "Soát quy cách nộp lab" (Hải, #6) làm thành script nội bộ của nhóm, không cần AI.

## 10. Tài liệu tham khảo

1. Jobscan — *Free Resume Scanner: Find the Keywords You're Missing*. https://www.jobscan.co/resume-matcher — công cụ so CV với JD, cho Match Rate; dùng ở mục 3.3 (research giải pháp có sẵn).
2. Teal — *Resume Job Description Match*. https://www.tealhq.com/tool/resume-job-description-match — so CV với JD, đánh dấu từ khóa, gợi ý bullet; dùng ở mục 3.3.
3. Teal Help Center — *How to tailor your resume for a specific job*. https://help.tealhq.com/en/articles/14435726-how-to-tailor-your-resume-for-a-specific-job — pattern CV master + chọn bullet theo JD (phương án No AI); dùng ở mục 3.3 và 6.2.
4. Rob Fitzpatrick — *The Mom Test*. https://www.momtestbook.com/ — nguyên tắc phỏng vấn hỏi về hành vi đã xảy ra; dùng ở mục 3.2.
5. Google PAIR — *People + AI Guidebook: User Needs + Defining Success*. https://pair.withgoogle.com/chapter/user-needs/ — augment hay automate, báo nhầm hay bỏ sót; dùng ở mục 6.4.
6. Anthropic — *Building effective agents* (12/2024). https://www.anthropic.com/research/building-effective-agents — phân biệt Workflow và Agent, chọn giải pháp đơn giản nhất; dùng ở mục 6.1–6.2.
7. Marty Cagan, SVPG — *The Four Big Risks* (2017). https://www.svpg.com/four-big-risks/ — Value, Usability, Feasibility, Viability; dùng ở mục 8.1.
