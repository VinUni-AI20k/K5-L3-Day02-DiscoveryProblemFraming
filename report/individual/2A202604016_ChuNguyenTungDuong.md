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
| Pitch Problem Card | Chuẩn bị ba card #6, #12, #19, ưu tiên card đọc PR lớn; thảo luận và đối chiếu các phương án với tất cả thành viên. | Sau thảo luận, chọn shortlist ba vấn đề và đề tài tìm lại bằng chứng từ paper. |
| Phản biện bài của bạn khác | Tham gia thảo luận và đối chiếu các đề tài cùng các thành viên. | Chưa bổ sung câu hỏi phản biện cụ thể tôi đã đặt. |
| Nhận phản biện | AI chỉ ra actor còn rộng, chưa rõ tiêu chí “PR lớn”, thiếu baseline và chưa so sánh với chia nhỏ PR. Phản biện trực tiếp từ thành viên khác chưa được bổ sung. | Card #6 giữ bước nghẽn ở trạng thái giả thuyết, có cách đo và phương án chia nhỏ PR, cải thiện mô tả trước khi cân nhắc AI. |
| Gom cluster / cây OST | Nhờ AI đọc CP1–CP2 của cả bốn thành viên, tổng hợp candidate có nguồn và chuẩn bị cluster, OST để review qua PR. Sau khi có shortlist, yêu cầu chuyển phạm vi OST sang tìm lại bằng chứng từ paper. | Có bảng truy vết 12 candidate, đề xuất năm cluster và OST cho problem paper trong CP3. Phân nhóm sơ bộ vẫn cần nhóm xác nhận. |
| Chọn candidate problem | Cùng các thành viên thảo luận, đối chiếu rồi chọn top 3 và đề tài “Tìm lại bằng chứng từ paper”; yêu cầu tổng hợp CP3 theo hướng này. | Bản tổng hợp giữ điểm shortlist 33/30/25, có lý do chọn L1 và lý do chưa chọn hai candidate còn lại. |
| Kiểm chứng / research | Nhờ AI research Zotero, Elicit và pattern RAG để chuẩn bị slide. Chưa có thông tin về việc tôi trực tiếp phỏng vấn hoặc chạy pilot. | Các nguồn được đưa vào notes và phụ lục slide. Research công cụ được tách khỏi bằng chứng về pain và kết quả thực nghiệm. |
| Quy trình nhóm | Yêu cầu chuyển bảng quy trình trên slide thành flowchart: quy trình hiện tại, phương án ghi chú có nguồn/Zotero và nhánh AI tùy chọn. | Slide v3 có bước người học mở PDF kiểm ngữ cảnh, fallback tìm thủ công khi liên kết thiếu hoặc sai, cùng boundary về nguồn và trích dẫn. |
| Problem Statement | Nhờ AI chuẩn bị nội dung CP5 cho slide, sau đó yêu cầu đối chiếu card gốc, shortlist và báo cáo nhóm để không dùng thời gian giả định làm baseline. | Slide nêu actor, bước nghẽn, impact giả thuyết và cách đo. Nội dung này chưa thay cho Problem Statement v0/v1 do nhóm tự chốt. |
| Mức can thiệp AI | Yêu cầu làm rõ phương án No AI First và so sánh với Rule, Workflow, Agent. | Phương án trên slide ưu tiên ghi chú có cấu trúc và Zotero; chỉ cân nhắc mức cao hơn nếu cách đơn giản chưa đủ. Nhánh Workflow được ghi là tùy chọn, chưa triển khai. |
| Quyết định | Yêu cầu giữ “Not Yet — Chưa đủ bằng chứng để triển khai AI” ở trạng thái đề xuất phân tích và chuẩn bị câu hỏi đáp. | Slide có bốn rủi ro, bước thử tiếp và ngưỡng dừng. Chưa ghi đây là quyết định cuối đã được cả nhóm xác nhận. |

