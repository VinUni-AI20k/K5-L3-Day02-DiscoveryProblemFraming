# Báo cáo cá nhân — 2A202604016_ChuNguyenTungDuong

> Hướng dẫn: [Worksheet](../../docs/01-worksheet.md).

**Chú giải ký hiệu**

Các quy trình, bước nghẽn và tác động trong CP2 là giả thuyết ban đầu.

| Ký hiệu | Ý nghĩa |
|---|---|
| **[CẦN XÁC MINH: ...]** | Cần bổ sung thông tin hoặc bằng chứng thực tế. |
| **[CẦN ĐO]** | Chưa có số đo thực tế, kể cả mức hiện tại (baseline). |
| **[CẦN XÁC ĐỊNH: ...]** | Chưa chốt mục tiêu, tiêu chí đánh giá hoặc người kiểm tra. |
| **GIẢ THUYẾT / BOTTLENECK GIẢ THUYẾT** | Nhận định hoặc bước nghẽn cần kiểm chứng. |
| **PHÁC THẢO** | Quy trình nháp, chưa đối chiếu với quan sát thực tế. |

## 1. Thông tin học viên

- Họ tên: Chu Nguyễn Tùng Dương
- MSSV: 2A202604016
- Lớp: L3B
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhóm 6
- Link repo nhóm: https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| #12 | Lặp lại | Khi phải điền thông tin khách hàng vào nhiều biểu mẫu, tôi muốn nắm rõ thông tin cần nhập ở từng biểu mẫu, để hoàn tất hồ sơ mà không bỏ sót. | Nhân viên nhập liệu | [CẦN XÁC MINH: loại biểu mẫu, thông tin phải nhập lại, thời gian và tần suất thực tế.] |
| #15 | Lặp lại | Khi đến kỳ tổng hợp báo cáo từ nhiều bảng dữ liệu và tài liệu, tôi muốn nắm được các thông tin cần báo cáo, để hoàn thành báo cáo đúng yêu cầu. | Nhân viên lập báo cáo | [CẦN XÁC MINH: nguồn dữ liệu, thời gian và tần suất lập báo cáo; bằng chứng thực tế.] |
| #6 | Tốn thời gian | Khi cần review một Pull Request lớn, tôi muốn hiểu các thay đổi và rủi ro liên quan, để đưa ra nhận xét có căn cứ. | Developer review Pull Request | [CẦN XÁC MINH: ví dụ Pull Request, thời gian review và bước gây chậm.] |
| #1 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị bài lab có nhiều file hướng dẫn, tôi muốn xác định những gì cần nộp, để chuẩn bị bài nộp đúng yêu cầu. | Sinh viên làm lab | [CẦN XÁC MINH: file đã đọc, thời gian tìm yêu cầu, lần gặp khó và bằng chứng.] |
| #4 | Cần đọc, tổng hợp nhiều thông tin | Khi ôn tập từ slide, PDF và ghi chú, tôi muốn nắm được kiến thức cần ôn trong các nguồn, để chuẩn bị cho kỳ học hoặc bài kiểm tra. | Sinh viên ôn tập | [CẦN XÁC MINH: môn học, nguồn tài liệu, thời gian tổng hợp và tần suất.] |
| #5 | Pain từ người khác | Khi chuẩn bị thi hoặc làm lab, tôi muốn nhận biết phần kiến thức mình còn thiếu, để tập trung ôn đúng nội dung. | Sinh viên chuẩn bị thi hoặc làm lab | [CẦN XÁC MINH: ai gặp khó khăn, biểu hiện cụ thể và bằng chứng từ người thật.] |
| #14 | Tốn thời gian | Khi nhận nhiều phiên bản tài liệu, tôi muốn nhận biết nội dung đã thay đổi, để làm việc dựa trên thông tin phù hợp. | Nhân viên đọc hoặc cập nhật tài liệu | [CẦN XÁC MINH: ví dụ phiên bản, thời gian đối chiếu và tần suất.] |
| #20 | Tốn thời gian | Khi cần xử lý yêu cầu liên quan đến sản phẩm, tôi muốn tìm được hóa đơn, phiếu bảo hành và giấy tờ cần thiết, để hoàn tất yêu cầu. | Người dùng hoặc chủ sở hữu sản phẩm | [CẦN XÁC MINH: lần tìm giấy tờ thực tế, thời gian tìm và loại yêu cầu.] |
| #19 | Pain từ người khác | Khi kiểm tra các khoản điện, nước và dịch vụ, tôi muốn đối chiếu chúng với hợp đồng thuê nhà, để biết khoản phải trả có phù hợp không. | Người thuê nhà | [CẦN XÁC MINH: ai thực sự gặp vấn đề, khoản cần đối chiếu, thời gian và bằng chứng.] |
| #18 | Cần đọc, tổng hợp nhiều thông tin | Khi cân nhắc mua một sản phẩm ở nhiều nơi bán, tôi muốn hiểu sự khác nhau về thông số và chính sách bảo hành, để chọn nơi mua phù hợp. | Người mua hàng | [CẦN XÁC MINH: sản phẩm, nơi bán, thời gian so sánh và lần mua thực tế.] |

