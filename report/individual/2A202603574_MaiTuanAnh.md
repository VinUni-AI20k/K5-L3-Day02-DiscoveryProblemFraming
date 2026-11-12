# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Mai Tuấn Anh
- MSSV: 2A202603574
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: RANDOM
- Link repo nhóm: https://github.com/AnhMT2k4/K5-L3A-DAY02-RANDOM-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Mỗi tuần nhóm phải tổng hợp tiến độ công việc từ tin nhắn, GitHub và Google Sheets để báo cáo. |Trưởng nhóm, Thành viên | Mỗi lần tổng hợp mất 30-60 phút |
| 2 |Tốn thời gian |Sinh viên phải tự kiểm tra và đối chiếu nội dung báo cáo với yêu cầu của giảng viên trước khi nộp. | Sinh viên, trưởng nhóm| Mất 30-60 phút mỗi lần kiểm tra báo cáo |
| 3 |Tốn thời gian |Sinh viên mất nhiều thời gian tìm kiếm tài liệu nghiên cứu phù hợp từ nhiều website, PDF và bài báo khoa học. |Sinh viên |Mất 1-2 giờ để tìm kiếm tài liệu cho một chủ đề |
| 4 |Cần đọc, tổng hợp nhiều thông tin |Khi làm đồ án, nhóm phải đọc nhiều tài liệu kỹ thuật khác nhau nhưng khó tổng hợp thành một kiến thức thống nhất. |Cả nhóm |Đọc nhiều nguồn, thông tin trùng lặp, đôi khi có mâu thuẫn trong thông tin|
| 5 |AI có thể tốt hơn |Khi phân chia công việc nhóm, trưởng nhóm khó đánh giá chính xác khối lượng và mức độ phức tạp của từng task. |Trưởng nhóm, thành viên |Task bị phân chia không đều, trễ deadline |
| 6 |Pain từ người khác |Người dùng gặp khó khăn khi tìm lại quyết định hoặc nội dung đã thống nhất trong các cuộc họp nhóm. |Trưởng nhóm, Thành viên |Phải hỏi lại hoặc tìm kiếm tin nhắn cũ nhiều lần|
| 7 |Cần đọc, tổng hợp nhiều thông tin |Khi phân tích dữ liệu, người thực hiện phải tổng hợp dữ liệu từ nhiều file Excel/CSV có cấu trúc và cách đặt tên khác nhau. | Data Analyst, sinh viên|Mất 30–90 phút để làm sạch và ghép dữ liệu |
| 8 |Lặp lại |Thành viên mới tham gia dự án thường xuyên hỏi lại cách cài đặt môi trường, chạy chương trình và cấu trúc thư mục. |Trưởng nhóm, thành viên cũ| Một câu hỏi được hỏi lại 3-5 lần|

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Ý "5" được giữ lại vì việc phân chia công việc chưa hợp lý có thể khiến một số thành viên quá tải và ảnh hưởng đến tiến độ nhóm.

