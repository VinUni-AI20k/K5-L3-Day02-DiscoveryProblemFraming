# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:D3
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 |Đào Ngọc Hân |Khi xe Xanh SM tiến vào bán kính đón khách nhưng bị khuất tầm nhìn (sảnh tòa nhà, phân khu đô thị, ngõ đông), tài xế và khách đặt xe muốn báo hiệu xe sắp cập điểm và nhận diện chính xác vị trí đứng thực tế của nhau mà không phải vừa lái xe vừa bấm gọi điện mô tả qua lại, để đón khớp ngay lần đầu và lái xe an toàn |Tài xế XanhSM và Khách hàng |**Bước 2 (1.0 phút)** và **Bước 3 (1.5–2.0 phút)** — tổng cộng **2.5–3.5 phút/cuốc**: tài xế vừa lái xe vừa phải bấm gọi thủ công (gây phân tâm), sau đó hai bên mất thời gian mô tả điểm mốc bằng lời do bất đồng góc nhìn trên đường| Quyến hỏi: về luật pháp, không cho phép sử dụng tai nghe khi lái xe? |
| 2 |Đào Ngọc Hân |Khi mở lại nhóm chat Zalo/Discord học tập hoặc dự án sau vài giờ bận, tôi muốn nắm ngay các quyết định đã chốt, deadline và phần việc giao cho mình giữa hàng trăm tin nhắn rời rạc, để không bỏ sót đầu việc chung hoặc phải hỏi lại cả nhóm |Học viên / thành viên nhóm dự án (tham gia đồng thời 3–4 nhóm chat hoạt động liên tục) |**Bước 3 (10 phút/lần/nhóm):** Phải đọc lướt và ghép ngữ cảnh từ luồng hội thoại phi cấu trúc vì câu chốt thường viết tắt (*"Chốt phương án 2 như bạn A nói ở trên nhé"*), buộc phải lội ngược tìm tin nhắn gốc |Rủi ro khi AI tóm tắt nhầm thông tin thời gian cuộc họp |
| 3 |Đào Ngọc Hân |Khi chi tiêu sinh hoạt hằng ngày qua nhiều tài khoản ngân hàng, quét mã QR và ví điện tử, tôi muốn gom các giao dịch lẻ về đúng danh mục chi tiêu vào cuối tuần, để biết mình đang vượt hạn mức ở nhóm nào trước khi hết tháng |Sinh viên / người đi làm trẻ thanh toán không tiền mặt qua 1–2 tài khoản ngân hàng chính và 1 ví điện tử |**Bước 2 (12 phút)** và **Bước 3 (8 phút)** — tổng **20 phút/tuần**: phải nhớ lại ngữ cảnh giao dịch chuyển khoản QR chỉ hiện tên chủ tài khoản cá nhân và nhập tay từng khoản lẻ | Vấn đề về cho phép truy cập thông tin của ngân hàng |
| 4 |Lê Thành Nguyên |Khi team đổi phiên bản prompt, tôi muốn biết bản mới tốt hơn hay tệ hơn bản cũ, để báo mentor có nên đưa lên bản chạy thật không |AI intern (người chấm); mentor dùng kết quả	 |Bước 3: đọc, đối chiếu nguồn, chấm 100 cặp câu trả lời, khoảng 90 phút/người/lần (cả quy trình khoảng 150 phút, 2 lần/tuần) | Nếu dùng LLM để kiểm tra thông tin kết quả của output của AI local của doanh nghiệp thì có thể rủi ro bảo mật |
| 5 |Lê Thành Nguyên |Khi mentor hỏi "cấu hình nào cho kết quả tốt nhất tuần trước", tôi muốn tìm lại đúng tham số và kết quả của từng lần chạy, để trả lời ngay mà không phải chạy lại |Tôi (người chạy thí nghiệm). Mentor là người hỏi và dùng kết quả |Bước 3, mở từng log để đọc tham số và metric rồi chép tay: khoảng 15 phút/lần (thêm 30–60 phút máy chạy nếu rơi vào bước 4) | Chưa rõ về hướng ứng dụng AI vào xử lý bài toán |
| 6 |Lê Thành Nguyên |Khi một intern mới vào nhóm, bạn ấy muốn tự cài được môi trường và chạy được project mẫu ngay trong ngày đầu, để không phải chờ người khác hỗ trợ  |Intern mới (người gặp khó). Tôi và mentor là người bị hỏi lại  |Bước 3–4, cài thư viện và gỡ lỗi xung đột phiên bản: 60–120 phút mỗi người, cộng 10–15 phút của người trả lời cho mỗi câu hỏi  |Có thể áp dụng chatbot vào để tăng hiệu quả làm việc được không |
| 7 |Nguyễn Thành Công |Khi nhận được nhiều CV cho một vị trí tuyển dụng, tôi muốn đánh giá mức độ phù hợp của từng ứng viên với yêu cầu công việc, để rút ngắn thời gian sàng lọc và không bỏ sót ứng viên tiềm năng. |Nhân viên tuyển dụng |Bước 2–3 – Đọc CV và đối chiếu với yêu cầu tuyển dụng, khoảng 3–5 phút/CV (ước tính).  |Trong thời đại ngày nay, ứng viên dùng AI để viết CV thì có hỗ trợ sàng lọc được hay không |
| 8 |Nguyễn Thành Công |Khi nhận được hóa đơn từ nhà cung cấp, tôi muốn đối chiếu thông tin với đơn đặt hàng và biên bản giao nhận, để đảm bảo tính chính xác trước khi thanh toán. |Nhân viên kế toán công nợ |Bước 4 – Đối chiếu thông tin giữa 3 loại chứng từ, khoảng 3–7 phút/hóa đơn (ước tính).  |Rủi ro về kinh tế khi thông tin và đối chiếu của AI sai lệch mà không được confirm lại |
| 9 |Nguyễn Thành Công |Khi tiếp nhận yêu cầu đổi trả, hoàn tiền hoặc tra cứu đơn hàng, tôi muốn xác định chính xác nội dung và mức độ ưu tiên của từng yêu cầu, để chuyển đến đúng bộ phận và xử lý kịp thời. |Nhân viên chăm sóc khách hàng |Bước 2–3 – Hiểu nội dung yêu cầu và tra cứu thông tin liên quan, ước tính 3–6 phút/ticket. | |
| 10 |Đồng Văn Quyến |Khi khách hàng gửi cùng một loại câu hỏi về đơn hàng/dịch vụ qua nhiều kênh, họ muốn được trả lời nhanh, chính xác và nhất quán, để không phải hỏi lại hoặc chờ lâu |Người phụ trách ghi biên bản, team member |Bước 3–4: viết lại và tách việc mất khoảng 20 phút/buổi, dễ ghi nhầm người phụ trách hoặc thiếu hạn chót |  |
| 11 |Đồng Văn Quyến |Khi nhận bàn giao ca trực, cần nắm đầy đủ diễn biến sức khỏe, thuốc đã dùng, chỉ định đang thực hiện, kết quả đang chờ và việc còn tồn của từng bệnh nhân, để chăm sóc tiếp chính xác và không bỏ sót việc của ca trước |điều dưỡng, bác sĩ |Bước 3: đọc và đối chiếu hồ sơ, y lệnh, kết quả đang chờ từ nhiều nguồn, khoảng 15–20 phút; hay sót kết quả đang chờ và thay đổi thuốc | Việc thao tác với thông tin của bệnh nhân và hệ thống quản lý bệnh viện có khả thi không |
| 12 |Đồng Văn Quyến |Khi vừa họp team xong, tôi muốn có bản tóm tắt các vấn đề đã bàn, cách giải quyết, việc cần làm, người phụ trách và hạn chót, để không ai bỏ sót việc |Người phụ trách ghi biên bản, team member  |Bước 3–4: viết lại và tách việc mất khoảng 20 phút/buổi, dễ ghi nhầm người phụ trách hoặc thiếu hạn chót |Khả năng cạnh tranh thị trường với các hệ sinh thái lớn rất khó?|

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A — Tổng hợp & bàn giao từ luồng thông tin phân mảnh** | `#2` Lội tin nhắn nhóm chat Zalo/Discord bị trôi · `#12` Viết biên bản & tách việc sau họp team · `#11` Tổng hợp hồ sơ bàn giao ca trực y tế · `#3` Gom và phân loại giao dịch chi tiêu đa kênh | Thông tin quan trọng (quyết định, đầu việc, y lệnh, giao dịch) nằm rải rác hoặc phi cấu trúc qua nhiều luồng/ứng dụng; người làm phải đọc lại từ đầu để lọc nhiễu và tổng hợp tránh bỏ sót |
| **B — Đối chiếu đa nguồn & chấm/sàng lọc theo tiêu chí** | `#4` Đối chiếu nguồn & chấm 100 cặp output khi đổi prompt · `#5` Tra cứu tham số & metric từ nhiều file log thí nghiệm · `#7` Sàng lọc hàng trăm CV theo JD · `#8` Đối chiếu 3 bên (Hóa đơn – PO – Biên bản giao nhận) | Phải mở song song nhiều tài liệu/bản ghi để so khớp từng trường dữ liệu hoặc chấm điểm thủ công lặp đi lặp lại theo bộ tiêu chí chuẩn, tốn nhiều giờ công và dễ sót lỗi do mỏi mắt |
| **C — Tiếp nhận, phân luồng & giải đáp yêu cầu lặp lại** | `#9` Phân loại & xác định ưu tiên ticket đổi trả/hoàn tiền · `#10` Trả lời câu hỏi khách hàng trùng lặp đa kênh · `#6` Gỡ lỗi cài môi trường lặp lại cho intern mới ngày đầu | Người phụ trách (CSKH, mentor) liên tục bị ngắt quãng bởi các câu hỏi, ticket hoặc sự cố quen thuộc lặp đi lặp lại, mất thời gian phân loại thủ công và trả lời lại cùng một nội dung |
| **D — Phối hợp & định vị điểm đón thời gian thực ngoài hiện trường** | `#1` Tài xế Xanh SM và khách gọi điện báo xe đến & mô tả vị trí đón thực tế khi bị khuất tầm nhìn | Bất cân xứng thông tin vị trí thực tế giữa hai phía đang di chuyển ngoài đường (lệch ghim GPS / khuất tầm nhìn), buộc phải gọi điện mô tả điểm mốc bằng lời ngay lúc đang lái xe gây trễ chuyến và mất an toàn |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian người làm việc phải tự tổng hợp, đối chiếu và xử lý lặp lại thông tin bằng tay,
         mà không tăng tỷ lệ bỏ sót việc hoặc đánh giá sai
