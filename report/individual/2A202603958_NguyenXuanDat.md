# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Nguyễn Xuân Đạt
- MSSV:2A202603958
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:3randomguy
- Link repo nhóm:https://github.com/hoangngochieu10012000/K5-L3-Day02-3randomguy-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Khi chuẩn bị họp tiến độ hằng tuần với giảng viên hướng dẫn, tôi muốn có sẵn hình ảnh tổng quan rõ ràng về việc ai đã hoàn thành task trong tuần vừa qua để báo cáo mạch lạc, không bị lúng túng và tránh việc bị mentor khiển trách vì đã chưa hoàn thành được nhiệm vụ được giao | Trưởng nhóm, Thành viên nhóm, Giảng viên hướng dẫn | Mỗi tuần mất khoảng 20-30 phút chỉ để đối chất, hỏi đáp xem ai đã làm được cái gì trogn tuần vừa rồi; bị mentor trách móc vì không minh bạch được tiến độ của từng thành viên và cả nhóm |
| 2 | Lặp lại | Khi họp nhóm, tôi muốn có sẵn danh sách đầu việc mình đã làm trogn tuần qua và  danh sách những vấn đề của thành viên khác mình tìm thấy khi làm việc liên quan đến phần làm việc của họ | Bản thân, Thành viên nhóm | Mỗi lần khi họp nhóm đều bối rối, không nhớ được hết phần việc mình cần làm và những vấn đề của thành viên khác mà mình tìm ra khi làm phần việc có liên quan đến họ |
| 3 | Tốn thời gian | Khi bắt đầu phân chia task cho sprint mới, tôi muốn có một danh sách công việc được phân tích rõ ràng về độ khó và khối lượng công việc, để có thể giao công bằng cho các thành viên, tránh việc vài người phải làm quá nhiều còn vài người lại chỉ cần làm quá ít | Cả nhóm | Các buổi họp thường sẽ kéo dài do phân chia công việc khoogn công bằng, sẽ có người phàn nàn rằng phần của mình quá dài hoặc không đủ khả năng làm |
| 4 | Tốn thời gian | Khi một thành viên thay đổi sơ đồ kiến trúc hệ thống (như ERD hoặc Use Case) trên công cụ thiết kế, tôi muốn hệ thống tự động thông báo hoặc cập nhật ngay lập tức các điểm thay đổi, để các thành viên khác không tiếp tục code theo bản cũ, tránh lệch pha gây tốn hàng giờ debug. |Thành viên làm BE, FE, tài liệu | Mỗi tuần có ít nhất 1-2 lần nhóm phải ngồi họp khẩn hoặc nhắn tin debug code do code bị lệch so với thiết kế database/sơ đồ mới cập nhật. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi đến hạn gộp code (merge) các nhánh tính năng chung vào nhánh chính của đồ án, tôi muốn các đoạn mã được quy chuẩn rõ ràng và kiểm duyệt kỹ, để không bị dính lỗi Conflict chồng chất, mất cả ngày giải quyết thay vì code tính năng mới. | Tất cả thành viên làm lập trình, người quản lí repo của nhóm | Mỗi đợt merge code trước deadline sprint thường tốn từ 2 đến 4 tiếng chỉ để gỡ lỗi conflict; đã từng có lần mất hẳn code do gộp nhầm nhánh. |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi các thành viên cùng nghiên cứu tài liệu lý thuyết hoặc công nghệ mới cho đồ án, tôi muốn có một kho lưu trữ và ghi chú chung tập trung, để khi viết báo cáo không bị lặp ý, tản mác hay lệch phong cách hành văn. | Các thành viên viết báo cáo và tài liệu | Tài liệu nghiên cứu rải rác ở Google Drive cá nhân, Zalo và tab trình duyệt; khi ghép nối thành chương báo cáo lý thuyết phải mất 2-3 buổi ngồi biên tập lại từ đầu vì văn phong quá rời rạc. |
| 7 | Pain từ người khác | Khi triển khai các task phát triển đồ án theo tiến độ chung, tôi muốn mọi thành viên đều cam kết tham gia họp và hoàn thành đúng hạn, để không xảy ra tình trạng "tàng hình" đến sát ngày nộp mới xin gắn tên, gây áp lực khủng khiếp cho người gánh việc. | Cả nhóm | Có thành viên vắng mặt trên 50% các buổi họp sprint, trễ deadline liên tục và chỉ liên lạc được vào 2 ngày cuối trước khi nộp đồ án. |
| 8 | Pain từ người khác | Khi nhóm cần họp trực tiếp hoặc ngồi code chung để giải quyết các tính năng khó, tôi muốn dễ dàng tìm ra các khoảng thời gian trống chung trong tuần của tất cả mọi người, để không bị kẹt vì lịch học và lịch làm thêm lệch nhau quá nhiều. | Cả nhóm | Mỗi lần hẹn họp nhóm online/offline đều phải nhắn tin căn kè mất 15-20 phút mà vẫn thiếu người vì lịch học phần lớn thời gian trong ngày bị lệch nhau. |
| 9 | Pain từ người khác | Khi cần thống nhất ý tưởng thiết kế giao diện (UI/UX) hoặc lựa chọn công nghệ giữa các thành viên, tôi muốn có một tiêu chí đánh giá minh bạch, để không mất quá nhiều thời gian tranh cãi cảm tính giữa các ý kiến trái chiều. | Cả nhóm | Các buổi thảo luận ý tưởng thường kéo dài hơn 2 tiếng mà không chốt được phương án vì mỗi người thích một kiểu giao diện/công nghệ khác nhau. |
| 10 | Lặp lại | Khi kết thúc mỗi buổi họp nhóm với mentor hoặc họp nội bộ, tôi muốn tự động ghi nhận lại các quyết định chính và danh sách action items, để không bị trôi việc và có căn cứ quy trách nhiệm rõ ràng. | Trưởng nhóm, thành viên viết biên bản cuộc họp | Biên bản họp thường ghi tản mác trên group chat Zalo/Discord, tuần sau thường xuyên quên mất ai chịu trách nhiệm làm task cũ. |
| 11 | Tốn thời gian | Khi đến hạn nộp các sản phẩm demo (artifact) theo từng mốc milestone của đồ án, tôi muốn có quy trình đóng gói và kiểm thử tự động (build/deploy test), để không bị lỗi vặt vào phút chót khi nộp bài cho hội đồng hoặc giảng viên. | Thành viên phụ trách kỹ thuật (DevOps/Lead) | Đêm trước ngày nộp milestone thường phải thức đến 3-4 giờ sáng để fix lỗi build local chạy được nhưng đưa lên server/máy khác thì lỗi. |

