# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Nguyễn Đình Quang  
- MSSV:2A202603620
- Email trường (không bắt buộc, repo có thể để public):26ai.quangnd@vinuni.edu.vn
- Tên nhóm:PhuongHoang
- Link repo nhóm:https://github.com/VinUni-AI20k/K5-L3-Day02-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi bắt đầu mỗi tiết học, tôi muốn biết nhanh ai có mặt mà không phải gọi tên từng em, để dành thời gian cho bài giảng | Giáo viên, trợ giảng | Bấm giờ điểm danh 5 tiết liên tiếp; đếm số tiết/ngày; số phút/tuần cộng dồn |
| 2 | Lặp lại | Khi mỗi tiết đổi giáo viên, tôi muốn biết em nào vắng từ tiết trước, để không phải hỏi lại cả lớp | Giáo viên bộ môn, học sinh | Đếm số lần phải hỏi lại trong 1 ngày học; số phút mỗi lần |
| 3 | Tốn thời gian | Khi có em vào lớp muộn, tôi muốn ghi nhận đúng giờ mà không ngắt bài giảng, để không ghi nhầm thành vắng | Giáo viên, học sinh đến muộn | Số em muộn/tiết; số lần bị ngắt bài/tiết; số ca ghi vắng sai thực ra là muộn trong học kỳ |
| 4 | Tốn thời gian | Khi cuối tuần hoặc cuối kỳ, tôi muốn có số liệu chuyên cần của cả lớp, để không phải nhập lại từ sổ giấy vào Excel | Giáo viên, giáo vụ | Bấm giờ một lần nhập và tổng hợp; số lớp/số sổ phải xử lý; số lỗi nhập phát hiện được |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi có em vắng nhiều bất thường, tôi muốn nhận ra sớm từ dữ liệu chuyên cần, để kịp hỏi thăm trước khi quá muộn | Giáo viên chủ nhiệm, học sinh | Hỏi giáo viên: lần gần nhất phát hiện em bỏ học dần là khi nào, bằng cách nào, sớm hay muộn mấy tuần |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi có khiếu nại "em có đi mà", tôi muốn kiểm chứng nhanh bằng dữ liệu, để không phải tranh cãi dựa vào trí nhớ | Giáo viên, giáo vụ, học sinh | Số khiếu nại/học kỳ; mất bao lâu để giải quyết một ca; cần đối chiếu mấy nguồn (sổ, Excel, tin nhắn) |
| 7 | Pain từ người khác | Khi bị ghi vắng dù có đi học, tôi muốn được xác nhận lại nhanh, để không bị trừ điểm oan | Học sinh | Hỏi 3-5 em: lần gần nhất bị ghi sai là khi nào, chuyện gì xảy ra sau đó, mất mấy ngày để sửa |
| 8 | Pain từ người khác | Khi con vắng mặt ở trường, tôi muốn biết sớm, để không phải lo hoặc chờ đến cuối ngày mới biết | Phụ huynh, giáo viên chủ nhiệm | Hỏi 3-5 phụ huynh: lần gần nhất biết con vắng muộn, họ đã làm gì; đo thời gian từ lúc vắng đến lúc phụ huynh biết |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Điểm danh đầu tiết, kể cả ghi nhận em đến muộn  | Việc lặp mỗi tiết, bấm giờ được ngay. Có nhiều phía để phỏng vấn (giáo viên, trợ giảng, học sinh). Đây là chỗ để so camera với gọi tên theo sơ đồ chỗ ngồi, QR, thẻ quẹt. | Đau nhất ở mất thời gian, ký hộ hay ghi nhầm người đến muộn thành vắng? Nếu chỉ là mất thời gian thì QR hoặc sơ đồ chỗ ngồi đã đủ. Camera cần đồng ý của phụ huynh và nhà trường vì dữ liệu khuôn mặt học sinh là dữ liệu nhạy cảm. |
| 2 | Phụ huynh biết con vắng quá muộn | Đo được độ trễ từ lúc vắng đến lúc phụ huynh biết. Có 3 phía để phỏng vấn (giáo viên chủ nhiệm, văn phòng, phụ huynh). | Chậm ở khâu nhận diện ai vắng hay ở khâu nhắn tin? Nếu là khâu nhắn tin thì camera không giải quyết được. Phụ huynh có thật sự muốn được báo ngay không? |
| 3 | Khiếu nại ghi vắng sai "em có đi mà"  | Có hậu quả cụ thể (bị trừ điểm oan), có hai phía (học sinh và giáo viên/giáo vụ). | Số khiếu nại có đủ nhiều để đáng giải không? Nguyên nhân chính là ký hộ, đến muộn hay nhập sai? Dữ liệu cũ có còn để đối chiếu không? |

