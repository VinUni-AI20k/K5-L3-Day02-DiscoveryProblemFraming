# Báo cáo cá nhân — 2A202603776_NguyenManhQuan

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Mạnh Quân
- MSSV: 2A202603776
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: H2
- Link repo nhóm: https://github.com/tran-hai21/K5-L3B-Day02-H2-DiscoveryProblemFraming

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
- Câu hỏi muốn nhóm phản biện: Làm thế nào để hệ thống ước lượng được độ khó kỹ thuật thực tế của một bài tập lớn khi đề bài mô tả quá ngắn hoặc sinh viên chưa từng tiếp cận công nghệ đó trước đây?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|Baseline 150 phút và target trích xuất 100% là cảm tính, phi thực tế| Đồng |Bấm giờ thực tế đọc 3 paper gần nhất: 110–135 phút; hạ target xuống 45 phút và chấp nhận độ chính xác trích xuất ≥ 85% kèm trích dẫn số trang|
|LLM dễ hallucinate số liệu thực nghiệm, mất công kiểm tra lại| Đồng ý | Bổ sung cơ chế grounding: bắt buộc trả về số kèm đoạn text gốc trong PDF để sinh viên hover chuột là đối chiếu được ngay |
|Thay vì dùng AI, có thể tra cứu sẵn trên Papers With Code|Không đồng ý|Các paper mới xuất bản trên arXiv hoặc bài nghiên cứu ngách thuộc đề tài tốt nghiệp chưa hề được cập nhật trên Papers With Code
---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày 3 card cá nhân: Card #1 (Bóc tách thông số paper PDF 10–20 trang — Cand #7), Card #2 (Ưu tiên bài tập dồn deadline — Cand #8), Card #3 (Tìm snippet/lời giải Discord — Cand #9). | Card #1 đạt 30/35 điểm, lọt vào shortlist cạnh tranh trực tiếp với bài học bạ của Hải; Card #2 và #3 giúp nhóm mở rộng lăng kính bài toán sinh viên/developer. |
| Phản biện bài của bạn khác | Đặt câu hỏi chất vấn trọng tâm:<br>• Hỏi Hiếu (Card #1 - Rác): *"Khó do người dân thiếu kiến thức hay do hệ thống thu gom chưa đồng bộ?"*<br>• Hỏi Thanh (Card #5 - Ôn thi): *"Làm sao đảm bảo AI không bỏ sót kiến thức hoặc tóm tắt sai nội dung?"*<br>• Hỏi Hải (Card #11 - Đề kiểm tra): *"Làm sao đảm bảo câu hỏi AI tạo ra đúng ma trận 4 mức độ, đánh giá đúng năng lực và không sai kiến thức?"* | Giúp Hiếu nhận ra rào cản phụ thuộc hạ tầng thu gom của bài rác; giúp Hải và Thanh chú trọng rủi ro sai lệch kiến thức chuyên môn. |
| Nhận phản biện | Tiếp nhận phản biện từ nhóm:<br>• Thanh hỏi (Card #1 - Paper): *"Paper nhiều công thức toán và bảng biểu, nếu AI hallucinate thì có mất công dò lại PDF gốc không?"*<br>• Hiếu hỏi (Card #2 - Deadline): *"Chỉ cần sort deadline là xong, trễ hạn do lười chứ AI xếp lịch chắc gì sinh viên đã làm theo?"*<br>• Hải hỏi (Card #3 - Discord): *"Nếu không nhớ đúng từ khóa thì tìm thế nào, bot index có vi phạm riêng tư server không?"* | Tôi đã sửa:<br>• Với Card #1: Bổ sung yêu cầu grounding trích dẫn số trang, hạ target trích xuất từ 100% xuống ≥ 85%.<br>• Với bài toán chung: Thấy rõ xử lý PDF toán/bảng biểu có rủi ro ảo giác cao trong lab, nên chủ động rút bài cá nhân để ủng hộ chọn bài học bạ của Hải vì dữ liệu bảng chuẩn hóa hơn. |
| Gom cluster / cây OST | Đưa Cand #7, #9 vào Cluster B (Bóc tách tri thức), Cand #8 vào Cluster C (Ra quyết định). Cùng nhóm thống nhất Outcome chung: giảm 70%–90% thời gian; kiên quyết gạch bỏ các solution đội lốt opportunity như "Chatbot AI", "RAG pipeline". | Tách bạch nhu cầu thật của người dùng khỏi giải pháp kỹ thuật, định hình đúng nhánh cơ hội giảm tải cho giáo viên. |
| Chọn candidate problem | Cùng nhóm chấm điểm shortlist theo 7 tiêu chí; phân tích trade-off và chủ động rút bài paper (30/35 điểm), ủng hộ chọn bài nhận xét học bạ (34/35 điểm) vì actor rõ, dữ liệu có cấu trúc và impact đo lường cụ thể. | Giúp nhóm đạt đồng thuận 100% chọn bài toán học bạ một cách khách quan, dựa trên tiêu chí khoa học chứ không thiên vị cá nhân. |
| Kiểm chứng / research | Phụ trách chính phần **Research giải pháp kỹ thuật đã có**:<br>• Trực tiếp test nhập dữ liệu vào ChatGPT/Claude web chat, chỉ ra 3 nhược điểm: copy-paste 45 lần tốn thời gian, rủi ro lộ PII, văn phong lệch chuẩn Thông tư 22.<br>• Phân tích hạn chế của Excel Mail Merge (rập khuôn) và gợi ý vnEdu (nghèo nàn). | Cung cấp luận cứ kỹ thuật chứng minh cần một Batch Workflow chuẩn hóa; định vị sản phẩm là công cụ chuẩn bị dữ liệu (Copilot) tương thích với vnEdu. |
| Quy trình nhóm | Phối hợp cùng Hiếu (vẽ sơ đồ 480' → 45') và Thanh (đối chiếu bottleneck 360'):<br>• Phân định ranh giới can thiệp: AI chỉ sinh bản nháp ở Bước 3, không tự ý can thiệp các bước khác.<br>• Thiết kế cơ chế fallback: Nếu AI lỗi hoặc mất mạng, tự động chuyển về bộ mẫu câu Rule-based trên Google Sheets để kịp hạn. | Đảm bảo quy trình có ranh giới rõ ràng và luôn có lối thoát an toàn (fail-safe) cho người dùng. |
| Problem Statement | Cùng nhóm nâng cấp từ v0 lên v1: bổ sung AI intervention point tại Bước 3, ranh giới bảo mật ẩn danh hóa 100% PII (chỉ dùng Mã HS/STT), và gắn cờ các ca đặc biệt (học sinh hòa nhập/biến cố) để GVCN tự viết tay. | Hoàn thiện bản phát biểu vấn đề chặt chẽ, đảm bảo đạo đức AI và an toàn dữ liệu học đường. |
| Mức can thiệp AI | • Tham gia phân tích ma trận Độ mơ hồ (TB) × Độ phức tạp (TB-Cao).<br>• Thiết kế 3 tiêu chí eval: Zero Hallucination (100% khớp điểm), Chuẩn Thông tư 22 (50–90 từ, tích cực), Đa dạng văn phong (trùng lặp < 5%).<br>• Phân tích câu hỏi PAIR: Báo nhầm tệ hơn Bỏ sót → thiết lập Strict Grounding. | Định hình chính xác mức Workflow (Rule → AI → Human → Rule), kiểm soát chặt chẽ luồng dữ liệu và chống ảo giác thông tin. |
| Quyết định | • Phân tích rủi ro Feasibility/Viability (chi phí API < 1.000 VNĐ/lớp).<br>• Đề xuất kịch bản pilot trên 1 lớp (chấm thử 10 em đại diện dải điểm) và chốt ngưỡng dừng: dừng AI nếu GV duyệt < 65% hoặc xuất hiện ảo giác điểm số > 0%. | Đưa ra quyết định Go có điều kiện an toàn, giúp nhóm tự tin về tính khả thi triển khai trong lab. |

---

## 5. Dùng AI

Tôi chủ động chuẩn bị ý tưởng, thực hiện nội dung và chịu trách nhiệm về báo cáo cá nhân; các quyết định chung do nhóm thống nhất. AI đóng vai trò phản biện, hỗ trợ kiểm tra logic và rà soát định dạng.

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm góc nhìn bài toán theo 4 lăng kính. | Gợi ý đúng nỗi đau đọc paper dài (#4) và gom tài liệu dự án (#5). | Đưa ra ý tưởng dạng giải pháp ("cần chatbot") và thiếu số liệu đo lường. | Viết lại theo Job Story chuẩn, gắn dấu hiệu thật (đọc 2–3 paper/tuần, mất 2–3h); bỏ ý #5. |
| CP2 Problem Card | Đóng vai PM phản biện điểm yếu của Card #1 (Paper). | Chỉ ra baseline 150' và target 100% là cảm tính; cảnh báo rủi ro ảo giác số liệu. | Khuyên bỏ bài vì "đã có Papers With Code" (không thực tế với paper mới trên arXiv). | Bác bỏ lời khuyên của AI; bấm giờ đọc thực tế (110–135'), hạ target xuống 45', thêm grounding text gốc. |
| CP4 Research | Tra cứu các giải pháp hiện có (Mail Merge, gợi ý vnEdu). | Liệt kê nhanh các công cụ và từ khóa cộng đồng giáo viên hay dùng. | Đánh giá quá cao ChatGPT web chat, cho rằng chỉ cần prompt mẫu là đủ dùng cho cả lớp. | Tự test thực tế, phát hiện thao tác lặp 45 lần rất chậm và dễ lộ PII → khẳng định cần Batch Workflow. |
| CP5 Quy trình | Gợi ý phân tách các bước giữa Rule, AI và Con người. | Gợi ý tách bước tiền xử lý dữ liệu (Rule) khỏi bước sinh văn bản (AI). | Đề xuất tự động hóa hoàn toàn (AI nộp thẳng vnEdu qua script), bỏ qua giáo viên duyệt. | Bác bỏ phương án tự động hoàn toàn; giữ bước GVCN duyệt (Human-in-the-loop) và thêm fallback Rule. |
| CP5–6 Problem Statement | Rà soát v0 để phát hiện từ ngữ giải pháp và nâng cấp lên v1. | Gợi ý đo lường Success Metric đa chiều (thêm tỷ lệ duyệt và độ trùng lặp). | Chèn nhiều thuật ngữ công nghệ phức tạp (RAG, fine-tuning, vector DB) vào mô tả vấn đề. | Xóa toàn bộ thuật ngữ công nghệ; bổ sung ranh giới ẩn danh PII và điểm can thiệp tại Bước 3. |
| CP6 Mức can thiệp / quyết định | Hỗ trợ cấu trúc 3 cột cho bảng eval và so sánh 4 mức can thiệp. | Cung cấp khung đánh giá rõ ràng (Tiêu chí - Đạt - Không đạt). | Khuyên chọn Agent để "tự động hóa linh hoạt" và lo ngại chi phí API quá cao. | Bác bỏ Agent vì over-engineering; tính lại chi phí (< 1.000 VNĐ/lớp) để khẳng định Viability Thấp; đặt ngưỡng dừng an toàn. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi lắng nghe phần trình bày của các bạn trong nhóm, tôi rút ra ba bài học quan trọng:
- Thứ nhất, bài toán phân loại rác của Hiếu tuy thiết thực nhưng phụ thuộc quá lớn vào hạ tầng vật lý bên ngoài (quy trình thu gom của công ty môi trường). Nếu rác sau phân loại vẫn bị gom chung một xe thì giải pháp AI nhận diện chính xác đến đâu cũng không mang lại giá trị thực tế.
- Thứ hai, bài toán bóc tách paper của tôi và bài toán codebase của Thanh phản ánh đúng áp lực của dân công nghệ. Tuy nhiên, câu hỏi của Thanh về việc *"nếu AI hallucinate số liệu benchmark thì người đọc có phải mở PDF gốc ra dò lại không"* đã chỉ rõ điểm yếu cốt tử: xử lý PDF phi cấu trúc chứa công thức toán và bảng biểu có rủi ro ảo giác rất cao, chi phí kiểm tra lại có khi tốn hơn tự đọc từ đầu.
- Thứ ba, bài toán nhận xét học bạ của Hải cho thấy một bài toán framing chuẩn mực: actor cụ thể (GVCN THPT), bối cảnh định kỳ (cuối kỳ), dữ liệu đầu vào dạng bảng chuẩn hóa, quy chuẩn đầu ra theo Thông tư 22 rõ ràng, và bottleneck 360 phút đo lường được.
- **Bài học lớn nhất:** Một bài toán AI tốt không cần công nghệ thời thượng, mà cần ranh giới dữ liệu rõ ràng, quy trình chuẩn mực và đo lường được giá trị thực tế giải phóng cho người dùng.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm tôi bị cuốn vào bẫy "solution-first" ở giai đoạn CP2 và đầu CP3. Với nền tảng kỹ thuật, phản xạ đầu tiên của cả nhóm là lập tức bàn về giải pháp: với bài paper thì bàn dùng LangChain hay LlamaIndex để làm RAG; với bài học bạ thì hào hứng bàn làm chatbot hoặc viết script Selenium tự động đăng nhập vnEdu để dán điểm.

Nhóm sực tỉnh khi xây dựng Cây Cơ Hội - Giải Pháp (OST) ở CP3. Khi đối chiếu quy tắc *"tầng Opportunity chỉ chứa nhu cầu hoặc nỗi đau, tuyệt đối không chứa tên công cụ"*, nhóm nhận ra các cụm từ "Chatbot AI" hay "Pipeline RAG" đều là giải pháp đội lốt. Nhóm đã xử lý dứt khoát: gạch bỏ toàn bộ tên giải pháp kỹ thuật, đưa bài toán về đúng nhu cầu cốt lõi của giáo viên: *cần hoàn thành nhận xét học bạ cá nhân hóa đúng hạn mà không bị kiệt sức*. Việc này giúp nhóm thoát khỏi định kiến công nghệ và tập trung vào luồng nghiệp vụ thực tế.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đã có một lần đổi ý mang tính quyết định ở CP3: **chủ động rút bài toán trích xuất paper (Candidate #7 đạt 30/35 điểm) để ủng hộ chọn bài toán nhận xét học bạ của Hải (Candidate #10 đạt 34/35 điểm).**

Ban đầu, tôi rất tâm huyết với bài đọc paper vì trực tiếp gặp khó khăn khi làm khóa luận, và tin rằng nhóm hiểu sâu domain này nên làm sẽ dễ. Tuy nhiên, Thanh đã phản biện sắc bén: *"Paper toàn công thức toán và bảng biểu phức tạp. Nếu AI bị ảo giác trích xuất nhầm con số accuracy hay bịa baseline, sinh viên vẫn phải mở PDF gốc dò lại từng dòng, vậy có thực sự giải quyết được nút thắt thời gian không?"*

Câu hỏi này buộc tôi nhìn thẳng vào thực tế: rủi ro hallucination khi bóc tách PDF phức tạp là rất cao, nếu đầu ra thiếu tin cậy thì giải pháp thất bại. Trong khi đó, bài học bạ của Hải có đầu vào dạng bảng Excel chuẩn mực, đầu ra bám sát khung Thông tư 22, khả năng kiểm soát chất lượng và grounding cao hơn nhiều. Nhận thấy tính khả thi vượt trội trong phạm vi lab, tôi đã vui vẻ đổi ý và bỏ phiếu chọn đề tài học bạ.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Quá trình kiểm chứng và research ở CP4 mang lại cho tôi hai bất ngờ lớn:
- Thứ nhất, khi trực tiếp test thử ChatGPT/Claude web chat trên dữ liệu 10 học sinh, tôi nhận ra trải nghiệm cực kỳ bất tiện: thao tác copy-paste lặp lại 40–45 lần rất tốn thời gian và dễ nhầm lẫn; nếu thiếu prompt chuẩn hóa, AI dễ sinh lời phê sáo rỗng hoặc dùng từ ngữ tiêu cực. Điều này cho thấy LLM thô không thể thay thế một Batch Workflow được thiết kế bài bản.
- Thứ hai, khảo sát 22 giáo viên cho thấy 81.8% sẵn sàng dùng công cụ hỗ trợ để tiết kiệm thời gian, nhưng 100% người được phỏng vấn kiên quyết từ chối việc để AI tự động nộp điểm vào hệ thống. Họ nhấn mạnh học bạ là hồ sơ danh dự đi theo học sinh suốt đời và gắn với trách nhiệm người thầy. Người dùng chỉ muốn được hỗ trợ soạn nháp (Augment) để giảm tải suy nghĩ, tuyệt đối không muốn giao phó việc đánh giá cho máy móc (Automate).

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất đối với tôi là **kỷ luật tách biệt hoàn toàn Vấn đề khỏi Giải pháp và định lượng hóa Tiêu chí thành công**.

Do thói quen lập trình, tôi rất hay vô thức chèn các từ ngữ công nghệ như *"cần xây dựng mô hình LLM để..."*. Việc ép bản thân xóa sạch các thuật ngữ đó để viết đúng format Lean UX (ai chịu đau, ở khoảnh khắc nào, nút thắt 360 phút ở đâu, hậu quả thực tế là gì) đòi hỏi sự kiểm soát tư duy rất chặt chẽ.

Ngoài ra, việc xác định Success Metric đa chiều cũng là một thách thức. Ban đầu tôi chỉ nghĩ đến việc giảm thời gian (480 phút xuống 45 phút). Nhóm đã phản biện rằng nếu chỉ đo thời gian thì sinh ngẫu nhiên cũng đạt được. Metric thực sự phải đo được chất lượng nội dung: tỷ lệ chấp thuận của GVCN $\ge 80\%$ và tỷ lệ trùng lặp văn bản $< 5\%$. Việc lượng hóa được chất lượng giúp Problem Statement trở nên sắc bén và thực tế.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại ngày làm việc hôm nay, tôi sẽ thay đổi hai điểm:
1. **Với bản thân:** Ở CP2, tôi sẽ đánh giá kỹ hơn tính khả thi kỹ thuật và rủi ro hallucination trước khi pitch bài paper, đồng thời chuẩn bị sẵn một file Excel bảng điểm mẫu (đã ẩn danh) để nhóm không mất thời gian tranh luận cấu trúc input ở các bước sau.
2. **Phản biện nhóm mạnh hơn:** Tôi sẽ phản biện quyết liệt hơn về **tính không đồng nhất của dữ liệu đầu vào giữa các trường**. Nhóm đang giả định file Excel xuất từ vnEdu/SMAS đều có cấu trúc giống nhau. Trên thực tế, mỗi trường có thể cấu hình cột điểm, hệ số và quy ước nề nếp khác nhau. Nếu không lường trước khâu xử lý ngoại lệ và chuẩn hóa dữ liệu ở bước Rule, hệ thống sẽ gặp lỗi ngay khi người dùng tải file lên. Tôi muốn nhóm kiểm chứng kỹ tính tương thích này ngay trong giai đoạn pilot.

**6.7. Hiểu bài:**

Bài toán của nhóm tập trung giải quyết áp lực kiệt sức của giáo viên chủ nhiệm THPT khi phải mất trung bình 360 phút / 45 học sinh để viết nhận xét học bạ thủ công vào mỗi kỳ khóa sổ vnEdu/SMAS, dẫn đến hệ quả lời phê bị rập khuôn sáo rỗng. Nhóm đã tái thiết kế quy trình 5 bước với tổng thời gian 45 phút: Tải bảng điểm ẩn danh $\rightarrow$ Rule tự động trích xuất đặc trưng điểm số và nề nếp $\rightarrow$ AI sinh bản nháp nhận xét cá nhân hóa chuẩn Thông tư 22 $\rightarrow$ GVCN trực tiếp rà soát và tinh chỉnh (Human-in-the-loop) $\rightarrow$ Rule xuất file đồng bộ chuẩn 1-click vào hệ thống. Thước đo thành công gồm: Giảm thời gian xuống $\le 45$ phút/lớp, tỷ lệ chấp thuận của giáo viên $\ge 80\%$, và tỷ lệ trùng lặp văn bản giữa các học sinh $< 5\%$. Ranh giới an toàn (Boundary) được thiết lập nghiêm ngặt: Tuyệt đối không đưa thông tin định danh cá nhân (PII) lên mô hình, gắn cờ các trường hợp học sinh đặc biệt để giáo viên tự viết tay, và không cho AI tự ý ghi đè dữ liệu lên cổng học bạ mà bắt buộc phải có giáo viên kiểm duyệt. Mức can thiệp được chọn là **Workflow** (kết hợp Rule tiền xử lý, AI sinh nháp, Con người duyệt và Rule xuất file) vì bài toán có các bước cố định, cần năng lực ngôn ngữ tự nhiên của LLM nhưng tuyệt đối không dùng Agent để tránh vi phạm quy chế sư phạm và rủi ro mất kiểm soát. Quyết định cuối cùng là **Go** cho một thử nghiệm nhỏ (pilot trên 1 lớp 45 học sinh, đánh giá trước 10 em đại diện); kèm ngưỡng dừng an toàn là nếu tỷ lệ chấp thuận của GVCN $< 65\%$ hoặc xuất hiện bất kỳ thông tin điểm số ảo giác nào ($> 0\%$), hệ thống sẽ lập tức dừng pipeline AI và chuyển về giải pháp Rule-based trên Google Sheets.

---

## 7. Tài liệu tham khảo

- Bộ Giáo dục và Đào tạo (2021), *Thông tư số 22/2021/TT-BGDĐT: Quy định về đánh giá học sinh trung học cơ sở và trung học phổ thông*.
- Google PAIR (People + AI Research), *People + AI Guidebook: Designing human-centered AI products*, [https://pair.withgoogle.com/guidebook](https://pair.withgoogle.com/guidebook).
- Teresa Torres (2021), *Continuous Discovery Habits*, Product Talk LLC (Kỹ thuật Opportunity Solution Tree).
- Rob Fitzpatrick (2013), *The Mom Test*, Founder Centric.
- Marty Cagan (2017), *Inspired: How to Create Tech Products Customers Love*, Wiley (Mô hình 4 Product Risks).
- Anthropic (2024), *Building Effective Agents*, [https://www.anthropic.com/research/building-effective-agents](https://www.anthropic.com/research/building-effective-agents).
- Ajay Agrawal, Joshua Gans, Avi Goldfarb (2018), *Prediction Machines*, Harvard Business Review Press (Mô hình AI Canvas).
