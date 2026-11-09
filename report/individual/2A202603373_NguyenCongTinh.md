# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Công Tĩnh
- MSSV: 2A202603373
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: hhuydaugg
- Link repo nhóm: https://github.com/hhuydaugg/K5-L3-Day02-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)
**Nhân vật:** Nam là một Junior Product Manager phụ trách tham gia kiểm thử, đánh giá và cải tiến các chức năng thuộc hệ thống chăm sóc khách hàng và xử lý sự cố của Xanh SM. Trong công việc hằng ngày, Nam thường xuyên tiếp nhận thông tin phản hồi từ nhân viên chăm sóc khách hàng, bộ phận vận hành, tài xế và người dùng. Nam có nhiệm vụ tổng hợp các lỗi phát sinh trong quá trình sử dụng hệ thống, ghi nhận những bất cập trong quy trình xử lý, phân tích phản hồi của các bên liên quan và phối hợp với đội ngũ kỹ thuật để đề xuất cải tiến sản phẩm. 

**Vì sao đây là ví dụ tốt:** actor cụ thể; quy trình lặp lại hằng tuần; bottleneck rõ; có baseline thời gian; so sánh được No AI / Rule / Workflow / Agent; và quan trọng nhất, **research làm nhóm đổi kết luận**.


| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Khi kết thúc mỗi đợt kiểm thử, tôi muốn tổng hợp toàn bộ lỗi phát sinh vào một danh sách, để không bỏ sót lỗi cần xử lý |Nam, QA, Developer |Sau mỗi đợt kiểm thử một chức năng hoặc một phiên bản hệ thống, Nam phải tổng hợp lại các lỗi được ghi nhận từ nhiều nguồn như file Excel, công cụ quản lý công việc, tin nhắn trao đổi và phản hồi của thành viên kiểm thử. Một đợt kiểm thử có thể phát sinh khoảng 30–50 lỗi. Nam phải kiểm tra từng lỗi, loại bỏ nội dung trùng lặp, chuẩn hóa tên lỗi, bổ sung trạng thái và người phụ trách. Công việc này có thể mất khoảng 60–90 phút cho mỗi đợt tổng hợp. Đây cũng là 1 case thường gặp trong thực tế ở mỗi đợt kiểm thử của các dự án khác https://www.atlassian.com/software/jira/templates/bug-report? |
| 2 |Lặp lại |Khi nhận phản hồi khách hàng, tôi muốn phân loại theo từng nhóm vấn đề, để dễ theo dõi và chuyển đúng bộ phận xử lý |Nam, CSKH |Mỗi ngày tiếp nhận khoảng 50–100 phản hồi cần phân loại.bao gồm các vấn đề như lỗi đăng nhập, đặt xe, thanh toán, thông tin chuyến đi hoặc thao tác trên ứng dụng. Việc phân loại phản hồi khách hàng là 1 vấn đề lớn và thường xuyên được thống kê trên các bài báo diễn đàn https://support.zendesk.com/hc/en-us/articles/4408832234394-Analyzing-the-metrics-that-matter-to-improve-customer-support |
| 3 |Cần đọc, tổng hợp nhiều thông tin |Khi có nhiều phản hồi từ khách hàng và nhân viên CSKH, tôi muốn phát hiện những vấn đề giống nhau, để xác định lỗi phổ biến và ưu tiên cải tiến |Nam, CSKH, Product Manager |Một vấn đề có thể xuất hiện trong nhiều phản hồi khác nhau, khó nhận diện thủ công,Nếu chỉ tìm kiếm bằng từ khóa, Nam có thể bỏ sót những phản hồi có cùng nguyên nhân nhưng khác cách diễn đạt. https://www.microsoft.com/en-us/research/publication/incident-aware-duplicate-ticket-aggregation-for-cloud-systems/?utm_source=chatgpt.com |
| 4 |Pain từ người khác |Khi nhân viên CSKH gặp lỗi trên hệ thống, họ muốn có hướng dẫn xử lý rõ ràng, để không phải liên hệ bộ phận kỹ thuật nhiều lần |Nhân viên CSKH, Developer |Trong quá trình tiếp nhận và xử lý phản ánh của khách hàng, nhân viên CSKH có thể gặp các lỗi hệ thống nhưng không có hướng dẫn xử lý cụ thể hoặc không biết tài liệu hướng dẫn nằm ở đâu..Nhân viên CSKH thường xuyên phải hỏi lại cách xử lý lỗi qua Slack |
| 5 |Pain từ người khác |Khi Developer nhận yêu cầu xử lý lỗi, họ muốn nhận được mô tả đầy đủ và chính xác, để không phải hỏi lại Nam hoặc CSKH |Developer, Nam, CSKH |Khi nhận yêu cầu xử lý lỗi từ Nam hoặc CSKH, Developer thường cần các thông tin như mô tả lỗi, thời điểm xảy ra, thiết bị hoặc phiên bản ứng dụng, các bước tái hiện, kết quả thực tế và ảnh/video minh họa. Tuy nhiên, phản ánh ban đầu đôi khi chỉ có nội dung chung chung như “ứng dụng bị lỗi”, “không đặt được xe” hoặc “không thanh toán được”.Developer phải yêu cầu bổ sung thông tin nhiều lần trước khi tái hiện được lỗi |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