### Problem Card #1 (bổ sung quy trình nháp)

Quy trình nháp hiện tại:

```text
[Bắt đầu tiết]
   -> Gọi tên / chuyền danh sách
   -> Học sinh đáp "có" / ký
   -> Em đến muộn vào sau: giáo viên ghi chú tay (hoặc quên)
   -> Nghi ngờ ký hộ? -> Có: đối chiếu thủ công
   -> Nhập lại vào Excel / hệ thống trường
   -> Cuối kỳ tổng hợp chuyên cần, xử lý khiếu nại
Bottleneck giả định: bước "gọi tên / ký" (mất ___ phút/tiết) và bước "em đến muộn" (ghi nhầm thành vắng)
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi con vắng mặt ở trường, tôi muốn biết sớm, để không phải lo hoặc chờ đến cuối ngày mới biết |
| Actor | Phụ huynh (người cần biết); giáo viên chủ nhiệm (người báo); văn phòng/giám thị (người tổng hợp) |
| Thời điểm / bối cảnh | Đầu buổi sáng và đầu mỗi tiết, ngay sau khi giáo viên phát hiện em vắng; trường hợp em đi học nhưng không vào lớp |
| Quy trình hiện tại (3–7 bước) | 1. Giáo viên điểm danh, phát hiện em vắng · 2. Ghi vào sổ đầu bài · 3. Cuối buổi văn phòng thu sổ, tổng hợp danh sách vắng · 4. Giáo viên chủ nhiệm nhắn hoặc gọi phụ huynh · 5. Phụ huynh phản hồi lý do (hoặc không phản hồi) · 6. Ghi nhận có phép / không phép |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả định, cần xác minh: khoảng chờ giữa bước 1 và bước 4 (từ lúc phát hiện vắng đến lúc phụ huynh biết) mất ___ phút/giờ. Chưa biết chậm ở khâu thu sổ hay khâu nhắn tin. |
| Impact (nếu không giải thì sao) | [Bạn tự đo]: ___ giờ trung bình từ lúc vắng đến lúc phụ huynh biết; ___ trường hợp phụ huynh không biết con vắng trong ngày/tháng; ___ giáo viên chủ nhiệm mất bao nhiêu phút/ngày để nhắn. Nếu không giải: phụ huynh lo lắng, em trốn học khó phát hiện sớm, giáo viên mất thời gian nhắn thủ công. |
| Success metric (baseline → target) | Thời gian từ lúc phát hiện vắng đến lúc phụ huynh biết từ ___ → dưới ___ phút; số phụ huynh không biết con vắng trong ngày giảm; không tăng số tin nhắn gây phiền cho phụ huynh |
| Phương án không dùng AI | Giáo viên nhắn phụ huynh ngay sau điểm danh qua nhóm Zalo/app liên lạc của trường; mẫu tin nhắn có sẵn; tin nhắn tự động từ phần mềm quản lý của trường khi giáo viên đánh dấu vắng |
| Giả thuyết về AI (nếu có) | Gần như không cần AI: khâu thông báo là Rule (đánh dấu vắng -> gửi tin theo mẫu). AI chỉ xét nếu cần soạn tin theo từng hoàn cảnh hoặc phân loại lý do phụ huynh trả lời. Boundary: AI không tự gửi tin khi giáo viên chưa xác nhận em vắng thật. |
| Cảm nhận nhanh | Rule (nghiêng về No AI). Camera không giải quyết được nếu nút thắt nằm ở khâu nhắn tin. |

Quy trình nháp hiện tại:

```text
[Giáo viên điểm danh] -> phát hiện em vắng
   -> Ghi vào sổ đầu bài
   -> Cuối buổi: văn phòng thu sổ, tổng hợp danh sách vắng
   -> Giáo viên chủ nhiệm nhắn / gọi phụ huynh
   -> Phụ huynh phản hồi lý do (hoặc im lặng)
   -> Ghi nhận có phép / không phép
