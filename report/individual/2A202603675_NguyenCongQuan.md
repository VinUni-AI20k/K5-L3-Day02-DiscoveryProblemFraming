# Báo cáo cá nhân — 2A202603675_NguyenCongQuan

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Nguyễn Công Quân
- MSSV:2A202603675
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:Nhom9999
- Link repo nhóm:https://github.com/Minh8246/K5-L3A-Day02-Nhom9999-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại / Pain từ người khác | Khi chuẩn bị bữa tối cho gia đình, tôi muốn xác định món ăn phù hợp, để có thể bắt đầu nấu mà không mất nhiều thời gian cân nhắc và trả lời lại câu hỏi hôm nay ăn gì. | Tôi và 6 người ăn trong gia đình | Tôi mất khoảng 10–15 phút để nghĩ món, xảy ra 4–5 lần/tuần; hôm nào em trai nấu thì thường hỏi “hôm nay nấu gì?”. |
| 2 | Tốn thời gian | Khi bắt đầu một ngày có nhiều nhiệm vụ từ trường, khóa học tiếng Anh và khóa học AI thực chiến, tôi muốn biết việc nào cần ưu tiên và thời hạn của từng việc, để hoàn thành đầy đủ thay vì phải làm gấp khi gần deadline. | Tôi | Tôi mất khoảng 25 phút/ngày (dao động 15–30 phút) để kiểm tra toàn bộ nhiệm vụ; trong tháng gần nhất có khoảng 4 lần tôi phải làm gấp cho kịp hạn nên kết quả chưa thực sự đầy đủ. |
| 3 | Tốn thời gian | Khi quay lại một công việc đang làm dở, tôi muốn biết chính xác mình đã làm đến đâu và bước tiếp theo là gì, để có thể tiếp tục công việc ngay. | Tôi | Mỗi lần quay lại tôi mất khoảng 10 phút để tìm trạng thái công việc; tình huống này xảy ra khoảng 3 lần/tuần. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi bắt đầu làm một bài lab, tôi muốn hiểu đầy đủ yêu cầu từ các nguồn liên quan, để không bỏ sót đầu ra hoặc quy định nộp bài. | Tôi và các thành viên cùng làm bài lab | Mỗi hôm làm lab tôi mất khoảng 15 phút để kiểm tra 5 nguồn: repo, slide, LMS, Discord và Outlook. |
| 5 | Lặp lại / Cần tổng hợp thông tin | Khi tổng hợp chi tiêu trong tháng, tôi muốn xác định mục đích và phân loại các giao dịch ngân hàng, để biết tiền đã được sử dụng vào đâu và đánh giá việc chi tiêu có hợp lý hay không. | Tôi | Tôi kiểm tra và ghi lại giao dịch 2 lần/tháng, mỗi lần khoảng 30 phút, tổng cộng khoảng 1 giờ/tháng; trong tháng vừa rồi có khoảng 5 giao dịch tôi không nhớ rõ đã chi vào việc gì. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Tôi tự scan các tình huống từ trải nghiệm của mình trước. Sau đó, AI hỗ trợ tách việc “kiểm tra nhiệm vụ” và “tìm lại trạng thái công việc đang làm dở” thành hai problem riêng, đồng thời diễn đạt lại các ý theo Job Story. Tôi thay ý “theo dõi thông tin khóa học” bằng “tổng hợp chi tiêu” vì ý cũ gần trùng với problem tổng hợp yêu cầu bài lab, còn vấn đề chi tiêu có trải nghiệm và số liệu thật. Tôi không giữ các gợi ý khác khi chưa có trải nghiệm thật để kiểm chứng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Quản lý nhiệm vụ và deadline từ nhiều nền tảng | Xảy ra hằng ngày, mất 15–30 phút và đã có khoảng 4 lần/tháng tôi phải làm gấp nên kết quả chưa đầy đủ. Quy trình, bottleneck và tác động đều đo được. | Một checklist/lịch chung không dùng AI có thể đã đủ hay chưa; việc tự động tổng hợp từ các nền tảng có khả thi không. |
| 2 | Tìm lại trạng thái của báo cáo đang làm dở | Xảy ra khoảng 3 lần/tuần, mỗi lần mất 10 phút; bottleneck xuất hiện rõ khi tôi chuyển qua lại giữa báo cáo, bài tiếng Anh và bài lab. | Thói quen ghi chú cuối mỗi phiên có thể giải quyết phần lớn vấn đề mà không cần AI hay không. |
| 3 | Tổng hợp và phân loại giao dịch chi tiêu | Có quy trình lặp lại 2 lần/tháng, mất tổng cộng khoảng 1 giờ/tháng và có khoảng 5 giao dịch chưa xác định được mục đích trong tháng vừa rồi. | Nội dung giao dịch ngân hàng có đủ rõ để phân loại không; mức giảm xuống 10 phút/lần có thực tế không. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu một ngày có nhiều nhiệm vụ từ trường, khóa học tiếng Anh và khóa học AI thực chiến, tôi muốn biết việc nào cần ưu tiên và thời hạn của từng việc, để hoàn thành đầy đủ thay vì phải làm gấp khi gần deadline. |
| Actor | Tôi — học viên đang đồng thời học ở trường, trung tâm tiếng Anh và khóa AI thực chiến, đồng thời tham gia nhóm build phase. |
| Thời điểm / bối cảnh | Đầu ngày hoặc trước khi bắt đầu một phiên làm việc, khi nhiệm vụ nằm rải rác trên Zalo, Discord, ứng dụng tiếng Anh, Cohort và web AI thực chiến. |
| Quy trình hiện tại (3–7 bước) | (1) Mở và kiểm tra 5 nền tảng: 7 phút; (2) liệt kê nhiệm vụ: 5 phút; (3) kiểm tra deadline và khối lượng: 5 phút; (4) xếp thứ tự ưu tiên: 8 phút. Tổng điển hình khoảng 25 phút, dao động 15–30 phút. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Xác định và xếp thứ tự việc cần làm trước, khoảng 8 phút/lần, vì phải cân nhắc đồng thời deadline và khối lượng. |
| Impact (nếu không giải thì sao) | Trong tháng gần nhất có khoảng 4 lần tôi phải làm gấp sát deadline nên kết quả chưa thực sự đầy đủ; thời gian kiểm tra cũng làm chậm thời điểm bắt đầu công việc. |
| Success metric (baseline → target) | Thời gian kiểm tra và ưu tiên từ khoảng 25 phút xuống tối đa 10 phút/ngày; số lần phải làm gấp từ khoảng 4 xuống tối đa 1 lần/tháng. Đo bằng thời gian bắt đầu/kết thúc kiểm tra và nhật ký deadline. |
| Phương án không dùng AI | Dùng một checklist hoặc lịch chung, tự nhập nhiệm vụ ngay khi nhận, đặt deadline, mức ưu tiên và nhắc việc theo quy tắc cố định. |
| Giả thuyết về AI (nếu có) | Một workflow có thể tổng hợp nội dung nhiệm vụ từ các nguồn và đề xuất thứ tự ưu tiên theo deadline/khối lượng; tôi vẫn kiểm tra và quyết định thứ tự cuối cùng. |
| Cảm nhận nhanh | Workflow (giả thuyết ban đầu, chưa chốt trước khi so sánh với phương án không AI). |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 25 phút/ngày (dao động 15–30 phút)

