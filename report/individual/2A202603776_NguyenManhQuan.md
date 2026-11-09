# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Nguyen Manh Quan
- MSSV:2A202603776
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:H2
- Link repo nhóm:https://github.com/tran-hai21/K5-L3B-Day02-H2-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Mỗi tối chủ nhật đều phải xem lại mức chi tiêu cho 1 tuần vừa rồi để có thể đưa ra nhưng phương án chi tiêu cho tuần tới | Quân |1 tuần 1 lần, 1 lần 45 phút |
| 2 |Cần đọc, tổng hợp nhiều thông tin | Khi có quá nhiều bài tập deadline cùng hạn, tôi muốn biết nên ưu tiên làm việc nào trước, để không trễ việc cũng như ảnh hưởng xấu đến kết quả học tập| Quân | Nhận điểm thấp vì miss mất 1 bài tập có deadline sớm hơn nhưng cái |
| 3 |Tốn thời gian |Khi tôi muốn Tìm lại 1 câu trả lời cũ, 1 ảnh, file hay đường link quan trọng trong discord trong Discord | Quân |15 - 30 phút / lần |
| 4 |Cần đọc, tổng hợp nhiều thông tin| Khi phải đọc nhiều paper khoa học, tài liệu kỹ thuật dài hoặc tài liệu thư viện mới trước deadline, tôi muốn có cách tóm tắt nhanh phương pháp và kết quả chính để kịp chọn hướng thử nghiệm cho đồ án/nghiên cứu|Quân | 2 - 3 lần / tuần, mất 2 - 3 tiếng mỗi lần đọc tài liệu nhưng khó nhớ hết để so sánh|
| 5 |Tốn thời gian |hi nhận task dự án mới/thực tập, luồng thảo luận nằm rải rác ở nhiều thread, tôi muốn gom lại thành một tài liệu tóm tắt yêu cầu để code đúng luồng ngay từ đầu. |Quân |Mất 1 - 2 ngày làm sai hướng hoặc phải hỏi lại mentor nhiều lần|


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.
Dùng AI gợi ý thêm 4 và 5 dữ lại 4 vì nó khá đúng và thiết thực nhưng lại không nhớ ra
-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp & so sánh paper nghiên cứu (#4)|	Quy trình rõ ràng, tốn nhiều giờ đọc lặp đi lặp lại; bài toán học thuật đo lường thời gian rất cụ thể|.	Khả năng AI bịa thông tin về công thức toán hoặc benchmark số liệu|
| 2 | Ưu tiên & lập lịch bài tập đa môn (#2)| Khó khăn khi dồn nhiều deadline; tác động trực tiếp tới điểm số| Sinh viên có tuân thủ lịch đề xuất hay không hay AI có đề xuất đúng hay  |.
| 3 |Tìm lại tài liệu / lời giải trong Discord (#3)| Tần suất gặp nhiều, tìm kiếm mặc định của Discord kém hiệu quả với ngữ cảnh dài hoặc code/ảnh đính kèm | Giới hạn quyền truy cập bot/API vào server và bảo mật dữ liệu chat riêng tư|

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận đề tài đồ án/khóa luận có nhiều paper dài (10–20 trang PDF), tôi muốn nhanh chóng trích xuất bài toán, phương pháp, bộ dữ liệu và kết quả benchmark chính của từng bài vào bảng đối chiếu, để chọn đúng baseline và viết tổng quan đề tài kịp tiến độ. |
| Actor | Sinh viên năm 4 ngành Khoa học Máy tính làm đồ án tốt nghiệp / nghiên cứu khoa học. |
| Thời điểm / bối cảnh | Giai đoạn chuẩn bị đề cương hoặc giữa các đợt milestone báo cáo tiến độ với giảng viên hướng dẫn. |
| Quy trình hiện tại (3–7 bước) | 1. Tải 5–7 file PDF từ arXiv/Google Scholar · 2. Đọc lướt Abstract, Introduction và Conclusion · 3. Đọc sâu phần Methodology để hiểu kiến trúc/thuật toán · 4. Đọc phần Experiments để tìm benchmark & metrics so sánh · 5. Tự ghi chép và tổng hợp vào bảng Notion/Sheets · 6. Viết đoạn so sánh tổng quan. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & 4 (Đọc sâu kiến trúc và đối chiếu kết quả thực nghiệm): Mất khoảng 150 phút/paper, dễ bị ngợp bởi thuật ngữ toán, phải đọc đi đọc lại để nhặt đúng con số so sánh. |
| Impact (nếu không giải thì sao) | Mất 15–20 tiếng cho mỗi đợt làm báo cáo; dễ bỏ sót baseline quan trọng dẫn đến chọn sai phương pháp thực nghiệm hoặc bị giảng viên yêu cầu làm lại từ đầu. |
| Success metric (baseline → target) | 150 phút/paper → dưới 40 phút/paper; trích xuất chính xác 100% tên tập dữ liệu, độ đo (accuracy, F1, latency) và điểm cải tiến cốt lõi. |
| Phương án không dùng AI | Dùng Notion template cố định sẵn các cột cần điền kết hợp kỹ năng đọc lướt theo cấu trúc bài báo; giảm thời gian kẻ bảng nhưng vẫn mất nguyên 70 phút tự bóc tách chi tiết kỹ thuật. |
| Giả thuyết về AI (nếu có) | AI (kết hợp Document Parser và RAG) tự động rút trích các trường thông tin kỹ thuật cốt lõi (Dataset, Model architecture, Metrics, Limitations) kèm số trang trích dẫn để sinh viên chỉ việc bấm xác minh lại.|
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```
HIỆN TẠI — 150 phút/paper

[1. Tải PDF: 10'] 
→ [2. Đọc lướt Abstract/Intro: 20'] 
→ [3. Đọc sâu Methodology: 45']  ← BOTTLENECK
→ [4. Tìm số liệu Experiments: 25'] ← BOTTLENECK 
→ [5. Tổng hợp vào bảng Notion/Sheets: 30'] 
→ [6. Viết tổng quan: 20']

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhiều bài tập lớn và đồ án dồn cùng một tuần hạn, tôi muốn nhanh chóng đánh giá độ khó kỹ thuật và sắp xếp thứ tự ưu tiên thực hiện, để không bỏ sót bài có hạn chót sớm và tối ưu hóa điểm số. |
| Actor | Sinh viên năm 4 ngành Khoa học Máy tính học song song nhiều môn chuyên ngành và đồ án. |
| Thời điểm / bối cảnh | Giữa kỳ hoặc cuối kỳ, các giảng viên đồng loạt mở cổng nộp bài tập lớn trong cùng 1–2 tuần.|
| Quy trình hiện tại (3–7 bước) | 1. Vào LMS/Teams/Canvas gom danh sách tất cả deadline · 2. Đọc lướt yêu cầu kỹ thuật từng bài (setup môi trường, code, viết báo cáo) · 3. Ước lượng công sức và thời gian hoàn thành từng bài · 4. Cân nhắc trọng số điểm và thời hạn nộp · 5. Sắp xếp thứ tự làm vào to-do list · 6. Bắt đầu làm bài đầu tiên. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & 4 (Ước lượng công sức và cân nhắc độ ưu tiên): Mất khoảng 25 phút, hay bị rối trí và tê liệt quyết định (decision paralysis) vì không rõ task nào tốn nhiều thời gian debug hơn. |
| Impact (nếu không giải thì sao) | Dễ đánh giá sai khối lượng công việc, sa đà vào bài chiếm trọng số điểm nhỏ dẫn đến miss deadline bài quan trọng hơn, bị trừ điểm hoặc rớt môn. |
| Success metric (baseline → target) | 40 phút lập lịch → dưới 10 phút; số bài bị nộp trễ hoặc nộp thiếu yêu cầu giảm từ 1–2 bài/kỳ xuống 0 bài.|
| Phương án không dùng AI | Dùng ma trận Eisenhower (khẩn cấp vs quan trọng) hoặc bảng Google Sheets tự tính theo công thức trọng số ngày còn lại; vẫn tốn thời gian tự đọc chi tiết đề bài để ước lượng độ phức tạp code. |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | Chưa biết |

Quy trình nháp hiện tại:

```
HIỆN TẠI — 40 phút/lần lập lịch

[1. Gom deadline từ LMS/Teams: 5'] 
→ [2. Đọc yêu cầu từng bài: 10'] 
→ [3. Ước lượng công sức kỹ thuật: 15'] ← BOTTLENECK
→ [4. Cân nhắc trọng số & ưu tiên: 10'] ← BOTTLENECK 
→ [5. Lên to-do list / lịch làm: 5'] 
→ [6. Bắt đầu làm: 0']

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi gặp lỗi code hoặc cần tài liệu tham khảo cũ đã từng trao đổi, tôi muốn tìm lại chính xác tin nhắn hướng dẫn, ảnh chụp lỗi hoặc file đính kèm trên Discord, để giải quyết ngay vấn đề kỹ thuật mà không cần hỏi lại mentor hay bạn bè |
| Actor | Sinh viên năm 4 ngành Khoa học Máy tính sinh hoạt trong các nhóm lab nghiên cứu, kênh Discord lớp học hoặc server đồ án. |
| Thời điểm / bối cảnh | Đang ngồi code/debug vào ban đêm hoặc sát giờ nộp bài, nhớ mang máng có người từng giải quyết lỗi tương tự trên server Discord vài tuần trước. |
| Quy trình hiện tại (3–7 bước) | 1. Nhập keyword vào thanh tìm kiếm mặc định của Discord · 2. Lọc theo kênh hoặc người gửi nếu còn nhớ · 3. Cuộn ngược từng thread/hội thoại để đọc ngữ cảnh thảo luận · 4. Kiểm tra mã lỗi, ảnh đính kèm hoặc snippet code xem có đúng trường hợp không · 5. Thử áp dụng giải pháp vào code cá nhân. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & 4 (Cuộn đọc ngữ cảnh và xác nhận đúng giải pháp): Mất khoảng 15–20 phút vì công cụ tìm kiếm Discord chỉ trả về tin nhắn lẻ tẻ, không tóm tắt ngữ cảnh câu trả lời hoàn chỉnh nằm ở đâu trong luồng chat. |
| Impact (nếu không giải thì sao) | Tốn 20–30 phút/lần tìm kiếm vô vọng, đành phải hỏi lại câu hỏi cũ trên nhóm gây loãng tin nhắn, hoặc tốn hàng giờ tự tìm cách fix từ đầu trên Google/Stack Overflow |
| Success metric (baseline → target) | 20 phút/lần tìm → dưới 2 phút/lần; độ chính xác tìm thấy đúng giải pháp/file trong 3 kết quả đầu tiên đạt trên 85% |
| Phương án không dùng AI | Dùng cú pháp tìm kiếm nâng cao của Discord (from:user, has:file, in:channel) kết hợp pin (ghim) tin nhắn quan trọng; hạn chế là không phải ai cũng nhớ cú pháp và không phải tin nhắn hữu ích nào cũng được ghim |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh |Agent |

Quy trình nháp hiện tại:

```
HIỆN TẠI — 15 - 30 phút/lần tìm kiếm

[1. Gõ keyword vào Discord Search: 2'] 
→ [2. Lọc kênh / người gửi: 3'] 
→ [3. Cuộn đọc từng thread tìm ngữ cảnh: 10'] ← BOTTLENECK
→ [4. Kiểm tra code/ảnh đính kèm xem đúng lỗi không: 5'] ← BOTTLENECK 
→ [5. Thử áp dụng giải pháp vào code: 0']

```

### Card muốn pitch nhất

- Card số: 2
- Vì sao: nó rất thiết thực cũng như là rất quan trọng trong cuộc sống hàng ngày không chri đối với sinh viên mà còn cả nhiều người đi làm bận rộn, vv
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|Baseline 150 phút và target trích xuất 100% là cảm tính, phi thực tế| Đồng |Bấm giờ thực tế đọc 3 paper gần nhất: 110–135 phút; hạ target xuống 45 phút và chấp nhận độ chính xác trích xuất ≥ 85% kèm trích dẫn số trang|
|LLM dễ hallucinate số liệu thực nghiệm, mất công kiểm tra lại| Đồng ý | Bổ sung cơ chế grounding: bắt buộc trả về số kèm đoạn text gốc trong PDF để sinh viên hover chuột là đối chiếu được ngay |
|Thay vì dùng AI, có thể tra cứu sẵn trên Papers With Code|Không đồng ý|Các paper mới xuất bản trên arXiv hoặc bài nghiên cứu ngách thuộc đề tài tốt nghiệp chưa hề được cập nhật trên Papers With Code
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
