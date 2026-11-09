# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: SonTuanCuong 
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi giao nhiệm vụ cho thành viên và họ đã làm một khoảng thời gian, người giao việc muốn biết họ đã xong bao nhiêu % nhiệm vụ và phần đó đóng góp bao nhiêu % vào dự án, để kịp điều chỉnh trước deadline (candidate #2)
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Sơn | Khi bắt đầu mỗi tuần, tôi muốn gom tất cả deadline trong tuần từ nhiều môn vào 1 chỗ, để dễ dàng nắm bắt được lịch và không bỏ sót môn nào. | Tôi, sinh viên học nhiều môn | Bước 2: tìm thông báo rải rác trong chat, 10 phút/lần | (Cường): Làm sao để gom lại được tất cả deadline trong nhiều ứng dụng. (Tuấn): Làm sao để có thể biết đâu là deadline đâu là bài tập |
| 2 | Sơn | Khi tôi giao một nhiệm vụ cho thành viên trong nhóm và họ đã làm một khoảng thời gian, tôi muốn biết họ đã xong bao nhiêu % nhiệm vụ và phần đó đóng góp bao nhiêu % vào dự án, để kịp điều chỉnh việc trước deadline | PM, Leader và các thành viên nhận việc | Bước 4–5: không có đơn vị chung để tính "%" nên câu trả lời mơ hồ, 10 phút chờ và hỏi lại mỗi lần; 2-3 lần hỏi lại/ngày | (Tuấn): Bổ sung chức năng: cá nhân dành thời gian bao lâu để hoàn thiện phần việc của mình được giao. (Tuấn & Cường) Làm sao để thành viên có thể sắp xếp được lịch dù đã có ứng dụng|
| 3 | Sơn | Khi tôi định học tiếng Trung 2 tiếng mỗi ngày, tôi muốn có sẵn khung giờ còn trống trong tuần, để giữ được thói quen đều thay vì bỏ buổi | Tôi | Bước 2: không xếp được khung giờ cố định, 60-75 phút/lần; chỉ thực hiện được 7-8/14 buổi trong 2 tuần gần nhất | (Tuấn & Cường): trên thị trường đã có nhiều ứng dụng tương tự như vậy, và nguyên nhân chính vẫn là việc nhàm chán do học 1 mình |
| 4 | Tuấn | Khi có một ý tưởng mới còn mơ hồ, tôi muốn có sẵn user story và tiêu chí nghiệm thu rõ ràng trước khi code, để AI không code sai hướng rồi phải làm lại | Vibe Coder, Khách hàng nhận sản phẩm | Bước 4–6, vòng “sinh code, thấy sai, giải thích lại”: yêu cầu chỉ rõ dần sau khi đã có code sai, nên tốn công gấp đôi | (Sơn & Cường): Vậy khác biệt gì so với những con AI hiện tại như ChatGPT, Claude,... |
| 5 | Tuấn | Khi nhận yêu cầu từ khách hàng, tôi muốn tìm được skill phù hợp hoặc tạo nhanh skill mới đúng yêu cầu đó, để AI làm đúng quy trình ngay từ đầu thay vì tôi giải thích lại mỗi lần | Vibe Coder | Bước 2–3 (tìm không ra hoặc không biết skill nào vừa) và bước 4–6 (không có cách kiểm thử skill ngoài chạy thật) | (Cường): nếu tạo skill thì những con AI hiện tại vẫn có khả năng xảy ra, thì liệu có thể sinh skill tốt hơn không. (Sơn): Số liệu thống kê nào có thể đánh giá được skill sinh ra. |
| 6 | Tuấn | Khi PM hỏi tính năng này mất bao lâu, họ muốn có ước lượng đáng tin, để cam kết với khách | PM, Khách hàng, Dev | Bước 2: ước lượng dựa trên bản demo, bỏ sót phần “ẩn” sau demo | (Sơn): "Thời gian đáng tin" lấy từ những thông số nào |
| 7 | Cường | Khi mở notebook để bắt đầu một bài lab mới, tôi muốn biết đoạn code đầu tiên cần viết, để bắt tay vào làm ngay thay vì đọc đi đọc lại đề | Tôi, học viên khóa AI thực chiến, mới học Python/ML, làm lab trên Google Colab | Bước 3, nghĩ cách chia bài thành các bước code: khoảng 8 phút/bài (ước lượng). Hiểu từng khái niệm nhưng chưa biết nên code phần nào trước, phần nào sau | (Sơn): có sinh code gợi ý không hay là chỉ sinh câu hỏi ôn tập. (Tuấn): Nếu bài lab không có nội dung trong bài giảng thì sao? |
| 8 | Cường | Khi chuẩn bị trước buổi học, tôi muốn nắm được ý chính của tài liệu dài, để vào lớp theo kịp bài | Tôi, học viên khóa AI thực chiến, học 4–5 buổi/tuần, chưa có nhiều nền tảng thực tế về AI | Bước 4, tra khái niệm chưa hiểu: khoảng 30 phút/buổi (ước lượng). Gặp khái niệm mới phải dừng đọc để tra, tra xong quay lại đọc tiếp | (Sơn): Đọc ở đây là nắm rõ hết lý thuyết, hay chỉ cần biết trong slide có những phần nào quan trọng? (Tuấn): Có tổng hợp lại kiến thức không |
| 9 | Cường | Khi tự viết lại một đoạn code từng chạy được nhờ tham khảo, tôi muốn nhớ được cách viết, để không phụ thuộc vào code có sẵn | Tôi, học viên mới học AI, thường tham khảo code mẫu hoặc code do ChatGPT gợi ý khi bị kẹt | Bước 2, tự viết lại: 10–15 phút cố gắng nhưng không viết được, phải bỏ cuộc và mở lại code cũ (ước lượng) | (Sơn): AI có tự sinh code không hay chỉ gợi ý.|

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Nắm và giữ kế hoạch thời gian | #1 Gom deadline nhiều môn, #2 Biết % tiến độ của thành viên, #3 Xếp khung giờ học tiếng Trung đều đặn, #6 Ước lượng thời gian đáng tin cho PM | Thông tin về thời gian (hạn nộp, giờ rảnh, tiến độ, thời lượng) nằm rải rác hoặc chỉ là ước lượng cảm tính, nên người làm không biết chắc mình đang ở đâu so với kế hoạch và hạn chót |
| B — Từ yêu cầu mơ hồ đến bước đầu tiên làm được | #4 User story và tiêu chí nghiệm thu trước khi code, #5 Tìm hoặc tạo skill đúng yêu cầu khách, #7 Biết đoạn code đầu tiên của bài lab | Có yêu cầu hoặc đề bài nhưng chưa rõ cần làm gì trước, làm gì sau; phải đoán, làm thử rồi sửa lại, nên tốn công làm đi làm lại |
| C — Hiểu và ghi nhớ kiến thức học | #8 Nắm ý chính tài liệu dài trước buổi học, #9 Nhớ cách viết lại đoạn code đã chạy được | Người học tiếp nhận kiến thức nhưng không giữ lại hoặc không hiểu đủ để tự dùng lại, nên phải tra cứu và quay lại đọc nhiều lần |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm số phút mỗi tuần mà học viên/thành viên nhóm mất vào việc tìm lại, đoán và làm lại khi thực hiện bài học và dự án nhóm
├── Opportunity: Hạn nộp, giờ rảnh, tiến độ và thời lượng nằm rải rác hoặc chỉ là ước lượng 
│     cảm tính, không biết chắc mình đang ở đâu so với kế hoạch và hạn chót
├── Opportunity B: Có yêu cầu hoặc đề bài nhưng chưa rõ cần làm gì trước, làm gì sau,
│     nên phải đoán, làm thử rồi sửa lại
└── Opportunity C: Tiếp nhận kiến thức nhưng không giữ lại hoặc không đủ hiểu để tự dùng lại,
      nên phải tra cứu và đọc lại nhiều lần

     ✗ "Dashboard tiến độ thành viên"           ← solution, gạch khỏi tầng này
     ✗ "Ứng dụng nhắc giờ học / lịch chung"     ← solution, gạch khỏi tầng này
     ✗ "AI sinh user story / sinh code gợi ý"   ← solution, gạch khỏi tầng này
     ✗ "Công cụ tóm tắt tài liệu dài"           ← solution, gạch khỏi tầng này
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- Dashboard tiến độ thành viên (từ candidate #2): là công cụ, không phải pain. Pain thật là không biết chắc tiến độ.
- Ứng dụng nhắc giờ học, lịch chung (từ candidate #1, #3): là công cụ. Pain thật là thông tin thời gian rải rác và không giữ được khung giờ cố định.
- AI sinh user story, sinh code gợi ý (từ candidate #4, #7, #9): là giải pháp. Pain thật là yêu cầu mơ hồ và không biết bắt đầu từ đâu.
- Công cụ tóm tắt tài liệu dài (từ candidate #8): là công cụ. Pain thật là mất nhiều thời gian tra cứu khi đọc.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #2 Biết % tiến độ của thành viên | 4 | 4 | 3 | 3 | 4 | 4 | 5 | **27** |
| #1 Gom deadline nhiều môn | 4 | 5 | 3 | 4 | 3 | 4 | 5 | **28** |
| #7 Biết đoạn code đầu tiên của bài lab | 5 | 4 | 2 | 2 | 4 | 3 | 4 | **24** |

**Candidate được chọn:** #2 — Biết thành viên đã xong bao nhiêu % nhiệm vụ được giao và đóng góp bao nhiêu % vào dự án

**Vì sao chọn:** Cả nhóm đều làm việc nhóm nên cùng gặp vấn đề này (không chỉ một người); bottleneck là một bước cụ thể (bước 4–5: thành viên trả lời tiến độ bằng cảm tính, người giao việc tự quy đổi %); đo được bằng số lần hỏi lại tiến độ (2–3 lần/ngày), số phút chờ (10 phút/lần) và độ lệch giữa % báo cáo với % thực tế; nhóm hiểu domain vì đang trải nghiệm hằng ngày.

**Vì sao loại các candidate còn lại:** 
- #3 (thói quen học tiếng Trung): Tuấn và Cường chỉ ra đã có nhiều ứng dụng tương tự và nguyên nhân chính là nhàm chán khi học một mình, không phải xếp lịch.
- #4, #5, #7, #9 (liên quan đến code và skill): đã có công cụ AI như ChatGPT và Claude làm gần đúng việc đó; chưa trả lời được khác biệt so với công cụ hiện có.

**Xử lý bất đồng (nếu có):** Điểm tổng của #1 (28) cao hơn #2 (27) một điểm, nhưng nhóm chọn #2. Lý do cần nhóm xác nhận bằng lập luận thật của mình, gợi ý: #1 có thể giải bằng một lịch chung duy nhất (No AI/Rule) và không còn nhiều điều để kiểm chứng, còn #2 vẫn chưa rõ "%" nên định nghĩa thế nào, đây là câu hỏi đáng kiểm chứng ở CP4. 

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
