# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).

## 1. Thông tin học viên

- Họ tên: Trần Nguyễn Anh Phong
- MSSV: 2A202603629
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomNewbie
- Link repository: https://github.com/duy321111/K5-L3-Day02-NhomNewbie-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)
Tôi là Phong, sinh viên năm 3 đang học 6 môn/kỳ của ngành Khoa học Máy tính trường Đại học Công Nghệ Thông Tin, ĐHQG TP.HCM. Công việc mỗi tuần là gom slide, giáo trình, ghi chú của 6 môn học về một chỗ rồi tự tóm tắt lại để cuối kỳ làm đề cương ôn thi.
Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tới sáng chủ nhật, tôi muốn gom slide, giáo trình, ghi chú của 6 môn học về một chỗ rồi tự tóm tắt lại để cuối kỳ làm đề cương ôn thi | Sinh viên | Mất khoảng 32-40 phút/tuần/môn |
| 2 | Lặp lại | Mỗi tuần khi tới sáng thứ hai, tôi phải kiểm tra lịch học, deadline và thông báo ở LMS, email trường, Zalo lớp để biết tuần này phải nộp gì | Sinh viên |	20-30 phút/tuần, vẫn thỉnh thoảng sót |
| 3 | Lặp lại | Khi làm đồ án (báo cáo), tôi phải định dạng lại tài liệu tham khảo (trích dẫn, danh mục tài liệu) cho mỗi bài theo chuẩn yêu cầu | Sinh viên | 30-45 phút/bài, hay sai format |
| 4 | Tốn thời gian | Khi làm đồ án, tôi  cần đọc và tổng hợp nhiều tài liệu Tiếng Anh để viết phần lý thuyết | Sinh viên | 1-2 giờ/bài, khó hiểu và mất thời gian dịch |
| 5 | Pain từ người khác | Gần tới deadline, nhóm trưởng hỏi tiến độ task nhưng report chưa sẵn sàng | Nhóm trưởng, thành viên | Trễ deadline cuả bản thân và cả nhóm |
| 6 | AI có thể tốt hơn | Khi gần tới kỳ thi, có nhiều đề thi và đáp án nhưng từ nhiều nguồn khác nhau, tôi muốn tổng hợp lại để ôn tập hiệu quả | Sinh viên | 1-2 tiếng/1 đề, đáp án chưa chắc chuẩn |
| 7 | Pain từ người khác | Gần tới deadline, nhóm trưởng không rõ ai làm phần nào, tin nhắn phân việc bị trôi trong box chat, sát giờ mới phát hiện thiếu nội dung | Cả nhóm  | 2 nhóm nhỏ nộp sát giờ |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.


