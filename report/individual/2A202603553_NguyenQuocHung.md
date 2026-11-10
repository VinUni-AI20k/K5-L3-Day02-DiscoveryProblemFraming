# Báo cáo cá nhân — 2A202603553_NguyenQuocHung

## 1. Thông tin học viên

- **Họ tên:** Nguyễn Quốc Hưng
- **MSSV:** 2A202603553
- **Tên nhóm:** BDHH
- **Link repo nhóm:** https://github.com/trinhcongduc112/K5-L3A-DAY02-BDHH-DiscoveryProblemFraming

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi ăn trưa ở căng tin vào giờ đông, tôi muốn gọi món và nhận đồ ăn nhanh hơn để kịp trở lại lớp học. | Sinh viên và nhân viên căng tin. | Khung giờ nghỉ trưa thường tập trung đông người; thời gian từ lúc vào hàng đến lúc nhận món được ước tính khoảng 20–25 phút, cần đo trực tiếp để xác nhận. |
| 2 | Tốn thời gian | Khi đến thư viện để tự học, tôi muốn biết khu vực nào còn chỗ để không phải đi qua nhiều phòng tìm bàn trống. | Sinh viên sử dụng thư viện. | Vào thời điểm đông người, việc tìm chỗ có thể phải lặp lại ở nhiều khu; thời gian ước tính 10–15 phút, chưa có số liệu đếm. |
| 3 | Lặp lại | Khi cần in tài liệu trước giờ học, tôi muốn nhận bản in đúng yêu cầu mà không phải xếp hàng lâu hoặc gửi lại tệp nhiều lần. | Sinh viên và nhân viên điểm in. | Gần giờ học, nhiều sinh viên có nhu cầu in cùng lúc; thời gian chờ ước tính 10–15 phút/lượt, chưa được đo thực tế. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi nhóm có nhiều lịch học khác nhau, tôi muốn xác định một buổi họp phù hợp để cả nhóm không phải nhắn tin qua lại quá nhiều. | Sinh viên làm bài tập nhóm. | Phải đối chiếu thời khóa biểu và tin nhắn của từng thành viên; một lần thống nhất lịch có thể mất 15–30 phút, cần kiểm chứng. |
| 5 | Pain từ người khác | Khi gửi xe ở bãi đông vào giờ tan học, tôi muốn xác định vị trí xe nhanh để không mất thời gian tìm kiếm và gây ùn tắc lối đi. | Sinh viên và nhân viên trông xe. | Mật độ xe tăng vào giờ cao điểm; thời gian tìm xe ước tính 5–10 phút, chưa có ghi nhận định lượng. |

**Ý kiến AI:** Tôi giữ lại hướng phân tích thời gian xếp hàng, tìm chỗ học và chờ in tài liệu vì có actor và quy trình rõ ràng. Tôi không chọn các ý tưởng đòi hỏi xây dựng ứng dụng ngay từ đầu khi chưa xác định được nguyên nhân của vấn đề.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Chờ gọi món và nhận đồ ăn tại căng tin giờ cao điểm | Có các bước rõ, bước nghẽn cụ thể và thời gian chờ có thể đo bằng đồng hồ. | Chậm chủ yếu ở khâu gọi món, thanh toán hay chế biến? |
| 2 | Mất thời gian tìm chỗ tự học trong thư viện | Ảnh hưởng trực tiếp đến thời gian học; có thể kiểm tra bằng cách quan sát các khu vực. | Thời điểm nào kín chỗ và có bao nhiêu bàn còn trống? |
| 3 | Xếp hàng in tài liệu trước giờ học | Nhu cầu lặp lại, có thể đo thời gian hoàn thành từng lượt in. | Thời gian chờ do số người xếp hàng hay do lỗi tệp in? |

### Problem Card #1 — Chờ lấy đồ ăn tại căng tin

| Trường | Nội dung |
|---|---|
| Job Story | Khi ăn trưa ở căng tin vào giờ đông, tôi muốn gọi món và nhận đồ ăn nhanh hơn để kịp trở lại lớp học. |
| Actor | Sinh viên ăn trưa tại căng tin. |
| Thời điểm / bối cảnh | Giờ nghỉ trưa, khi nhiều sinh viên đến cùng lúc. |
| Quy trình hiện tại (3–7 bước) | Đến quầy → Xem món → Xếp hàng gọi món → Thanh toán → Chờ chế biến và nhận món. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Xếp hàng gọi món, ước tính 10 phút/lượt. |
| Impact (nếu không giải thì sao) | Giảm thời gian nghỉ ngơi, có thể vào lớp muộn; quầy phục vụ dễ bị ùn ứ. |
| Success metric (baseline → target) | Tổng thời gian dự kiến 23 phút/lượt → tối đa 15 phút/lượt; đo từ lúc đến quầy đến khi nhận món. Baseline hiện là ước tính. |
| Phương án không dùng AI | Tách hàng gọi món và hàng nhận món, hiển thị thực đơn rõ ràng, dùng số thứ tự và chuẩn bị sẵn món bán chạy. |
| Giả thuyết về AI (nếu có) | Có thể dự báo nhu cầu từng món theo khung giờ nếu sau này có đủ lịch sử đơn hàng; chưa cần ở bước đầu. |
| Cảm nhận nhanh | Rule. |