[Mở 5 nền tảng: 7'] → [Liệt kê nhiệm vụ: 5']
→ [Kiểm tra deadline/khối lượng: 5']
→ [Xếp thứ tự ưu tiên: 8'] ← BOTTLENECK
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi quay lại một báo cáo đang làm dở sau khi chuyển sang bài tiếng Anh hoặc bài lab, tôi muốn biết chính xác mình đã làm đến đâu và bước tiếp theo là gì, để có thể tiếp tục công việc ngay. |
| Actor | Tôi — người phải chuyển đổi giữa báo cáo ở trường, bài tập tiếng Anh và lab của khóa AI thực chiến. |
| Thời điểm / bối cảnh | Khi quay lại báo cáo sau một khoảng gián đoạn để xử lý nhiệm vụ khác có deadline gần hơn. |
| Quy trình hiện tại (3–7 bước) | (1) Mở báo cáo và thư mục tài liệu: 1 phút; (2) đọc lại phần đã viết để khôi phục trạng thái: 4 phút; (3) tìm lại tài liệu liên quan: 3 phút; (4) xác định phần cần viết tiếp: 2 phút. Tổng 10 phút. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Đọc lại phần đã viết để nhớ và xác định trạng thái hiện tại, khoảng 4 phút/lần. |
| Impact (nếu không giải thì sao) | Xảy ra khoảng 3 lần/tuần, làm mất khoảng 30 phút/tuần chỉ để khôi phục ngữ cảnh và làm chậm tiến độ báo cáo. |
| Success metric (baseline → target) | Thời gian khôi phục ngữ cảnh từ 10 phút xuống 3–4 phút/lần; tổng thời gian mất cho việc này từ khoảng 30 phút xuống tối đa 12 phút/tuần. Đo bằng thời điểm mở lại và bắt đầu viết tiếp. |
| Phương án không dùng AI | Cuối mỗi phiên ghi ba dòng: đã hoàn thành gì, đang dừng ở đâu và bước tiếp theo là gì; gắn link tài liệu cần dùng tiếp. |
| Giả thuyết về AI (nếu có) | Một workflow có thể đọc báo cáo cùng ghi chú gần nhất, tóm tắt trạng thái và gợi ý phần tiếp theo; tôi kiểm tra trước khi tiếp tục viết. |
| Cảm nhận nhanh | Rule hoặc Workflow; phương án ghi chú không AI có thể đã đủ. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 10 phút/lần, khoảng 3 lần/tuần

[Mở báo cáo/tài liệu: 1']
→ [Đọc lại để khôi phục trạng thái: 4'] ← BOTTLENECK
→ [Tìm tài liệu liên quan: 3']
→ [Xác định phần viết tiếp: 2']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi tổng hợp chi tiêu trong tháng, tôi muốn xác định mục đích và phân loại các giao dịch ngân hàng, để biết tiền đã được sử dụng vào đâu và đánh giá việc chi tiêu có hợp lý hay không. |
| Actor | Tôi — người đang tự theo dõi chi tiêu cá nhân bằng lịch sử ngân hàng và ghi chú. |
| Thời điểm / bối cảnh | Khoảng 2 lần/tháng, khi tôi mở lịch sử giao dịch để ghi lại và đánh giá chi tiêu của tháng. |
| Quy trình hiện tại (3–7 bước) | (1) Mở và lọc lịch sử giao dịch: 2 phút; (2) đọc từng giao dịch và nhớ lại mục đích: 15 phút; (3) phân loại rồi ghi vào ghi chú: 8 phút; (4) tổng hợp và đánh giá chi tiêu: 5 phút. Tổng 30 phút/lần. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Nhớ lại mục đích của từng giao dịch, khoảng 15 phút/lần; mô tả giao dịch không phải lúc nào cũng đủ để nhận biết khoản chi. |
| Impact (nếu không giải thì sao) | Mất khoảng 1 giờ/tháng; tháng vừa rồi có khoảng 5 giao dịch tôi không nhớ rõ mục đích, nên không biết tiền đã đi đâu và khó đánh giá chi tiêu có hợp lý hay không. |
| Success metric (baseline → target) | Thời gian tổng hợp từ 30 xuống tối đa 10 phút/lần; giao dịch không xác định được mục đích từ khoảng 5 xuống tối đa 1 giao dịch/tháng. Đo trên ghi chú chi tiêu cuối tháng. |
| Phương án không dùng AI | Ghi mục đích ngay sau khi chi, dùng danh sách nhóm chi tiêu cố định và bổ sung nội dung chuyển khoản dễ nhận biết khi có thể. |
| Giả thuyết về AI (nếu có) | AI gợi ý nhóm chi tiêu từ mô tả giao dịch và lịch sử đã xác nhận; các giao dịch mơ hồ phải được tôi kiểm tra trước khi lưu. |
| Cảm nhận nhanh | Rule hoặc Workflow; chưa cần Agent. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 30 phút/lần, 2 lần/tháng

[Mở/lọc lịch sử giao dịch: 2']
→ [Đọc và nhớ lại mục đích: 15'] ← BOTTLENECK
→ [Phân loại, ghi chú: 8']
→ [Tổng hợp, đánh giá: 5']
```

### Card muốn pitch nhất

- Card số: 1 — Quản lý nhiệm vụ và deadline từ nhiều nền tảng.
- Vì sao: Đây là vấn đề xảy ra hằng ngày, có tác động rõ nhất (khoảng 4 lần/tháng phải làm gấp) và có thể đo cả thời gian lẫn số lần sát deadline. Bài toán cũng cho phép so sánh rõ phương án checklist không AI với Rule hoặc Workflow.
- Câu hỏi muốn nhóm phản biện: Một checklist/lịch chung không dùng AI có đủ giúp giảm số lần phải làm gấp từ khoảng 4 xuống tối đa 1 lần/tháng không, hay bottleneck tổng hợp và ưu tiên từ nhiều nguồn thực sự cần Workflow?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Actor ban đầu chỉ ghi “tôi”, chưa cho thấy vì sao có nhiều loại nhiệm vụ và nhiều nguồn. | Đồng ý | Cụ thể hóa actor là học viên đang đồng thời học ở trường, trung tâm tiếng Anh, khóa AI và tham gia nhóm build phase. |
| Metric chỉ đo thời gian kiểm tra; làm nhanh hơn chưa chắc giúp tránh trễ hoặc làm gấp. | Đồng ý | Bổ sung outcome metric: số lần phải làm gấp giảm từ khoảng 4 xuống tối đa 1 lần/tháng. |
| Giả thuyết Workflow có nguy cơ nhảy sang AI quá sớm vì checklist/lịch chung có thể đã đủ. | Đồng ý | Bổ sung phương án không AI và giữ Workflow là giả thuyết ban đầu; câu hỏi pitch yêu cầu nhóm phản biện xem mức đơn giản hơn có đủ không. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tôi trình bày ba candidate #7 quản lý nhiệm vụ/deadline, #8 tiếp tục báo cáo đang làm dở và #9 phân loại giao dịch chi tiêu, kèm actor, bottleneck và số liệu hiện có. | Candidate #7 được đưa vào shortlist và sau đó được nhóm chọn để làm tiếp. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Với candidate #2, người học xác định phát âm đúng/sai bằng cách nào và việc nghe lại nhiều lần có phải do thiếu cách đánh giá không? Với candidate #5, khó khăn chính là hiểu thông báo lỗi hay tìm cách sửa, và công cụ giải thích lỗi có đủ nếu thiếu kiến thức Python nền tảng không? | Giúp nhóm tách biểu hiện bề mặt khỏi nguyên nhân và nhận ra candidate #5 còn thiếu số liệu về tần suất/thời gian. |
| Nhận phản biện | Câu hỏi tôi nhận được từ Hà Huy Thái: cách hiện tại tôi quản lý deadline là gì, vì sao chưa hiệu quả, và việc làm gấp là do không biết ưu tiên hay do khối lượng công việc quá nhiều? | Tôi ghi nhận không được mặc định “xếp ưu tiên” là nguyên nhân duy nhất; CP4 cần kiểm chứng riêng giả định về thông tin phân tán, cách ưu tiên và tình trạng quá tải. |
| Gom cluster / cây OST | Tôi cung cấp ba candidate #7–#9 cùng số liệu; nhóm xếp chúng vào cluster C “Quản lý công việc và thông tin cá nhân”. Tôi cùng nhóm phân biệt opportunity với các solution như chatbot, ứng dụng quản lý hay AI Agent. | OST tập trung vào outcome giảm tình trạng làm gấp sát deadline và ba opportunity: ưu tiên, nắm deadline và cân đối tiến độ. |
| Chọn candidate problem | Tôi cùng nhóm đối chiếu shortlist theo 7 tiêu chí. Candidate #7 đạt 34 điểm, cao nhất trong ba candidate được chấm. | Nhóm thống nhất chọn #7 vì actor/quy trình rõ, có baseline khoảng 25 phút/ngày và hậu quả khoảng 4 lần/tháng phải làm gấp. |
| Kiểm chứng / research | Tôi phụ trách research ba hướng hiện có: Todoist để tập trung task, Zapier cho workflow Discord–Todoist và Motion để tự sắp lịch. Tôi đối chiếu tài liệu chính thức, bước được giải và khoảng trống. | Research cho thấy nên thử thay đổi quy trình hoặc workflow phạm vi nhỏ trước; việc thu thập task từ toàn bộ nguồn và chất lượng dữ liệu đầu vào vẫn là rủi ro cần kiểm chứng. |
| Quy trình nhóm | Tôi dùng số liệu từ Problem Card #1 để chi tiết hóa quy trình hiện tại thành bốn bước có actor, input, output và thời gian; đồng thời xây dựng quy trình tương lai giả thuyết gồm Rule/Workflow, AI hỗ trợ và bước con người kiểm tra. | Nhóm có cơ sở so sánh trước/sau: từ khoảng 25 phút/ngày xuống mục tiêu tối đa 10 phút/ngày, với boundary và phương án quay về rõ ràng để đưa sang CP6 đánh giá. |
| Problem Statement |Không dùng AI; không trực tiếp viết Problem Statement (xem mục 4). |Không ảnh hưởng |
| Mức can thiệp AI |Không dùng AI  | Không ảnh hưởng|
| Quyết định |không trực tiếp viết mục 6–8 (xem mục 4) |Không ảnh hưởng |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Hỗ trợ tách các tình huống tôi tự scan và diễn đạt lại theo Job Story. | Giúp phân biệt problem với solution và nhắc bổ sung số liệu đo được. | Ban đầu giữ hai ý “yêu cầu bài lab” và “thông tin khóa học” dù chúng khá trùng nhau; một số gợi ý chưa có bằng chứng thật. | Tôi nhận ra điểm trùng, thay ý thứ hai bằng vấn đề chi tiêu có số liệu thật và loại các ý chưa kiểm chứng. |
| CP2 Problem Card | Hỗ trợ cấu trúc ba card, chuyển mô tả quy trình thành sơ đồ và đóng vai PM hoài nghi để phản biện. | Giúp làm rõ actor, bottleneck, baseline–target và phương án không AI. | Ban đầu AI chỉ chú ý metric thời gian và đề xuất phân bổ thời gian từng bước trước khi tôi xác nhận. | Tôi xác nhận lại thời gian theo trải nghiệm, bổ sung metric số lần phải làm gấp và giữ Workflow chỉ là giả thuyết để nhóm phản biện. |
| CP4 Research | Dùng AI để tìm và so sánh các pattern quản lý tập trung, workflow trigger–action và auto-scheduling; sau đó truy về tài liệu chính thức. | Giúp lập bảng so sánh theo đúng bước quy trình, điểm mạnh, khoảng trống và bài học thay vì chỉ liệt kê tên công cụ. | Kết quả tìm kiếm và trang giới thiệu sản phẩm có thể nhấn mạnh lợi ích nhưng không chứng minh công cụ hỗ trợ toàn bộ nguồn dữ liệu của nhóm. | Tôi giới hạn claim theo tài liệu chính thức, ghi rõ phần nào chỉ giải Discord hoặc yêu cầu nhập task trước, và yêu cầu tự mở/kiểm tra link trước khi chốt. |
| CP5 Quy trình | Nhờ AI chuyển mô tả và số liệu đã có trong Problem Card #1 thành bảng actor–input–output–thời gian, rồi gợi ý cách trình bày quy trình tương lai và bảng before/after. | Giúp tách rõ bước Rule/Workflow, bước AI hỗ trợ, bước con người kiểm tra, boundary và phương án quay về. | Các mốc khoảng 1–4 phút trong quy trình tương lai do AI phân bổ từ target 10 phút, chưa phải số liệu đã được pilot chứng minh; bước AI/optimization cũng chưa được CP6 chốt. | Tôi giới hạn tự động nhập ở Discord theo research, giữ Zalo/Cohort/web khóa học ở bước kiểm tra thủ công, ghi rõ thời gian tương lai là kỳ vọng cần đo khi pilot và coi toàn bộ quy trình là giả thuyết để CP6 so sánh với No AI/Rule. |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi nghe 6 card của Minh và Thái, tôi thấy card nào chỉ mô tả triệu chứng thì rất khó chấm. Ở card phát âm, tôi hỏi Minh: nghe lại bản ghi 5 lần là do thiếu cách đánh giá, hay do chưa biết cách phát âm? Ở card lỗi Python, tôi hỏi Thái: khó ở chỗ hiểu thông báo lỗi, hay ở chỗ tìm cách sửa? Cả hai câu đều để tách biểu hiện bề mặt khỏi nguyên nhân thật, vì nguyên nhân khác nhau thì cách giải cũng khác nhau. Sau đó card #5 của Thái bị loại vì chưa có số phút hay tần suất nào. Tôi rút ra rằng không nên chọn vấn đề vì giải pháp nghe hấp dẫn, mà phải so actor, quy trình, bottleneck và bằng chứng đo được.
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có, và chính tôi là người mắc. Ở CP2, ô "Cảm nhận nhanh" của card #1 tôi ghi Workflow. AI phản biện rằng tôi đang nhảy sang AI quá sớm, nên tôi thêm phương án checklist không AI và ghi rõ Workflow chỉ là giả thuyết. Nhưng đến CP5, khi vẽ quy trình tương lai ở mục 4.2, tôi vẫn gắn nhãn "RULE/WORKFLOW" cho bước đồng bộ và "AI/OPTIMIZATION" cho bước đề xuất thứ tự, trong khi nhóm chưa so sánh 4 mức. Sang CP6, nhóm nhận ra bước 1 chỉ là automation không có AI, còn bước 4 làm được bằng cách sắp theo hạn và gắn cờ quá tải, tức cả hai đều là Rule. Nhóm chọn Rule và để bước AI ở Not Yet. Tôi học được rằng ghi chữ "giả thuyết" là chưa đủ: một khi nhãn AI đã nằm trên sơ đồ, người đọc vẫn hiểu là nhóm đã chọn AI.
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Card #1 của tôi đặt bottleneck ở bước xếp thứ tự ưu tiên, tức là tôi ngầm coi làm gấp là do không biết việc nào cần làm trước. Khi tôi pitch, Thái hỏi: làm gấp là do không biết ưu tiên, hay do khối lượng quá nhiều và thiếu thời gian? Lúc đó tôi chưa có số liệu để tách hai nguyên nhân này. Vì vậy nhóm đưa vào assumption map giả định "khó xếp ưu tiên góp phần khiến làm gấp, bên cạnh thiếu thời gian và trì hoãn" để kiểm chứng ở CP4. Kết quả là học viên C làm gấp dù đã có danh sách và biết thứ tự, đúng điều Thái nghi ngờ. Từ đó, Problem Statement v1 tách việc làm gấp theo 4 nguyên nhân và đưa trường hợp thiếu thời gian ra ngoài target.
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Có hai điều. Thứ nhất, snapshot C cho thấy ngay cả khi danh sách và thứ tự đã đúng, người học vẫn làm gấp vì ca làm thêm kéo dài. Nghĩa là quản lý thông tin tốt hơn không giải được mọi trường hợp. Thứ hai là ở phần research tôi phụ trách: không công cụ nào lấy được nhiệm vụ từ cả 5 nguồn. Zapier chỉ nối được Discord, còn Zalo, ứng dụng tiếng Anh, Cohort và web khóa AI vẫn phải nhập tay. Khi rà soát, trang tích hợp Zapier tôi trích không có câu "kiểm tra 15 phút/lần"; phải lấy từ trang giá, và trang giá còn cho biết gói Free không có Filter. Chính thông tin này quyết định thiết kế sau đó: task từ Discord chỉ là task ứng viên, người học phải duyệt.
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là chấp nhận rằng số liệu của chính tôi chưa đủ làm bằng chứng. Con số 25 phút/ngày và 4 lần/tháng tôi đưa ra ở CP1 theo trí nhớ về tháng gần nhất, vậy mà nó trở thành baseline của cả bài. Problem Statement buộc phải ghi rõ đây là ước lượng của một người, và phải thêm 2 tuần ghi nhật ký để đo lại. Khó thứ hai là giữ bottleneck ở bước 4 (8 phút) trong khi bước 1–2 cộng lại tốn 12 phút. Nhóm phải viết rõ lý do: bước 1–2 chỉ tốn thời gian, còn bước 4 là chỗ chọn sai dẫn đến làm gấp.
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Tôi sẽ bấm giờ vài ngày trước khi pitch #7: chỉ cần một bảng ghi đơn giản là baseline đã mạnh hơn nhiều so với ước lượng theo trí nhớ. Khi vẽ quy trình tương lai, tôi sẽ để trống nhãn mức can thiệp cho đến khi CP6 so sánh xong No AI, Rule, Workflow và Agent. Với research, tôi sẽ tự mở từng link và trích nguyên văn trước khi đưa vào bảng. Điểm tôi muốn phản biện nhóm mạnh hơn là phần phỏng vấn: nhóm chưa hỏi người được phỏng vấn có muốn giao việc chọn ưu tiên cho hệ thống hay không, nên câu trả lời "augment" ở mục 6.4 vẫn chỉ là định hướng cần kiểm chứng.
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Problem sẽ chỉ ra được điểm đau --> Quy trình chỉ ra chỗ đau xuất hiện --> Boundary giới hạn cách giải để tránh rủi ro --> Mức can thiệp chọn công cụ đơn giản nhất để đạt metric --> Quyết định xác định có thử hay không, thử thế nào và khi nào phải dừng.
Nhóm tập trung giải quyết tình trạng học viên phải chạy deadline khoảng 4 lần mỗi tháng khi vừa học ở trường, vừa tham gia khóa tiếng Anh và khóa AI. Hiện tại, mỗi ngày học viên mất khoảng 25 phút để mở 5 nền tảng, tổng hợp nhiệm vụ, kiểm tra thời hạn, ước lượng khối lượng và chọn việc cần làm trước. Riêng bước xếp thứ tự ưu tiên mất khoảng 8 phút. Đây là điểm nghẽn vì người học phải quyết định trong khi danh sách có thể còn thiếu nhiệm vụ hoặc khối lượng công việc đã được ước lượng sai. Do số lần làm gấp phụ thuộc vào số deadline trong tháng, nhóm chọn tỷ lệ nhiệm vụ phải làm gấp làm chỉ số chính và theo dõi riêng theo từng nguyên nhân. Hai tiêu chí đi kèm là thời gian kiểm tra và chọn việc tối đa 10 phút mỗi ngày, đồng thời số nhiệm vụ bị bỏ sót không được tăng. Người học vẫn giữ quyền quyết định. Hệ thống không tự thêm nhiệm vụ vào danh sách chính, tự sửa hoặc suy đoán thời hạn, gửi tin nhắn hay nộp bài. Người học cần kiểm tra khi có nhiệm vụ mới, khi thời hạn chưa rõ, khi còn dưới 48 giờ đến hạn hoặc khi hệ thống báo quá tải. Các thao tác như sắp xếp theo hạn, nhắc trước 48 giờ và gắn cờ quá tải đều có điều kiện xử lý rõ ràng. Qua tìm hiểu, nhóm nhận thấy Todoist và Zapier có thể thực hiện các thao tác này mà không cần viết mã. Vì vậy, nhóm chọn tự động hóa bằng quy tắc (Rule) và không dùng AI trong đợt thử nghiệm. Nhóm quyết định Go với phạm vi nhỏ, triển khai pilot 6 tuần gồm 2 tuần đo hiện trạng (baseline) và 4 tuần áp dụng Rule. Hai bước dự kiến dùng AI được xếp ở mức Not Yet, còn phương án Agent là No-Go vì cần truy cập tin nhắn cá nhân. Pilot sẽ dừng ngay khi chạm bất kỳ ngưỡng nào trong 4 ngưỡng dừng đã xác định.
---

## 7. Tài liệu tham khảo

-
