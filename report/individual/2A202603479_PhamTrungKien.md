# Báo cáo cá nhân — 2A202603479_PhamTrungKien

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Phạm Trung Kiên
- MSSV: 2A202603479
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Ban3
- Link repo nhóm: https://github.com/LysLama/K5-L3A-DAY02-Ban3-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

Mình quét lại các pain từng ghi ở bài Day02 cũ (Vinpearl / VinFast / Xanh SM / Vinhomes / Vinmec), rồi bổ sung actor khác trong cùng chuỗi — mỗi dòng một việc, không tách một quy trình thành 3 bài.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi inbox đầy review 1–3 sao từ Booking, Agoda và Google cùng lúc, tôi muốn soạn xong từng phản hồi đúng giọng khách sạn trước khi hết ca, để không vỡ hạn 24 giờ | CSKH property Vinpearl (người gõ thư) | Một review thường mất khoảng 12–15 phút. Cuối tuần mình ước ~35–40 review/người/ca. Có hôm hai ca viết khác giọng hẳn dù cùng một SOP |
| 2 | Lặp lại | Khi khách đứng cạnh hỏi “xe này + pin này hết bao nhiêu sau ưu đãi”, tôi muốn lấy đúng giá khu vực và chương trình tháng đang chạy, để gửi Zalo luôn mà không phải cộng Excel lại từ đầu | Tư vấn showroom VinFast | Khoảng 15–20 phút/khách. Ngày đông làm cả chục bảng. Tháng đổi ưu đãi là hay lệch vài dòng so với bảng giá in |
| 3 | Lặp lại | Khi đóng ca, tôi muốn gắn một nguyên nhân gốc cho từng chuyến hủy (tài xế muộn / khách hủy / app lỗi), để sáng hôm sau khỏi đọc lại đống ghi chú khi làm báo cáo tuần | Nhân viên chất lượng Xanh SM | Mỗi ca cả trăm note ngắn của khách và tài xế. Gắn tay khoảng 1–2 phút/note. Để dồn cuối tuần thì ngồi cả tiếng đồng hồ |
| 4 | Tốn thời gian | Khi giờ cao điểm sảnh đông, tôi muốn biết căn hộ có cho khách vào không trước khi mở cửa, để hàng không dài và mình khỏi gọi đi gọi lại | Bảo vệ / lễ tân tòa Vinhomes | Mỗi lượt hay mất 10–15 phút vì phải gọi cư dân. Buổi tối sau 18h hàng dài rõ; khách gắt vì đứng chờ |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi bệnh nhân sắp vào phòng, tôi muốn gom tiền sử, dị ứng và thuốc đang dùng từ vài lần khám cũ thành một trang, để bác sĩ không hỏi lại từ đầu | Điều dưỡng tiền khám Vinmec | Lướt EMR + ghi tay khoảng 8–10 phút/ca. Hồ sơ dài thì dễ sót dòng dị ứng |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận ca sáng, tôi muốn biết ca đêm còn bao nhiêu review chưa trả và cái nào gần vỡ SLA, để phân việc trước khi mở từng ticket | Trưởng ca / Guest Experience property | Handover hay chỉ là tin nhắn rời. Mình từng thấy mở lại 3 tab OTA mất gần 20 phút chỉ để đếm việc tồn |
| 7 | Pain từ người khác | Khi bị trừ điểm chuyến hủy mà mình không muộn, tôi muốn lý do trên hệ thống khớp việc thật, để khỏi phải khiếu nại nội bộ mất cả buổi | Tài xế Xanh SM | Tài xế hay nhắn group chất lượng nhờ xem lại nhãn. Một case làm rõ thường 30–45 phút (đối chiếu GPS + note) |
| 8 | Pain từ người khác | Khi đang họp mà lễ tân gọi “có khách bên dưới”, tôi muốn xác nhận cho vào trong một thao tác ngắn, để khỏi ngắt họp và khách khỏi đứng sảnh | Cư dân Vinhomes; khách thăm; lễ tân | Cư dân bị gọi 1–2 lần/lượt khách. Giờ cao điểm có người tắt máy → lễ tân gọi lại → khách chờ thêm |
| 9 | Pain từ người khác | Khi vừa gọi tên bệnh nhân, tôi muốn nhìn một bản tóm tắt dị ứng/thuốc trước mặt, để khỏi lật EMR giữa buổi và khỏi hỏi lại người nhà những câu đã hỏi ở quầy | Bác sĩ khám ngoại trú Vinmec | Mất khoảng 8–10 phút đầu ca nếu tờ tóm tắt chưa có. Người nhà phàn nàn bị hỏi trùng |
| 10 | Lặp lại | Khi hết ngày, tôi muốn đối chiếu các báo giá đã gửi khách với bảng giá chính thức trong ngày, để bắt lệch ưu đãi trước khi khách chốt cọc | Trưởng showroom / salesteam lead VinFast | Cuối ngày soi 10–20 file PDF/sheet. Lệch một dòng phụ kiện là phải gọi lại khách; ước 30–40 phút/ngày |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Năm ý gốc (Vinpearl review, VinFast báo giá, Xanh SM gắn nhãn, Vinhomes khách thăm, Vinmec tóm tắt EMR) mình giữ vì đã đào ở bài trước, có số phút.
- AI gợi ý tách review Vinpearl thành “đọc”, “tra SOP”, “soạn thư” — mình **bỏ**, trùng một quy trình.
- AI gợi ý “chatbot tự trả lời OTA” — **bỏ**, đó là giải pháp; bài trước từng bị AI dụ tự đăng / tự hoàn tiền.
- **Giữ** thêm #6–#10 vì đổi actor thật (trưởng ca, tài xế, cư dân, bác sĩ, trưởng showroom), không phải viết lại cùng một pain.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Phản hồi đánh giá OTA Vinpearl (#1) | Có số phút thật từ bài trước; quy trình 5 bước rõ; so được No AI / Rule / Workflow | Property có chịu dùng bản nháp máy soạn không? Giọng “đủ Vinpearl” đo sao? |
| 2 | Gắn nhãn hủy chuyến Xanh SM (#3) | Lặp mỗi ca; nối được pain tài xế (#7); metric đếm được | Taxonomy đã chuẩn chưa? Note ngắn có gắn đúng được không? |
| 3 | Tóm tắt tiền sử Vinmec (#5, nối #9) | Có phút đo; bác sĩ/người nhà cùng đau; quy trình ngắn | EMR có cho lab đụng không; “không sót dị ứng” khó chứng trong buổi |

### Problem Card #1 — Phản hồi đánh giá OTA (Vinpearl)

| Trường | Nội dung |
|---|---|
| Job Story | Khi inbox đầy review một đến ba sao trên Booking, Agoda và Google, tôi muốn hiểu khách đang phàn nàn gì rồi viết thư trả lời đúng giọng khách sạn, để kịp hạn hai mươi bốn giờ và các ca không viết mỗi người một kiểu |
| Actor | Nhân viên CSKH ở property Vinpearl, kèm quản lý Guest Experience duyệt trước khi đăng |
| Thời điểm / bối cảnh | Trong ca trực, nặng nhất cuối tuần và mùa cao điểm, vì review đổ về cả ba kênh cùng lúc |
| Quy trình hiện tại (3–7 bước) | Lấy review mới vào inbox. Đọc rồi phân loại khiếu nại. Tra SOP, voucher và hạn mức xin lỗi. Soạn thư tiếng Việt hoặc tiếng Anh rồi nhờ quản lý duyệt. Đăng lên OTA và ghi log nội bộ. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Chỗ nặng nhất là bước soạn thư, thường khoảng năm phút, vì dễ lệch giọng giữa các ca và lúc viết gấp hay hứa ngoài SOP. Đọc phân loại với tra SOP cũng mỗi bước khoảng bốn phút, cộng lại đoạn giữa khá mệt. |
| Impact (nếu không giải thì sao) | Cuối tuần một người có thể cầm khoảng ba mươi lăm đến bốn mươi review một ca, dễ mất cả buổi chỉ để trả lời. Property đông khách thì cả tuần vài chục giờ CSKH. Trễ hạn hai mươi bốn giờ thì điểm review và hạng OTA tụt. |
| Success metric (baseline → target) | Hiện khoảng mười lăm phút một review, muốn xuống dưới ba phút. Ít nhất chín mươi lăm phần trăm review được trả lời trong hai mươi bốn giờ. Mọi thư gửi đi vẫn phải có người duyệt, không tự đăng. |
| Phương án không dùng AI | Có sẵn mẫu xin lỗi theo chủ đề, checklist SOP, gom inbox ba kênh. Cách này đỡ loạn format nhưng vẫn mất thời gian đọc review cảm xúc và chọn đúng chính sách. |
| Giả thuyết về AI | Máy gợi ý chủ đề và mức nghiêm trọng rồi viết bản nháp đúng giọng. Phần SOP và voucher vẫn theo rule có sẵn. CSKH sửa và bấm duyệt rồi mới đăng. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
Hiện tại: khoảng 12 đến 15 phút một review
Cuối tuần ước 35 đến 40 review mỗi người mỗi ca

1. Lấy review từ OTA vào inbox (khoảng 1 phút)
2. Đọc và phân loại khiếu nại (khoảng 4 phút) — chỗ nghẽn vì nhiều ý, viết cảm xúc
3. Tra SOP, voucher, hạn mức xin lỗi (khoảng 4 phút) — SOP nằm rải nhiều file
4. Soạn thư tiếng Việt hoặc Anh rồi xin duyệt (khoảng 5 phút) — BOTTLENECK, dễ lệch giọng
5. Đăng lên OTA và ghi log (khoảng 1 phút)
```

### Problem Card #2 — Gắn nhãn nguyên nhân hủy chuyến (Xanh SM)

| Trường | Nội dung |
|---|---|
| Job Story | Khi hết ca, tôi muốn gắn đúng lý do gốc cho từng chuyến hủy (tài xế muộn, khách đổi ý, lỗi app), để làm báo cáo tuần khỏi phải đọc lại cả đống ghi chú từ đầu |
| Actor | Nhân viên chất lượng Xanh SM; quản lý vận hành là người đọc báo cáo tuần |
| Thời điểm / bối cảnh | Cuối mỗi ca, rồi dồn sang cuối tuần khi tổng hợp chất lượng |
| Quy trình hiện tại (3–7 bước) | Xuất danh sách chuyến hủy trong ca. Mở từng ghi chú của khách và tài xế. Đọc rồi gắn nhãn nguyên nhân theo danh mục. Ghi vào sheet tổng hợp. Cuối tuần cộng theo nhãn rồi viết báo cáo. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Nặng ở đoạn đọc ghi chú rồi gắn nhãn, thường một đến hai phút mỗi note. Một ca cả trăm note thì chỉ việc gắn nhãn cũng mất hai đến ba giờ. |
| Impact (nếu không giải thì sao) | Báo cáo tuần chậm hoặc gắn sai lý do. Quản lý không biết nên ưu tiên sửa tài xế, app hay quy trình đón. Để dồn cuối tuần thì phải ngồi đọc lại note thô. |
| Success metric (baseline → target) | Hiện gắn tay khoảng hai phút một ghi chú, muốn người chỉ còn duyệt dưới hai mươi giây. Trên mẫu kiểm, nhãn đúng từ chín mươi phần trăm trở lên. Báo cáo tuần ra đúng hạn, không phải đọc lại thô. |
| Phương án không dùng AI | Danh mục nguyên nhân cố định, bắt chọn dropdown khi đóng ticket hủy, báo cáo lấy từ sheet. Đỡ phải nghĩ nhãn, nhưng note dài hoặc mơ hồ vẫn đọc mệt. |
| Giả thuyết về AI | Máy đề xuất một hai nhãn từ nội dung ghi chú. Người chất lượng xác nhận. Rule chặn nhãn ngoài danh mục. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
Hiện tại: khoảng 1 đến 2 phút một ghi chú, mỗi ca cả trăm ghi chú

1. Xuất danh sách chuyến hủy (khoảng 5 phút mỗi ca)
2. Mở và đọc ghi chú khách hoặc tài xế (khoảng 1 phút mỗi ghi chú) — chỗ nghẽn
3. Gắn nhãn nguyên nhân gốc (khoảng 1 phút mỗi ghi chú) — BOTTLENECK
4. Ghi vào sheet tổng hợp (khoảng 15 giây mỗi ghi chú)
5. Cuối tuần cộng số và viết báo cáo (khoảng 45 đến 60 phút)
```

### Problem Card #3 — Tóm tắt tiền sử trước khám (Vinmec)

| Trường | Nội dung |
|---|---|
| Job Story | Khi bệnh nhân sắp vào phòng khám, tôi muốn có sẵn tiền sử, dị ứng và thuốc đang dùng lấy từ các lần khám cũ, để bác sĩ khỏi mất tám đến mười phút đầu buổi vì hồ sơ chưa sẵn |
| Actor | Điều dưỡng tiền khám và bác sĩ khám ngoại trú ở Vinmec |
| Thời điểm / bối cảnh | Ngay trước giờ bác sĩ gọi tên, với bệnh nhân đã khám nhiều lần trên EMR |
| Quy trình hiện tại (3–7 bước) | Mở EMR và lướt các lần khám cũ. Ghi tay tiền sử, dị ứng, thuốc đang dùng. Hỏi lại bệnh nhân cho đủ. Đưa tờ tóm tắt cho bác sĩ trước giờ khám. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Nặng ở đoạn lướt EMR rồi ghi tay, cả thảy khoảng tám đến mười phút một ca. Làm gấp thì dễ sót dòng dị ứng. |
| Impact (nếu không giải thì sao) | Bác sĩ mất gần mười phút đầu ca. Sót dị ứng thì rủi ro cao. Giờ đông thì hàng chờ dài thêm, người nhà cũng bị hỏi trùng. |
| Success metric (baseline → target) | Hiện chuẩn bị hồ sơ khoảng mười phút, muốn xuống dưới hai phút. Trên bộ case kiểm không bỏ sót dị ứng hoặc thuốc đang dùng. Máy không được tự kê đơn hay chẩn đoán. |
| Phương án không dùng AI | Checklist tiền khám cố định và một trang mẫu trong EMR. Đỡ sót trường, nhưng vẫn mất thời gian đọc nhiều lần khám dài. |
| Giả thuyết về AI | Máy đọc EMR rồi viết bản tóm tắt có mục rõ. Điều dưỡng duyệt trước khi đưa bác sĩ. Case lạ thì chuyển lên xử lý tay. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
Hiện tại: khoảng 8 đến 10 phút mỗi ca trước giờ khám

1. Lướt EMR nhiều lần khám cũ (khoảng 5 phút) — BOTTLENECK
2. Ghi tay tiền sử, dị ứng, thuốc (khoảng 3 phút) — chỗ nghẽn, dễ sót
3. Hỏi lại bệnh nhân cho đủ (khoảng 1 đến 2 phút)
4. Đưa tờ tóm tắt cho bác sĩ (khoảng 1 phút)
```

### Card muốn pitch nhất

- Card số: 1 (phản hồi đánh giá OTA Vinpearl)
- Vì sao: Mình đã đào sâu bài này ở Day02 trước, có số phút và năm bước rõ. Gắn được hạn trả lời hai mươi bốn giờ và hạng OTA. Dễ nói với nhóm là vẫn cần người duyệt, không tự đăng. Cũng vừa để so bốn mức can thiệp trong lab.
- Câu hỏi muốn nhóm phản biện: Nếu chỉ dùng mẫu SOP theo chủ đề, không dùng AI, liệu có kéo từ khoảng mười lăm phút xuống dưới năm phút không? Phần nào vẫn bắt buộc phải đọc hiểu review?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Mốc mười lăm phút có thể chỉ nhớ miệng, chưa bấm giờ từng bước | Đồng ý một phần | Giữ khoảng mười hai đến mười lăm phút như bài trước, nhưng tách phút từng bước và ghi là ước lượng, CP4 sẽ hỏi lại người thật |
| Đang nói nghẽn ở cả bước 2, 3 và 4, chưa chốt một bước chính | Đồng ý | Chốt nghẽn chính là bước soạn thư khoảng năm phút; đọc và tra SOP là nghẽn phụ |
| Gợi ý cho máy tự đăng OTA hoặc tự gửi voucher | Không đồng ý | Giữ ranh giới: chỉ soạn nháp, CSKH duyệt; không tự đăng, không hứa bồi thường ngoài SOP |
| Metric mới đo tốc độ, chưa nói chất lượng giọng và đúng SOP | Đồng ý | Thêm điều kiện mọi bản gửi đều có người duyệt; sau này ở Problem Statement sẽ ghi rõ không được hứa ngoài SOP |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
| -------------------------- | -------------- | -------------------------------- |
| Pitch Problem Card         |                |                                  |
| Phản biện bài của bạn khác |                |                                  |
| Nhận phản biện             |                |                                  |
| Gom cluster / cây OST      |                |                                  |
| Chọn candidate problem     |                |                                  |
| Kiểm chứng / research      |                |                                  |
| Quy trình nhóm             |                |                                  |
| Problem Statement          |                |                                  |
| Mức can thiệp AI           |                |                                  |
| Quyết định                 |                |                                  |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ gợi ý thêm actor quanh 5 pain Vingroup cũ | Gợi ý được trưởng ca, tài xế, cư dân, trưởng showroom — đỡ trùng một quy trình | Hay tách Vinpearl thành 3 dòng; đẩy giải pháp kiểu tự trả lời OTA | Gộp lại 1 dòng/quy trình; bỏ solution; chỉ giữ ý có người thật chịu pain |
| CP2 Problem Card | Nhờ đóng vai PM hoài nghi phản biện card #1 (Vinpearl) | Chỉ ra bottleneck đang ôm 3 bước và metric thiếu chất lượng | Gợi ý tự đăng OTA / tự gửi voucher | Chốt bottleneck chính = bước 4 (~5'); tách phút từng bước; giữ HITL, cấm tự đăng |
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