**Quy trình nháp hiện tại (thời gian ước tính):**

```text
Đến quầy (2') → Xem món (2') → Xếp hàng gọi món (10') [BOTTLENECK]
→ Thanh toán (2') → Chờ chế biến và nhận món (7')
Tổng: 23 phút
```

### Problem Card #2 — Tìm chỗ tự học tại thư viện

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến thư viện để tự học, tôi muốn biết khu vực nào còn chỗ để không phải đi qua nhiều phòng tìm bàn trống. |
| Actor | Sinh viên đến thư viện vào giờ đông. |
| Thời điểm / bối cảnh | Buổi chiều và trước các đợt kiểm tra, khi nhiều bàn học đã có người. |
| Quy trình hiện tại (3–7 bước) | Đến thư viện → Đi đến khu học → Tìm bàn trống → Chuyển sang khu khác nếu hết chỗ → Ổn định chỗ ngồi. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tìm bàn trống, ước tính 8 phút/lượt. |
| Impact (nếu không giải thì sao) | Mất thời gian học, tăng việc đi lại giữa các khu và dễ bỏ cuộc nếu không tìm được chỗ. |
| Success metric (baseline → target) | Tổng thời gian dự kiến 19 phút/lượt → tối đa 8 phút/lượt; đo từ lúc vào thư viện đến khi ngồi học. Baseline hiện là ước tính. |
| Phương án không dùng AI | Bảng chỉ dẫn các khu vực, cập nhật số chỗ trống theo khu bằng kiểm đếm thủ công hoặc nút xác nhận đơn giản. |
| Giả thuyết về AI (nếu có) | Chưa cần AI nếu việc cập nhật chỗ trống được thực hiện bằng quy tắc và kiểm đếm đơn giản. |
| Cảm nhận nhanh | Rule. |

**Quy trình nháp hiện tại (thời gian ước tính):**

```text
Đến thư viện (1') → Đi tới khu học (3') → Tìm bàn trống (8') [BOTTLENECK]
→ Chuyển khu nếu hết chỗ (5') → Ổn định chỗ ngồi (2')
Tổng: 19 phút
```

### Problem Card #3 — Xếp hàng in tài liệu

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần in tài liệu trước giờ học, tôi muốn nhận bản in đúng yêu cầu mà không phải xếp hàng lâu hoặc gửi lại tệp nhiều lần. |
| Actor | Sinh viên sử dụng điểm in tài liệu gần trường. |
| Thời điểm / bối cảnh | Trước giờ vào lớp hoặc gần hạn nộp bài. |
| Quy trình hiện tại (3–7 bước) | Chuẩn bị tệp → Xếp hàng → Xác nhận số trang và định dạng → In tài liệu → Thanh toán và nhận bản in. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Xếp hàng chờ đến lượt, ước tính 8 phút/lượt. |
| Impact (nếu không giải thì sao) | Có nguy cơ đến lớp muộn, in vội và kiểm tra thiếu trang. |
| Success metric (baseline → target) | Tổng thời gian dự kiến 17 phút/lượt → tối đa 10 phút/lượt; đo từ lúc đến điểm in đến khi nhận bản in. Baseline hiện là ước tính. |
| Phương án không dùng AI | Nhận tệp trước qua một biểu mẫu cố định, chuẩn hóa thông tin in và thông báo số thứ tự nhận tài liệu. |
| Giả thuyết về AI (nếu có) | Chưa cần AI vì việc nhận tệp và xếp lượt là quy trình có quy tắc rõ. |
| Cảm nhận nhanh | Rule. |

**Quy trình nháp hiện tại (thời gian ước tính):**

```text
Chuẩn bị tệp (2') → Xếp hàng (8') [BOTTLENECK]
→ Xác nhận yêu cầu in (2') → In tài liệu (4') → Thanh toán, nhận bản in (1')
Tổng: 17 phút
```

### Card muốn pitch nhất