- "Tự động kiểm thử code sau mỗi lần cập nhật" tôi loại bỏ vì phụ thuộc nhiều vào quy trình phát triển phần mềm và hệ thống kiểm thử của từng dự án, khó quan sát trong phạm vi khảo sát hiện tại.
- "Hệ thống quản lý và nhắc nhở deadline tự động" tôi loại bỏ vì có nhiều công cụ hiện có hỗ trợ chức năng này, vấn đề chưa thể hiện rõ mức độ khó khăn hoặc nhu cầu cần giải quyết.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tổng hợp tiến độ báo cáo hàng tuần - Weekly Report | Công việc lặp lại, có quy trình rõ ràng, mất nhiều thời gian tổng hợp từ nhiều nguồn.|  Chưa xác định chính xác bước nào tốn thời gian nhất và chất lượng báo cáo sau khi rút ngắn thời gian.|
| 2 |Tìm kiếm tài liệu nghiên cứu - Research Search |Sinh viên phải tìm kiếm từ nhiều website, PDF và bài báo khoa học. Có thể đo thời gian tìm kiếm và mức độ phù hợp của tài liệu. |Chưa xác định tiêu chí đánh giá tài liệu phù hợp và mức độ khó khăn giữa các ngành học. |
| 3 |Phân chia công việc nhóm - Task Assignment | Trưởng nhóm khó đánh giá khối lượng và độ phức tạp của task, dẫn đến phân chia không đồng đều.|Chưa xác định mức độ ảnh hưởng của năng lực từng thành viên và độ chính xác khi ước lượng task. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến thời điểm báo cáo tiến độ hằng tuần, tôi muốn tổng hợp nhanh công việc và kết quả từ nhiều nguồn, để gửi báo cáo đầy đủ, chính xác và đúng hạn. |
| Actor | Trưởng nhóm dự án chịu trách nhiệm gửi báo cáo cho giảng viên.|
| Thời điểm / bối cảnh | Cuối tuần hoặc đầu tuần mới|
| Quy trình hiện tại (3–7 bước) |1. Kiểm tra công việc trên GitHub -> 2. Thu thập tiến độ từ Google Sheets -> 3. Đọc tin nhắn và cập nhật từ các thành viên -> 4. Tổng hợp kết quả vào Google Docs -> 5. Viết nội dung đánh giá tiến độ, khó khăn và công việc tiếp theo -> 6. Kiểm tra, chỉnh sửa và gửi báo cáo. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước tổng hợp và viết nội dung báo cáo mất nhiều thời gian do phải đọc, đối chiếu dữ liệu từ nhiều nguồn. Ước tính 25–30 phút cho phần này. |
| Impact (nếu không giải thì sao) | Mất 30-60 phút mỗi lần báo cáo. Nếu chậm hoặc thiếu thông tin giảng viên có thể khó nắm bắt tiến độ và đưa ra quyết định kịp thời.|
| Success metric (baseline → target) | Thời gian hoàn thành báo cáo: 60 phút → dưới 20 phút. Đảm bảo báo cáo đầy đủ các mục và không tăng số lần phải chỉnh sửa.|
| Phương án không dùng AI | Sử dụng mẫu báo cáo cố định, dashboard theo dõi tiến độ và checklist các thông tin cần thu thập. |
| Giả thuyết về AI (nếu có) | AI có thể hỗ trợ tổng hợp dữ liệu từ nhiều nguồn, phân loại tiến độ, nhận diện vấn đề và tạo bản nháp nội dung báo cáo. Người phụ trách kiểm tra trước khi gửi.|
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:
1. Kiếm tra trên GitHub(5') -> 2. Thu thập tiến độ từ Sheets(10') -> 3.Đọc tin nhắn và cập nhập từ các thành viên(10') -> 4. Tổng hợp kết quả vào Docs(15') -> 5. Viết nội dung báo cáo(15') -> 6. Kiểm tra và gửi báo cáo (5').



### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi thực hiện bài tập lớn hoặc đồ án, tôi muốn tìm được những tài liệu nghiên cứu phù hợp với chủ đề, để tiết kiệm thời gian và có đủ nguồn thông tin đáng tin cậy phục vụ nghiên cứu. |
| Actor | Sinh viên |
| Thời điểm / bối cảnh | Khi bắt đầu nghiên cứu một đề tài, xây dựng cơ sở lý thuyết hoặc tìm tài liệu tham khảo cho báo cáo. |
| Quy trình hiện tại (3–7 bước) | 1. Xác định chủ đề và từ khóa tìm kiếm -> 2. Tìm kiếm trên Google Scholar và các website khoa học -> 3. Mở từng bài báo hoặc tài liệu PDF -> 4. Đọc tiêu đề, abstract và nội dung chính -> 5. Xem xét mức độ liên quan -> 6. Lưu lại những tài liệu phù hợp.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước đọc và đánh giá tài liệu mất nhiều thời gian vì phải mở từng tài liệu, kiểm tra nội dung và xác định mức độ liên quan đến đề tài. |
| Impact (nếu không giải thì sao) | Ước tính mất 1–2 giờ để tìm tài liệu cho một chủ đề. Việc tìm kiếm không hiệu quả có thể khiến sinh viên bỏ sót tài liệu quan trọng hoặc sử dụng nguồn không phù hợp.|
| Success metric (baseline → target) | Thời gian tìm kiếm: 1–2 giờ → dưới 30 phút. Tỷ lệ tài liệu được đánh giá là phù hợp không thấp hơn phương pháp tìm kiếm hiện tại.|
| Phương án không dùng AI | Xây dựng bộ từ khóa tìm kiếm, sử dụng bộ lọc theo năm xuất bản, lĩnh vực, loại tài liệu và lưu trữ tài liệu bằng Zotero.|
| Giả thuyết về AI (nếu có) | AI có thể hỗ trợ tìm kiếm theo ngữ nghĩa, tóm tắt nội dung, phân loại tài liệu và đề xuất những bài nghiên cứu có liên quan đến chủ đề.|
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:
1. Xác định chủ đề và từ khóa tìm kiếm(5') -> 2. Tìm kiếm trên Google và các website(5') -> 3. Mở từng bài báo hoặc PDF(10') -> 4. Đọc tiêu đề và nội dung(60') -> 5. Xem xét mực độ liên quan(10') -> 6.Lưu lại những tại liệu phù hợp(10').

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu một dự án hoặc nhận danh sách công việc mới, tôi muốn đánh giá khối lượng và độ phức tạp của từng task dựa trên năng lực thành viên, để phân chia công việc hợp lý và đảm bảo tiến độ chung. |
| Actor | Trưởng nhóm, thành viên|
| Thời điểm / bối cảnh | Khi bắt đầu dự án, lập kế hoạch sprint hoặc khi phát sinh task mới cần phân công.|
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận danh sách công việc cần thực hiện -> 2. Phân tích yêu cầu của từng task -> 3. Ước lượng thời gian và độ khó -> 4. Xem xét năng lực và khối lượng công việc hiện tại của từng thành viên -> 5. Phân công task cho các thành viên -> 6. Theo dõi tiến độ và điều chỉnh khi cần.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–4: Trưởng nhóm phải tự đọc, đánh giá độ phức tạp của từng task và đối chiếu với năng lực thành viên. Việc ước lượng thường mang tính chủ quan.|
| Impact (nếu không giải thì sao) | Một số thành viên có thể bị quá tải trong khi thành viên khác có ít việc hơn. Task khó có nguy cơ bị giao cho người chưa đủ kinh nghiệm, dẫn đến chậm deadline và phải phân công lại.|
| Success metric (baseline → target) | Thời gian lập kế hoạch và phân công task giảm ít nhất 30%. Tỷ lệ task hoàn thành đúng hạn tăng so với cách phân công ban đầu. |
| Phương án không dùng AI | Dựa vào thông tin của từng thành viên và quy tắc phân bổ khối lượng công việc |
| Giả thuyết về AI (nếu có) | AI phân tích mô tả task, ước lượng độ phức tạp, xác định kỹ năng cần thiết và đề xuất thành viên phù hợp dựa trên năng lực và khối lượng công việc hiện tại. Trưởng nhóm quyết định phân công cuối cùng.|
| Cảm nhận nhanh | Workflow  |

Quy trình nháp hiện tại:
1. Tiếp nhận danh sách công việc cần thực hiện. -> 2. Phân tích yêu cầu của từng task. -> 3. Ước lượng thời gian và độ khó. -> 4. Xem xét năng lực và khối lượng công việc hiện tại của từng thành viên. -> 5. Phân công task cho các thành viên. -> 6. Theo dõi tiến độ và điều chỉnh khi cần.
Quy trình nháp tương lai:
1. Nhập danh sách task -> 2. AI phân tích yêu cầu từng task -> 3. AI ước lượng độ phức tập và đề xuất phương án phân công theo kỹ năng thành viên -> 4. Trưởng nhóm xem xét và xác nhận -> 5. Theo dõi và cập nhập tiến độ.

### Card muốn pitch nhất