---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Gom và tóm tắt tài liệu học tập | Workflow rõ, mất nhiều thời	gian, metric rõ | Gom và tóm tắt chưa biết cái nào dài hơn, tùy thuộc tình huống |
| 2 | Kiểm tra lịch học, deadline và thông báo | Workflow ngắn, rõ | Tần suất sót deadline chưa đếm (bao nhiêu lần/kỳ, hậu quả gì). LMS có xuất lịch được không, hay chỉ phần thông báo viết tự do ở Zalo mới cần AI? |
| 3 | Đọc và tổng hợp tài liệu tiếng Anh | Actor rõ, impact đo được, có thể so sánh No AI, Workflow và Agent | Thời gian chủ yếu mất ở đọc hiểu hay ở tra thuật ngữ và dịch? Số bài mỗi đồ án chưa điền. AI có tóm tắt sai hoặc bịa trích dẫn không, và công cụ dịch thông thường đã đủ chưa? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tới sáng chủ nhật, tôi muốn gom slide, giáo trình, ghi chú của 6 môn về một chỗ và có sẵn bản tóm tắt, để cuối kỳ có đề cương ôn thi mà không phải dồn việc vào phút chót |
| Actor | Sinh viên (tôi) đang học 6 môn/kỳ |
| Thời điểm / bối cảnh | Sáng chủ nhật hằng tuần, tài liệu nằm ở LMS, Zalo, Drive, ghi chú tay |
| Quy trình hiện tại (3–7 bước) | 1. Gom file từ LMS/Zalo/Drive (7') → 2. Đọc lại slide + giáo trình của tuần (14') ← BOTTLENECK → 3. Rút ý chính, ghi lại (9') → 4. Đối chiếu ghi chú tay/ghi chú bạn (4') → 5. Lưu vào tài liệu tổng hợp (2') (giả định) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2: đọc lại để rút ý, ~14 phút/môn/tuần (giả định, cần bấm giờ) |
| Impact (nếu không giải thì sao) | ~36 phút/môn × 6 môn ≈ 3,6 giờ/tuần, khoảng 50 giờ/kỳ (15 tuần). Nếu không làm đều thì dồn cuối kỳ, ôn dàn trải và dễ sót chương |
| Success metric (baseline → target) | Baseline 36 phút/môn/tuần → target ≤15 phút/môn/tuần; đề cương phủ ≥90% chủ đề trong đề cương môn học của giảng viên |
| Phương án không dùng AI | Dùng đề cương môn học làm khung, chỉ ghi ý chính ngay trên slide khi nghe giảng, chia môn với 2-3 bạn rồi trao đổi tóm tắt |
| Giả thuyết về AI (nếu có) | AI đọc nhiều file và rút ý theo từng chương nhanh hơn, sinh viên chỉ duyệt và bổ sung. Cần kiểm chứng: AI có sót ý quan trọng không |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
1. Gom file từ LMS/Zalo/Drive (7')
→ 2. Đọc lại slide + giáo trình của tuần (14') ← BOTTLENECK
→3. Rút ý chính, ghi lại (9')
→ 4. Đối chiếu ghi chú tay/ghi chú bạn (4')
→ 5. Lưu vào tài liệu tổng hợp (2')
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu tuần mới vào sáng thứ hai, tôi muốn biết ngay tuần này phải nộp gì, hạn nào, nộp ở đâu, để không sót hoặc nộp sai |
| Actor | Sinh viên (nhóm trưởng còn phải nhắc cả nhóm) |
| Thời điểm / bối cảnh | Sáng thứ hai hằng tuần, thông tin nằm ở LMS, email trường, Zalo lớp |
| Quy trình hiện tại (3–7 bước) | 1. Mở LMS xem lịch/deadline (6') → 2. Mở email trường (6') → 3. Lướt Zalo lớp tìm thông báo (9') ← BOTTLENECK → 4. Chép deadline vào lịch/ghi chú (4') → 5. Kiểm tra hình thức nộp (1') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: thông báo viết tự do lẫn trong chat Zalo |
| Impact (nếu không giải thì sao) | 20-30 phút/tuần ≈ 5-7 giờ/kỳ, cộng việc “thỉnh thoảng sót” (cần đếm số lần/kỳ và hậu quả: trừ điểm, nộp trễ) |
| Success metric (baseline → target) | Baseline 20-30 phút/tuần → target ≤5 phút/tuần; số lần sót deadline/kỳ: từ ___ xuống 0 |
| Phương án không dùng AI | Đồng bộ lịch LMS vào Google Calendar (nếu LMS cho xuất lịch), bộ lọc email trường, nhờ lớp trưởng ghim thông báo trên Zalo |
| Giả thuyết về AI (nếu có) | AI chỉ đáng dùng cho phần đọc thông báo viết tự do ở Zalo. LMS và email có cấu trúc thì Rule là đủ |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
1. Mở LMS xem lịch/deadline (6')
→ 2. Mở email trường (6')
→ 3. Lướt Zalo lớp tìm thông báo (9') ← BOTTLENECK
→ 4. Chép deadline vào lịch/ghi chú (4')
→ 5. Kiểm tra hình thức nộp (1')
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm đồ án, tôi muốn nắm nhanh ý chính của các tài liệu tiếng Anh, để viết phần lý thuyết mà không mất 1-2 giờ cho mỗi bài |
| Actor | 	Sinh viên (tôi) làm đồ án (báo cáo) |
| Thời điểm / bối cảnh | Giai đoạn viết phần cơ sở lý thuyết của đồ án, tài liệu là bài báo/chương sách tiếng Anh |
| Quy trình hiện tại (3–7 bước) | 1. Chọn bài, đọc abstract (10') → 2. Đọc hiểu và tra thuật ngữ/dịch (40') ← BOTTLENECK → 3. Ghi ý chính + nguồn (20') → 4. Tổng hợp, viết vào phần lý thuyết (20') = ~90' (giả định chia bước, lấy mốc giữa của 1-2 giờ) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2: đọc hiểu và tra thuật ngữ, ~40 phút/bài (giả định; cần tách “đọc” và “dịch” để bấm giờ riêng) |
| Impact (nếu không giải thì sao) | ~90 phút/bài. Nếu mỗi đồ án đọc ~5 bài thì ≈ 7,5 giờ/đồ án (số bài cần bạn điền). Nếu không giải: viết chậm, hiểu sai, dễ trễ hạn |
| Success metric (baseline → target) | Baseline 90 phút/bài → target ≤50 phút/bài; 100% trích dẫn đúng nguồn và đúng số trang |
| Phương án không dùng AI | Đọc theo thứ tự abstract → kết luận → hình/bảng → phần liên quan; công cụ dịch + từ điển chuyên ngành; công cụ quản lý trích dẫn |
| Giả thuyết về AI (nếu có) | AI tóm tắt và giải thích thuật ngữ giúp rút ngắn bước đọc hiểu. Rủi ro lớn: AI tóm tắt sai hoặc bịa trích dẫn, nên bắt buộc đối chiếu bản gốc |
| Cảm nhận nhanh | Workflow (có người kiểm) |

Quy trình nháp hiện tại:

```text
1. Chọn bài, đọc abstract (10')
→ 2. Đọc hiểu và tra thuật ngữ/dịch (40') ← BOTTLENECK
→ 3. Ghi ý chính + nguồn (20')
→ 4. Tổng hợp, viết vào phần lý thuyết (20')
```

### Card muốn pitch nhất

- Card số: #1 (Gom và tóm tắt tài liệu học tập)
- Vì sao: 
	- Impact lớn nhất trong các card (3,6 giờ/tuần, 50 giờ/kỳ)
	- Việc lặp lại hằng tuần nên dễ bấm giờ và kiểm chứng ngay trong tuần này.
	- Bottleneck nhiều khả năng là một bước cụ thể (đọc lại để rút ý), đúng chỗ AI có lợi thế (đọc nhiều nguồn, tổng hợp).
	- Có thể so sánh rõ No AI / Workflow / Agent, và có nhiều bạn cùng gặp nên dễ tìm bằng chứng ở các bước sau.
- Câu hỏi muốn nhóm phản biện: Ở bước đọc và rút ý, nên để AI rút ý rồi sinh viên chỉ duyệt, hay để sinh viên tự rút ý rồi AI chỉ kiểm tra sót? Cách nào ít rủi ro hơn khi AI có thể bỏ sót chương quan trọng mà sinh viên không biết?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Bottleneck “14 phút” và cách chia 5 bước là suy đoán, chưa có bằng chứng bấm giờ | Đồng ý | Ghi rõ là giả định; lên kế hoạch bấm giờ từng bước cho 1 môn trong 1 tuần rồi cập nhật số vào card  |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Chọn ra top 3 problem card của bản thân và trình bày | 2/3 card chấm điểm ở top 2 và 3, không được chọn làm card của nhóm |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:<Br> 1. Card 1 của Duy: Nếu có hướng dẫn từng bước thì có dễ làm hơn không?<Br> 2. Card 2 của Duy: Thường tìm trong slide hay video mà mất nhiều thời gian vậy?<Br> 3. Card 1 của Trường: Nếu có sẵn mẫu đề cương thì có làm nhanh hơn không?<Br> 4. Card 2 của Trường: Tìm tài liệu trên Drive hay Notion lâu hơn?<Br> 5. Card 3 của Trường: Làm sao biết mình yếu phần nào, hay chỉ tự cảm thấy vậy?<Br> 6. Card 2 của Sơn: Nếu danh sách trên Lark chưa cập nhật thì có ảnh hưởng nhiều không? | 1. Chưa biết hướng dẫn từng bước có giúp được không<Br> 2. Chưa rõ loại tài liệu nào khó tìm nhất<Br> 3. Chưa thử làm bằng mẫu có sẵn<Br> 4. Chưa rõ chỗ nào mất thời gian nhất<Br> 5. Chưa có cách xác định rõ phần yếu<Br> 6. Chưa rõ mức độ ảnh hưởng khi cập nhật chậm |
| Nhận phản biện | Câu hỏi tôi nhận được:<Br> 1. Card 1 (Gom và tóm tắt tài liệu), Duy: Trong mấy bước đó thì bước nào mất thời gian nhất?<Br> 2. Card 1 (Gom và tóm tắt tài liệu), Sơn: Nếu chia nhau làm đề cương rồi gửi cho nhau thì có nhanh hơn không?<Br> 3. Card 2 (Kiểm tra lịch học và deadline), Duy: Lần gần nhất quên deadline là khi nào, có bị ảnh hưởng gì không?<Br> 4. Card 2 (Kiểm tra lịch học và deadline), Trường: Nếu ghi deadline vào Google Calendar thì có còn bị quên không?<Br> 5. Card 3 (Đọc tài liệu tiếng Anh), Duy: Mất thời gian do đọc không hiểu hay do phải dịch nhiều từ?<Br> 6. Card 3 (Đọc tài liệu tiếng Anh), Sơn: Nếu dùng Google Dịch thì có nhanh hơn không? | 1. Chưa đo từng bước<Br> 2. Chưa thử chia nhau làm<Br> 3. Chưa rõ quên bao nhiêu lần<Br> 4. Chưa thử dùng lịch để theo dõi<Br> 5. Chưa rõ bước nào mất nhiều thời gian<Br> 6. Chưa so sánh với Google Dịch |
| Quy trình nhóm | Quy trình hiện tại có actor/input/output/thời gian, bottleneck; quy trình tương lai có bước con người kiểm tra, boundary, phương án quay về; có bảng before/after. Có 2 sơ đồ quy trình, ảnh trích dẫn đầy đủ | Giúp nhóm xác định bottleneck và hạn chế của quy trình hiện tại; làm cơ sở đề xuất quy trình tương lai có sự kiểm tra của con người và phương án fallback. Hoàn thiện nội dung phân tích Before/After, giúp bài nhóm có cơ sở so sánh, đánh giá tính khả thi và minh họa rõ ràng bằng 2 sơ đồ workflow |
| Problem Statement | Làm Problem Statement V0 | Tạo cơ sở ban đầu để nhóm thống nhất vấn đề cần giải quyết, xác định phạm vi và các pain points chính. Làm nền tảng cho việc phân tích quy trình hiện tại, xác định bottleneck và phát triển các đề xuất cải tiến ở những phần tiếp theo của bài nhóm |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Check lại lỗi của các problem | Có thể phát hiện ra lỗi sai | | |
| CP2 Problem Card | | | | |
| CP5–6 Problem Statement | 1. Dùng AI để nhờ code hộ 2 sơ đồ trong Mermaid<Br> 2. Trình bày các bảng 1 cách nhanh chóng<Br> 3. So sánh trên 2 workflow để tạo bảng Before/After<Br> 4. Nhờ AI phản biện phần Problem Statement v0 | Rút gọn thời gian | 1. AI trình bày Input/Output của các bước workflow không được khớp nhau lắm | 1. Chỉnh lại theo nhận định của mình<Br> 2. Trả lời phản biện của AI và đề xuất cách sửa |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
- Khi nghe top 3 problems của các bạn khác, em nhận thấy cùng một vấn đề, cùng một bối cảnh (như học tập của em, Trường và Duy) thì mỗi người đều có những cách nhìn ra các vấn đề khác nhau. Những vấn đề tưởng như đơn giản thì khi phân tích sâu hơn lại ra nhiều vấn đề khác như thời gian. Ví dụ ở card của em thì có phần đọc và tóm tắt ý chính được bỏ thành 1 bottleneck, nhưng nếu đo thời gian riêng của 2 hành động thì hành động nào tốn thời gian hơn lại trở thành bottleneck.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
- Không có.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
- Có. Đối với Problem Card 2 của bản thân thì em từng muốn dùng AI để tự động hóa hoàn toàn. Nhưng sau khi bị phản biện thì em nhận thấy rằng bước dùng AI để check LMS hay Gmail là khó vì có bảo mật và cũng không cần thiết khi có cấu trúc và chỉ cần Rule là đủ.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
- Không có.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
- Điều khó nhất đối với em là xác định đúng vấn đề và giới hạn phạm vi cần giải quyết. Ngoài ra, việc chuyển một vấn đề thành metric có thể đo lường cũng là một thử thách.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
- Nếu được làm lại, em sẽ dành nhiều thời gian hơn để có thể kiểm chứng các problem, đặc biệt là về mặt thời gian. Hầu hết các problem chỉ được ước lượng thời gian khi trải qua trong quá khứ chứ chưa được đo đạc lại một cách cụ thể, nên các số liệu chỉ là giả định. EM cũng muốn phản biện nhóm nhiều hơn về các bottleneck, metric đánh giá và boundary giữa công việc của AI với con người.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
- Problem: Sinh viên đại học dựng đề cương cho các môn học từ slide, giáo trình và ghi chú Notion, Drive.
- Quy trình hiện tại: (1) sinh viên tìm và mở lại tài liệu; (2) đọc lướt để xác định các chương; (3) tóm tắt từng chương thành ý chính; (4) đánh dấu phần chưa nắm; (5) gộp thành đề cương; (6) xuất ra để ôn.
- Quy trình tương lai: Mỗi đợt ôn thi, với từng môn: (1) script gom tài liệu vào một thư mục; (2) sinh viên lấy danh sách chương chuẩn từ đề cương giảng viên; (3) AI tóm tắt từng chương kèm chỉ nguồn; (4) script đối chiếu độ phủ chương; (5) sinh viên duyệt, sửa, đánh dấu phần chưa nắm; (6) sinh viên gộp thành đề cương và xuất để ôn.
- Metric: Giảm thời gian dựng đề cương (từ 150 - 180 xuống dưới 60 phút/1 môn).
- Boundary: AI không tự quyết định chương nào được bỏ qua; không tự đánh dấu một chủ đề là “đã nắm”; không thêm kiến thức ngoài tài liệu đã gom; không sửa hoặc xóa tài liệu gốc. Sinh viên không dùng bản nháp để ôn khi chưa duyệt xong. Nếu AI sai hoặc ngừng hoạt động, sinh viên quay về tự tóm tắt theo template cũ.
- Mức can thiệp AI: chọn Workflow.
- Quyết định: Not yet.
---

## 7. Tài liệu tham khảo

- Bài mẫu được cung cấp: Day 2 - Lab 2 Assignment - Deliverables Example.
- Slide: Discovery & Problem Framing.
