# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Đoàn Đăng Khoa | Khi Bộ/Sở ban hành công văn, thông tư mới, tôi muốn biết nhanh điểm nào thay đổi ảnh hưởng đến môn và khối mình dạy, để kịp điều chỉnh ma trận đề và kế hoạch bài dạy. | Giáo viên bộ môn (người áp dụng); tổ trưởng chuyên môn (người phổ biến, giải đáp, duyệt) | Bước 3-4 (lọc phần liên quan, đối chiếu với cái cũ): ước tính ~30-60 phút/văn bản. Bước 5 (chờ họp tổ) gây độ trễ tính bằng ngày. | Tại sao lại cần 1 người duyệt sau khi đã sử dụng AI, có phải tự xây ra 1 nghề khác cho giáo viên không? |
| 2 | Đoàn Đăng Khoa | Khi đã có ma trận đề và cần nhiều mã đề tương đương, tôi muốn các mã đúng ma trận, độ khó tương đương, không trùng hay lộ câu, để không mất nhiều buổi soạn đề và rà soát. | Giáo viên bộ môn (người ra đề); tổ trưởng chuyên môn (người duyệt); học sinh (làm các mã đề khác nhau) | Bước 2 (soạn câu tương đương cho nhiều mã) và bước 5 (rà soát chéo giữa các mã). Ước tính nhiều giờ cho mỗi bộ đề. | Tại sao không thay đổi mã đề đơn giản chỉ thay các số trong đề đã soạn ra mà phải sử dụng LLM để tạo đề (Khánh) |
| 3 | Đoàn Đăng Khoa | Khi phải viết nhận xét cho từng học sinh theo các tiêu chí tôi đã đặt, tôi muốn không phải nghĩ lại câu chữ từ đầu cho mỗi em mà vẫn đúng mức độ của em đó, để giảm thời gian và giữ nhất quán giữa các học sinh. | Giáo viên bộ môn / GVCN; học sinh, phụ huynh. | Bước 3–4: quyết định mức độ và suy nghĩ lời văn để viết nhận xét. Ước tính ~3–5 phút/em, khoảng ~2–3 giờ/lớp. | Nếu như dùng tool tự động thì có thể giải quyết được vấn đề này không (Khoa) |
| 4 | Lê Quốc Khánh | Khi nhóm đang chọn dự án và phân công công việc, tôi muốn biết chính xác năng lực thực tế của từng thành viên, để giao đúng người đúng việc và tránh giao việc vượt quá khả năng hiện tại. | Trưởng nhóm / người phân công (chịu trách nhiệm chính), toàn bộ thành viên nhóm (bị ảnh hưởng) | Bước 3: Hỏi thêm / đoán năng lực → mất 20-40 phút, thông tin thiếu khách quan | Liệu có thực sự cần AI không, khi leader phải nắm được tình hình của nhóm và chọn đề tài phù hợp (Khoa) |
| 5 | Lê Quốc Khánh | Khi mỗi ngày phải kiểm tra nhiều nhóm lớp, nhóm dự án và các deadline, tôi muốn nhìn nhanh những việc quan trọng trong ngày, để không bỏ sót hoặc nộp muộn. | Tôi (sinh viên) | Bước 3: Check lại nhiều lần vì thông tin phân tán → mất 10-15 phút | Liệu có khả thi và cần thiết không, chi phí vận hành có quá lớn so với 1 việc có thể tự giác làm là xong không (Minh) |
| 6 | Lê Quốc Khánh | Khi phải tìm tài liệu học tập từ nhiều nguồn trong khóa học AI, tôi muốn gom nhanh những phần quan trọng, để học tập hiệu quả hơn và không lãng phí thời gian. | Tôi (sinh viên) | Bước 3: Đọc lướt + lọc thông tin quan trọng từ nhiều nguồn → mất 30-50 phút | Có thể sử dụng notebook LLM để tổng hợp luôn không (Huy) |
| 7 | Nguyễn Quang Huy | Khi đến tối Chủ Nhật trước buổi họp khóa luận sáng thứ Hai, tôi muốn gom đầy đủ kết quả chạy thực nghiệm mô hình, bộ tham số đã thử và các vướng mắc trong tuần về một chỗ, để gửi báo cáo tiến độ cho GVHD trước 22h mà không bị sót số liệu hay phải giải thích lại ngữ cảnh. | Sinh viên năm cuối ngành Toán-Tin ứng dụng đang làm khóa luận tốt nghiệp (cùng 4 bạn trong lab và GVHD đọc báo cáo). | Bước 5 — Viết phần nhận định & giải thích nguyên nhân thay đổi kết quả thực nghiệm (mất ~20 phút, cộng với 20 phút ở bước 1-2 do phải lục tìm ngữ cảnh rời rạc). | Sử dụng WanDB có thể ghi lại log rồi thì có cần thiết gom lại kết quả để chạy mô hình này không (Khoa) |
| 8 | Nguyễn Quang Huy | Khi viết phần Tổng quan nghiên cứu (Related Work) cho khóa luận từ 25-30 bài báo đã tải về, tôi muốn đối chiếu được các bài theo bài toán, giả thiết toán học (như tính lồi chặt, tính trơn Lipschitz), bộ dữ liệu và hạn chế của từng phương pháp, để chỉ ra khoảng trống nghiên cứu (research gap) có căn cứ xác đáng. | Sinh viên năm cuối Toán-Tin ứng dụng đang viết Chương 1-2 khóa luận tốt nghiệp hoặc chuẩn bị seminar nhóm nghiên cứu. | Bước 2 & 3 — Mở lại từng PDF để dò tìm đúng giả thiết toán học và tốc độ hội tụ (mất ~135 phút/đợt tổng hợp ~15-20 bài, vì mỗi bài ký hiệu một kiểu). | Liệu có thể sử dụng các LLM thông thường để thực hiện research này không (Minh) |
| 9 | Nguyễn Quang Huy | Khi hoàn thiện từng chương khóa luận trên Overleaf mỗi cuối tuần, tôi muốn biết các mục tài liệu tham khảo mới thêm đã đủ trường thông tin (tác giả, năm, tên hội nghị/tạp chí, chuẩn viết tắt) theo format IEEE hay chưa, để không bị lỗi hiển thị hoặc phải dò sửa thủ công từng dòng trước khi nộp bản nháp. | Sinh viên năm cuối viết khóa luận tốt nghiệp / bài báo khoa học bằng LaTeX trên Overleaf. | Bước 2 & 3 — Dò lỗi bằng mắt trên PDF và lên Google Scholar tìm lại bản xuất bản chính thức thay cho bản arXiv/thiếu trường (mất ~20 phút/lần kiểm tra). | Sử dụng tool như Zotero liệu có tối ưu hơn luôn không, vì Zotero đã chỉnh lại format thống nhất theo kiểu mình đã chọn rồi (Khoa) |
| 10 | Lã Thái Minh | Khi đến cuối tháng nhận bill trọ và tiền ăn chung, tôi muốn đối soát nhanh ai đã ứng trước khoản nào và chia đều tiền, để đóng tiền đúng hạn cho chủ trọ. | 2 roommate | Bước 2 & 3: Tìm kiếm và phân loại bill chung/riêng từ nhiều nguồn tin nhắn, ảnh chụp, app ngân hàng (mất 50 phút do dữ liệu nằm rải rác, ảnh mờ, dễ quên). | Liệu có thực sự cần tool để làm việc này không (Khánh) |
| 11 | Lã Thái Minh | Khi cả hai đứa đều bận học và làm việc, tôi muốn phân chia rõ người làm từng việc dọn dẹp (đổ rác, rửa bát), để phòng sạch sẽ mà không phải nhắc nhở, tị nạnh nhau. | 2 roommate | Bước 2 & 3: Bàn bạc, nghĩ món và thống nhất ý kiến khi cả hai đều mệt mỏi (mất 20-25 phút). | Làm chung với nhau thì có nhanh hơn không (Huy) |
| 12 | Lã Thái Minh | Khi đến giờ nấu bữa tối, tôi muốn biết nhanh hôm nay nấu món gì từ đồ còn trong tủ lạnh, để không mất công bàn cãi và tránh đồ ăn bị hỏng. | 2 bạn cùng phòng (hoặc người phụ trách nấu ăn ngày hôm đó). | Bước 2 & 4: Đùn đẩy, trì hoãn và tranh cãi xem lượt dọn/đổ rác thuộc về ai (mất 15–20 phút tranh luận và gây khó chịu cả ngày). | Note lại đồ ăn đã cất thời gian nào rồi lấy ra dùng rồi thì đã giải quyết được vấn đề chưa (Huy) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | #1, #6, #8 | Phải đọc nhiều tài liệu dài, rồi lọc ra vài đoạn liên quan đến việc mình đang làm và đối chiếu với cái đã có. |
| B | #7, #10 | Thông tin nằm rải rác ở nhiều chỗ, mất công lục lại và gom về một bản trước khi dùng được (để báo cáo hoặc đối soát). |
| C | #4, #5, #11 | Chia việc và nhớ việc đang dựa vào đoán, nhắc nhau hoặc check đi check lại, nên dễ giao sai, quên hoặc tị nạnh. |
| D | #2, #3, #9 | Đã có sẵn chuẩn (ma trận, tiêu chí, format), nhưng vẫn phải viết hoặc kiểm tra thủ công từng bản lặp lại. |
| Để riêng | #12 | Chốt một quyết định nhỏ hằng ngày (nấu gì) giữa hai người. Không hợp cluster nào nên không bỏ vào cluster. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm ≥ 50% số phút mỗi tuần mà người dạy và người học trong nhóm dành cho việc
         tìm, gom và rà soát thông tin lặp lại, trong khi số lỗi hoặc sót bị phát hiện
         sau đó không tăng.
         (Đơn vị đo: phút/tuần/người. Mốc ban đầu lấy từ các ước tính trong bảng pitch,
          sẽ đo lại thực tế cho candidate được chọn.)