├── Opportunity A (Cluster A): Thông tin quan trọng nằm rải rác, phi cấu trúc ở nhiều luồng nên phải đọc lại từ đầu mới lọc ra được, dễ bỏ sót
│   ├── #2  Câu chốt, deadline, việc được giao chìm giữa hàng trăm tin nhắn; lội ngược tìm tin gốc khoảng 10 phút/lần/nhóm
│   ├── #12 Sau họp phải viết lại biên bản và tách việc, khoảng 20 phút/buổi, dễ ghi nhầm người phụ trách hoặc thiếu hạn chót
│   ├── #11 Khi nhận ca phải đọc, đối chiếu hồ sơ, y lệnh, kết quả đang chờ từ nhiều nguồn, 15–20 phút, hay sót thay đổi thuốc
│   └── #3  Giao dịch QR chỉ hiện tên người nhận, phải nhớ lại ngữ cảnh và nhập tay từng khoản, khoảng 20 phút/tuần
├── Opportunity B (Cluster B): Phải mở song song nhiều tài liệu hoặc bản ghi để so khớp, chấm thủ công theo tiêu chí, tốn giờ công và dễ sót lỗi
│   ├── #4  Mỗi lần đổi prompt phải đối chiếu nguồn và chấm tay 100 cặp câu trả lời, khoảng 150 phút/lần, 2 lần/tuần
│   ├── #5  Mở từng file log để chép tay tham số và metric, khoảng 15 phút/lần; mất log thì phải chạy lại
│   ├── #7  Đọc từng CV để so với yêu cầu công việc, khoảng 3–5 phút/CV
│   └── #8  Đối chiếu 3 chứng từ (hóa đơn, đơn đặt hàng, biên bản giao nhận), khoảng 3–7 phút/hóa đơn
└── Opportunity C (Cluster C): Người phụ trách liên tục bị ngắt quãng bởi câu hỏi, ticket, sự cố quen thuộc, phải phân loại và trả lời lại cùng một nội dung
    ├── #9  Phải hiểu nội dung, xác định mức ưu tiên từng yêu cầu đổi trả/hoàn tiền để chuyển đúng bộ phận, 3–6 phút/ticket
    ├── #10 Khách hỏi cùng một loại câu hỏi qua nhiều kênh, phải trả lời tay từng lần và khó giữ câu trả lời nhất quán
    └── #6  Intern mới gặp cùng các lỗi cài môi trường, mỗi người mất 60–120 phút, người hướng dẫn bị hỏi lại 10–15 phút/câu