Bottleneck giả định: khoảng chờ từ "phát hiện vắng" đến "phụ huynh biết" (___ phút/giờ)
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi bị ghi vắng dù có đi học, tôi muốn được xác nhận lại nhanh bằng dữ liệu đáng tin, để không bị trừ điểm oan và giáo viên không phải tranh cãi dựa vào trí nhớ |
| Actor | Học sinh (người bị ảnh hưởng); giáo viên, giáo vụ (người xử lý khiếu nại) |
| Thời điểm / bối cảnh | Khi công bố chuyên cần giữa kỳ hoặc cuối kỳ; khi học sinh phát hiện mình bị ghi vắng |
| Quy trình hiện tại (3–7 bước) | 1. Học sinh thấy bị ghi vắng · 2. Báo giáo viên ("em có đi mà") · 3. Giáo viên nhớ lại, lục sổ hoặc hỏi bạn cùng lớp · 4. Đối chiếu nhiều nguồn (sổ, Excel, tin nhắn) · 5. Quyết định sửa hoặc giữ nguyên · 6. Cập nhật lại hệ thống, thông báo học sinh |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả định, cần xác minh: bước 3-4 (tìm lại bằng chứng) mất ___ phút/ca, và nhiều ca không có bằng chứng để kết luận. Chưa biết nguyên nhân chính là ký hộ, đến muộn hay nhập sai. |
| Impact (nếu không giải thì sao) | [Bạn tự đo]: ___ khiếu nại/học kỳ; ___ ngày để giải quyết một ca; ___ % ca không có bằng chứng để kết luận. Nếu không giải: học sinh bị trừ điểm oan, mất niềm tin vào số liệu, giáo viên tốn thời gian tranh luận. |
| Success metric (baseline → target) | Thời gian giải quyết một khiếu nại từ ___ → dưới ___ phút; tỷ lệ ca có bằng chứng đối chiếu tăng từ ___ → ___; số khiếu nại do ghi sai giảm |
| Phương án không dùng AI | Lưu điểm danh dạng số có dấu thời gian (Google Sheet, QR có khung giờ); chốt và công bố chuyên cần hằng tuần để học sinh kiểm tra sớm; quy trình khiếu nại có mẫu và hạn xử lý rõ |
| Giả thuyết về AI (nếu có) | Có thể không cần AI: gốc rễ là dữ liệu điểm danh không có dấu vết. AI chỉ xét ở việc gắn cờ bất thường (vắng lẻ tẻ, mẫu ký hộ) để giáo viên xem lại. Boundary: AI không tự quyết ai đúng ai sai; không dùng làm bằng chứng duy nhất. |
| Cảm nhận nhanh | No AI / Rule (chuẩn hóa cách ghi nhận và lưu vết). Chưa biết nếu cần AI phát hiện bất thường. |

Quy trình nháp hiện tại:

```text
[Học sinh thấy bị ghi vắng]
   -> Báo giáo viên "em có đi mà"
   -> Giáo viên nhớ lại / lục sổ / hỏi bạn cùng lớp
   -> Đối chiếu nhiều nguồn (sổ, Excel, tin nhắn)
   -> Quyết định sửa hoặc giữ nguyên
   -> Cập nhật hệ thống, thông báo học sinh
Bottleneck giả định: bước "tìm lại bằng chứng" (___ phút/ca, nhiều ca không có bằng chứng)
```