- Card số: 1 – Weekly Report (Tổng hợp báo cáo tiến độ hằng tuần).
- Vì sao: Vấn đề xảy ra lặp lại theo tuần, có quy trình hiện tại tương đối rõ ràng và có thể đo được thời gian thực hiện. Nhóm có thể thử nghiệm trên các nguồn dữ liệu quen thuộc như GitHub, Google Sheets và tin nhắn. Đây là vấn đề AI có thể hỗ trợ nhưng vẫn cần người phụ trách kiểm tra trước khi gửi.
- Câu hỏi muốn nhóm phản biện: Nếu AI giúp rút ngắn thời gian tổng hợp báo cáo từ 60 phút xuống dưới 20 phút, cần đánh giá thêm tiêu chí nào để chứng minh báo cáo vẫn đầy đủ, chính xác và đáng tin cậy?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Metric ban đầu chủ yếu đo thời gian hoàn thành, chưa phản ánh chất lượng báo cáo. Báo cáo được tạo nhanh hơn nhưng thiếu thông tin hoặc sai dữ liệu thì chưa thể xem là thành công.| Yes | Bổ sung tiêu chí chất lượng bên cạnh thời gian: báo cáo phải đầy đủ các mục, thông tin chính xác và không làm tăng số lần phải chỉnh sửa. Người phụ trách vẫn kiểm tra bản nháp trước khi gửi.|

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Chuẩn bị và trình bày Problem Card về việc tổng hợp báo cáo tiến độ hằng tuần| Làm rõ actor, bối cảnh, quy trình hiện tại, bottleneck và metric để nhóm có cơ sở phản biện.|
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Trong 50–60 tin nhắn mỗi ngày, thực tế có bao nhiêu thông báo quan trọng bị bỏ lỡ? Vấn đề là số lượng tin nhắn quá nhiều hay do chưa có cách lọc thông báo hiệu quả?| Giúp bạn xác định cần có số liệu cụ thể về tủ lệ thông báo quan trọng bị bỏ lỡ.|
| Nhận phản biện | Câu hỏi tôi nhận được: Khó khăn chính là tìm tài liệu phù hợp hay đọc và đánh giá chất lượng tài liệu? Có số liệu về thời gian trung bình để chọn được một tài liệu hữu ích không?| Tôi đã sửa gì: Tôi đã sửa gì: Làm rõ hơn bottleneck trong quy trình tìm kiếm và lựa chọn tài liệu, phân biệt giữa khó khăn khi tìm tài liệu và khó khăn khi đánh giá chất lượng. Đồng thời bổ sung metric về thời gian trung bình để tìm được một tài liệu hữu ích nhằm đo lường vấn đề cụ thể hơn.|
| Gom cluster / cây OST | Tôi và các bạn cùng thảo luận để gom thành 5 cluter| Giúp nhóm phân chia được cluster|
| Chọn candidate problem | Tôi đã tham gia chấm điểm các problem của nhóm cùng với nhóm|    Giúp nhóm chọn được problem có điểm cao nhất |
| Kiểm chứng / research | Cùng với nhóm đi tham gia phỏng vấn các nhóm trưởng khác | Thu thập bằng chứng thực tế |
| Quy trình nhóm | Phân tích quy trình Weekly Report gồm 6 bước, ước tính tổng thời gian khoảng 60 phút; đề xuất quy trình tương lai rút xuống khoảng 20 phút.| Xác định phần tổng hợp và viết báo cáo là bottleneck cần ưu tiên cải thiện.|
| Problem Statement | Cùng nhóm thảo luận phân tích các trường | Giúp nhóm thống nhất actor, nhu cầu, bối cảnh và tác động của vấn đề.|
| Mức can thiệp AI | Định hướng AI hỗ trợ tổng hợp dữ liệu, phân loại tiến độ và tạo bản nháp; người phụ trách kiểm tra, chỉnh sửa và quyết định gửi.| Giữ quyền kiểm soát nội dung cuối cùng ở con người, hạn chế rủi ro báo cáo sai hoặc thiếu thông tin.|
| Quyết định | Cùng với nhóm thảo luận về các rủi ro và kết luận| Giúp nhóm thông nhất các rủi ro và kết luận |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý và mở rộng danh sách problem theo các lăng kính như lặp lại, tốn thời gian và cần tổng hợp nhiều thông tin.| Có thêm góc nhìn, tránh chỉ tập trung vào vấn đề kỹ thuật; hỗ trợ diễn đạt ý tưởng thành Job Story.| Một số ý tưởng còn chung chung, chưa có bằng chứng về tần suất hoặc mức độ ảnh hưởng.| Sửa 1 vài thông tin chính xác hơn|
| CP2 Problem Card | Hỗ trợ cấu trúc Job Story, actor, quy trình, bottleneck, impact và success metric cho các candidate.| Giúp trình bày các problem theo cùng cấu trúc để dễ so sánh.| Metric có thể chỉ tập trung vào tốc độ hoặc đặt mục tiêu khi chưa có baseline đủ chắc chắn.| Đối chiếu quy trình, ghi rõ các bước và thời gian ước tính; bổ sung yêu cầu chất lượng bên cạnh thời gian.|
| CP4 Research | | | | |
| CP5 Quy trình |Hỗ trợ rà soát quy trình hiện tại và đề xuất các bước AI có thể hỗ trợ trong quy trình tương lai. | Giúp nhìn rõ điểm nghẽn ở khâu đọc, đối chiếu dữ liệu và viết báo cáo.| Đề xuất tự động hóa có thể bỏ qua bước xác minh dữ liệu hoặc chưa tính đến trường hợp AI tổng hợp sai.| Không giao toàn bộ quyết định cho AI.|
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
- Mỗi người đều có 1 vấn đề riêng,  các bạn đều chỉ khá rõ actor, quy trình và khó khăn trong từng vấn đề của mình.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
- Chưa có

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