**Dùng AI:** Hỗ trợ diễn đạt Job Story và phân loại các vấn đề tôi đã chọn.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | #6 — Developer mất thời gian đọc PR lớn để hiểu thay đổi và xác định rủi ro | Phạm vi một lượt review; có thể đối chiếu nhận xét với diff và mã nguồn. | PR lớn đến mức nào? Thời gian tập trung ở bước nào? Chia nhỏ PR đã đủ chưa? |
| 2 | #12 — Nhân viên nhập lại thông tin khách hàng trên nhiều biểu mẫu | Có thể theo dõi trường nhập lặp và thời gian xử lý từng hồ sơ. | Biểu mẫu nào bắt buộc nhập riêng? Đã có lỗi nhập liệu hay chưa? |
| 3 | #19 — Người thuê nhà kiểm tra điện, nước, dịch vụ và đối chiếu hợp đồng | Có thể xem xét từng khoản thu cùng điều khoản và chứng từ liên quan. | Người thuê có đủ dữ liệu không? Khó ở tính toán, tìm tài liệu hay chờ giải đáp? |

### Problem Card #1 — Vấn đề #6: Đọc Pull Request lớn

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần review một Pull Request lớn, tôi muốn hiểu các thay đổi và rủi ro liên quan, để đưa ra nhận xét có căn cứ. |
| Actor | Developer được giao review PR. [CẦN XÁC MINH: vai trò và mức độ quen codebase.] |
| Thời điểm / bối cảnh | Khi nhận PR có nhiều thay đổi cần đọc hiểu trước khi góp ý. [CẦN XÁC MINH: PR cụ thể và tiêu chí “lớn”.] |
| Quy trình hiện tại (3–7 bước) | 1. Đọc mô tả PR và yêu cầu liên quan · 2. Xem các file thay đổi · 3. Đọc diff · 4. Lần theo mã liên quan để hiểu tác động · 5. Đối chiếu với test và kết quả kiểm tra sẵn có · 6. Ghi nhận xét và câu hỏi cho tác giả. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 4, lần theo mã liên quan để hiểu ảnh hưởng của thay đổi. Thời gian: [CẦN ĐO]. |
| Impact (nếu không giải thì sao) | Có thể kéo dài lượt review hoặc bỏ sót rủi ro. [CẦN XÁC MINH: trường hợp thực tế và mức ảnh hưởng.] |
| Success metric (baseline → target) | Thời gian review: [CẦN ĐO: baseline, phút/PR] → [CẦN XÁC ĐỊNH: target, phút/PR]. Đo từ lúc bắt đầu đọc đến khi gửi nhận xét, trừ thời gian chờ. So sánh các PR tương đương về phạm vi và độ quen codebase; đối chiếu nhận xét với mã nguồn và test. [CẦN XÁC ĐỊNH: người kiểm tra và tiêu chí chất lượng.] |
| Phương án không dùng AI | Chia PR theo mục tiêu thay đổi, bổ sung mô tả và dùng checklist review. |
| Giả thuyết về AI (nếu có) | Tóm tắt thay đổi kèm vị trí mã và gợi ý phần liên quan cần xem. Reviewer kiểm lại mã nguồn trước khi nhận xét; chỉ dùng mã nguồn được phép chia sẻ. |
| Cảm nhận nhanh | Chưa biết. Cần thử chia nhỏ PR và cải thiện mô tả trước. |