### Card muốn pitch nhất

- Card số: 1 (Điểm danh đầu tiết, kể cả em đến muộn)
- Vì sao: Đo được ngay bằng bấm giờ, có nhiều phía để phỏng vấn, và là chỗ rõ nhất để so sánh camera với QR, sơ đồ chỗ ngồi, thẻ quẹt. Dù kết luận là No AI/Rule, lập luận so sánh vẫn chặt.
- Câu hỏi muốn nhóm phản biện: Nếu QR có khung giờ đã đủ cho phần lớn lớp học, thì có tình huống nào (lớp đông, học sinh nhỏ tuổi chưa có điện thoại, trốn tiết giữa giờ) khiến camera đếm số người thật sự đáng đầu tư? Hay chúng ta đang chọn camera vì nó hấp dẫn chứ không vì bằng chứng?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa có số liệu thực tế về thời gian điểm danh mỗi tiết, số lần học sinh đến muộn và tần suất ghi nhận sai. | Đồng ý | Không tự đặt số liệu mà bổ sung các chỉ số cần đo như thời gian điểm danh, số học sinh đến muộn và số trường hợp ghi nhầm vắng thành muộn để kiểm chứng thực tế. |
| Chưa xác định rõ nguyên nhân chính gây mất thời gian là gọi tên, ký điểm danh hay xử lý học sinh đến muộn. | Đồng ý | Quay lại phân tích quy trình As-Is, xác định các bước gây gián đoạn và đưa việc bấm giờ từng công đoạn vào kế hoạch kiểm chứng để tìm đúng bottleneck. |
| Chưa có đủ bằng chứng cho thấy camera nhận diện là phương án tốt hơn QR, sơ đồ chỗ ngồi hoặc thẻ quẹt. | Đồng ý | Bổ sung việc so sánh các phương án dựa trên thời gian thực hiện, độ chính xác và tình huống sử dụng thực tế. Không mặc định camera là giải pháp tốt nhất khi chưa có dữ liệu chứng minh. |
| Chưa làm rõ các trường hợp học sinh đến muộn, ký hộ hoặc ghi nhầm người đến muộn thành vắng có ảnh hưởng như thế nào đến quy trình. | Đồng ý | Bổ sung các tình huống này vào nội dung phỏng vấn giáo viên, trợ giảng và học sinh để xác định vấn đề xảy ra thường xuyên ở đâu và gây ảnh hưởng như thế nào. |
| Camera có thể phát sinh rủi ro về quyền riêng tư và dữ liệu khuôn mặt học sinh, đồng thời chưa chắc cần thiết nếu QR hoặc phương án đơn giản đã đáp ứng nhu cầu. | Đồng ý | Đưa yêu cầu đồng ý của phụ huynh và nhà trường vào điều kiện xem xét camera. Đồng thời, giữ QR, sơ đồ chỗ ngồi và thẻ quẹt làm các phương án cần so sánh trước khi quyết định. |
| Chưa có baseline để xác định mục tiêu giảm thời gian điểm danh và cải thiện độ chính xác có khả thi hay không. | Đồng ý | Chưa chốt mục tiêu bằng các con số tự giả định. Nhóm sẽ đo thời gian điểm danh và số trường hợp ghi nhận sai trước, sau đó mới xác định target và tiêu chí đánh giá phù hợp. |