- Tôi đã đổi ý sau 1 lần phản biện, khi mà các thành viên chỉ rõ metric giảm thời gian chưa đủ, cần phải có độ chính xác và rõ ràng hơn.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Qua hoạt động kiểm chứng, tôi nhận thấy cần quan tâm đến cách các nhóm khác đang thu thập, quản lý và tổng hợp tiến độ. Điều này giúp tôi hiểu rằng một vấn đề chỉ thực sự có cơ sở để lựa chọn khi có thể tìm thấy những khó khăn tương tự từ người gặp vấn đề.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

-Khi viết Problem Statement cho Weekly Report, nhóm phải thống nhất được ai là người gặp vấn đề, họ cần thực hiện công việc gì, gặp khó khăn trong hoàn cảnh nào và hậu quả của khó khăn đó.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
- Tôi sẽ chú ý hơn đến chất lượng thông tin đầu ra, chẳng hạn tỷ lệ thông tin chính xác, số nội dung bị thiếu và số lần phải chỉnh sửa. Khi phản biện nhóm, tôi muốn đặt nhiều câu hỏi hơn về tính khả thi của các metric, dữ liệu đầu vào và những trường hợp AI có thể tổng hợp sai.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Problem của nhóm RANDOM là trưởng nhóm mất nhiều thời gian tổng hợp tiến độ công việc hằng tuần từ GitHub, Google Sheets và tin nhắn của các thành viên. Quy trình hiện tại gồm 6 bước, mất khoảng 60 phút, trong đó khâu tổng hợp dữ liệu và viết báo cáo là bottleneck chính. Nhóm đặt mục tiêu giảm thời gian hoàn thành báo cáo xuống dưới 20 phút nhưng vẫn phải đảm bảo thông tin đầy đủ, chính xác và không tăng số lần chỉnh sửa. Về boundary, nhóm tập trung hỗ trợ công việc tổng hợp báo cáo tiến độ, không thay thế hoàn toàn vai trò quản lý và đánh giá của trưởng nhóm. AI được sử dụng để thu thập, phân loại thông tin tiến độ, nhận diện khó khăn và tạo bản nháp báo cáo. Người phụ trách vẫn phải kiểm tra, chỉnh sửa và xác nhận nội dung trước khi gửi cho giảng viên. Cuối cùng, nhóm lựa chọn hướng sử dụng AI như một công cụ hỗ trợ thay vì giao toàn bộ quy trình và quyền quyết định cho AI.
---

## 7. Tài liệu tham khảo

-