```

Không đưa vào cây:

- **Cluster D (#1, đón khách khuất tầm nhìn):** pain về phối hợp vị trí theo thời gian thực giữa hai bên đang di chuyển ngoài đường, không phải tổng hợp, đối chiếu hay xử lý thông tin lặp lại, nên không phục vụ outcome trên. Nhóm giữ lại như một hướng riêng nếu muốn đổi outcome.

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ "AI tóm tắt nhóm chat" (#2): đây là tính năng. Pain thật là câu chốt, deadline bị chìm giữa hàng trăm tin nhắn.
- ✗ "Kết nối, truy cập dữ liệu ngân hàng để tự phân loại chi tiêu" (#3): đây là giải pháp. Pain thật là giao dịch QR thiếu ngữ cảnh, phải nhớ và nhập tay.
- ✗ "Dùng LLM để chấm, kiểm tra output của mô hình" (#4): đây là cách làm. Pain thật là chấm tay lâu và hai người chấm lệch nhau.
- ✗ "Chatbot hỗ trợ intern hoặc trả lời khách" (#6, #10): đây là công cụ. Pain thật là trả lời lặp lại cùng một câu hỏi.
- ✗ "AI sàng lọc CV" (#7): đây là công cụ. Pain thật là đọc và đối chiếu từng CV với yêu cầu công việc.
- ✗ "AI đối chiếu chứng từ" (#8): đây là giải pháp. Pain thật là đối chiếu tay 3 loại chứng từ, dễ sót sai lệch.
- ✗ "Dùng tai nghe để gọi khi lái xe" (#1): đây là cách làm. Pain thật là phải liên lạc và mô tả vị trí bằng lời trong lúc đang lái.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