**Kết luận sau phản biện:** Nhóm nhận thấy cần kiểm chứng nguyên nhân gây mất thời gian trước khi lựa chọn công nghệ. Problem Card #1 vẫn được giữ lại vì có thể đo thời gian trực tiếp và phỏng vấn nhiều đối tượng liên quan. Tuy nhiên, camera chưa được xác định là giải pháp cuối cùng. Nhóm sẽ so sánh camera với QR, sơ đồ chỗ ngồi và thẻ quẹt, đồng thời xem xét phương án Rule hoặc No AI nếu các giải pháp đơn giản đã đáp ứng được nhu cầu. Quyết định cuối cùng sẽ dựa trên kết quả kiểm chứng thực tế thay vì mức độ hấp dẫn của công nghệ.

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Problem Card điểm danh đầu tiết (kể cả em đến muộn). Nêu lý do chọn: đo được ngay bằng bấm giờ, có nhiều phía để phỏng vấn, so sánh được camera với QR, sơ đồ chỗ ngồi, thẻ quẹt. Đặt câu hỏi cho nhóm: nếu QR có khung giờ đã đủ cho phần lớn lớp học thì camera đếm số người có thật sự đáng đầu tư, hay mình chọn camera vì nó hấp dẫn. | Câu hỏi này kéo cuộc thảo luận về việc so sánh với phương án đơn giản hơn trước khi nghĩ đến AI. Sau khi hội tụ, nhóm chọn candidate quản lý kho làm hướng tiếp tục.|
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Hỏi Bảo (bài đánh giá CV giúp sinh viên dễ kiếm việc) : "Dữ liệu bạn lấy ở đâu ? tiêu chuẩn đánh giá CV như nào ? So với việc gửi CV lên AI khác thì có gì hơn" | Câu hỏi chạm đúng điểm yếu mà nhóm sau đó ghi nhận ở bài JD/CV: thị trường đã có nhiều công cụ review CV, cần xác định khoảng trống thật.|
| Nhận phản biện | Câu hỏi tôi nhận được (dành cho dự án điểm danh đầu giờ): "Áp dụng như thế nào trong việc điểm danh ? So với các AI điểm danh hiện tại có thì tốt hơn điều gì ?" | Tôi đã sửa gì: tìm những phương pháp tối ưu hơn về chi phí, đặt QR có khung giờ, sơ đồ chỗ ngồi, thẻ quẹt/NFC lên so sánh trước camera AI, vì camera còn có rủi ro ánh sáng, nhận diện nhầm và quyền riêng tư. Với bài quản lý kho của nhóm, tôi cũng nhận hai phản biện: "vấn đề cốt lõi có thể là dữ liệu chưa ghi đủ chứ không phải thiếu AI" và "baseline 15–30 phút mới là ước lượng". Tôi đồng ý cả hai: đưa chuẩn hóa ghi nhận và Rule lên trước, thay baseline bằng số đo từ phỏng vấn. |
| Gom cluster / cây OST | Tôi đóng góp opportunity “ghi nhận giao dịch không được ghi ngay” vào cây OST, tập trung vào tình huống chủ cửa hàng vừa bán hàng vừa quản lý kho nên dễ bỏ sót việc cập nhật tồn kho. Tôi đề xuất giải pháp hỗ trợ ghi nhận giao dịch nhanh, giảm thao tác thủ công và giúp chủ cửa hàng theo dõi hàng hóa chính xác hơn. | Cây OST của nhóm có 1 outcome và 5 opportunity; nhóm chủ động tách opportunity khỏi solution và ghi rõ "chưa kết luận cần dùng AI". |
| Chọn candidate problem | Đưa bài quản lý kho vào danh sách 6 candidate, cung cấp bối cảnh thực tế từ cửa hàng điện tử của gia đình và chấp nhận không mặc định xây AI Agent. | Nhóm chọn quản lý kho cho hộ kinh doanh nhỏ để validation, đồng thời giữ nguyên "chưa kết luận phải xây Agent". |
| Kiểm chứng / research | Tôi tham gia phỏng vấn 4 người tại cửa hàng gia đình, tìm hiểu quy trình bán hàng, quản lý kho và xác định bottleneck là giao dịch chưa được ghi nhận ngay khi bán. | Kết quả làm đổi bottleneck: từ "tra cứu trong sổ" (chỉ 1–5 phút/lần) sang "giao dịch không được ghi ngay và ghi đủ lúc bán". Actor mở rộng thành 4 vai trò. Research cho thấy KiotViet, Sapo, MISA eShop đã lo phần trừ tồn và lịch sử giá; khoảng trống thật là bước ghi nhận lúc đông khách. |
| Quy trình nhóm | Nhóm xác định opportunity, xây dựng cây OST, chọn problem để kiểm chứng, phỏng vấn và research, xác định bottleneck rồi thống nhất problem statement và giải pháp. Tôi tham gia đóng góp ý kiến, tổng hợp thông tin và hoàn thiện báo cáo. | Bottleneck là giao dịch chưa được ghi nhận ngay khi bán. Nhóm đề xuất ghi nhận giao dịch tức thời, tự động cập nhật tồn kho và cảnh báo hàng sắp hết; ưu tiên giải quyết vấn đề trước, chưa kết luận cần xây AI Agent. |
| Problem Statement | Viết Problem Statement v1 từ v0 (Actor, quy trình, bottleneck, impact, success metric, boundary, AI intervention point, rủi ro) và 5 tiêu chí đánh giá đầu ra của AI. | Có bản v1 với boundary rõ (AI không tự ghi sổ, không đặt giá, không đoán khi thiếu dữ liệu) và tiêu chí đo được để nhóm đánh giá đầu ra. |
| Mức can thiệp AI | Phụ trách CP6: đặt bài vào ma trận độ mơ hồ × độ phức tạp, so sánh 4 mức (No AI / Rule / Workflow / Agent), điền AI Canvas, trả lời hai câu hỏi Google PAIR. | Chọn Workflow trên nền No AI/Rule; loại Agent vì sai tồn kho hoặc giá gây thiệt hại thật và dữ liệu chưa đủ; hướng augment, ưu tiên tránh bỏ sót hơn báo nhầm. |
| Quyết định | Đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability), viết kết luận 8.2, ngưỡng dừng, hạn chế và hướng tiếp theo, tài liệu tham khảo. | Nhóm chưa Go: Feasibility cao vì dữ liệu chưa đủ, giả định #4 (người bán chịu nói/chụp ảnh và xác nhận) và #5 (AI nhận đúng tên hàng điện tử) còn thiếu bằng chứng. Cần kiểm chứng trên 10 giao dịch thật trước khi quyết định. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI gợi ý thêm các vấn đề liên quan đến quản lý thời gian, lưu trữ thông tin và quản lý công việc. | Gợi ý thêm góc nhìn và nhóm vấn đề mà tôi chưa nghĩ tới. | Một số gợi ý chung chung, chưa có trải nghiệm hoặc bằng chứng cụ thể từ cuộc sống của tôi. | Chỉ giữ những vấn đề phù hợp với trải nghiệm thực tế của bản thân và gia đình; bỏ các vấn đề chưa có bằng chứng. |
| CP2 Problem Card | Nhờ AI phản biện Problem Card (quản lý hàng hóa tại cửa hàng điện tử của gia đình, và card điểm danh đầu tiết). | Chỉ ra 3 điểm yếu của card kho: thiếu số liệu, dữ liệu ghi chép chưa đầy đủ thì AI khó tra cứu chính xác, chưa rõ AI hỗ trợ công đoạn nào. Với card điểm danh, gợi ý so sánh với QR, NFC trước khi dùng camera. | Chưa chỉ ra rằng phần mềm bán hàng có sẵn (KiotViet, Sapo, MISA eShop) đã giải được phần tra cứu và tính tồn; phải đến research ở CP4 tôi mới thấy điều này. Phản biện cũng thiên về đòi thêm số liệu hơn là hỏi quy trình ghi nhận thực tế diễn ra thế nào. | Đồng ý các điểm hợp lý: không tự đặt số liệu, bổ sung bước chuẩn hóa ghi chép trước khi dùng AI, giới hạn AI ở một công đoạn cụ thể. |
| CP4 Research | Nhờ AI tìm và tóm tắt các công cụ có sẵn cho bài quản lý kho: Knote, MISA AMIS CRM, KiotViet, Sapo POS, MISA eShop. | Tìm nhanh được 5 công cụ và chỉ ra pattern "ảnh hoặc câu nói → đơn nháp → người xác nhận", giúp nhóm thấy AI ở bước ghi nhận đã có tiền lệ ở Việt Nam. | Số liệu "tiết kiệm 80% thời gian" của MISA AMIS CRM là của bên bán; Knote thiết kế cho quán ăn (tên món ngắn), chưa có bằng chứng chạy tốt với tên model hàng điện tử dài. | Ghi rõ đó là số liệu của bên bán, không dùng làm bằng chứng; đưa thành giả định #5 (Feasibility) cần thử với 10 giao dịch thật của cửa hàng; đối chiếu thông tin với kết quả phỏng vấn 4 người tại cửa hàng. |
| CP5 Quy trình | Nhờ AI gợi ý khung các bước quy trình nhập hàng, bán hàng, ghi nhận, kiểm tra tồn để làm bản nháp. | Có khung quy trình ban đầu để nhóm chỉnh nhanh thay vì bắt đầu từ trang trắng. | Quy trình quá lý tưởng, mặc định giao dịch được ghi ngay lúc bán, bỏ sót tình huống thật: nhân viên bán xong mới ghi, ghi tạm ra giấy rồi tổng hợp cuối ngày. | Sửa theo snapshot phỏng vấn: thêm bước ghi tạm ra giấy và tổng hợp cuối ngày (10–15 phút/ngày), thêm bước đếm kho (20–30 phút/lần), xác định lại bottleneck nằm ở bước ghi nhận. |
| CP5–6 Problem Statement | Nhờ AI soạn bản nháp Problem Statement v1 và 5 tiêu chí đánh giá đầu ra của AI. | Sắp xếp đủ các trường và viết tiêu chí "đạt / không đạt" rõ ràng. | Bản nháp viết trước khi có kết quả phỏng vấn nên lấy "tra cứu" làm bottleneck và baseline 3–5 phút, trong khi phỏng vấn cho thấy tra giá chỉ 1–5 phút và nguyên nhân gốc là ghi nhận lúc bán. Các target (giảm một nửa thời gian, ≥ 90% giao dịch ghi đủ) cũng không có căn cứ đo. | Đối chiếu với 4 snapshot phỏng vấn, chuyển bottleneck sang ghi nhận giao dịch, mở rộng actor thành 4 vai trò, ghi rõ các con số chỉ là đề xuất chờ đo baseline. |
| CP6 Mức can thiệp / quyết định | Nhờ AI soạn bản nháp ma trận, so sánh 4 mức, AI Canvas, PAIR, 4 rủi ro và kết luận. | So sánh có hệ thống 4 mức, gợi ý lập luận "bỏ sót tệ hơn báo nhầm" và các điều kiện kiểm chứng trước khi Go. | Ngưỡng dừng (70%, 10%) và pilot do AI đề xuất, chưa có căn cứ từ dữ liệu thật; điểm can thiệp AI ban đầu (trích xuất ghi chép và tra cứu) lệch so với bằng chứng CP4 (AI nên hỗ trợ bước ghi nhận). | Giữ hướng Workflow trên nền No AI/Rule nhưng ghi rõ ngưỡng chỉ là đề xuất; đặt giả định #4 (người bán chịu nói hoặc chụp ảnh và xác nhận) và #5 làm điều kiện kiểm chứng trước khi quyết định Go. |