Bằng chứng phần chuẩn bị chung: [PR #6 — cluster và OST](https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming/pull/6), [PR #8 — slide và tổng hợp CP3](https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming/pull/8). Bản slide chỉnh tiếp là `nhom6-paper-evidence-6min-v3.pptx`, hiện xuất riêng ngoài Git.

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI diễn đạt lại 10 vấn đề tôi đã chọn thành Job Story và phân loại bốn lăng kính. | Giữ mã vấn đề để đối chiếu, làm rõ actor và tách mô tả pain khỏi giải pháp. | AI không có dữ liệu trải nghiệm để xác nhận thời gian, tần suất hoặc mức ảnh hưởng. | Giữ các ký hiệu cần xác minh và cần đo; không dùng phần diễn đạt lại làm bằng chứng thực tế. |
| CP2 Problem Card | Nhờ AI phác thảo ba card, quy trình và phản biện dưới góc nhìn PM khó tính. | Làm rõ bước nghẽn, cách đo, phương án không dùng AI và câu hỏi cần xác minh cho từng card. | Actor, bước nghẽn và thời gian chưa được kiểm qua tình huống cụ thể. Một số chú thích và cách diễn đạt ban đầu dài, thiếu tự nhiên. | Đổi ưu tiên từ vấn đề #1 sang #6, giữ #12 và #19; yêu cầu viết theo ví dụ của lab, rút gọn lời chú thích và giữ nhãn giả thuyết. |
| CP4 Research | Nhờ AI tổng hợp tài liệu về Zotero, Elicit và RAG cho slide problem paper. | Có nguồn tham khảo và đối chiếu khả năng đã có với phương án ghi chú có nguồn. | Khả năng công cụ không chứng minh pain phổ biến hoặc giải pháp hiệu quả với người dùng của nhóm. Shortlist gọi mốc thời gian là baseline trong khi card gốc ghi là giả định. | Yêu cầu đối chiếu tài liệu, không dùng số giả định làm baseline và không tạo kết quả phỏng vấn hoặc pilot. |
| CP5 Quy trình | Nhờ AI phác thảo quy trình trước/sau và dựng sơ đồ trên slide. | Thể hiện điểm nghẽn giả thuyết, bước con người kiểm ngữ cảnh và phương án quay về tìm thủ công. | Bản slide đầu dùng bảng nhiều chữ, chưa thể hiện luồng xử lý rõ. Quy trình vẫn chưa đối chiếu với quan sát thực tế. | Yêu cầu thay bằng flowchart có mũi tên, nhấn bước người học xác minh và ghi rõ nhánh AI chưa triển khai. |
| CP5–6 Problem Statement | Nhờ AI soạn nội dung đề xuất cho slide, gồm actor, pain, metric và boundary. | Kết nối problem với quy trình, cách đo thời gian và kiểm chất lượng bằng chứng. | AI đã hỗ trợ soạn nội dung, không chỉ phản biện. Mục tiêu giảm 30% và quy mô pilot 10 yêu cầu/3 paper chưa có dữ liệu để xác nhận. | Yêu cầu phân biệt baseline chưa đo với target đề xuất; giữ CP4–CP6 trong báo cáo nhóm để thành viên hoàn thiện và tự chốt. |
| CP6 Mức can thiệp / quyết định | Nhờ AI so sánh No AI/Rule/Workflow/Agent, phân tích bốn rủi ro và chuẩn bị Q&A. | Làm rõ lý do thử No AI trước, boundary về trích dẫn và điều kiện chỉ thử Workflow khi mức đơn giản chưa đủ. | Mức rủi ro và đề xuất Not Yet chưa phải kết quả kiểm chứng hay quyết định được nhóm xác nhận. | Yêu cầu ghi rõ trạng thái đề xuất, không trình bày như đang xây AI Agent hoặc đã đạt target. Chưa chốt Go cho triển khai AI. |
| CP7 Biên tập | Cung cấp các ý trả lời về trải nghiệm của mình, nhờ AI sắp xếp và sửa câu chữ. | Tổ chức các ý về làm việc nhóm, tính khả thi, việc nghĩ đến hệ thống trích dẫn trước, thông tin về Zotero và kế hoạch đo hiệu quả. | AI không biết những việc ngoài thông tin tôi cung cấp, như câu hỏi phản biện cụ thể hoặc kết quả phỏng vấn. | Bổ sung trực tiếp những gì mình đã làm và suy nghĩ; không tạo thêm cuộc phỏng vấn, kết quả pilot hoặc câu hỏi của thành viên khác. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Qua việc trao đổi với tất cả thành viên và đối chiếu các đề tài, tôi học thêm cách làm việc nhóm khi lựa chọn một vấn đề chung. Khi chọn top 3 và đề tài tìm lại bằng chứng trong paper, tôi chú ý đến tính khả thi của phương án.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có. Nhóm từng muốn làm một hệ thống trích dẫn ngay từ đầu, tức là đã nghĩ đến cách giải trước khi làm rõ bài toán. Sau phần thảo luận và đối chiếu các đề tài, nhóm chọn vấn đề tìm lại bằng chứng trong paper để tiếp tục xem xét.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Sau khi thảo luận và đối chiếu các phương án cùng các thành viên, tôi đồng ý chọn đề tài tìm lại bằng chứng trong paper.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Tôi có bất ngờ khi biết Zotero đã có liên kết quay lại PDF. Đây là khả năng của công cụ sẵn có liên quan trực tiếp đến đề tài nhóm chọn.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Tôi đã hiểu sự khác nhau giữa baseline thực đo và target đề xuất, cũng như lý do thử No AI trước. Phần khó nhất với tôi là diễn đạt lập luận bằng lời của mình.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi muốn nhóm lập kế hoạch rõ ràng để đo hiệu quả của từng cách tiếp cận. Tôi muốn việc so sánh các phương án được đưa thành một phần cụ thể trong kế hoạch làm việc của nhóm.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán nhóm chọn là sinh viên mất thời gian tìm lại bằng chứng trong paper đã đọc. Khó khăn còn nằm ở việc kiểm định nhận định bằng bằng chứng trong bài. Các vị trí trích dẫn cần được hệ thống hóa để thuận tiện khi tìm lại.

---

## 7. Tài liệu tham khảo

-
