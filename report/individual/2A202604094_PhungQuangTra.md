# Báo cáo cá nhân — Phùng Quang Trà - 2A202604094

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Phùng Quang Trà
- MSSV:2A202604094
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:4ward
- Link repo nhóm:https://github.com/phungtr/K5-L3B-Day02-4Ward-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |lặp lại| khi mà mỗi tháng tôi muốn tổng kết lại chi tiêu để kiểm tra lại phát sinh chi tiêu | Người dùng thông thường | mỗi tháng l lần vào ngày đầu tiên|
| 2 |tốn thời gian |khi qua 1 ngày làm việc tôi muốn tổng kết lại để kiểm tra danh sách task đã hoàn thành chưa hoàn thành và sắp tới| Dân văn phòng| sau mỗi một ngày công |
| 3 |cần đọc tổng hợp lại nhiều thông tin|khi tôi muốn đẩy bộ hồ sơ mới trên quy trình giải ngân online do bên khách hàng yêu cầu giải ngân online do bên khách hàng yêu cầu sau mỗi  3 ngày  có 1 bộ hồ sơ mới|CRO nhập liệu|bị khách hàng phản hồi do xử lý chậm|
| 4 |Pain từ người khác |Khi theo dõi sức khỏe cho bệnh nhân khách hàng là người cao tuổi tôi muốn theo dõi, cập nhập lại lịch trình dể theo dõi vẫn đề sức  khỏe sát sao|Bác sĩ, Y tá | trễ lịch tiêm cụ A|
| 5 |Lặp lại|Sau các buổi tập luyện tôi muốn theo dõi mình đã thực hiện được bao lâu để đánh giá giới hạn bản thân| vận động viên | bị chấn thương do quá sức trong quá tập luyện|

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.


---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