## 6. Reflection (CP7)

Trả lời dựa trên trải nghiệm thực tế của bản thân, tối thiểu 200 từ cho các câu từ 6.1 đến 6.6 (không tính câu 6.7 vì câu này được đánh giá riêng theo tiêu chí C5). **Không sử dụng AI viết thay.**

**6.1. Học được gì:**

Qua việc quan sát và trao đổi với các nhóm khác, tôi nhận thấy mỗi lĩnh vực có những cách tiếp cận khác nhau trong việc phân tích vấn đề và xác định điểm nghẽn (bottleneck). Điều này giúp tôi hiểu rõ hơn về sự đa dạng trong quá trình tìm kiếm và phân tích vấn đề.

**6.2. Về "solution-first":**

Ở giai đoạn đầu, nhóm tôi đã mắc phải sai lầm khi nhanh chóng hướng cuộc thảo luận sang công nghệ AI Agent. Sau khi xem xét lại định hướng của bài lab, nhóm nhận ra cách tiếp cận này chưa phù hợp. Vì vậy, chúng tôi đã chủ động dừng việc bàn về giải pháp và quay lại xây dựng quy trình As-Is nhằm xác định chính xác điểm nghẽn thực tế.

**6.3. Đổi ý khi bị phản biện:**

Có. Lúc đầu, tôi đưa ra đề xuất xây dựng AI Agent có khả năng tự động thực hiện toàn bộ quy trình. Tuy nhiên, sau khi các thành viên trong nhóm phân tích và phản biện những rủi ro liên quan đến tính khả thi và an toàn kỹ thuật (Feasibility/Viability), tôi đã thay đổi quan điểm. Phương án được lựa chọn sau đó là Workflow AI sử dụng RAG để hỗ trợ tra cứu, kết hợp với sự kiểm duyệt của con người (HITL).

