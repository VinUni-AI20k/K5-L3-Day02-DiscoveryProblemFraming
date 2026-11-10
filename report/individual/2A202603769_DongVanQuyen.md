# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đồng Văn Quyến
- MSSV: 2A202603769
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: d3
- Link repo nhóm: https://github.com/congnt180263/K5-L3B-Day02-D3-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi vừa meeting với team xong, tôi muốn có 1 bản báo cáo các vấn đề đã họp, cách giải quyết, công việc cần làm và hạn chót để không ai bỏ sót việc | team member | 30-40p/ buổi, 2 buổi/tuần  |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi cần biết vì sao lại chọn phương án A, tôi cần phải đọc nhiều tài liệu liên quan, hỏi nhiều người để có thể nắm bắt được thông tin | team member | 10-20 phút /mail, 5 lần/tuần |
| 3 | Pain từ người khác | Khách hàng gửi cùng 1 loại câu hỏi về đơn hàng/ dịch vụ qua nhiều kênh tới cskh, họ cần được trả lời nhanh chóng, chính xác, nhất quán | khách hàng, cskh | khoảng 40% ticket/tuần là câu hỏi trùng, phản hồi trung bình 4 giờ |
| 4 | Cần tổng hợp nhiều thông tin | Khi làm bài lab, tôi cần tổng hợp nhiều file, nắm rõ các rule, yêu cầu, quy tắc chấm điểm để đạt được kết quả tốt nhất | Học viên | 2 lần / ngày,  5 ngày / tuần |
| 5 | Pain từ người khác · Cần đọc, tổng hợp nhiều thông tin · Lặp lại | Khi nhận bàn giao ca trực của bệnh nhân, bác sĩ cần phải nắm được tình hình sức khỏe, kết quản đang chờ, các công việc còn tồn đọng để đảm bảo sức khỏe bệnh nhân, không bỏ sót công việc | Bác sĩ, điều dưỡng | Bàn giao mất 15–45 phút/lần, 2–3 lần/ngày |
| 6 | Tốn thời gian | Khi cả nhóm cần chốt lịch họp ngoài giờ, tôi muốn tìm được khung giờ mọi người đều rảnh, để không phải nhắn qua lại nhiều lần | Team member |15–20 tin nhắn qua lại/lần chốt lịch, 2 lần/tuần |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- bỏ ý chốt lịch họp ngoài giờ, vì đây là pain nhỏ, gg calendar đã có thể giải quyết được

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Báo cáo sau meeting | Đây là 1 quy trình lặp lại hàng tuần, và cũng quan trọng để có thể kịp tiến độ hoàn thành công việc của team | Biên bản "đủ tốt" đo thế nào, có cần rv lại báo cáo không |
| 2 | Bàn giao ca trực | Vấn đề lớn ảnh hưởng tới sức khỏe của bệnh nhân | Chỉ research trên internet nên chưa thể nắm rõ quy trình |
| 3 | Trả lời CSKH | Quy trình rõ ràng, đa số câu hỏi trùng lặp, đã có sẵn kịch bản trả lời | Đã có nhiều công cụ như chatbot trả lời tự động phục vụ việc giải quyết những vấn đề đơn giản |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa họp team xong, tôi muốn có bản tóm tắt các vấn đề đã bàn, cách giải quyết, việc cần làm, người phụ trách và hạn chót, để không ai bỏ sót việc |
| Actor | Người phụ trách ghi biên bản, team member |
| Thời điểm / bối cảnh | ngay sau buổi họp |
| Quy trình hiện tại (3–7 bước) | 1. Ghi chú tay trong lúc họp · 2. Nghe lại ghi âm hoặc hỏi lại người khác chỗ chưa rõ · 3. Viết lại biên bản (vấn đề, quyết định) · 4. Tách danh sách việc cần làm, gán người và hạn · 5. Gửi lên group/email · 6. Nhắc lại việc khi gần tới hạn |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: viết lại và tách việc mất khoảng 20 phút/buổi, dễ ghi nhầm người phụ trách hoặc thiếu hạn chót |
| Impact (nếu không giải thì sao) | 30–40 phút/buổi × 2 buổi/tuần ≈ 70 phút/tuần cho 1 người; việc bị quên phải bàn lại ở buổi sau |
| Success metric (baseline → target) | Thời gian làm biên bản giảm xuống còn 10p/ lần, phân việc đúng người, deadline được báo trước 2 ngày, số việc bị quên gần bằng 0 |
| Phương án không dùng AI | teamplate biên bản cố định  |
| Giả thuyết về AI (nếu có) | sử dụng stt và ai tự tổng hợp sau đó điền vào form các nội dung, danh sách việc, người thư ký review và chốt biên bản trước khi gửi |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |  Workflow