Quy trình nháp:

~~~text
PHÁC THẢO — tổng thời gian: [CẦN ĐO]

[1 Đọc mô tả PR và yêu cầu liên quan: CẦN ĐO]
→ [2 Xem các file thay đổi: CẦN ĐO]
→ [3 Đọc diff: CẦN ĐO]
→ [4 Lần theo mã liên quan để hiểu tác động: CẦN ĐO] ← BOTTLENECK GIẢ THUYẾT
→ [5 Đối chiếu với test và kết quả kiểm tra: CẦN ĐO]
→ [6 Ghi nhận xét và câu hỏi cho tác giả: CẦN ĐO]
~~~

### Problem Card #2 — Vấn đề #12: Nhập lại thông tin khách hàng

| Trường | Nội dung |
|---|---|
| Job Story | Khi phải điền thông tin khách hàng vào nhiều biểu mẫu, tôi muốn nắm rõ thông tin cần nhập ở từng biểu mẫu, để hoàn tất hồ sơ mà không bỏ sót. |
| Actor | Nhân viên nhập thông tin khách hàng. [CẦN XÁC MINH: bộ phận, loại hồ sơ và quyền chỉnh sửa biểu mẫu.] |
| Thời điểm / bối cảnh | Khi tiếp nhận hoặc cập nhật hồ sơ có trường thông tin lặp giữa các biểu mẫu. [CẦN XÁC MINH: biểu mẫu, trường trùng và tần suất.] |
| Quy trình hiện tại (3–7 bước) | 1. Nhận thông tin khách hàng · 2. Xác định biểu mẫu cần điền · 3. Điền biểu mẫu đầu · 4. Nhập lại trường trùng vào biểu mẫu khác · 5. Đối chiếu thông tin · 6. Sửa lỗi nếu có và hoàn tất hồ sơ. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 4, nhập lại các trường trùng. Thời gian: [CẦN ĐO]. |
| Impact (nếu không giải thì sao) | Có thể tốn công nhập lặp và sửa thông tin không nhất quán. [CẦN XÁC MINH: lỗi thực tế, thời gian sửa và ảnh hưởng.] |
| Success metric (baseline → target) | Thời gian hoàn tất hồ sơ: [CẦN ĐO: baseline, phút/hồ sơ] → [CẦN XÁC ĐỊNH: target, phút/hồ sơ]. Đo trên cùng loại hồ sơ, ghi thời gian từng bước và số trường sai hoặc không nhất quán sau đối chiếu. [CẦN XÁC ĐỊNH: người kiểm tra và tiêu chí chất lượng.] |
| Phương án không dùng AI | Dùng nguồn thông tin chuẩn, thống nhất biểu mẫu hoặc chuyển dữ liệu theo quy tắc nếu được phép. |
| Giả thuyết về AI (nếu có) | Gợi ý ghép các trường có tên hoặc cách diễn đạt khác nhau khi quy tắc cố định không đủ. Nhân viên kiểm lại từng trường và chỉ dùng dữ liệu được phép chia sẻ. |
| Cảm nhận nhanh | Chưa biết. Cần kiểm tra khả năng chuẩn hóa biểu mẫu trước. |

Quy trình nháp:

~~~text
PHÁC THẢO — tổng thời gian: [CẦN ĐO]

[1 Nhận thông tin khách hàng: CẦN ĐO]
→ [2 Xác định biểu mẫu cần điền: CẦN ĐO]
→ [3 Điền biểu mẫu đầu: CẦN ĐO]
→ [4 Nhập lại trường trùng vào biểu mẫu khác: CẦN ĐO] ← BOTTLENECK GIẢ THUYẾT
→ [5 Đối chiếu thông tin: CẦN ĐO]
→ [6 Sửa lỗi nếu có và hoàn tất hồ sơ: CẦN ĐO]
~~~

### Problem Card #3 — Vấn đề #19: Đối chiếu chi phí thuê nhà