**6.4. Bất ngờ từ kiểm chứng:**

Điều khiến tôi bất ngờ nhất sau quá trình kiểm chứng là nguyên nhân chính khiến quy trình bị kéo dài không nằm ở việc thiếu thiết bị đọc lỗi OBD-II. Thay vào đó, vấn đề xuất phát từ việc thợ phải dành quá nhiều thời gian để tìm kiếm và đọc các tài liệu kỹ thuật PDF có dung lượng lên đến hàng nghìn trang.

**6.5. Điều khó nhất khi viết Problem Statement:**

Khó khăn lớn nhất của tôi là giữ cho Problem Statement tập trung vào vấn đề thực tế mà không đưa các giải pháp hoặc công nghệ vào nội dung phát biểu. Bên cạnh đó, việc xác định rõ phạm vi (Boundary) cũng rất quan trọng, đặc biệt là phải làm rõ những nhiệm vụ AI được phép thực hiện và những nhiệm vụ AI không được phép can thiệp.

**6.6. Nếu làm lại:**

Nếu có cơ hội thực hiện lại, tôi sẽ đề xuất nhóm tiến hành phỏng vấn và kiểm chứng thực tế theo phương pháp Mom Test sớm hơn. Đồng thời, tôi sẽ chủ động phản biện sâu hơn về các tiêu chí đánh giá (Eval metrics), đặc biệt là khả năng xác định tính khả thi của giải pháp trước khi đưa ra quyết định cuối cùng.

**6.7. Hiểu bài (Chuỗi logic):**

Vấn đề mà nhóm tôi lựa chọn tập trung vào tình trạng thời gian chẩn đoán các lỗi phức tạp tại xưởng ô tô còn kéo dài. Quy trình hiện tại được thực hiện từ bước tiếp nhận triệu chứng, đọc mã lỗi OBD-II cho đến việc tìm kiếm thông tin trong tài liệu kỹ thuật bằng phương pháp thủ công. Mục tiêu đặt ra là giảm 30% thời gian chẩn đoán và nâng cao độ chính xác trong việc dự trù phụ tùng. Về phạm vi (Boundary), AI chỉ được sử dụng để tra cứu và tổng hợp nội dung tài liệu, không được tự đưa ra quyết định sửa chữa. Với những giới hạn này, Workflow AI kết hợp RAG và HITL được đánh giá là phù hợp hơn so với Agent tự động hoàn toàn. Cuối cùng, nhóm quyết định Go với phương án Workflow AI vì giải pháp này đáp ứng được yêu cầu về tính khả thi và đảm bảo an toàn trong quá trình vận hành.
## 7. Tài liệu tham khảo

-
