# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Phạm Lê Chuẩn
- MSSV: 2A202603784
- Email trường (không bắt buộc, repo có thể để public): 26ai.chuanpl@vinuni.edu.vn
- Tên nhóm: H1
- Link repo nhóm:https://github.com/huyvu-03/K5-L3B-Day02-H1-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi hệ thống đang chạy báo lỗi, tôi muốn biết nhanh vấn đề nằm ở đâu và khắc phục ngay | IT, Sysadmin | Thường mất 20-30 phút mỗi bài lần chỉ để dò lỗi cú pháp hoặc tìm hiểu nguyên nhân gây lỗi.| 
| 2 | Tốn thời gian | Khi đến đầu và cuối mỗi ca học, tôi muốn thao tác điểm danh diễn ra nhanh chóng hoặc tự động, để không mất thời gian của buổi học | Sinh viên, Giảng viên/trợ giảng | Mất khoảng 5-10 phút đầu và cuối mỗi ca để quét mã/gọi tên. |
| 3 | Pain từ người khác | Khi sát kỳ thi, tôi muốn có một nơi lưu trữ chung dễ tìm kiếm, tra cứu | Học viên, trợ giảng, bạn cùng lớp | Mất khoảng 15 - 20 phút để tìm kiếm và tải về các tài liệu cần thiết. |
| 4 | Lặp lại |  Khi điện thoại báo đầy bộ nhớ, tôi muốn lọc và chuyển ảnh/tài liệu quan trọng sang máy tính lưu trữ offline một cách nhanh gọn, để giải phóng dung lượng mà không tốn tiền mua dung lượng đám mây. | Người dùng | Mỗi tháng tốn khoảng 45 phút cắm cáp, lướt tìm từng file/ảnh cũ để cắt dán thủ công sang ổ cứng máy tính | 
| 5 | Cần đọc, tổng hợp nhiều thông tin | Tôi muốn tự động sắp xếp lịch trình, đặt lịch, nhắc hẹn | Con người | Mất thời gian để tự kiểm tra, sắp xếp |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Điểm danh đầu/cuối giờ | Quy trình lặp lại rất rõ ràng, tốn thời gian cố định mỗi buổi học, có baseline đo thời gian chính xác, đối tượng bị ảnh hưởng (học viên, trợ giảng) cụ thể. | Giải pháp không dùng AI (mã QR tĩnh/chữ ký) hay tự động hóa bằng AI (nhận diện khuôn mặt/giọng nói) mới là tối ưu và khả thi nhất. |
| 2 | Phát hiện và báo cáo lỗi trong hệ thống | Vấn đề rất phổ biến với người làm kĩ thuật, tốn thời gian, bước nghẽn rõ ràng. Dễ dàng so sánh được hiệu quả giữa việc tự tra cứu và dùng AI. | Việc thiết lập ngưỡng đánh giá chất lượng đầu ra của AI (AI giải thích lỗi đúng/sai) khó định lượng chính xác bằng phút. |
| 3 | Sắp xếp lịch trình, nhắc hẹn | Pain point có thật và xảy ra thường xuyên khi làm việc nhóm, có bước nghẽn rõ ràng là đối chiếu lịch từ nhiều nguồn. Có thể ứng dụng mức can thiệp Workflow. | Không chắc sinh viên/người dùng có sẵn sàng cấp quyền truy cập toàn bộ lịch cá nhân (Google Calendar, Zalo) cho một công cụ AI hay không. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story |Khi đến đầu và cuối mỗi ca học, tôi muốn thao tác điểm danh diễn ra nhanh chóng hoặc tự động, để không mất thời gian của buổi học và không lo bị đánh vắng do quên điểm danh lúc về.|
| Actor | Sinh viên và Giảng viên/Trợ giảng |
| Thời điểm / bối cảnh | Đầu và cuối mỗi buổi học lý thuyết hoặc thực hành lab tại trường |
| Quy trình hiện tại (3–7 bước) | 
1. Giảng viên mở danh sách/tạo mã QR
2. Sinh viên xếp hàng quét mã hoặc chờ đọc tên
3. Hệ thống/Giảng viên ghi nhận trạng thái
4. Chốt danh sách vắng|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 (Sinh viên xếp hàng chờ quét mã hoặc chờ đọc tên), mất khoảng 5–10 phút mỗi lần |
| Impact (nếu không giải thì sao) | Mất 10–20 phút tổng cộng mỗi buổi học chỉ cho thủ tục; lớp học bị ồn ào gián đoạn; sinh viên vội chuyển phòng học dễ quên điểm danh và bị đánh vắng oan. |
| Success metric (baseline → target) | Tổng thời gian điểm danh giảm từ 10 phút/lần (baseline) xuống dưới 2 phút/lần (target). |
| Phương án không dùng AI | Truyền tay tờ danh sách ký tên trong lớp, hoặc dán cố định mã QR tĩnh trên bàn học để sinh viên tự quét (Rule). |
| Giả thuyết về AI (nếu có) | Hệ thống camera điểm danh tự động nhận diện khuôn mặt khi sinh viên bước vào/ra khỏi phòng học, tự động cập nhật trạng thái vào hệ thống đào tạo.|
| Cảm nhận nhanh | Rule / Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 10 phút/lần