├── Opportunity A: Phải đọc lại cả văn bản hoặc cả bài báo chỉ để tìm vài đoạn liên quan,
│                  rồi tự đối chiếu với cái cũ.
├── Opportunity B: Thông tin nằm rải rác nhiều nơi nên mất thời gian lục và gom lại
│                  trước khi dùng được.
├── Opportunity C: Chia việc và nhớ hạn đang dựa vào đoán và nhắc nhau, nên dễ giao
│                  quá sức, quên hoặc cãi nhau.
└── Opportunity D: Cùng một chuẩn nhưng phải viết hoặc kiểm tra tay từng bản,
                   tốn công và dễ lệch giữa các bản.
```


Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ~~Chatbot tóm tắt công văn cho giáo viên~~ (có tên công cụ, người dùng đau ở chỗ phải lọc phần liên quan, không phải ở chỗ thiếu chatbot)
- ~~Tool tự sinh nhận xét cho học sinh~~ (đây là cách giải, pain thật là phải nghĩ lại câu chữ cho từng em)
- ~~Bảng nhắc deadline mỗi ngày~~ (đây là tính năng, pain thật là thông tin phân tán nên phải check nhiều lần)
- ~~Trợ lý AI chia việc cho thành viên~~ (có chữ AI, pain thật là leader chưa nắm rõ năng lực từng người)
- ~~Dùng LLM tạo mã đề~~ (đây là công cụ, pain thật là soạn và rà soát nhiều mã tương đương mất nhiều giờ)

### 2.4. Chấm điểm shortlist (1-5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #1 Theo dõi văn bản quy định mới | 5 | 5 | 3 | 4 | 4 | 4 | 4 | 29 |
| #8 Đối chiếu bài báo cho Related Work | 4 | 4 | 4 | 5 | 3 | 4 | 4 | 28 |
| #2 Nhiều mã đề tương đương | 4 | 3 | 2 | 3 | 2 | 3 | 3 | 20 |

**Candidate được chọn:** #1 (problem card #3 của Khoa), theo dõi và áp dụng văn bản quy định mới của Bộ/Sở.

**Vì sao chọn:** #1 có tổng cao nhất (29/35). Điểm cao nhất ở hai tiêu chí nền: Actor rõ (5) và Quy trình rõ (5), với hai vai cụ thể và 7 bước, bước nghẽn xác định rõ là bước 3-4 và bước 5. Impact đo được (4) vì có sẵn 3 chỉ số: thời gian từ lúc nhận văn bản đến lúc biết việc cần làm, số lần hỏi lại tổ trưởng, và số lỗi áp dụng sai khi duyệt đề. So sánh được 4 mức (4) vì đã mô tả được phương án không dùng AI: tóm tắt 1 trang theo mẫu cố định, tổ trưởng phân công luân phiên.

**Vì sao loại các candidate còn lại:**
- #8: số ~135 phút/đợt là số của một người, chưa kiểm chứng với người khác. Mỗi bài báo ký hiệu một kiểu nên có rủi ro trích sai giả thiết toán học, mà lỗi kiểu này khó phát hiện nếu không mở lại từng bài. Câu hỏi của Minh (dùng LLM thông thường có làm được việc này không) cũng chưa có câu trả lời rõ.
- #2: pain mới ở mức "nhiều giờ", chưa có số đo. Chưa có cách đo "độ khó tương đương" giữa các mã đề. Câu hỏi của Khánh (chỉ đổi số trong đề đã soạn) chưa bị bác bỏ, nên phương án rule-based chưa chắc thua LLM.
- #3, #6: #3 cùng cụm D với #2, chưa rõ cách đo "đúng mức độ của từng em". #6 cùng cluster A với #8, nguồn tài liệu của khóa học rộng và Huy đã hỏi về notebook LLM, chưa có lý do tách khỏi công cụ có sẵn.
- #4, #5, #10, #11, #12: thông tin đầu vào mang tính cá nhân hoặc chủ quan (năng lực thành viên, việc nhà, bữa ăn), việc nhỏ 10-50 phút, và các câu hỏi "có thực sự cần tool không" chưa có lời đáp rõ.
- #7, #9: #7 bị hỏi vì đã có công cụ ghi log thí nghiệm; #9 bị hỏi vì công cụ quản lý tài liệu tham khảo có thể làm được việc này. Cả hai chưa chứng minh được phần việc còn lại mà công cụ có sẵn không làm.

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1-5) | Đã có bằng chứng (1-5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4-6 giả định; xóa dòng thừa.*

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

**Tiêu chí đánh giá đầu ra của AI (3-5 tiêu chí):**

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