AI gợi ý 

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Phân loại phản hồi khách hàng theo nhóm vấn đề |Công việc lặp lại hằng ngày, số lượng phản hồi lớn, dễ mất thời gian và phân loại sai |Có thể dùng Rule thay vì AI hay không? |
| 2 |Phát hiện vấn đề trùng lặp từ phản hồi khách hàng và CSKH |Cần đọc, đối chiếu nhiều nguồn, khó nhận diện lỗi phổ biến và nguyên nhân chung |AI có phát hiện chính xác các phản hồi cùng bản chất nhưng khác cách diễn đạt không? |
| 3 |Xây dựng hướng dẫn xử lý lỗi cho nhân viên CSKH |Giảm việc hỏi lại bộ phận kỹ thuật, giúp nhân viên xử lý nhanh và nhất quán |Có đủ tài liệu hướng dẫn đáng tin cậy và cập nhật không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story |Khi nhận phản hồi khách hàng, tôi muốn phân loại theo từng nhóm vấn đề, để dễ theo dõi và chuyển đúng bộ phận xử lý.|
| Actor |Nam – Junior Product Manager; nhân viên CSKH |
| Thời điểm / bối cảnh |Hằng ngày, khi tiếp nhận phản hồi từ khách hàng qua các kênh chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |1. Tiếp nhận phản hồi. 2. Đọc nội dung. 3. Xác định nhóm vấn đề. 4. Ghi nhận vào bảng theo dõi. 5. Chuyển bộ phận phụ trách. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Đọc và phân loại thủ công từng phản hồi; giả định mất 1–2 phút/phản hồi. |
| Impact (nếu không giải thì sao) |Tốn thời gian, phân loại không nhất quán, chuyển sai bộ phận và chậm xử lý phản hồi. |
| Success metric (baseline → target) |Baseline giả định: 50–100 phản hồi/ngày. Target: giảm ít nhất 50% thời gian phân loại, độ chính xác từ 90% trở lên. |
| Phương án không dùng AI |Xây dựng danh mục nhóm lỗi, biểu mẫu nhập liệu và quy tắc phân loại cố định. |
| Giả thuyết về AI (nếu có) |AI có thể đọc hiểu nội dung phản hồi và tự động đề xuất nhóm vấn đề phù hợp. |
| Cảm nhận nhanh | Workflow kết hợp AI |