Quy trình nháp hiện tại: HIỆN TẠI — khoảng 35 phút/buổi

[1 Ghi chú trong họp: (trong giờ họp)] → [2 Nghe lại/hỏi lại: 8']
→ [3 Viết lại biên bản: 12'] → [4 Tách việc + gán người/hạn: 8'] ← BOTTLENECK (3+4 = 20')
→ [5 Format + gửi group: 5'] → [6 Nhắc việc khi tới hạn: 2']

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận bàn giao ca trực, cần nắm đầy đủ diễn biến sức khỏe, thuốc đã dùng, chỉ định đang thực hiện, kết quả đang chờ và việc còn tồn của từng bệnh nhân, để chăm sóc tiếp chính xác và không bỏ sót việc của ca trước |
| Actor | điều dưỡng, bác sĩ |
| Thời điểm / bối cảnh | Giờ giao ca (khoảng 6h30–7h30 và 16h–17h) |
| Quy trình hiện tại (3–7 bước) | 	1. Ca giao ghi sổ bàn giao/hồ sơ · 2. Bàn giao miệng tại phòng trực · 3. Ca nhận đọc lại hồ sơ, y lệnh, kết quả xét nghiệm · 4. Đi buồng kiểm tra bệnh nhân · 5. Gọi/nhắn hỏi lại ca trước chỗ thiếu · 6. Ký nhận bàn giao |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: đọc và đối chiếu hồ sơ, y lệnh, kết quả đang chờ từ nhiều nguồn, khoảng 15–20 phút; hay sót kết quả đang chờ và thay đổi thuốc |
| Impact (nếu không giải thì sao) | 15–45 phút/lần, 2–3 lần/ngày, mọi điều dưỡng đều làm; khoảng 80% sai sót y khoa nghiêm trọng liên quan đến trao đổi thông tin khi bàn giao |
| Success metric (baseline → target) | Số lần phải hỏi lại ca trước/ca giảm, số việc bị đo sót giảm|
| Phương án không dùng AI |Áp dụng bảng kiểm SBAR/I-PASS giấy + bàn giao tại giường. |
| Giả thuyết về AI (nếu có) | AI tóm tắt hồ sơ điện tử của từng bệnh nhân thành mẫu SBAR, đánh dấu kết quả đang chờ và việc tồn; điều dưỡng kiểm tra lại tại giường |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết | Rule

Quy trình nháp hiện tại:
HIỆN TẠI — khoảng 40 phút/lần giao ca (18 bệnh nhân)

[1 Ca giao ghi sổ: 8'] → [2 Bàn giao miệng: 10']
→ [3 Đọc hồ sơ, y lệnh, kết quả chờ: 15'] ← BOTTLENECK
→ [4 Đi buồng kiểm tra: (song song/sau giao ca)] → [5 Hỏi lại ca trước: 5'] → [6 Ký nhận: 2']

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story |	Khi khách hàng gửi cùng một loại câu hỏi về đơn hàng/dịch vụ qua nhiều kênh, họ muốn được trả lời nhanh, chính xác và nhất quán, để không phải hỏi lại hoặc chờ lâu |
| Actor | Nhân viên cskh |
| Thời điểm / bối cảnh | Suốt giờ làm việc, cao điểm khi có đợt sale |
| Quy trình hiện tại (3–7 bước) | 1. Nhận tin nhắn từ nhiều kênh · 2. Đọc và phân loại câu hỏi · 3. Tra cứu đơn hàng trên hệ thống · 4. Tìm câu trả lời mẫu · 5. Soạn và gửi trả lời · 6. Đóng ticket |
| Bottleneck (bước nào, mất bao nhiêu phút) | 	Bước 3–4: tra đơn và tìm câu trả lời đúng chính sách mất khoảng 5–7 phút/ticket, dù 40% là câu hỏi trùng |
| Impact (nếu không giải thì sao) | Khoảng 40% ticket/tuần là câu hỏi trùng; phản hồi trung bình 4 giờ; khách hỏi lại qua kênh khác làm tăng số ticket |
| Success metric (baseline → target) | Thời gian phản hồi trung bình từ 4 giờ xuống dưới 1 giờ với nhóm câu hỏi trùng; tỉ lệ khách hỏi lại giảm |
| Phương án không dùng AI | Bộ câu trả lời mẫu (FAQ/macro) theo 10 loại câu hỏi hay gặp + trang tra cứu đơn hàng cho khách tự xem |
| Giả thuyết về AI (nếu có) | AI phân loại câu hỏi và soạn nháp trả lời từ dữ liệu đơn hàng + chính sách; nhân viên duyệt trước khi gửi |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết | Rule

Quy trình nháp hiện tại:
HIỆN TẠI — khoảng 10 phút/ticket (chưa tính thời gian chờ trong hàng đợi)

[1 Nhận tin nhiều kênh: 1'] → [2 Đọc + phân loại: 1']
→ [3 Tra cứu đơn hàng: 3'] → [4 Tìm câu trả lời/hỏi trưởng nhóm: 3'] ← BOTTLENECK (3+4 = 6')
→ [5 Soạn + gửi: 2'] → [6 Đóng ticket: 0,5']

```text

```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Công việc hàng ngày đểu cần họp mặt với team để có thể cập nhật tiến độ dự án, hoàn thành công việc dự án theo tiến độ

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Hiện tại, các công cụ có sẵn trên thị trường đều đã đáp ứng tốt về vấn đề ghi lại cuộc họp +  phân task | Có | Bỏ bài toán này |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | đưa ra 3 top idea để nhóm nhận định, góp ý, nhận được ý kiến về mức độ cạnh tranh của các existing solution hiện tại so với idea của mình| Có mức đóng góp tốt, đặc biệt là idea chuyển giao ca giữa các điều dưỡng trong bệnh viện  |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | về luật pháp, không cho phép sử dụng tai nghe khi lái xe?, Nếu dùng LLM để kiểm tra thông tin kết quả của output của AI local của doanh nghiệp thì có thể rủi ro bảo mật, Rủi ro về kinh tế khi thông tin và đối chiếu của AI sai lệch mà không được confirm lại  |
| Nhận phản biện | Câu hỏi tôi nhận được: Khả năng cạnh tranh thị trường với các hệ sinh thái lớn rất khó? | Tôi đã sửa gì: quyết định bỏ qua idea làm agent tổng hợp công việc sau cuộc họp |
| Gom cluster / cây OST | | |
| Chọn candidate problem | Đóng góp idea vào pitching + phản biện | Cùng team đưa ra được idea khả thi nhất |
| Kiểm chứng / research | TÌm kiếm các công cụ hiện tại trên thị trường, điểm mạnh, điểm yếu và kiểm chứng các link trả về | Đưa ra được các bằng chứng cụ thể |


---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Scan các idea về những lĩnh vực chưa tham gia vào quá trình nghiệp vụ(bệnh viện) | AI mở rộng bài toán tới các bài toán chưa rõ nghiệp vụ | Gợi ý bài toán "chốt lịch họp" quá nhỏ và hời hợt, không có giá trị xây dựng giải pháp riêng. |  bổ sung dữ liệu thực tế qua research|
| CP2 Problem Card | Đóng vai PM phản biện card tóm tắt họp (#1) và giao ca bệnh viện (#2). | Cảnh báo tính cạnh tranh khốc liệt với các ông lớn (Teams, Zoom, Otter) ở card họp và rủi ro trách nhiệm pháp lý ở card y tế. | AI gợi ý giải pháp Agent tự động tham gia họp và tự giao việc luôn cho thành viên (vượt quá nhu cầu, dễ gây phiền toái). | Giữ ranh giới chỉ làm bản nháp to-do list để con người chốt; sau đó quyết định bỏ card họp để chọn bài toán đối chiếu hóa đơn có ground-truth rõ hơn. |
| CP4 Research | Tìm kiếm các công cụ và pattern đã giải quyết bài toán đối chiếu hóa đơn 3 bên trên thị trường. | Tìm ra các case study rất sát như Bizzi.vn, Rossum.ai và kiến trúc mẫu AWS Textract Invoice Processing. | AI trả về 2 link 404 bị chết (akaBot và n8n category link); mô tả các tool thương mại như thể đã tự động hóa 100% không cần người. | Tự mở từng link kiểm tra và loại bỏ link chết |
| CP5 Quy trình | Chuyển luồng nghiệp vụ 5 bước của nhóm thành cú pháp sơ đồ Mermaid. | Tạo cú pháp Mermaid nhanh, màu sắc phân biệt rõ các nhánh khớp 100% và nhánh ngoại lệ lệch số liệu. | AI hay tự ý gộp bước "đối chiếu số học" và "soạn nháp giải trình" làm một, làm lu mờ điểm nghẽn chính. | Tách riêng Bước 3 (Rule so khớp toán học) và Bước 4 (AI soạn nháp giải trình), bổ sung thời gian đo đếm cụ thể cho từng bước. |
| CP5–6 Problem Statement | Rà soát lỗ hổng trong 6 trường của Problem Statement v0. | Chỉ ra điểm yếu: metric "chính xác 95%" là quá nguy hiểm với tiền bạc (lọt 5% lỗi thanh toán có thể gây thất thoát lớn). | AI gợi ý metric mơ hồ như "nâng cao trải nghiệm kế toán viên" hoặc "tự động hóa hoàn toàn luồng duyệt". | Nhóm tiếp thu phản biện của AI để tách metric thành: (1) Tốc độ thao tác con người, (2) Tỷ lệ bắt lỗi 100% bằng Rule số học, và siết chặt Boundary cấm AI tự ý duyệt chi. |
| CP6 Mức can thiệp / quyết định | Brainstorm định vị ma trận 2×2 và so sánh 4 mức (No AI, Rule, Workflow, Agent). | Phân tích rõ vì sao bài toán thuộc ô "Độ mơ hồ thấp × Độ phức tạp cao" và chỉ ra rủi ro nghiêm trọng nếu dùng Agent. | AI có xu hướng thích "vẽ" ra Agent đa năng (tự chat với NCC, tự chuyển khoản ngân hàng) vì nghe hấp dẫn về mặt công nghệ. | Giữ vững lập trường chọn Workflow: dùng Rule cho phép tính số học, AI chỉ làm nhiệm vụ OCR đọc chứng từ khó và soạn nháp, Kế toán trưởng giữ quyền duyệt chi cuối cùng. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5).

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi nghe bạn nguyên phân tích về problem 4, tôi nhận ra các bottle neck bạn ghi đều có số liệu cụ thể, thay vì chỉ ghi chung chung, bạn ấy đã đưa ra số liệu cụ thể (chấm 100 cặp câu trả lời, khoảng 90 phút/người/lần (cả quy trình khoảng 150 phút, 2 lần/tuần)), từ đó rút ra bài học 1 problem card tốt không thể chung chung mơ hồ mà cần có số liệu cụ thể và bằng chứng đo đếm được

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Ở giai đoạn pitching, tôi đề xuất 1 agent có thể tự động ghi âm cuộc họp và đièn task cho từng người theo phân công khi chưa thực sự hiểu rõ về các vấn đề và những công cụ hiện tại đã có thể làm tốt problem này, vì vậy khi nhận câu hỏi phản biện, tôi cùng cả nhóm đã quay trở lại phân tích quy trình, nhận diện rõ đâu là bottle neck thật sự trước khi đề xuất công nghệ

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đã đổi ý hoàn toàn sau phiên phản biện ở CP3. Ban đầu, tôi rất tâm huyết với Card #1 (Báo cáo sau meeting) và Card #2 (Bàn giao ca trực y tế). Tuy nhiên, khi nhóm phản biện rằng bài toán tóm tắt cuộc họp đã bị các hệ sinh thái lớn (Zoom, Teams) độc chiếm và rất khó đo lường thế nào là tóm tắt "đúng", đồng thời bài toán bệnh viện tiềm ẩn rủi ro an toàn sinh mạng và bảo mật dữ liệu không thể tiếp cận được  tôi đã bị thuyết phục. Tôi đồng thuận từ bỏ 2 ý tưởng của mình để cùng nhóm chọn Candidate #8 của Công (Đối chiếu hóa đơn 3 bên) vì nó có ground-truth số học 100% rõ ràng và khả thi hơn rất nhiều.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Ở giai đoạn research, ban đầu tôi vẫn nghĩ các công cụ kế toán hàng đầu đã sử dụng AI là 1 công cụ chính trong việc kiểm soát số tiền hay tự động chuyển khoản, nhưng sau khi tham khảo các link trên internet, tôi đã nhận ra mình nhầm: họ tách biệt hoàn toàn AI chỉ làm OCR đọc chứng từ phi câu trúc thành JSOM, còn khâu khớp số tiền bắt buộc phải chạy bằng rule , cuối cùng phải có con người chịu trách nhiệm duyệt chi cuối cùng

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khi viết Problem Statement điều khó nhất là xác định boundary và success metric. Với boundary: nhóm đã phải tranh luận để biến nó thành ranh giới kỹ thuật cụ thể. Ngoài ra, metric cần phải cụ thể, đo lường được

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ phản biện nhóm quyết liệt hơn ngay từ đầu để không sa vào bẫy "thần thánh hóa AI". Tôi sẽ chặn ngay các ý tưởng đòi để AI tự động chuyển tiền hay tự tính toán số học, vì trong kế toán, sai lệch một con số nhỏ cũng có thể gây thất thoát tiền bạc rất lớn. 

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Problem của nhóm là nhân viên kế toán công nợ mất từ 3.0–4.5 phút/bộ chỉ để dò mắt đối chiếu từng dòng hàng giữa 3 chứng từ khác nhau. Quy trình để giải quyết vấn đề gồm 5 bước tuần tự: Rule gom chứng từ, AI đọc phiếu giao nhận sang JSON, rule khớp số 3 bên, AI hỗ trợ tìm kiếm chỉ ra dòng lệch, và cuối cùng là con người kiểm tra. Metric là đo lường được thời gian thao tác của kế toán kho sẽ giảm xuống dưới 2 phút, đạt tỷ lệ tìm kiếm sai lệch hơn 95%  trên bộ test. Boundary là AI không được phép tự tính toán số tiền, tự động chuyển khoản, kế toán là điểm cuối trước khi hạch toán. Về mức can thiệp AI, đây sẽ là ở mức workflow, không chọn agent vì rủi ro thất thoát tài chính. Quyết định bài toán là go 
---

## 7. Tài liệu tham khảo

-
https://aws.amazon.com/textract/
https://github.com/aws-samples/amazon-textract-invoice-processor
https://meinvoice.vn/
https://rossum.ai/solutions/accounts-payable/