| Trường | Nội dung |
|---|---|
| Job Story | Khi kiểm tra các khoản điện, nước và dịch vụ, tôi muốn đối chiếu chúng với hợp đồng thuê nhà, để biết khoản phải trả có phù hợp không. |
| Actor | Người thuê nhà trực tiếp kiểm tra các khoản phải trả. [CẦN XÁC MINH: loại hình thuê, cách chia chi phí và người giữ hợp đồng.] |
| Thời điểm / bối cảnh | Khi nhận thông báo tiền điện, nước và dịch vụ trước khi thanh toán. [CẦN XÁC MINH: chu kỳ, thông báo và chứng từ nhận được.] |
| Quy trình hiện tại (3–7 bước) | 1. Nhận thông báo khoản thu · 2. Tìm hợp đồng và chứng từ · 3. Đọc điều khoản về đơn giá, cách tính · 4. Đối chiếu từng khoản · 5. Ghi khoản khớp và khoản thiếu căn cứ · 6. Hỏi bên thu tiền nếu cần làm rõ. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 4, đối chiếu từng khoản với điều khoản và dữ liệu tính tiền. Thời gian: [CẦN ĐO]. |
| Impact (nếu không giải thì sao) | Có thể mất thêm công kiểm tra và phải hỏi lại về các khoản chưa rõ. [CẦN XÁC MINH: tình huống thực tế, thời gian và ảnh hưởng.] |
| Success metric (baseline → target) | Thời gian kiểm tra một thông báo: [CẦN ĐO: baseline, phút/thông báo] → [CẦN XÁC ĐỊNH: target, phút/thông báo]. Ghi riêng thời gian chờ phản hồi; kiểm kết quả bằng hợp đồng và chứng từ, phân biệt khoản đã khớp với khoản còn thiếu căn cứ. [CẦN XÁC ĐỊNH: người kiểm tra và tiêu chí chất lượng.] |
| Phương án không dùng AI | Lập bảng đối chiếu khoản thu với điều khoản và chứng từ; tính lại theo công thức, hỏi bên thu tiền khi thiếu dữ liệu. |
| Giả thuyết về AI (nếu có) | Hỗ trợ tìm điều khoản liên quan trong hợp đồng. Người thuê kiểm lại bản gốc và phép tính. |
| Cảm nhận nhanh | Chưa biết. Cần thử bảng đối chiếu và xác định dữ liệu còn thiếu trước. |

Quy trình nháp:

~~~text
PHÁC THẢO — tổng thời gian: [CẦN ĐO]

[1 Nhận thông báo khoản thu: CẦN ĐO]
→ [2 Tìm hợp đồng và chứng từ: CẦN ĐO]
→ [3 Đọc điều khoản về đơn giá, cách tính: CẦN ĐO]
→ [4 Đối chiếu từng khoản: CẦN ĐO] ← BOTTLENECK GIẢ THUYẾT
→ [5 Ghi khoản khớp và khoản thiếu căn cứ: CẦN ĐO]
→ [6 Hỏi bên thu tiền nếu cần làm rõ: CẦN ĐO]
~~~

### Card muốn pitch nhất

- Card số: 1 — vấn đề #6.
- Vì sao: Có thể giới hạn vào một lượt review PR và xem cụ thể bước đọc hiểu nào gây chậm.
- Câu hỏi muốn nhóm phản biện: Nếu chia PR nhỏ hơn và mô tả rõ hơn, reviewer còn khó xác định rủi ro ở bước nào?

### AI đã phản biện card thế nào

#### Phản biện Card #1 — Đọc Pull Request lớn