Quy trình nháp hiện tại:
```
[1 Tiếp nhận phản hồi: 1'] → [2 Đọc và hiểu nội dung: 1–2']
→ [3 Xác định nhóm vấn đề: 1–2'] ← BOTTLENECK
→ [4 Ghi nhận vào bảng theo dõi: 1'] → [5 Chuyển bộ phận phụ trách: 1']
→ [6 Theo dõi trạng thái xử lý: 1–2']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story |Khi có nhiều phản hồi từ khách hàng và nhân viên CSKH, tôi muốn phát hiện những vấn đề giống nhau, để xác định lỗi phổ biến và ưu tiên cải tiến.|
| Actor |Nam – Junior Product Manager; nhân viên CSKH; Product Manager; Developer. |
| Thời điểm / bối cảnh |Khi tổng hợp phản hồi khách hàng, kết quả kiểm thử và báo cáo sự cố định kỳ. |
| Quy trình hiện tại (3–7 bước) |1. Thu thập phản hồi từ các nguồn. 2. Đọc nội dung từng phản hồi. 3. Đối chiếu các nội dung tương tự. 4. Nhóm các vấn đề trùng lặp. 5. Xác định lỗi phổ biến. 6. Báo cáo và đề xuất ưu tiên cải tiến. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Phải đọc và đối chiếu nhiều nội dung khác nhau; giả định mất 60–90 phút cho mỗi lần tổng hợp. |
| Impact (nếu không giải thì sao) |Bỏ sót lỗi có cùng nguyên nhân, thống kê sai số lượng sự cố, chậm phát hiện vấn đề nghiêm trọng và ưu tiên cải tiến chưa chính xác. |
| Success metric (baseline → target) |Baseline giả định: 60–90 phút/lần tổng hợp. Target: giảm ít nhất 50% thời gian; độ chính xác phát hiện nhóm vấn đề trùng lặp đạt từ 90% trở lên. |
| Phương án không dùng AI |Dùng từ khóa, mã lỗi, danh mục sự cố và bộ lọc trong Google Sheets để nhóm dữ liệu. |
| Giả thuyết về AI (nếu có) |AI có thể đọc hiểu ngữ nghĩa, nhận diện các phản hồi khác cách diễn đạt nhưng cùng bản chất, tự động nhóm và gợi ý vấn đề cần ưu tiên. |
| Cảm nhận nhanh | Agent kết hợp Workflow (cần kiểm chứng với Rule và Workflow đơn giản hơn). |

Quy trình nháp hiện tại:

```
[1 Thu thập phản hồi từ nhiều nguồn: 5'] → [2 Đọc và rà soát nội dung: 15']
→ [3 Đối chiếu các phản hồi tương tự: 20'] ← BOTTLENECK
→ [4 Nhóm các vấn đề trùng lặp: 15'] → [5 Thống kê tần suất và mức độ xuất hiện: 10']
→ [6 Xác định mức độ ưu tiên: 5'] → [7 Lập báo cáo và đề xuất cải tiến: 5']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhân viên CSKH gặp lỗi trên hệ thống, họ muốn có hướng dẫn xử lý rõ ràng, để không phải liên hệ bộ phận kỹ thuật nhiều lần. |
| Actor |Nhân viên CSKH; Developer; Nam – Junior Product Manager. |
| Thời điểm / bối cảnh |Khi nhân viên CSKH gặp lỗi trong quá trình sử dụng hệ thống chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |1. Nhân viên phát hiện lỗi. 2. Tìm hướng dẫn xử lý. 3. Không tìm được thì liên hệ kỹ thuật. 4. Mô tả tình trạng lỗi. 5. Nhận hướng dẫn. 6. Thực hiện và phản hồi kết quả. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Nhân viên phải tìm kiếm tài liệu hoặc chờ Developer phản hồi; giả định mất 10–20 phút cho mỗi trường hợp cần hỗ trợ. |
| Impact (nếu không giải thì sao) |Tăng thời gian xử lý, gây quá tải cho Developer, ảnh hưởng trải nghiệm khách hàng và hiệu suất CSKH. |
| Success metric (baseline → target) |Baseline giả định: 10–20 phút/lần hỗ trợ. Target: giảm ít nhất 40% thời gian tìm kiếm hướng dẫn và giảm số lượt hỏi lại kỹ thuật. |
| Phương án không dùng AI |Xây dựng thư viện FAQ, tài liệu hướng dẫn và quy trình xử lý lỗi theo từng tình huống. |
| Giả thuyết về AI (nếu có) |AI có thể tìm kiếm tài liệu, hiểu tình huống nhân viên mô tả và đưa ra hướng dẫn xử lý phù hợp. |
| Cảm nhận nhanh |Workflow kết hợp AI hoặc Agent tra cứu tài liệu. |

Quy trình nháp hiện tại:

```
[1 Phát hiện lỗi trong quá trình hỗ trợ khách hàng: 1']
→ [2 Tìm kiếm tài liệu hướng dẫn: 3–5']
→ [3 Không tìm thấy hướng dẫn phù hợp: 1']
→ [4 Liên hệ bộ phận kỹ thuật: 2']
→ [5 Chờ phản hồi và hướng dẫn xử lý: 10–20'] ← BOTTLENECK
→ [6 Thực hiện theo hướng dẫn: 3–5']
→ [7 Phản hồi kết quả xử lý: 1']

```

### Card muốn pitch nhất

- Card số:2
- Vì sao:
 +Phải đọc và tổng hợp lượng lớn phản hồi từ nhiều nguồn.
 +Các phản hồi có thể khác cách diễn đạt nhưng cùng một nguyên nhân.
 +Khó phát hiện lỗi phổ biến nếu chỉ kiểm tra thủ công.
 +Có thể đo thời gian, độ chính xác và tỷ lệ phát hiện lỗi trùng lặp.
 +Có cơ hội so sánh rõ ràng giữa Rule, Workflow và Agent.
- Câu hỏi muốn nhóm phản biện:
Liệu AI Agent có thực sự cần thiết để phát hiện và nhóm các vấn đề trùng lặp, hay một Workflow kết hợp AI phân loại ngữ nghĩa đã đủ giải quyết bài toán với chi phí thấp và dễ kiểm soát hơn?
### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Chưa chứng minh được các phản hồi khác nhau thực sự có cùng nguyên nhân. |Đồng ý |Bổ sung bước đối chiếu, xác minh nhóm lỗi và kiểm chứng bằng dữ liệu thực tế. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: |1. Vấn đề tài xế taxi điện cạn pin dưới 5%:Nếu hệ thống đề xuất trạm sạc gần nhất nhưng trạm đó hết trụ, đang bảo trì hoặc không phù hợp với loại xe, làm thế nào để đảm bảo thông tin đưa ra thực sự chính xác và an toàn cho tài xế? 2. Vấn đề sinh viên đối chiếu bài lab với rubric:Nếu AI đánh giá bài làm đã đáp ứng rubric nhưng thực tế nội dung còn sai hoặc thiếu yêu cầu chuyên môn, sinh viên có thể quá tin tưởng vào kết quả AI và nộp bài không đạt chất lượng hay không? 3. Vấn đề thư ký tổng hợp quyết định sau cuộc họp: Nếu trong cuộc họp có những quyết định chưa thống nhất hoặc chưa xác định rõ người chịu trách nhiệm, AI sẽ phân biệt đâu là quyết định chính thức và đâu chỉ là ý kiến đề xuất như thế nào? |
| Nhận phản biện | Câu hỏi tôi nhận được:câu 1:Nếu áp dụng tự động hóa việc phân loại phản hồi, làm sao để đảm bảo độ chính xác của hệ thống khi các phản hồi của khách hàng thường sử dụng ngôn ngữ không chính thống, từ lóng hoặc diễn đạt không rõ ràng? câu 2:Việc đối chiếu thủ công mất 20 phút/lần là một con số giả định, vậy nếu hệ thống tự động tìm ra các nhóm phản hồi tương tự, thì PM có thực sự tiết kiệm được thời gian không, hay vẫn phải mất thời gian xác thực lại các nhóm đó vì máy tính có thể gom nhóm sai logic nghiệp vụ?  câu 3:Thay vì xây dựng hệ thống hướng dẫn xử lý lỗi (knowledge base) cho CSKH, tại sao không tập trung vào việc tối ưu hóa quy trình báo lỗi hoặc tự động hóa các lỗi thường gặp để CSKH có thể tự xử lý mà không cần đến Developer? | Tôi đã sửa gì:câu 1: tôi sẽ dùng ai như một công cụ hỗ trợ phân loại.Tôi đề xuất xử lý theo 4 bước:Chuẩn hóa dữ liệu: AI nhận diện lỗi chính tả, từ viết tắt, từ lóng và các cách diễn đạt khác nhau nhưng có ý nghĩa tương tự. Phân loại theo danh mục nghiệp vụ: Xây dựng bộ nhóm vấn đề cố định, chẳng hạn lỗi đặt xe, thanh toán, đăng nhập, định vị và thông tin chuyến đi.Đánh giá độ tin cậy: Nếu AI có độ tin cậy cao, hệ thống đề xuất nhóm phân loại; nếu độ tin cậy thấp hoặc phản hồi không rõ ràng, hệ thống chuyển cho PM/CSKH xác nhận.Cải thiện liên tục: Những trường hợp AI phân loại sai sẽ được nhân viên điều chỉnh và bổ sung vào dữ liệu tham chiếu để cải thiện hệ thống. câu 2:Tôi đồng ý rằng 20 phút/lần hiện mới là số liệu giả định, chưa phải kết quả đo lường thực tế.AI có thể hỗ trợ PM ở những công đoạn tốn nhiều thời gian nhất:Tự động đọc và so sánh: AI phân tích nội dung phản hồi từ khách hàng, CSKH và kết quả kiểm thử. Phát hiện nội dung tương tự: Nhận diện những phản hồi khác cách diễn đạt nhưng có thể liên quan đến cùng một vấn đề.Đề xuất nhóm vấn đề: Tổng hợp các phản hồi thành từng nhóm, hiển thị số lượng, nội dung đại diện và lý do đề xuất gom nhóm.PM xác thực: PM kiểm tra các nhóm được đề xuất, chỉnh sửa những trường hợp AI gom sai nguyên nhân nghiệp vụ trước khi đưa vào báo cáo. Câu 3: Tôi cho rằng đây là một ý kiến hợp lý. Thực tế, xây dựng Knowledge Base, tối ưu quy trình báo lỗi và tự động hóa các lỗi thường gặp không phải những giải pháp đối lập mà có thể kết hợp với nhau. |
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