- **Card số:** 1.
- **Vì sao:** Thời gian chờ tại căng tin tác động trực tiếp đến sinh hoạt hằng ngày, dễ quan sát các bước và kiểm tra hiệu quả cải tiến.
- **Câu hỏi muốn nhóm phản biện:** Nếu chỉ thay đổi cách xếp hàng mà không tăng nhân viên, thời gian nhận món có giảm đáng kể không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa xác định thời gian chờ nhiều nhất ở gọi món hay chế biến. | Có | Tách bước gọi món và nhận món để có thể đo riêng. |
| Số phút ước tính chưa phải baseline đo được. | Có | Ghi rõ thời gian ước tính và xác định phép đo từ lúc đến quầy đến lúc nhận món. |
| Phương án đặt món trước có thể chuyển điểm nghẽn sang khâu chế biến. | Có | Ưu tiên kiểm tra thay đổi quy trình quầy trước khi tính đến công cụ đặt món. |

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày vấn đề chờ gọi món và nhận đồ ăn ở căng tin, cùng quy trình 5 bước. | Vấn đề có actor, bottleneck và metric rõ để so sánh. |
| Phản biện bài của bạn khác | Đặt câu hỏi: “Tìm chỗ trong thư viện lâu là do thiếu chỗ hay do thiếu thông tin về chỗ trống?” | Phân biệt được nguyên nhân vận hành và nguyên nhân thiếu thông tin. |
| Nhận phản biện | Xem xét câu hỏi: “Nếu giảm thời gian xếp hàng nhưng đồ ăn vẫn chế biến chậm thì có giải quyết được vấn đề không?” | Điều chỉnh phân tích để đo riêng thời gian gọi món và thời gian nhận món. |
| Gom cluster / cây OST | Nhóm các vấn đề thành ba pain: chờ đến lượt, tìm thông tin sẵn có và phối hợp lịch trình. | Làm rõ outcome chung là giảm thời gian không tạo giá trị cho sinh viên. |
| Chọn candidate problem | Đề xuất vấn đề căng tin vì phù hợp một thử nghiệm quy trình nhỏ. | Ưu tiên một candidate có thể đo trước/sau. |
| Kiểm chứng / research | Xác định các dữ liệu cần ghi: số người xếp hàng, thời gian gọi món, thời gian nhận món, khung giờ và món bán chạy; đối chiếu các cách tổ chức hàng chờ. | Chưa kết luận nguyên nhân chính khi chưa có đủ dữ liệu đo thực tế. |
| Quy trình nhóm | So sánh quy trình 5 bước với phương án tách quầy gọi món, thanh toán và nhận món. | Xác định chỗ có thể giảm thao tác lặp và tránh chen hàng. |
| Problem Statement | Đề xuất metric về tổng thời gian từ lúc đến quầy đến khi nhận món và boundary về xác nhận đơn hàng. | Bài toán được giới hạn vào cải tiến phục vụ giờ cao điểm. |
| Mức can thiệp AI | So sánh No AI, Rule, Workflow và Agent. | Ưu tiên Rule vì đánh số và phân luồng hàng chờ không đòi hỏi AI. |
| Quyết định | Đề xuất Not Yet đối với việc triển khai công cụ mới cho đến khi có số đo trước/sau; trước mắt kiểm tra phương án tổ chức lại quầy. | Có hướng kiểm chứng cụ thể trước khi mở rộng giải pháp. |

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm các góc nhìn để phân loại các vấn đề sinh hoạt thường ngày. | Giúp phân biệt vấn đề với giải pháp. | Một số ý tưởng thiên về làm ứng dụng dù chưa có nhu cầu rõ. | Giữ các vấn đề có quy trình quan sát và đo được. |
| CP2 Problem Card | Phản biện card về thời gian chờ và đề xuất cách tách bước. | Chỉ ra sự khác nhau giữa xếp hàng và chờ chế biến. | Dễ coi thời gian ước tính là dữ liệu chắc chắn. | Ghi rõ ước tính và cách đo baseline. |
| CP4 Research | Dùng để lập danh sách phương án quản lý hàng chờ có thể so sánh. | Gợi ý phân luồng quầy, số thứ tự và đặt món trước. | Chưa chứng minh các giải pháp phù hợp với căng tin cụ thể. | Không xem các gợi ý là bằng chứng kiểm chứng vấn đề. |
| CP5 Quy trình | Rà soát các bước của quy trình trước và sau. | Phát hiện bước có thể tách và bước có thể rút gọn. | Chưa tính đến việc quầy nhận món có thể trở thành điểm nghẽn mới. | Giữ bước nhân viên xác nhận món và đo cả thời gian chờ nhận món. |
| CP5–6 Problem Statement | Nhờ chỉ ra các điểm chưa rõ về metric và phạm vi. | Giúp xác định đầu vào, đầu ra và người kiểm tra. | Ban đầu mở rộng sang hệ thống quản lý toàn bộ căng tin. | Giới hạn vào thời gian phục vụ giờ cao điểm. |
| CP6 Mức can thiệp / quyết định | So sánh Rule, Workflow và Agent. | Nêu lợi ích, chi phí và độ phức tạp của từng mức. | Đề xuất dự báo thông minh khi chưa có dữ liệu lịch sử. | Ưu tiên Rule, chưa triển khai giải pháp AI. |

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Tôi nhận ra rằng những bất tiện thường gặp ở trường có thể đến từ các nguyên nhân rất khác nhau. Chờ đồ ăn ở căng tin liên quan đến năng lực phục vụ, còn việc tìm chỗ trong thư viện có thể là vấn đề thông tin hoặc số lượng chỗ ngồi thực tế. Vì vậy, tôi không thể chỉ nhìn thấy người dùng mất thời gian rồi kết luận rằng cần một ứng dụng mới. Điều quan trọng là xác định bước nào trong quy trình tạo ra sự chậm trễ.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có. Khi phân tích vấn đề căng tin, phương án đặt món trực tuyến xuất hiện khá sớm. Tuy nhiên, tôi nhận thấy đặt món trước chưa chắc giúp nhận món nhanh hơn nếu bếp vẫn xử lý chậm. Tôi chuyển trọng tâm về việc tách các bước gọi món, thanh toán và chế biến. Nhờ vậy, giải pháp được đánh giá theo điểm nghẽn thực sự thay vì mức độ hiện đại của công cụ.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Ban đầu tôi cho rằng phần lớn thời gian chờ nằm ở hàng gọi món. Khi xem lại quy trình, tôi nhận ra thời gian chờ chế biến cũng có thể dài và thay đổi theo từng loại món. Tôi sửa Problem Card để đo riêng hai khoảng thời gian, đồng thời không khẳng định một bước là nguyên nhân chính khi chưa quan sát đủ lượt phục vụ.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều khiến tôi chú ý là cùng một biểu hiện “chờ lâu” có thể do nhiều nguyên nhân: khách đến cùng lúc, thao tác thanh toán kéo dài hoặc món ăn cần chế biến lâu. Qua đối chiếu các phương án tổ chức hàng chờ, tôi thấy việc tạo thêm kênh đặt món có thể khiến khâu chế biến quá tải nếu không phân luồng. Tôi cũng nhận ra chưa thể đưa ra kết luận định lượng đáng tin cậy khi chưa đo thời gian phục vụ thực tế.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là chuyển nhận xét “căng tin phục vụ chậm” thành một bài toán có thể đo. Tôi phải xác định rõ actor là sinh viên dùng căng tin vào giờ cao điểm, phạm vi tính từ lúc đến quầy đến khi nhận món và metric là thời gian hoàn thành một lượt. Tôi cũng xác định boundary là phương án không tự thay đổi đơn đã thanh toán và phải có nhân viên xác nhận khi phát sinh sai lệch.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Tôi sẽ quan sát nhiều khung giờ hơn, ghi thời gian cho từng bước và phân biệt món có sẵn với món cần chế biến. Tôi cũng sẽ hỏi người dùng về lần gần nhất họ phải chờ, thay vì hỏi họ có thích một tính năng mới hay không. Khi phản biện, tôi sẽ tập trung vào bằng chứng cho từng giả thuyết và khả năng phát sinh điểm nghẽn mới sau khi thay đổi quy trình.

**6.7. Hiểu bài:** Giải thích bằng 5–8 câu chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Vấn đề được chọn là sinh viên mất nhiều thời gian gọi món và nhận đồ ăn ở căng tin vào giờ cao điểm. Quy trình hiện tại gồm đến quầy, xem món, xếp hàng gọi món, thanh toán và chờ nhận món. Điểm nghẽn cần kiểm tra là thời gian xếp hàng gọi món so với thời gian chế biến. Metric chính là tổng thời gian từ lúc đến quầy đến khi nhận món, với mốc 23 phút chỉ là ước tính ban đầu và mục tiêu không quá 15 phút. Boundary là mọi thay đổi đơn hàng và trường hợp sai món vẫn phải được nhân viên kiểm tra, xác nhận. Nhóm ưu tiên mức Rule, sử dụng đánh số thứ tự và phân luồng phục vụ thay vì triển khai Agent. Quyết định là **Not Yet** đối với công cụ mới cho đến khi có đủ dữ liệu đo, đồng thời thử cải tiến quy trình bằng cách đơn giản trước.