**Nếu có dùng AI để gợi ý thêm:** sau khi tham khảo thêm ai, tôi quyết định giữ lại tính năng 9, 10, 11 và bỏ ý "Tìm quyết định cũ trong Slack" do rủi ro về quyền riêng tự khi cấp quyền truy cập vào các công cụ trao đổi thoogn tin

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Problem #1: Theo dõi và báo cáo tiến độ với Mentor | Pain cực kỳ thực tế: Bất kỳ nhóm làm đồ án nào cũng gặp tình trạng này hằng tuần. | Chất lượng nội dung tóm tắt: Liệu bản nháp do AI hoặc hệ thống tự động tổng hợp có thực sự phản ánh đúng ngữ cảnh công việc và "độ mượt" của tiến độ không, hay PM vẫn phải sửa lại gần như toàn bộ? |
| 2 | Problem #4: Đồng bộ tài liệu thiết kế hệ thống | Tác động kỹ thuật cao (High Impact): Tránh được tình trạng "mỗi người code một phách" do không đồng bộ database/sơ đồ. | Thói quen của thành viên: Liệu các thành viên trong nhóm có thực hiện nghiêm túc việc cập nhật sơ đồ ngay khi đổi ý tưởng thiết kế không, hay họ vẫn sửa code trước rồi mới quên cập nhật tài liệu sau? |
| 3 | Problem #5: Quản lý mã nguồn và xử lý Git Conflict | Đặc thù ngành phần mềm: Đây là nỗi đau kinh điển của mọi sinh viên CNTT khi làm đồ án nhóm. | Hiệu quả tuân thủ quy chuẩn: Liệu việc áp dụng quy chuẩn nhánh (branching strategy) và bắt buộc Code Review có làm chậm tốc độ release tính năng của các thành viên trong giai đoạn nước rút sát deadline không? |