[1 GV/TA mở danh sách hoặc tạo mã QR: 1'] 
→ [2 Sinh viên xếp hàng quét mã hoặc chờ đọc tên: 5-8'] ← BOTTLENECK
→ [3 Hệ thống/GV ghi nhận trạng thái: 1'] 
→ [4 Chốt danh sách vắng: 1']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm các bài lab bị báo lỗi, tôi muốn biết nhanh dòng lệnh/code nào đang sai, để sửa ngay thay vì loay hoay tra cứu lan man. |
| Actor | Học viên IT / Sinh viên |
| Thời điểm / bối cảnh | Trong các buổi làm bài tập thực hành, lab tại phòng máy hoặc ở nhà |
| Quy trình hiện tại (3–7 bước) |
1. Chạy code hoặc cấu hình bị báo lỗi
2. Đọc thông báo log và copy mã lỗi
3. Tìm kiếm trên Google và đọc các thread StackOverflow
4. Copy code sửa thử và debug
5. Chạy lại kiểm tra thành công |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (Search Google & đọc các thread StackOverflow), mất khoảng 15–20 phút mỗi lỗi khó |
| Impact (nếu không giải thì sao) | Mất nhiều thời gian cho một lỗi cú pháp hoặc cấu hình nhỏ, làm chậm tiến độ hoàn thành bài lab và gây nản chí. |
| Success metric (baseline → target) | Tổng thời gian xử lý một lỗi giảm từ 30 phút (baseline) xuống dưới 5 phút (target). |
| Phương án không dùng AI | Tra cứu tài liệu môn học offline, hỏi bạn cùng lớp hoặc trợ giảng |
| Giả thuyết về AI (nếu có) | AI phân tích đoạn mã log lỗi và chỉ ra chính xác dòng code cần sửa kèm giải thích nguyên nhân. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 30 phút/lỗi khó

[1 Chạy code/cấu hình bị báo lỗi: 1'] 
→ [2 Đọc thông báo log/copy mã lỗi: 2'] 
→ [3 Search Google & đọc các thread StackOverflow: 15'] ← BOTTLENECK
→ [4 Copy code sửa thử & debug: 10'] 
→ [5 Chạy lại thành công: 2']

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhiều task, lịch học và lịch họp nhóm mới, tôi muốn tự động tìm giờ trống để xếp lịch, để không bị trùng lặp và lỡ việc. |
| Actor | Sinh viên, Freelancer |
| Thời điểm / bối cảnh | Đầu tuần hoặc khi có lịch hẹn họp nhóm, lớp học phát sinh mới |
| Quy trình hiện tại (3–7 bước) |
1. Nhận tin nhắn yêu cầu xếp lịch hoặc task mới
2. Mở Google Calendar, lịch học trường và note cá nhân
3. Dò thủ công tìm khe thời gian trống không bị trùng
4. Nhắn tin chốt giờ với các bên liên quan
5. Tự gõ tạo event mới trên Google Calendar |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (Đối chiếu lịch từ nhiều nguồn để so khớp giờ trống), mất khoảng 15–20 phút/lần |
| Impact (nếu không giải thì sao) | Dễ bị trùng lịch, quên lịch hẹn quan trọng với nhóm hoặc lỡ deadline công việc. |
| Success metric (baseline → target) | Thời gian chốt lịch giảm từ 30 phút/lần (baseline) xuống dưới 5 phút/lần (target). |
| Phương án không dùng AI | Dùng một bảng Excel/Notion cố định để thủ công tô màu các khung giờ bận trong tuần|
| Giả thuyết về AI (nếu có) | Công cụ tự động đọc lịch trống từ các nguồn và đề xuất ngay các khung giờ phù hợp nhất để chốt hẹn.|
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 30 phút mỗi lần xếp lịch tuần/hẹn mới

[1 Nhận tin nhắn yêu cầu họp/task mới: 2'] 
→ [2 Mở Google Calendar, lịch học trường và note cá nhân: 5'] 
→ [3 Dò thủ công tìm khe thời gian trống không bị trùng: 15'] ← BOTTLENECK
→ [4 Nhắn tin chốt giờ với các bên liên quan: 5'] 
→ [5 Tự gõ tạo event mới trên Google Calendar: 3']
```

### Card muốn pitch nhất

- Card số: Card #2 (Sửa lỗi bài lab)
- Vì sao: Đây là vấn đề xảy ra thường xuyên nhất trong các buổi thực hành, có quy trình rõ ràng (từ đọc log đến search lỗi), bước nghẽn cụ thể và đo lường được thời gian tiết kiệm thực tế.
- Câu hỏi muốn nhóm phản biện: Câu hỏi muốn nhóm phản biện: Liệu việc dùng Workflow/AI để dịch log lỗi và chỉ chỗ sửa có làm giảm khả năng tự tư duy và fix bug của sinh viên không?

### AI đã phản biện card thế nào

| # | Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|---|
| 1 |Baseline 30 phút chỉ là ước lượng chủ quan, thiếu số liệu thực tế đo bằng đồng hồ. | Đồng ý | Bổ sung cam kết tự bấm giờ thực tế trong 2 buổi lab gần nhất để có số liệu chính xác. |
| 2 | Chưa tính đến các lỗi hệ thống/mạng phức tạp mà AI không thể đọc được log cục bộ. | Đồng ý | Thêm điều kiện giới hạn (boundary): AI chỉ hỗ trợ các lỗi cú pháp, logic code thông thường, không thay thế việc cấu hình hạ tầng mạng phức tạp. | 
| 3 | Gợi ý đẩy thẳng lên mức Agent tự động sửa và chạy lại code. | Không đồng ý | Giữ nguyên mức Workflow: AI chỉ đóng vai trò phân tích và gợi ý dòng code sửa, học viên vẫn phải là người trực tiếp sửa và chạy lại để đảm bảo tính chủ động học tập. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày Problem Card #2 "Sửa lỗi bài lab" (đọc log lỗi và tra cứu). | Bài được đánh giá cao về độ rõ ràng quy trình và được đưa vào shortlist. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Bài điểm danh dùng mã QR tĩnh có cần đến AI không?" | Nhóm nhận ra bài điểm danh chỉ cần mức Rule, không cần dùng AI gây lãng phí. |
| Nhận phản biện | Câu hỏi tôi nhận được: "Dùng AI tự sửa code lỗi có làm sinh viên giảm tư duy không?" | Tôi đã sửa: Lùi mức can thiệp từ Agent về Workflow (AI chỉ giải thích log + gợi ý, sinh viên tự sửa). |
| Gom cluster / cây OST | Gom các bài toán tra cứu code, xem log vào nhóm "Hỗ trợ học tập / Debug". | Xác định đúng Outcome là giảm thời gian tra cứu trên StackOverflow khi gặp lỗi lab. |
| Chọn candidate problem | Bảo vệ quan điểm chọn bài "Sửa lỗi bài lab" dựa trên tiêu chí dễ bấm giờ đo lường baseline. | Thuyết phục nhóm đồng thuận chọn bài này làm đề tài chính cho nhóm. |
| Kiểm chứng / research | Phỏng vấn 2 sinh viên IT về thời gian sửa lỗi lab và tìm 2 công cụ AI debug hiện có. | Xóa bỏ giả định cảm tính; xác nhận bước nghẽn tốn thời gian nhất là đọc và search Google. |
| Quy trình nhóm | Vẽ sơ đồ quy trình hiện tại (5 bước thủ công) và quy trình tương lai. | Phân định rõ bước nào dùng Rule, bước nào AI phân tích, và bước nào con người kiểm tra. |
| Problem Statement | Đóng góp ý kiến gọt giũa 6 trường cho phiên bản v0 và v1. | Loại bỏ các từ khóa giải pháp ra khỏi statement và bổ sung metric đo tỉ lệ sửa lại. |
| Mức can thiệp AI | Phân tích ma trận độ mơ hồ/phức tạp để chọn mức độ can thiệp. | Thống nhất chọn mức Workflow thay vì Agent để kiểm soát rủi ro bài toán. |
| Quyết định | Đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability) và xây dựng pilot. | Chốt quyết định "Go (phạm vi nhỏ)" kèm ngưỡng dừng (stop criteria) sau 2 tuần. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm các problem lặp lại/tốn thời gian theo vai trò sinh viên IT. | Nhớ ra các bài toán liên quan đến phân loại log và đọc tài liệu lab. | Đưa ra ý tưởng quá rộng và mơ hồ như "Trợ lý AI quản lý toàn bộ việc học". | Bỏ các ý tưởng rộng, chỉ giữ lại bài toán có quy trình và thao tác thật. |
| CP2 Problem Card | Đóng vai PM hoài nghi để phản biện Problem Card cá nhân. | Chỉ ra baseline thời gian 30 phút ban đầu chỉ là ước lượng cảm tính. | Gợi ý đẩy bài toán lên thành Agent tự động sửa lỗi và chạy lại code. | Thêm cam kết tự bấm giờ thật và giữ boundary: người dùng phải tự sửa code. |
| CP4 Research | Tìm 2–3 công cụ/pattern đã giải bài toán tương tự trên thị trường. | Gợi ý nhanh danh sách các extension AI debug và plugin hỗ trợ lập trình. | Đưa ra link tài liệu bị hỏng (link chết) và trích dẫn sai tính năng của gói miễn phí. | Tự mở từng link kiểm tra lại thông tin và xác minh giá trị thực tế của công cụ. |
| CP5 Quy trình | Chuyển mô tả dạng văn bản sang sơ đồ quy trình dạng văn bản/Mermaid. | Chuyển đổi định dạng nhanh, trực quan. | Gộp bước "Search Google" và "Debug code" làm một, làm mất điểm nghẽn (bottleneck). | Tách riêng bước search Google (15') ra khỏi bước debug để giữ đúng điểm nghẽn. |
| CP5–6 Problem Statement | Soát lỗi Problem Statement và chỉ ra các từ ngữ lồng ghép giải pháp. | Phát hiện trúng các từ ngữ mang tính giải pháp vội vàng (chatbot, AI). | Tự viết lại Problem Statement bằng văn phong chung chung, mất ngữ cảnh bài lab. | Tự chỉnh sửa lại câu statement, giữ nguyên bối cảnh kỹ thuật bài lab của nhóm. |
| CP6 Mức can thiệp / quyết định | Gợi ý bộ tiêu chí đánh giá đầu ra (eval) và các loại rủi ro cho bài toán. | Gợi ý tiêu chí hay: "Không bịa ra các thư viện/hàm code không tồn tại". | Đánh giá rủi ro Feasibility quá thấp (cho rằng tích hợp AI debug rất dễ). | Nâng mức rủi ro Feasibility lên Trung bình và tự bổ sung ngưỡng dừng cụ thể cho pilot. |
---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Học được các góc nhìn thực tế mới và cách thu hẹp một ý tưởng rộng thành Problem Card rõ ràng, đo lường được.
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có, nhóm từng vội bàn ngay cách dùng AI. Nhóm nhận ra khi bắt tay vẽ quy trình hiện tại bị vướng, sau đó quyết định gác lại giải pháp để phân tích đúng điểm nghẽn (bottleneck) trước.
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Ban đầu em muốn dùng Agent tự sửa code lỗi, nhưng sau khi bị phản biện là sẽ làm giảm tư duy tự học, em đã lùi về mức Workflow (AI chỉ phân tích log và gợi ý).
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Có. Khi phỏng vấn mới biết bước mà nhóm tưởng là tốn thời gian nhất lại không phải là nỗi đau (pain point) thực sự của người dùng.
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Là phải mô tả trúng điểm nghẽn cốt lõi mà tuyệt đối không được chèn giải pháp hay từ khóa "AI" vào.
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Em sẽ đi phỏng vấn thực tế sớm hơn và ép nhóm phải bấm giờ đo thời gian (baseline) thật thay vì chỉ ngồi đoán.
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Bài làm đi từ việc tìm một problem thực tế, vẽ lại quy trình để xác định nút thắt, từ đó đo lường hiệu quả bằng metric. Tiếp theo là đặt boundary an toàn, đánh giá độ phức tạp để chọn mức can thiệp AI (Rule/Workflow/Agent) phù hợp, và đối chiếu rủi ro để đưa ra quyết định Go hay Not Yet.
---

## 7. Tài liệu tham khảo
Gemini 3.5-flash-lite
-