> Ghi chú: số phút và tần suất trong các card dưới đây là **ước lượng**, chưa đo thực tế. Sẽ kiểm chứng lại ở CP4.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | CRO nhập và đẩy hồ sơ giải ngân online (CP1 #3) | Actor rõ, quy trình có bước cụ thể, lặp lại đều (~3 ngày/1 bộ), đã có khách phản hồi chậm | Chậm nhất ở bước nào: đọc giấy tờ, nhập liệu hay chờ duyệt? |
| 2 | Tổng kết chi tiêu cuối tháng (CP1 #1) | Mình tự trải qua, lặp lại mỗi tháng, đo được thời gian | Mất bao lâu mỗi lần? Có app nào đã làm tốt chưa? |
| 3 | Tổng kết task cuối ngày làm việc (CP1 #2) | Xảy ra mỗi ngày, nhiều người văn phòng gặp | Pain có đủ lớn không, hay chỉ mất vài phút? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách hàng yêu cầu giải ngân online và có bộ hồ sơ mới, tôi muốn kiểm tra đủ giấy tờ và nhập hồ sơ lên hệ thống nhanh, để khách không phải chờ và phản hồi vì xử lý chậm |
| Actor | CRO nhập liệu (người chịu ảnh hưởng gián tiếp: khách hàng chờ giải ngân) |
| Thời điểm / bối cảnh | Khoảng 3 ngày có 1 bộ hồ sơ mới, xử lý trong giờ làm việc |
| Quy trình hiện tại (3–7 bước) | 1. Nhận hồ sơ từ khách → 2. Kiểm tra đủ giấy tờ → 3. Đọc, trích thông tin từ giấy tờ → 4. Nhập vào hệ thống giải ngân → 5. Đẩy hồ sơ lên duyệt → 6. Sửa và đẩy lại nếu bị trả về |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: đọc và nhập thông tin, ~45 phút/bộ (hơn nửa tổng thời gian) |
| Impact (nếu không giải thì sao) | ~10 bộ/tháng; khách phản hồi do xử lý chậm ~2 lần/tháng; ~3/10 bộ bị trả về vì nhập sai hoặc thiếu, mỗi lần mất thêm ~15 phút |
| Success metric (baseline → target) | Thời gian xử lý 1 bộ hồ sơ: ~80 phút → 40 phút; số bộ bị trả về: 3 -> 1 /tháng; thời gian khách chờ (từ lúc nhận hồ sơ đến lúc đẩy duyệt): đo baseline trước, mục tiêu ≤ 1 ngày làm việc. Đo bằng ghi giờ nhận / bắt đầu / đẩy duyệt mỗi bộ trong 1 tháng |
| Phương án không dùng AI | Checklist giấy tờ bắt buộc; mẫu nhập liệu chuẩn; form cho khách tự điền trước thông tin cơ bản |
| Giả thuyết về AI (nếu có) | Đọc giấy tờ scan và điền sẵn các trường, CRO chỉ kiểm tra lại |
| Cảm nhận nhanh | Rule trước (checklist + bắt buộc đủ trường khi nhập); chỉ lên Workflow nếu bước đọc giấy tờ vẫn là bottleneck sau khi đã có Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~80 phút/bộ hồ sơ (ước lượng)

[Nhận hồ sơ: 5'] → [Kiểm tra đủ giấy tờ: 10'] → [Đọc, trích thông tin: 20']
→ [Nhập hệ thống: 25'] ← BOTTLENECK (bước 3–4: 45') → [Đẩy duyệt: 5']
→ [Sửa nếu bị trả: 15', ~3/10 bộ]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến ngày đầu tháng, tôi muốn biết tháng trước mình đã chi bao nhiêu và chi phát sinh vào đâu, để điều chỉnh chi tiêu tháng sau |
| Actor | Người dùng cá nhân (chính mình) |
| Thời điểm / bối cảnh | Ngày đầu mỗi tháng, 1 lần/tháng |
| Quy trình hiện tại (3–7 bước) | 1. Mở app ngân hàng / ví điện tử → 2. Xem lịch sử giao dịch → 3. Chép từng khoản vào sổ hoặc Excel -> 4. Phân loại (ăn uống, đi lại…) → 5. Cộng tổng, tìm khoản phát sinh |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: chép và phân loại giao dịch từ nhiều app, 10 phút |
| Impact (nếu không giải thì sao) | Không biết tiền đi đâu; vượt ngân sách 2/3 tháng gần đây; hay bỏ dở giữa chừng (chỉ tổng kết xong 1/3 tháng) |
| Success metric (baseline → target) | Thời gian tổng kết: ~23 phút → 10 phút; số tháng tổng kết xong: 1/3 → 3/3. Đo bằng bấm giờ mỗi lần tổng kết |
| Phương án không dùng AI | Dùng 1 tài khoản chính; app quản lý chi tiêu có sẵn; Excel template phân loại |
| Giả thuyết về AI (nếu có) | Tự phân loại giao dịch theo nội dung chuyển khoản |
| Cảm nhận nhanh | Rule hoặc No AI |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~23 phút/tháng (ước lượng)

[Mở các app: 3'] → [Xem lịch sử: 5'] → [Chép giao dịch: 5']
→ [Phân loại: 5'] ← BOTTLENECK (bước 3–4: 10') → [Cộng tổng, tìm phát sinh: 5']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc một ngày làm việc, tôi muốn biết task nào đã xong, chưa xong và sắp tới, để sáng hôm sau bắt đầu ngay mà không bỏ sót việc |
| Actor | Nhân viên văn phòng |
| Thời điểm / bối cảnh | Cuối mỗi ngày làm việc, 5 lần/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Xem lại email / chat trong ngày → 2. Đối chiếu danh sách task → 3. Đánh dấu xong / chưa xong → 4. Ghi task mới phát sinh → 5. Sắp xếp việc cho ngày mai |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 1: lục lại email/chat tìm việc phát sinh, ~15 phút/ngày |
| Impact (nếu không giải thì sao) | ~33 phút/ngày ≈ 2,75 giờ/tuần; bỏ sót việc ~2 lần/tuần; trễ deadline, bị nhắc lại |
| Success metric (baseline → target) | Thời gian tổng kết: ~33 phút → 15 phút/ngày; số việc bỏ sót: 2 → 0 /tuần. Đo bằng bấm giờ và ghi số việc bị nhắc lại trong 2 tuần |
| Phương án không dùng AI | Ghi task ngay khi nhận; dùng Trello / Notion / Todoist; thói quen review 10 phút cuối ngày |
| Giả thuyết về AI (nếu có) | Tóm tắt email/chat trong ngày thành danh sách việc cần làm |
| Cảm nhận nhanh | No AI hoặc Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~33 phút/ngày (ước lượng)

[Xem email/chat: 15'] ← BOTTLENECK → [Đối chiếu task: 5']
→ [Đánh dấu: 3'] → [Ghi task mới: 5'] → [Sắp việc ngày mai: 5']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Có quy trình nghiệp vụ rõ, lặp lại đều, có bằng chứng thật (khách phản hồi chậm), bottleneck nằm ở bước đọc và nhập liệu
- Câu hỏi muốn nhóm phản biện: Chậm là do bước nhập liệu, hay do hồ sơ thiếu giấy tờ phải quay lại hỏi khách? Với ~10 bộ/tháng cho 1 CRO, impact có đủ lớn không, hay cần nhiều CRO cùng gặp?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card 1: Khách phàn nàn "chậm" là chuyện chờ nhiều ngày, nhưng CRO chỉ mất ~80 phút làm 1 bộ. Có thể chậm thật nằm ở thời gian chờ (hồ sơ nằm hàng đợi, chờ bổ sung giấy tờ, chờ duyệt) chứ không phải ở bước nhập liệu | Có | Thêm metric "thời gian khách chờ từ lúc nhận hồ sơ đến lúc đẩy duyệt", đo baseline trước khi kết luận bottleneck |
| Card 1: ~3/10 bộ bị trả về vì thiếu hoặc sai. Lỗi này checklist và bắt buộc đủ trường (Rule) có thể giải được, đang nhảy sang AI quá sớm | Có | Đổi "Cảm nhận nhanh" từ Workflow sang Rule trước, chỉ lên Workflow nếu sau đó bước đọc giấy tờ vẫn nghẽn |
| Card 1: Khối lượng nhỏ (~10 bộ/tháng ≈ 13 giờ/tháng), tiết kiệm tối đa ~7 giờ/tháng. Có đáng đầu tư công cụ mới không? | Một phần | Giữ card để nhóm phản biện, ghi vào câu hỏi pitch: cần xem nhiều CRO cùng gặp không thì impact mới đủ lớn |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Vai trò nhóm trưởng | Fork và quản lý repo nhóm; review và merge 9 pull request (#1–#9), trong đó 7 PR từ nhánh của Tuấn Anh, Khánh và Thành. | Bài CP1–CP2 của cả 4 thành viên và bảng pitch (`group_report.md` mục 2.1) được gộp vào nhánh `main` của repo nhóm. |
| Pitch Problem Card | Pitch 3 card của mình trong nhóm (dòng 1–3 bảng pitch, `group_report.md` mục 2.1): (1) CRO nhập và đẩy hồ sơ giải ngân online, (2) tổng kết chi tiêu cuối tháng, (3) tổng kết task cuối ngày. Đại diện nhóm lên trình bày pitch card CRO trước lab coach và các nhóm khác. | Card CRO (Card #1) trở thành candidate problem chung và là bài nhóm mang lên trình bày. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt cho nhóm trưởng nhóm 11 (bài AI hỗ trợ người dùng ghi note task): "Note của bạn có đặt sẵn lịch thông báo không?" | Bạn ấy trả lời nhóm chưa tính tới trường hợp này. |
| Nhận phản biện | Câu hỏi tôi nhận được từ lab coach khi lên trình bày pitch card CRO: "Liên kết với VNeID vậy mà AI agent riêng thì xử lý như thế nào?" | Tôi đã sửa gì: làm rõ phương án trên problem: đây là agent nội bộ nhưng có liên kết VNeID, nên dữ liệu hồ sơ phải lấy về từ kho dữ liệu của nhà nước và tạo kho dữ liệu local riêng. |
| Gom cluster / cây OST | Gom 12 candidate thành 4 cluster và dựng cây OST với outcome "giảm thời gian xử lý một bộ hồ sơ giải ngân online". | Cluster và cây OST ở `group_report.md` mục 2.2–2.3; "agent nội bộ liên kết VNeID" bị gạch khỏi tầng opportunity vì đó là giải pháp. |
| Chọn candidate problem | Với tư cách nhóm trưởng, tôi chọn card CRO làm candidate chung để tránh xung đột trong nhóm. Lý do chọn card này: actor rõ (CRO nhập liệu), quy trình 6 bước vẽ được, lặp lại đều (~1 bộ/3 ngày), đã có khách phản hồi vì xử lý chậm. | Toàn bộ nội dung nhóm trình bày (problem, quy trình, bottleneck, metric, phương án) lấy từ card CRO. |
| Kiểm chứng / research | Chưa thực hiện: chưa phỏng vấn, survey hay research. Các con số trong card CRO là ước lượng tôi tự đưa ra, chưa được kiểm chứng. | Chưa có bằng chứng xác nhận hoặc phản bác pain, tần suất và thời lượng; cần phỏng vấn 2–3 người trực tiếp làm hồ sơ giải ngân để có baseline thật. |
| Quy trình nhóm | Cung cấp quy trình nháp 6 bước của Card #1: nhận hồ sơ → kiểm tra giấy tờ → đọc, trích thông tin → nhập hệ thống → đẩy duyệt → sửa nếu bị trả về; bottleneck ước lượng ở bước 3–4 (~45 trong ~80 phút mỗi bộ). | Nhóm dùng quy trình này khi trình bày. |
| Problem Statement | Nội dung lấy từ Card #1: actor là CRO nhập liệu; bottleneck ở bước đọc và nhập thông tin; impact ~10 bộ/tháng, khách phản hồi vì xử lý chậm ~2 lần/tháng, ~3/10 bộ bị trả về; metric thời gian xử lý ~80 → 40 phút/bộ, số bộ bị trả về 3 → 1/tháng, thời gian khách chờ mục tiêu ≤ 1 ngày làm việc (số liệu ước lượng, chưa đo baseline); boundary: AI chỉ hỗ trợ OCR, kiểm tra và phân loại giấy tờ, không tự duyệt hồ sơ, kiểm soát viên duyệt cuối. | Là phần problem nhóm mang lên trình bày. |
| Mức can thiệp AI | Card #1 ban đầu đề xuất Rule trước (checklist giấy tờ + bắt buộc đủ trường khi nhập), chỉ lên Workflow nếu bước đọc giấy tờ vẫn nghẽn. Khi trình bày, nhóm gọi phương án là agent nội bộ có liên kết VNeID. Làm rõ phạm vi: AI chỉ hỗ trợ OCR và kiểm soát giấy tờ giúp CRO khi đẩy hồ sơ lên; hồ sơ cuối cùng vẫn phải qua kiểm soát viên. | Mức phù hợp là **Workflow**: quy trình có các bước cố định, AI chỉ làm bước đọc (OCR), kiểm tra và phân loại giấy tờ, kiểm soát viên vẫn duyệt cuối. Không dừng ở Rule vì Rule không đọc được giấy tờ scan. Mục đích ban đầu: giảm tải cho kiểm soát viên và giúp CRO phân loại giấy tờ. |
| Quyết định | Cùng nhóm chốt **Go** cho phương án Workflow: AI hỗ trợ OCR, kiểm tra và phân loại giấy tờ giúp CRO, kiểm soát viên vẫn duyệt cuối. | Lý do: AI chỉ làm một bước trong quy trình cố định và kiểm soát viên vẫn duyệt cuối, nên khi AI đọc sai vẫn có người chặn lại; mục đích là giảm tải cho kiểm soát viên và giúp CRO phân loại giấy tờ. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Không dùng AI; tự scan 5 problem. | | | |
| CP2 Problem Card | Nhờ AI phản biện Problem Card (kết quả ở bảng "AI đã phản biện card thế nào", mục 3; cả 3 điểm AI chỉ ra đều thuộc Card #1). | Chỉ ra khách phàn nàn "chậm" có thể do thời gian chờ (hồ sơ nằm hàng đợi, chờ bổ sung giấy tờ, chờ duyệt), không chỉ do ~80 phút CRO xử lý; chỉ ra ~3/10 bộ bị trả về vì thiếu/sai có thể xử lý bằng Rule. | AI chỉ tính impact theo khối lượng của 1 CRO (~10 bộ/tháng ≈ 13 giờ/tháng) để hỏi có đáng đầu tư công cụ mới không, chưa xét trường hợp nhiều CRO cùng gặp; tôi chỉ đồng ý một phần. | Thêm metric "thời gian khách chờ" và đo baseline trước khi kết luận bottleneck; đổi Cảm nhận nhanh từ Workflow sang Rule trước; giữ card và đưa câu hỏi "có nhiều CRO cùng gặp không" vào câu hỏi pitch cho nhóm. |
| CP3 Cluster / cây OST | Nhờ AI gợi ý cách gom 12 candidate thành cluster và dựng cây OST từ Card #1. | Tách được giải pháp (agent liên kết VNeID, AI đọc giấy tờ scan) ra khỏi tầng opportunity. | | Tôi thấy đánh giá  của ai là đúng và không có nhận định gì|
| CP4 Research | Không dùng AI. | | | |
| CP5 Quy trình | Không dùng AI. | | |  |
| CP5–6 Problem Statement | Không dùng AI. | | | |
| CP6 Mức can thiệp / quyết định | Không dùng AI. | | | |
| CP7 Báo cáo cá nhân | Dùng Claude Code để tổng hợp bằng chứng có trong repo (commit, PR, bảng pitch, bảng phản biện AI) vào mục 4–5, ghi lại các câu phản biện tôi cung cấp, điền phần của tôi trong `TEAM.md` và gợi ý câu hỏi tự soi cho mục 6. | Gom nhanh bằng chứng có thật trong repo; chỉ ra những ô bắt buộc phải tự làm. | AI không biết những gì diễn ra trên lớp (ai hỏi gì, kết quả CP4–CP6), nên không tự điền được các ô đó. | Tự cung cấp câu hỏi phản biện thật, tự điền các ô về kết quả nhóm và tự viết mục 6 (AI chỉ gợi ý câu hỏi tự soi). |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Em thấy phần lớn problem của các bạn xoay quanh việc học và làm nhóm, hay gặp nhất là thông tin nằm rải rác ở chat, LMS, email. Khi em hỏi nhóm 11 note có đặt sẵn lịch thông báo không thì nhóm bạn chưa tính tới, nên em học được là phải nghĩ hết các tình huống dùng thật của người dùng.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có. Lúc dựng cây OST, nhóm em để "agent nội bộ liên kết VNeID" ở tầng opportunity dù đó là giải pháp. Khi nhận ra, nhóm gạch ý này đi và quay lại outcome là giảm thời gian xử lý một bộ hồ sơ giải ngân online.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Khi lab coach hỏi "Liên kết với VNeID vậy mà AI agent riêng thì xử lý như thế nào?", em làm rõ dữ liệu hồ sơ phải lấy từ kho dữ liệu của nhà nước và lưu ở kho local riêng, đồng thời thu hẹp vai trò AI xuống chỉ hỗ trợ OCR, kiểm tra và phân loại giấy tờ, kiểm soát viên vẫn duyệt cuối.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Nhóm em chưa kiểm chứng: chưa phỏng vấn, survey hay research, nên chưa có kết quả nào để bất ngờ. Các con số trong card CRO vẫn là ước lượng của em, cần hỏi 2–3 người trực tiếp làm hồ sơ giải ngân để có baseline thật.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là viết bottleneck và metric khi chưa có số đo thật. Card ghi nghẽn ở bước đọc và nhập (~45 trong ~80 phút/bộ), nhưng việc khách phản hồi chậm có thể do hồ sơ nằm chờ chứ không chỉ do nhập liệu, nên em phải thêm metric thời gian khách chờ và ghi rõ các số là ước lượng.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Em sẽ hỏi người làm hồ sơ thật trước để thay các con số ước lượng, và chuẩn bị sẵn câu trả lời về nguồn dữ liệu VNeID trước khi lên trình bày. Là nhóm trưởng, em lẽ ra nên hỏi lại khi nhóm chốt Workflow, vì card ban đầu ghi thử Rule (checklist) trước, chỉ lên Workflow nếu bước đọc giấy tờ vẫn nghẽn.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán nhóm em chọn là CRO nhập liệu phải kiểm tra, đọc và nhập hồ sơ giải ngân online lên hệ thống, nhưng xử lý chậm khiến khách phản hồi khoảng 2 lần/tháng và khoảng 3/10 bộ bị trả về vì thiếu hoặc sai. Quy trình gồm nhận hồ sơ, kiểm tra giấy tờ, đọc và trích thông tin, nhập hệ thống, đẩy duyệt và sửa nếu bị trả về, tổng khoảng 80 phút/bộ, trong đó bottleneck là bước đọc và nhập (khoảng 45 phút). Metric là giảm thời gian xử lý từ ~80 xuống 40 phút/bộ, số bộ bị trả về từ 3 xuống 1/tháng và thời gian khách chờ không quá 1 ngày làm việc, đo bằng cách ghi giờ nhận, bắt đầu và đẩy duyệt từng bộ trong 1 tháng; các số hiện vẫn là ước lượng. Boundary là AI chỉ hỗ trợ OCR, kiểm tra và phân loại giấy tờ, không tự duyệt hồ sơ; CRO kiểm tra lại các trường AI điền và kiểm soát viên duyệt cuối. Mức can thiệp là Workflow vì quy trình có các bước cố định và AI chỉ làm một bước trong đó, còn Rule (checklist) thì không đọc được giấy tờ scan. Nhóm chốt Go cho Workflow vì nếu AI đọc sai thì vẫn có người chặn lại trước khi hồ sơ được duyệt.

---

## 7. Tài liệu tham khảo

- [docs/01-worksheet.md](../../docs/01-worksheet.md): mẫu Job Story, Problem Card và prompt phản biện (CP1–CP2).
- [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md): bài làm mẫu (CP0).
- [RULES.md](../../RULES.md), [RUBRIC.md](../../RUBRIC.md): quy định dùng AI và tiêu chí chấm.
- [report/team/group_report.md](../team/group_report.md): bảng pitch của nhóm (mục 2.1).