### Problem Card #1 — Báo cáo tiến độ tuần với mentor

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị buổi họp tiến độ hằng tuần với giảng viên hướng dẫn, tôi muốn có sẵn bảng tổng hợp ai đã làm xong task nào, task nào trễ và vì sao, để báo cáo mạch lạc trong 5 phút đầu buổi họp mà không phải hỏi lại từng người |
| Actor | Trưởng nhóm đồ án (người trực tiếp báo cáo với mentor) |
| Thời điểm / bối cảnh | Tối trước hoặc sáng ngày họp mentor, mỗi tuần 1 lần; task đang ghi rải rác trên Trello/Excel, commit trên GitHub và tin nhắn Zalo/Discord |
| Quy trình hiện tại (3–7 bước) | 1. Mở bảng task (Trello/Excel) xem trạng thái · 2. Nhắn Zalo hỏi từng thành viên "tuần này làm được gì" · 3. Chờ trả lời, hỏi lại người chưa trả lời · 4. Đối chiếu với commit GitHub để xác nhận · 5. Viết tóm tắt: việc đã xong, việc trễ, vướng mắc · 6. Trình bày với mentor |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3, hỏi và chờ thành viên trả lời: khoảng 20–30 phút/tuần (ước lượng theo trí nhớ, cần bấm giờ thật 2 tuần tới), có khi phải chờ đến sát giờ họp |
| Impact (nếu không giải thì sao) | Khoảng 20–30 phút/tuần chỉ để đối chất tiến độ; trưởng nhóm lúng túng khi mentor hỏi; nhóm đã bị mentor nhắc vì không minh bạch được tiến độ từng người; thành viên làm ít khó bị phát hiện sớm |
| Success metric (baseline → target) | (1) Thời gian chuẩn bị báo cáo: 20–30 phút → dưới 10 phút; (2) Số lần mentor hỏi "phần này ai làm, xong chưa?" mà trưởng nhóm không trả lời được: đếm 3 buổi gần nhất làm baseline → giảm về 0 |
| Phương án không dùng AI | Quy ước mỗi thành viên tự cập nhật trạng thái task trên Trello/GitHub Projects trước 21h hôm trước buổi họp + template báo cáo cố định 3 mục (Đã xong / Đang làm / Vướng mắc) |
| Giả thuyết về AI (nếu có) | AI đọc trạng thái task + commit GitHub trong tuần, soạn nháp báo cáo theo template; trưởng nhóm kiểm và sửa trước khi trình bày. AI không tự đánh giá ai "lười" |
| Cảm nhận nhanh | Rule (nhắc cập nhật + gom số liệu) + Workflow (AI soạn nháp) — cần kiểm chứng xem template + quy ước đã đủ chưa |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 40–50 phút/tuần (ước lượng)