| Điểm yếu | Vì sao là điểm yếu | Câu hỏi cần xác minh |
|---|---|---|
| Actor còn rộng | Người mới vào dự án và người quen module có thể vướng ở các bước khác nhau. | Reviewer gặp khó là ai, quen phần code đó đến đâu và phụ trách kiểm tra gì? |
| Chưa rõ “PR lớn” và bước nghẽn | Số dòng hoặc số file chưa đủ thể hiện độ khó; thời gian từng bước chưa được đo. | PR cụ thể khó ở đâu và reviewer mất nhiều thời gian nhất ở bước nào? |
| Thiếu trường hợp thực tế | Chưa có PR hoặc lịch sử nhận xét cho thấy thời gian tăng thêm hay rủi ro bị bỏ sót. | Lần review nào phải đọc lại, hỏi thêm ngữ cảnh hoặc bỏ sót rủi ro? |
| Metric chưa có baseline và tiêu chí chất lượng | Review nhanh hơn chưa chắc nhận xét tốt hơn; thời gian chờ cũng làm lệch so sánh. | Đo trên các PR nào, trừ thời gian chờ ra sao và ai kiểm chất lượng nhận xét? |
| Chưa so sánh với cách cải thiện PR | Chia nhỏ thay đổi, mô tả rõ và checklist có thể đã giảm được công đọc hiểu. | Sau khi thử những cách này, phần khó nào còn lại? |

#### Phản biện Card #2 — Nhập lại thông tin khách hàng

| Điểm yếu | Vì sao là điểm yếu | Câu hỏi cần xác minh |
|---|---|---|
| Chưa rõ vai trò và quyền xử lý | Người nhập liệu có thể không được sửa biểu mẫu hoặc chuyển dữ liệu. | Ai nhập, ai quản lý biểu mẫu và được phép thay đổi những gì? |
| Chưa xác nhận nhập lặp là bước nghẽn | Hồ sơ có thể chậm vì thiếu thông tin, chờ duyệt hoặc sửa dữ liệu nguồn. | Thời gian nhập lại so với các bước còn lại là bao nhiêu? |
| Thiếu hồ sơ minh họa | Chưa rõ trường trùng có cùng ý nghĩa hay bắt buộc nhập riêng. | Hồ sơ nào cho thấy trường bị nhập lặp hoặc có lỗi? Có thể dùng bản đã che thông tin cá nhân không? |
| Metric chưa kiểm soát độ phức tạp hồ sơ | Các loại hồ sơ khác nhau khó so trực tiếp; cần theo dõi cả lỗi sau nhập. | Đo trên loại hồ sơ nào và kiểm trường sai hoặc không nhất quán bằng cách nào? |
| Chưa loại trừ phương án dùng quy tắc | Nếu cấu trúc ổn định, ánh xạ trường cố định có thể đủ. | Vì sao nguồn chuẩn, biểu mẫu chung hoặc quy tắc chuyển dữ liệu chưa đáp ứng được? |

#### Phản biện Card #3 — Đối chiếu chi phí thuê nhà

| Điểm yếu | Vì sao là điểm yếu | Câu hỏi cần xác minh |
|---|---|---|
| Chưa rõ điều kiện của người thuê | Ở riêng, ở ghép và không giữ hợp đồng dẫn đến cách kiểm tiền khác nhau. | Ai kiểm tiền, giữ tài liệu gì và có phải chia chi phí không? |
| Chưa tách thời gian đối chiếu khỏi thời gian chờ | Thiếu chứng từ có thể khiến người thuê phải chờ, dù thao tác tính toán không khó. | Lần gần nhất chậm ở tìm tài liệu, tính toán hay chờ bổ sung dữ liệu? |
| Thiếu khoản thu cụ thể để kiểm tra | Chưa có trường hợp cho thấy khoản nào khó kiểm và ảnh hưởng ra sao. | Khoản nào từng phải hỏi lại, có chứng từ gì và kết quả làm rõ thế nào? |
| Metric chưa rõ điểm kết thúc | Kiểm xong phần dữ liệu sẵn có khác với giải đáp xong mọi khoản. | Khi nào coi là kiểm xong và dùng nguồn nào xác nhận kết quả? |
| Chưa so sánh với bảng đối chiếu thông thường | Điều khoản ngắn và công thức rõ có thể chỉ cần bảng tính; AI không bổ sung được chứng từ bị thiếu. | Sau khi dùng bảng đối chiếu, phần nào vẫn cần hỗ trợ đọc hiểu? |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
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
| CP1 Scan | AI diễn đạt lại các vấn đề tôi đã chọn thành Job Story và phân loại lăng kính | | | |
| CP2 Problem Card | AI phác thảo card, quy trình và phản biện để tôi kiểm tra | | | |
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