[1 Xem bảng task: 5'] → [2 Nhắn hỏi từng người: 10'] → [3 Chờ + hỏi lại: 10–20'] ← BOTTLENECK
→ [4 Đối chiếu commit GitHub: 5–10'] → [5 Viết tóm tắt: 10'] → [6 Trình bày với mentor]
```

### Problem Card #2 — Đồng bộ tài liệu thiết kế hệ thống (ERD/Use Case)

| Trường | Nội dung |
|---|---|
| Job Story | Khi một thành viên sửa sơ đồ thiết kế (ERD, Use Case) trên công cụ thiết kế, tôi muốn những người bị ảnh hưởng biết ngay phần nào thay đổi, để không tiếp tục code theo bản cũ rồi mất hàng giờ debug |
| Actor | Thành viên làm Backend/Frontend và người viết tài liệu trong nhóm đồ án |
| Thời điểm / bối cảnh | Giữa sprint, khi thiết kế database hoặc luồng nghiệp vụ được chỉnh sửa trên draw.io/dbdiagram/Figma trong lúc các thành viên khác đang code song song |
| Quy trình hiện tại (3–7 bước) | 1. Một người sửa sơ đồ trên công cụ thiết kế · 2. (Có khi quên) nhắn lên group Zalo/Discord "mình sửa ERD rồi" · 3. Người khác không đọc hoặc không biết cụ thể đổi bảng/cột nào · 4. Tiếp tục code theo bản cũ · 5. Lỗi xuất hiện khi ghép code/chạy thử · 6. Họp khẩn hoặc nhắn tin debug tìm nguyên nhân · 7. Sửa code cho khớp thiết kế mới |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3: thông báo thay đổi không có hoặc không rõ đổi gì. Hậu quả dồn sang bước 6: mỗi lần debug lệch thiết kế mất khoảng 1–2 giờ (ước lượng, cần ghi lại các lần xảy ra) |
| Impact (nếu không giải thì sao) | 1–2 lần/tuần phải họp khẩn hoặc debug do code lệch thiết kế; mỗi lần khoảng 1–2 giờ × 2–3 người liên quan; tài liệu cuối kỳ không khớp code thật |
| Success metric (baseline → target) | Số lần debug do lệch thiết kế: 1–2 lần/tuần → dưới 1 lần/2 tuần; thời gian từ lúc sửa sơ đồ đến lúc người liên quan xác nhận đã đọc: chưa đo → dưới 24h |
| Phương án không dùng AI | Lưu file sơ đồ (dbdiagram/.drawio) trong repo GitHub; mọi thay đổi phải qua Pull Request có mô tả "đổi bảng/cột gì" và tag người liên quan; quy ước 1 người giữ quyền sửa ERD |
| Giả thuyết về AI (nếu có) | AI đọc diff giữa 2 phiên bản sơ đồ và viết tóm tắt dễ hiểu "thêm cột X vào bảng Y, ảnh hưởng API Z"; người sửa duyệt trước khi gửi |
| Cảm nhận nhanh | Rule (PR + thông báo tự động khi file sơ đồ đổi); AI chỉ là phần phụ để tóm tắt diff |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — mỗi lần lệch thiết kế mất khoảng 1–2 giờ × 2–3 người

[1 Sửa sơ đồ] → [2 Nhắn group (hay quên)] ← BOTTLENECK
→ [3 Người khác không biết đổi gì] → [4 Code theo bản cũ]
→ [5 Lỗi khi ghép code] → [6 Họp khẩn/debug: 60–120'] → [7 Sửa code]
```

### Problem Card #3 — Quản lý mã nguồn và xử lý Git conflict

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến hạn merge các nhánh tính năng vào nhánh chính trước deadline sprint, tôi muốn code được review và merge dần theo quy chuẩn, để không phải mất 2–4 tiếng gỡ conflict dồn cục vào phút cuối |
| Actor | Thành viên lập trình và người quản lý repo của nhóm |
| Thời điểm / bối cảnh | 1–2 ngày trước deadline sprint, khi mọi người cùng đẩy code lên sau nhiều ngày code riêng trên nhánh của mình |
| Quy trình hiện tại (3–7 bước) | 1. Mỗi người code trên nhánh riêng nhiều ngày không pull nhánh chính · 2. Sát deadline, mọi người cùng tạo PR/merge · 3. Conflict xuất hiện ở nhiều file · 4. Người quản lý repo đọc từng conflict, hỏi tác giả nên giữ đoạn nào · 5. Gỡ conflict, chạy thử · 6. Phát hiện lỗi do gộp sai, sửa tiếp |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4–5: đọc và gỡ conflict, mất 2–4 tiếng mỗi đợt merge |
| Impact (nếu không giải thì sao) | 2–4 tiếng/đợt merge của người quản lý repo, chưa tính thời gian các thành viên bị gọi hỏi; đã từng mất code do gộp nhầm nhánh; thời gian code tính năng mới bị cắt ngay trước deadline |
| Success metric (baseline → target) | Thời gian gỡ conflict mỗi đợt merge: 2–4 tiếng → dưới 30 phút; số lần mất code do merge sai: đã có ít nhất 1 lần → 0 |
| Phương án không dùng AI | Branching strategy đơn giản (feature branch ngắn, merge ít nhất 2 lần/tuần); branch protection trên GitHub bắt buộc PR + 1 người review; CI chạy build/test khi mở PR; quy ước pull nhánh chính mỗi ngày |
| Giả thuyết về AI (nếu có) | AI có sẵn (Copilot code review, giải thích conflict) hỗ trợ đọc PR và gợi ý cách gộp; người review vẫn quyết định cuối |
| Cảm nhận nhanh | No AI / Rule là chính — gốc vấn đề là thói quen merge dồn cục, không phải thiếu AI |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 2–4 tiếng mỗi đợt merge

[1 Code nhánh riêng nhiều ngày] → [2 Cùng merge sát deadline]
→ [3 Conflict nhiều file] → [4 Đọc conflict + hỏi tác giả] ← BOTTLENECK
→ [5 Gỡ conflict + chạy thử] → [6 Sửa lỗi do gộp sai]
```

### Card muốn pitch nhất

- Card số: 1 — Báo cáo tiến độ tuần với mentor
- Vì sao: Quy trình lặp lại đều mỗi tuần, actor rõ (trưởng nhóm), bottleneck rõ (hỏi và chờ thành viên trả lời), có thể bấm giờ đo baseline ngay trong 2 tuần tới, và so sánh được đủ 4 mức No AI / Rule / Workflow / Agent. Card #2 và #3 có impact kỹ thuật lớn nhưng tôi nghiêng về việc Rule/quy trình Git là đủ, AI không phải trọng tâm.
- Câu hỏi muốn nhóm phản biện: "Nếu chỉ cần quy ước mỗi người tự cập nhật Trello trước 21h hôm trước buổi họp + template báo cáo, thì có còn cần AI không? Vấn đề thật là thiếu công cụ hay là thành viên không chịu cập nhật?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 20–30 phút (card #1) và 1–2 giờ debug (card #2) chỉ dựa vào trí nhớ | Đồng ý | Ghi rõ "ước lượng" trong card; kế hoạch bấm giờ thật 2 buổi họp mentor tới và ghi log mỗi lần debug do lệch thiết kế |
| Card #1: nếu thành viên không cập nhật task thì AI cũng không có dữ liệu để tổng hợp — gốc vấn đề có thể là kỷ luật nhóm (gần với problem #7), không phải thiếu công cụ | Đồng ý một phần | Thêm phương án No AI (quy ước cập nhật + template) và đưa vào câu hỏi muốn nhóm phản biện; giữ AI ở mức soạn nháp từ dữ liệu đã có |
| Gợi ý để AI tự chấm điểm mức độ đóng góp của từng thành viên và gửi thẳng cho mentor | Không đồng ý | Giữ boundary: AI chỉ soạn nháp, trưởng nhóm kiểm và trình bày; AI không đánh giá con người vì dễ sai và gây mâu thuẫn trong nhóm |
| Card #3: conflict là hệ quả của cách làm việc (merge dồn cục), dùng AI gỡ conflict chỉ chữa triệu chứng | Đồng ý | Đổi cảm nhận nhanh của card #3 sang No AI / Rule (branching strategy, branch protection, CI) |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Problem Card #1 (Báo cáo tiến độ tuần với mentor) | Card này cùng nhóm với candidate nhóm chọn "Tổng hợp báo cáo tuần từ nhiều nguồn" |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Tôi thấy PC của thành viên 1 không đủ thực tế để tiếp tục phát triển | cả nhóm suy nghĩ và đồng tình |
| Nhận phản biện | Câu hỏi tôi nhận được: Không nhận được phản biện trực tiếp về card trong buổi pitch. | Tôi đã sửa gì: không sửa ghì ở khoảng thời gian phản biện này cả |
| Gom cluster / cây OST | Hỗ trợ CP3 theo phân công nhóm (người chính là Nguyễn Công Hoàn)  | giảm thời gian hoàn thiện bài tập |
| Chọn candidate problem | Ủng hộ candidate "Tổng hợp báo cáo tuần" vì actor và baseline rõ * | Nhóm chọn candidate này, bất đồng về "Tìm bàn trống nhà ăn" được giải quyết bằng việc xem xét dữ liệu khả thi |
| Kiểm chứng / research | Hỗ trợ CP4 theo phân công nhóm (người chính là Nguyễn Công Hoàn).  | giảm thời gian hoàn thiện bài tập |
| Quy trình nhóm | Phụ trách chính CP5: quy trình trước/sau và bảng before/after theo phân công nhóm  | đã hoàn thiện công việc được phân công |
| Problem Statement | Phụ trách chính Problem Statement v0 theo phân công nhóm  | đã hoàn thiện công việc được phân công |
| Mức can thiệp AI | Hỗ trợ CP6, người chính là Hoàng Ngọc Hiệu  |  |
| Quyết định | đề xuất chọn go cho việc thí điểm phạm vi nhỏ | Nhóm chọn Go, phạm vi thí điểm nhỏ  |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI gợi ý thêm problem theo vai trò PM/nhóm trưởng  | Gợi ý được một vài pain tôi chưa nghĩ tới, ví dụ ghi chú họp và việc deploy | Có ý quá rộng hoặc có rủi ro quyền truy cập dữ liệu, ví dụ tìm quyết định cũ trong Slack  | Chọn lại các ý theo tiêu chí có quy trình rõ và có bằng chứng; bỏ ý tìm quyết định cũ vì rủi ro quyền riêng tư |
| CP2 Problem Card | AI soạn nháp 3 Problem Card, các trường và sơ đồ quy trình từ bảng scan của tôi | Điền nhanh đủ các trường, trình bày sơ đồ rõ ràng | AI tự đặt con số thời gian (20–30 phút, 1–2 giờ debug) và công cụ (Trello, Excel, draw.io) khi chưa có số đo thật | Ghi "ước lượng" trong card, bỏ các công cụ chưa xác nhận, sẽ bấm giờ thật 2 tuần  |

| CP5 Quy trình | Sử dụng ai để điều chỉnh sơ đồ before/after | giảm thời gian vẽ tay các sơ đồ| | |

** | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?** tôi cảm nhận được sự khác biệt về cách chọn và tạo problem của các bạn khác với các chuyên ngành khác nhau

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.** không có

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?** kết quả kiểm chứng phần lớn đều giống như những gì đã được dự đoán trước đó

**6.5. Điều khó nhất khi viết Problem Statement là gì?** viết được rõ ràng ý và thông tin của mình về vấn đề này

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?** nếu được làm lại, tôi sẽ tối ưu lại thời gian triển khai công việc, phân chia rõ ràng hơn khi đã làm qua một lần

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Khởi đầu bằng problem, nhóm xác định nút thắt lớn nhất là việc trưởng nhóm tốn quá nhiều thời gian và gặp hội chứng "trang trắng" khi phải tự đọc hiểu dữ liệu cộc lốc của thành viên để viết phần nhận định tiến độ và rủi ro. Để giải quyết, quy trình được tối ưu hóa từ 7 bước thủ công thành 5 bước, kết hợp Google Form thu thập dữ liệu chuẩn hóa và script tự động gom bảng. Metric tập trung vào việc giảm tổng thời gian làm báo cáo xuống dưới 25 phút, đồng thời đảm bảo PM phải sửa lại dưới 30% bản nháp và Mentor nắm bắt vấn đề trong vòng 3 phút đọc. Boundary quy định AI tuyệt đối không tự gửi báo cáo đi và không tự bịa thêm số liệu ngoài dữ liệu đầu vào thực tế. Với đặc thù độ mơ hồ cao và quy trình tuyến tính, nhóm chọn mức can thiệp AI ở cấp độ Workflow, nơi AI làm nhiệm vụ sinh bản nháp 3 phần còn con người đóng vai trò chốt chặn kiểm duyệt. Cuối cùng, với 4 rủi ro đều ở mức thấp, nhóm đưa ra quyết định Go với hình thức pilot thử nghiệm nhóm nhỏ trong 2 tuần.

---

## 7. Tài liệu tham khảo
- Các vấn đề đã gặp phải khi làm đồ án với nhóm đại học ở vài tháng trước
-
