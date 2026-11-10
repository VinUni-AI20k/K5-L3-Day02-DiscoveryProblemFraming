# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3): Hội tụ nhóm — Opportunity Solution Tree và chấm điểm candidate

### 1. Các candidate problem của nhóm

Sau phần pitch cá nhân, nhóm có 6 candidate:

| # | Thành viên | Candidate problem |
|---:|---|---|
| 1 | Bùi Đăng Quang | Lọc và so sánh các tin phòng/căn hộ phù hợp trước khi đi xem |
| 2 | Mai Huy Hoạt | Hỗ trợ chẩn đoán hình ảnh của xe ô tô tại gara |
| 3 | Nguyễn Gia Bảo | Đối chiếu JD và đề xuất bullet/keyword để sửa CV cho sinh viên năm 3/4 |
| 4 | Nguyễn Vũ Thành Long | Hỗ trợ quản lý kho hàng cho người dùng lớn tuổi tại các hộ kinh doanh nhỏ |
| 5 | Bùi Lê Công Tuấn | Tìm tài liệu học tập và hướng dẫn LAB |
| 6 | Nguyễn Đình Quang | Hỗ trợ điểm danh học sinh/sinh viên bằng camera |

---

### 2. Opportunity Solution Tree (OST)

#### Outcome khi hội tụ

Nhóm không cố gộp cả 6 candidate vào một sản phẩm chung. OST được sử dụng để phân biệt:

- **Outcome:** kết quả muốn cải thiện.
- **Opportunity:** pain hoặc nhu cầu của người dùng.
- **Solution:** những cách có thể can thiệp để giải quyết opportunity.

Candidate được chọn để tiếp tục discovery là **quản lý kho cho hộ kinh doanh nhỏ**.

#### OST của candidate được chọn

```text
OUTCOME
Giảm thời gian tra cứu, đối chiếu và sai lệch tồn kho
trong hoạt động nhập – xuất – tồn tại hộ kinh doanh nhỏ

├── OPPORTUNITY 1
│   Người quản lý có thể bỏ sót hoặc ghi nhận không nhất quán
│   các giao dịch nhập và bán hàng
│
│   ├── Solution: Chuẩn hóa mẫu ghi chép nhập – xuất
│   ├── Solution: Biểu mẫu nhập liệu đơn giản, dễ sử dụng
│   └── Solution: Kiểm tra các trường giao dịch còn thiếu
│
├── OPPORTUNITY 2
│   Người quản lý mất thời gian khi tìm lại giá bán,
│   lịch sử giao dịch hoặc thông tin nhập hàng
│
│   ├── Solution: Sổ/bảng tính có cấu trúc và bộ lọc
│   ├── Solution: Tra cứu theo sản phẩm, ngày và giao dịch
│   └── Solution: Hỗ trợ hỏi đáp trên dữ liệu đã ghi nhận
│
├── OPPORTUNITY 3
│   Người quản lý khó xác định lượng tồn khi thông tin
│   nhập – xuất nằm ở nhiều nơi hoặc chưa được đối chiếu
│
│   ├── Solution: Quy trình đối chiếu dữ liệu thống nhất
│   ├── Solution: Rule tự động tính nhập – xuất – tồn
│   └── Solution: Bảng tổng hợp tồn kho và lịch sử biến động
│
├── OPPORTUNITY 4
│   Người quản lý khó phát hiện chênh lệch giữa
│   số lượng ghi chép và hàng hóa thực tế
│
│   ├── Solution: Checklist kiểm kê định kỳ
│   ├── Solution: Báo cáo đối chiếu tồn sổ và tồn thực tế
│   └── Solution: Cảnh báo các chênh lệch cần kiểm tra
│
└── OPPORTUNITY 5
    Người lớn tuổi có thể gặp khó khăn với thao tác
    phức tạp của các công cụ quản lý hiện tại

    ├── Solution: Giao diện tối giản, chữ rõ và ít bước
    ├── Solution: Các thao tác tra cứu được hướng dẫn sẵn
    └── Solution: Hỗ trợ tương tác bằng ngôn ngữ tự nhiên
```

**Lưu ý:** Các opportunity trên là giả thuyết cần kiểm chứng với người dùng. Những đề xuất như “xây chatbot quản lý kho”, “xây AI Agent quản lý kho” là **solution**, không phải opportunity. Nhóm chưa kết luận cần dùng AI.

---

### 3. Tiêu chí chấm điểm candidate

Nhóm sử dụng thang điểm **1–5** cho 7 tiêu chí:

| Tiêu chí | Ý nghĩa |
|---|---|
| **Actor rõ** | Xác định rõ người đang gặp problem |
| **Quy trình rõ** | Có thể mô tả quy trình hiện tại bằng các bước cụ thể |
| **Pain có bằng chứng** | Có trải nghiệm, quan sát hoặc người thật làm cơ sở kiểm chứng |
| **Impact đo được** | Có thể xác định chỉ số đo lường và baseline |
| **Dễ validation** | Dễ tiếp cận người dùng để phỏng vấn, quan sát, kiểm chứng |
| **So sánh mức can thiệp** | Có thể so sánh No AI / Rule / Workflow / Agent |
| **Vừa sức bài tập** | Phạm vi phù hợp với thời gian và nguồn lực nhóm |

**Điểm tối đa: 35 điểm.** Điểm số là đánh giá sơ bộ của nhóm tại giai đoạn hội tụ, chưa thay thế bằng chứng validation.

---

### 4. Bảng chấm điểm candidate

| Rank | Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Dễ validation | So sánh mức can thiệp | Vừa sức | Tổng |
|---:|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **1** | **Quản lý kho cho hộ kinh doanh nhỏ** | 5 | 5 | 5 | 5 | 5 | 5 | 4 | **34** |
| **2** | Camera hỗ trợ điểm danh | 5 | 5 | 4 | 5 | 5 | 4 | 4 | **32** |
| **3** | Lọc và so sánh phòng/căn hộ | 5 | 5 | 4 | 4 | 5 | 5 | 4 | **32** |
| **4** | Chẩn đoán hình ảnh xe tại gara | 4 | 4 | 4 | 5 | 3 | 4 | 3 | **27** |
| **5** | Đối chiếu JD và sửa CV | 5 | 4 | 3 | 4 | 5 | 3 | 3 | **27** |
| **6** | Tìm tài liệu học tập và hướng dẫn LAB | 5 | 4 | 3 | 3 | 5 | 3 | 3 | **26** |

*Hai candidate ở rank 2–3 cùng 32 điểm; hai candidate ở rank 4–5 cùng 27 điểm. Thứ tự trình bày phản ánh thứ tự ưu tiên thảo luận của nhóm.*

---

### 5. Lý do chấm điểm

#### Rank 1 — Quản lý kho cho hộ kinh doanh nhỏ — 34/35

Candidate được nhóm đánh giá cao nhất vì:

- **Actor cụ thể:** người quản lý hoặc chủ hộ kinh doanh nhỏ, đặc biệt là người lớn tuổi.
- **Pain có cơ sở thực tế:** tình huống tại hộ kinh doanh của gia đình thành viên trong nhóm.
- **Quy trình rõ:** nhập hàng, bán hàng, kiểm tra tồn, tra cứu giao dịch.
- **Impact liên quan trực tiếp đến vận hành:** khó biết chính xác lượng hàng còn lại, tìm lại giá đã bán, đối chiếu lịch sử nhập – xuất, nguy cơ sai lệch tồn kho.
- **Dễ tiếp cận:** nhóm có thể phỏng vấn và quan sát người dùng thật.
- **Có thể so sánh nhiều mức can thiệp:**
  - **No AI:** sổ sách, bảng tính hoặc phần mềm quản lý kho.
  - **Rule:** tự động tính nhập – xuất – tồn.
  - **Workflow:** dữ liệu giao dịch → tính tồn → AI hỗ trợ tra cứu/tổng hợp.
  - **Agent:** chủ động hỗ trợ quản lý và nhắc bất thường trong kho.
- Problem đủ gần thực tế để tiếp tục kiểm chứng nhưng vẫn còn giả định cần nghiên cứu.

**Điểm chưa chắc lớn nhất:**

> Nếu dữ liệu giao dịch đầu vào chưa được ghi nhận đầy đủ thì AI hoặc Agent cũng không thể cho kết quả tồn kho chính xác.

Đây là giả định quan trọng cần kiểm chứng ở bước tiếp theo.

#### Rank 2 — Camera hỗ trợ điểm danh — 32/35

**Điểm mạnh:**

- Actor rõ: giảng viên/giáo viên và học sinh, sinh viên.
- Quy trình điểm danh hiện tại dễ quan sát.
- Impact dễ đo bằng thời gian điểm danh và tỷ lệ sai sót.
- Nhóm dễ tiếp cận người dùng để khảo sát.

**Điểm chưa chắc:**

- Có nhiều giải pháp đơn giản hơn như QR, mã lớp, NFC hoặc thẻ sinh viên.
- Camera AI có rủi ro về ánh sáng, góc camera, nhận diện nhầm, dữ liệu khuôn mặt và quyền riêng tư.
- Cần chứng minh camera tạo giá trị đủ lớn so với Rule đơn giản.

#### Rank 3 — Lọc và so sánh phòng/căn hộ — 32/35

**Điểm mạnh:**

- Có trải nghiệm thực tế gần đây từ thành viên trong nhóm.
- Actor rõ: người đang tìm thuê phòng/căn hộ.
- Quy trình cụ thể: `tìm tin → đọc → liên hệ → hỏi thêm → so sánh → shortlist → đi xem`.
- Dễ tìm người từng thuê trọ để phỏng vấn.
- Có thể so sánh No AI / Rule / Workflow / Agent.

**Điểm chưa chắc:**

- Dữ liệu từ listing có thể không chính xác hoặc cập nhật chậm.
- Một phần root cause thuộc về dữ liệu từ sale/chủ nhà, không chỉ công cụ tìm kiếm.
- Phát hiện tin trùng và xác định tình trạng còn phòng có Feasibility Risk tương đối lớn.

#### Rank 4 — Chẩn đoán hình ảnh xe tại gara — 27/35

**Điểm mạnh:**

- Impact có thể lớn vì liên quan trực tiếp tới kiểm tra và sửa xe.
- Có use case rõ cho Computer Vision.

**Điểm yếu:**

- Cần dữ liệu ảnh lỗi xe có nhãn.
- Cần chuyên gia kỹ thuật xác minh kết quả.
- AI chẩn đoán sai có thể dẫn đến kiểm tra hoặc sửa chữa sai hướng.
- Nhóm khó tiếp cận dữ liệu và chuyên môn hơn ba candidate phía trên.

#### Rank 5 — Đối chiếu JD và sửa CV — 27/35

**Điểm mạnh:**

- Actor rõ: sinh viên năm 3/4 chuẩn bị xin việc.
- Dễ tìm người dùng khảo sát và pilot bằng JD, CV.

**Điểm yếu:**

- Thị trường đã có nhiều công cụ ATS, keyword matching, CV review.
- Một phần problem có thể giải bằng Rule hoặc checklist.
- Nếu không kiểm soát phạm vi, AI dễ chuyển thành viết lại CV hoặc tạo kinh nghiệm không có thật.
- Cần xác định pain chính là thiếu keyword, khó viết bullet hay chưa hiểu JD.

#### Rank 6 — Tìm tài liệu học tập và hướng dẫn LAB — 26/35

**Điểm mạnh:**

- Actor rất dễ tiếp cận; pain quen thuộc với sinh viên.
- Quy trình dễ khảo sát.

**Điểm yếu:**

- Root cause rộng: tài liệu rải rác, không biết từ khóa, chưa tổ chức tài liệu hoặc tài liệu thực sự chưa tồn tại.
- Tổ chức tài liệu và search thông thường có thể đã giải quyết phần lớn problem.
- Impact khó đo rõ hơn các candidate khác.
- Khó chứng minh AI tạo thêm giá trị nếu nguồn tài liệu chưa chuẩn hóa.

---

### 6. Candidate được nhóm chọn

Nhóm thống nhất chọn hướng đề tài:

> **AI Agent hỗ trợ quản lý kho hàng dành cho người dùng lớn tuổi tại các hộ kinh doanh nhỏ.**

Tuy nhiên, sau phản biện, nhóm **không mặc định phải xây AI Agent ngay từ đầu**.

**Problem được giữ lại để tiếp tục discovery:**

> **Người quản lý tại các hộ kinh doanh nhỏ gặp khó khăn trong việc ghi nhận, tra cứu và đối chiếu thông tin nhập – xuất – tồn kho, đặc biệt khi dữ liệu đang được quản lý thủ công hoặc phân tán.**

Việc có cần AI hay không và mức can thiệp Rule, Workflow hay Agent sẽ được quyết định sau bước validation.

---

### 7. Vì sao chọn candidate quản lý kho

#### 7.1. Có người dùng thật để tiếp cận

Một thành viên có thể trực tiếp quan sát và phỏng vấn người đang quản lý cửa hàng/hộ kinh doanh.

#### 7.2. Pain có tác động thực tế

Sai lệch tồn kho có thể ảnh hưởng trực tiếp tới nhập hàng, bán hàng, kiểm kê, doanh thu và quản lý vốn.

#### 7.3. Quy trình hiện tại tương đối rõ

```text
Nhập hàng
    ↓
Ghi nhận thông tin
    ↓
Bán hàng
    ↓
Ghi nhận giao dịch
    ↓
Khi cần kiểm tra: tìm lại dữ liệu
    ↓
Đối chiếu nhập – xuất
    ↓
Kiểm tra hàng thực tế
    ↓
Xác định tồn kho
```

#### 7.4. Có bottleneck đáng kiểm chứng

Khâu ghi nhận và tìm lại dữ liệu có thể thiếu đầy đủ hoặc nhất quán, khiến việc kiểm tra tồn kho phải đối chiếu nhiều nguồn. Đây vẫn là **giả thuyết**, chưa phải kết luận sau khảo sát.

#### 7.5. Có thể so sánh nhiều mức giải pháp

```text
No AI
  → Chuẩn hóa sổ/bảng ghi chép

Rule
  → Tự động tính nhập – xuất – tồn

Workflow
  → Rule tính tồn + AI hỗ trợ tìm kiếm/tổng hợp

Agent
  → Chủ động theo dõi, cảnh báo và hỗ trợ người dùng
```

Đặc điểm này phù hợp với mục tiêu bài tập: xác định **mức can thiệp vừa đủ**, thay vì mặc định xây AI.

---

### 8. Vì sao không chọn các candidate còn lại

#### Camera hỗ trợ điểm danh

- Có nhiều phương án đơn giản hơn camera AI như QR hoặc NFC.
- Phải xử lý dữ liệu khuôn mặt, quyền riêng tư và nguy cơ nhận diện sai.
- Nếu pain chủ yếu là thời gian điểm danh thì Rule đơn giản có thể đủ tốt.

**Kết luận:** Nguy cơ sử dụng công nghệ phức tạp hơn mức problem yêu cầu (**over-engineering**).

#### Lọc và so sánh phòng/căn hộ

- Dữ liệu phụ thuộc sale/chủ nhà và các nền tảng bên ngoài.
- Tin đăng có thể sai hoặc lỗi thời; khó kiểm soát trạng thái còn phòng theo thời gian thực.
- Việc phát hiện listing trùng có nhiều trường hợp khó xác định.
- Nhóm kiểm soát được ít phần của data pipeline hơn bài quản lý kho.

**Kết luận:** Pain có thật và actor rõ nhưng Feasibility Risk cao hơn candidate được chọn.

#### Chẩn đoán hình ảnh xe tại gara

- Cần dữ liệu chuyên ngành và người có chuyên môn xác nhận kết quả.
- Sai sót có hậu quả cao hơn.
- Phạm vi Computer Vision tương đối lớn.

#### Đối chiếu JD và sửa CV

- Có nhiều sản phẩm tương tự trên thị trường.
- Một phần problem có thể giải bằng keyword matching.
- Cần nghiên cứu thêm để xác định khoảng trống thực sự.

#### Tìm tài liệu học tập và hướng dẫn LAB

- Problem còn rộng và root cause chưa rõ.
- Có khả năng chỉ cần tổ chức lại tài liệu và cải thiện search.
- Impact khó định lượng hơn các candidate khác.

---

### 9. Kết luận hội tụ

Kết quả CP3 của nhóm là:

> **Chọn problem quản lý kho cho hộ kinh doanh nhỏ để tiếp tục validation.**

Điều nhóm **chưa kết luận** là:

> “Phải xây AI Agent quản lý kho.”

Giả định quan trọng được nhận ra sau phản biện:

> **Nếu dữ liệu nhập – xuất chưa được ghi nhận đầy đủ thì AI cũng không thể đưa ra tồn kho chính xác.**

**Các câu hỏi cần kiểm chứng tiếp theo:**

1. Người dùng hiện ghi nhận dữ liệu như thế nào?
2. Dữ liệu thường thiếu ở bước nào?
3. Sai lệch tồn kho xảy ra bao nhiêu lần?
4. Khâu nào gây mất thời gian nhất?
5. Phần mềm hoặc bảng tính thông thường đã giải được bao nhiêu?
6. Phần còn lại có thật sự cần AI hay không?

**Định hướng tiếp theo:** Phỏng vấn, quan sát thực tế, xác định baseline và đối chiếu các mức can thiệp trước khi quyết định solution.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Người bán hàng mất thời gian hằng tuần để tra giá đã bán, hỏi lại giá và đếm tồn kho | Value | 5 | 3 | Đã kiểm chứng (3.2): xảy ra hằng tuần ở cả 4 vai trò, nhưng mỗi lần tra giá chỉ 1–5 phút |
| 2 | Nguyên nhân gốc nằm ở bước **ghi nhận** giao dịch (ghi muộn, ghi sót, ghi rải rác), không phải ở bước **tra cứu** | Value | 5 | 4 | Đã kiểm chứng (snapshot #2, #3) |
| 3 | Người đứng quầy không kịp gõ hoặc ghi tay từng giao dịch lúc đông khách | Usability | 5 | 3 | Đã kiểm chứng (snapshot #2: "Lúc đông khách thì bán xong mới ghi, đôi khi quên mất") |
| 4 | Người bán sẵn sàng **nói một câu ngắn** ("bán 2 tai nghe Sony 350 nghìn") hoặc **chụp ảnh giấy ghi tạm** thay cho việc gõ tay, và chịu bấm xác nhận trước khi lưu | Usability | 5 | 1 | Kiểm chứng tiếp |
| 5 | AI nhận diện đúng tên hàng, số lượng và giá từ giọng nói hoặc ảnh tiếng Việt với danh mục hàng điện tử (tên model dài, viết tắt, cùng một món nhiều mức giá) | Feasibility | 5 | 2 | Kiểm chứng tiếp |
| 6 | Khi AI ghi sai, người bán phát hiện và sửa được ngay ở bước xác nhận, nên sai sót không lọt vào số liệu tồn kho; chi phí công cụ nằm trong mức cửa hàng chấp nhận | Viability | 4 | 2 | Sau |

**Đã kiểm chứng trong buổi:** #1, #2, #3 (phỏng vấn 4 người, mục 3.2).

**Cần kiểm chứng tiếp:** #4 và #5. Đây là hai giả định quan trọng cao, bằng chứng thấp, quyết định có nên đưa AI vào bước ghi nhận hay không. Cách kiểm chứng: lấy 10 giao dịch thật của cửa hàng, cho người đứng quầy đọc thử vào một công cụ ghi đơn bằng giọng nói (ví dụ Knote ở 3.3), đếm số đơn AI nhận đúng tên hàng, số lượng và giá; hỏi người bán có chịu dùng cách này lúc đông khách không.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn (4 người tại cửa hàng điện tử của gia đình Long; người được hỏi không phải thành viên nhóm)

**Snapshot #1: Chủ cửa hàng**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Chủ cửa hàng |
| Câu nói đáng nhớ nhất (nguyên văn) | "Có hôm khách hỏi giá hàng nhập tháng trước mà phải tìm lại sổ mới nhớ được." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Khách hỏi lại giá bán của một mặt hàng đã bán trước đó, chủ cửa hàng phải tìm sổ ghi chép. |
| Hiện đang xử lý bằng cách nào (workaround)? | Tra sổ, hỏi nhân viên hoặc kiểm tra tin nhắn đặt hàng. |
| Mất bao lâu, bao lần? | Khoảng 3–5 phút/lần, 3–4 lần/tuần. |
| Insight / opportunity rút ra | Lịch sử giao dịch nằm rải rác ở sổ, tin nhắn và trí nhớ của nhân viên, chưa tập trung một chỗ. |

**Snapshot #2: Nhân viên đứng quầy**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Nhân viên bán hàng |
| Câu nói đáng nhớ nhất (nguyên văn) | "Lúc đông khách thì bán xong mới ghi, đôi khi quên mất." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Bỏ sót một số giao dịch nhỏ trong lúc cửa hàng đông khách. |
| Hiện đang xử lý bằng cách nào (workaround)? | Ghi tạm ra giấy rồi tổng hợp vào cuối ngày. |
| Mất bao lâu, bao lần? | Khoảng 10–15 phút tổng hợp mỗi ngày. |
| Insight / opportunity rút ra | Ghi nhận bằng tay ngay lúc bán gây gián đoạn công việc, nhất là giờ cao điểm. Đây là nguồn gốc của dữ liệu thiếu. Cơ hội: giảm thao tác ghi nhận xuống mức người bán làm được ngay cả khi đang bận. |

**Snapshot #3: Người phụ trách kho**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Thành viên gia đình phụ trách kho |
| Câu nói đáng nhớ nhất (nguyên văn) | "Muốn biết còn bao nhiêu thì nhiều lúc vẫn phải ra đếm." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Số lượng hàng trên sổ không khớp với hàng thực tế. |
| Hiện đang xử lý bằng cách nào (workaround)? | Kiểm đếm trực tiếp và ghi lại số lượng. |
| Mất bao lâu, bao lần? | 20–30 phút/lần, khoảng 2 lần/tuần. |
| Insight / opportunity rút ra | Tồn kho không được cập nhật theo từng giao dịch nên sổ không phản ánh đúng thực tế. |

**Snapshot #4: Người hỗ trợ bán hàng**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Thành viên gia đình hỗ trợ bán hàng |
| Câu nói đáng nhớ nhất (nguyên văn) | "Nhiều mặt hàng phải hỏi lại người nhà vì không nhớ giá nhập hoặc giá bán." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Không chắc giá bán của một mặt hàng khi chủ cửa hàng vắng mặt. |
| Hiện đang xử lý bằng cách nào (workaround)? | Gọi điện hoặc nhắn tin hỏi chủ cửa hàng. |
| Mất bao lâu, bao lần? | 1–3 phút/lần, khoảng 3 lần/tuần. |
| Insight / opportunity rút ra | Thông tin giá nhập và giá bán chỉ nằm trong đầu chủ cửa hàng, chưa được chia sẻ cho những người cùng bán. |

**Tổng hợp:**

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn tại cửa hàng | 4 người (4 vai trò khác nhau) | 4/4 người gặp vấn đề hằng tuần. Thời gian mất mỗi tuần: tra giá (chủ) 9–20 phút; hỏi lại giá (người hỗ trợ) 3–9 phút; tổng hợp sổ cuối ngày 10–15 phút/ngày; kiểm đếm kho 40–60 phút | Mỗi lần **tra giá chỉ mất 1–5 phút**, ngắn hơn nhóm nghĩ. Phần tốn thời gian nhất là **tổng hợp sổ và đếm kho**, không phải tra cứu. Nhân viên không kịp ghi tay lúc đông khách, nên giải pháp nào đòi gõ nhiều thao tác tại quầy cũng có rủi ro |
| Research công cụ có sẵn (3.3) | 5 công cụ | Phần mềm bán hàng (KiotViet, Sapo, MISA eShop) đã tự trừ tồn kho và lưu lịch sử giá. Đã có công cụ AI tạo đơn từ giọng nói và ảnh (Knote, MISA AMIS CRM) | Công cụ AI giọng nói hiện tối ưu cho món ăn có tên ngắn; chưa có bằng chứng chạy tốt với tên model hàng điện tử |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

- **Đổi bottleneck:** từ "tra cứu thông tin trong sổ" sang **"giao dịch không được ghi ngay và ghi đủ lúc bán, vì ghi tay quá chậm khi đông khách"**. Tra giá chỉ là triệu chứng (1–5 phút/lần). Nguyên nhân là dữ liệu ghi muộn, ghi sót, nằm rải rác, dẫn tới phải tổng hợp cuối ngày (10–15 phút/ngày) và đếm kho bằng tay (40–60 phút/tuần).
- **Mở rộng actor:** từ "gia đình chủ cửa hàng" thành **4 vai trò cùng bán hàng**: chủ cửa hàng, nhân viên đứng quầy, người phụ trách kho, người hỗ trợ bán.
- **Xác định cơ hội cho AI:** bước có độ mơ hồ cao nhất là chuyển **lời nói hoặc ảnh giấy ghi tạm** (đầu vào tự do, viết tắt, nhiều cách nói) thành **giao dịch có cấu trúc** (tên hàng, số lượng, giá). Đây là điểm AI hỗ trợ có cơ sở từ bằng chứng. Các bước còn lại (trừ tồn kho, lưu lịch sử giá, báo cáo) là logic cố định, phần mềm bán hàng có sẵn đã làm được.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Knote** (app ghi đơn bằng AI của KiotViet) | https://apps.apple.com/us/app/knote/id6738162895 | **Ghi nhận giao dịch** bằng giọng nói hoặc tin nhắn: nói "2 phở 50k" là AI tự lên đơn | Nhận diện giọng nói tiếng Việt; gõ tắt cũng tự gợi ý đúng sản phẩm; có dùng thử miễn phí 300 đơn | Thiết kế cho quán ăn, tên món ngắn; chưa rõ độ chính xác với tên model điện tử dài; trả phí sau dùng thử | Đã có tiền lệ AI giải đúng bottleneck "ghi nhận lúc bận" ở Việt Nam. Nhóm cần **kiểm chứng với danh mục hàng điện tử** (giả định #5) trước khi tự xây |
| **MISA AMIS CRM — Thêm đơn hàng bằng AI** | https://amis.misa.vn/274495/them-don-hang-bang-ai-tren-misa-amis-crm-nhanh-hon-chinh-xac-hon-tiet-kiem-80-thoi-gian/ | **Ghi nhận giao dịch** từ ngôn ngữ tự nhiên, ảnh hoặc file PDF | AI trích xuất thông tin và tạo sẵn đơn đầy đủ dữ liệu; sửa đơn bằng cách nhập yêu cầu | Dành cho nhân viên kinh doanh doanh nghiệp (CRM), quá nặng cho cửa hàng nhỏ; con số "tiết kiệm 80%" là của bên bán | Pattern "**ảnh hoặc câu nói → đơn nháp → người xác nhận**" áp dụng được cho giấy ghi tạm cuối ngày (snapshot #2) |
| **KiotViet** (phần mềm quản lý bán hàng) | https://apps.apple.com/vn/app/kiotviet/id1146695068 | Lưu giao dịch → tự trừ tồn kho → tra lịch sử bán và giá | Phổ biến ở Việt Nam; cảnh báo hàng tồn; chạy trên điện thoại và máy tính | Có phí hằng tháng; nhiều tính năng nên người mới dễ bối rối; vẫn cần người nhập giao dịch | Phần tra giá và tính tồn đã giải được bằng logic cố định. **AI không cần làm lại phần này**, chỉ cần đưa dữ liệu vào đúng và đủ |
| **Sapo POS** | https://www.sapo.vn/blog/hang-ton-kho-la-gi | Theo dõi xuất – nhập – tồn từng sản phẩm | Hơn 20 báo cáo kho; app Android và iOS; nhiều người dùng chung một dữ liệu | Có phí sau dùng thử; phải nhập danh mục hàng và giá ban đầu | Dữ liệu dùng chung giải pain của người hỗ trợ bán ("phải hỏi lại người nhà vì không nhớ giá") |
| **MISA eShop** | https://www.misaeshop.vn/?p=50457 | Ghi nhận tại quầy (quét mã vạch, tính tiền, in hóa đơn) → báo cáo doanh thu, tồn kho | Bản mobile miễn phí trọn đời cho hộ kinh doanh doanh thu ≤ 1 tỷ/năm | Hộ doanh thu trên 1 tỷ/năm trả phí sau 3 tháng; hàng không có mã vạch vẫn phải chọn tay | Quét mã vạch là phương án **không dùng AI** để so sánh ở CP6: nếu đa số hàng có mã vạch, có thể không cần AI ở bước ghi nhận |

**Kết luận research:**

- Phần **lưu trữ, trừ tồn kho, tra lịch sử giá** đã được phần mềm bán hàng có sẵn giải bằng logic cố định, nên nhóm không xây lại.
- Khoảng trống thật là **bước ghi nhận lúc đông khách**. Thị trường đã có công cụ AI chuyển giọng nói hoặc ảnh thành đơn hàng (Knote, MISA AMIS CRM), nghĩa là điểm can thiệp AI này **khả thi và có tiền lệ**.
- Hướng đề xuất cho CP5–6: **trợ lý AI ở bước ghi nhận**. Người bán nói một câu hoặc chụp ảnh giấy ghi tạm → AI tạo giao dịch nháp → người bán xác nhận → phần mềm bán hàng lưu và tự trừ tồn kho. Trước khi chốt, nhóm phải so sánh với phương án quét mã vạch (No AI) và kiểm chứng giả định #4, #5.

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại (As-Is Process)

Sơ đồ quy trình hiện tại:

```text
[Khách hỏi thông tin sản phẩm / giá bán / lịch sử mua]
       │
       ▼
[Nhân viên/Chủ cửa hàng mở sổ sách ghi chép & hỏi người thân]
       │
       ▼
[Tra cứu thủ công qua sổ chép tay / file ghi riêng lẻ] ──▶ (BOTTLENECK)
       │
       ▼
[Đi ra kho/kệ hàng thực tế để kiểm tra số lượng tồn và đối chiếu]
       │
       ▼
[Báo lại giá/tình trạng tồn cho khách & Ghi chép giao dịch thủ công]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Khách hàng & Người bán | Tên sản phẩm / Yêu cầu tra giá bán hoặc số lượng | Nhu cầu tra cứu thông tin sản phẩm | 1 - 2 phút / lượt | Khách hỏi trực tiếp tại cửa hàng hoặc qua điện thoại/Zalo |
| 2 | Người bán | Nhu cầu tra cứu | Thông tin lịch sử sổ chép tay / File excel lẻ | 2 - 3 phút / lượt | Ghi chép không đồng bộ, nhiều sổ theo từng mốc thời gian |
| 3 | Người bán | Sổ chép tay / Bộ nhớ cá nhân | Giá bán đợt trước & Lịch sử xuất bán | **5 - 10 phút / lượt** | **Bottleneck chính:** Tìm lại giá bán cũ, giao dịch chưa ghi chép đầy đủ |
| 4 | Người bán | Thông tin tra cứu sổ sách | Số lượng thực tế trên kệ/kho | 3 - 5 phút / lượt | Phải trực tiếp ra kho kiểm tra đối chiếu vì số liệu ghi chép thiếu chính xác |
| 5 | Người bán & Khách hàng | Thông tin chốt | Báo giá cho khách & Ghi nhận sổ bán | 2 - 3 phút / lượt | Ghi tay thông tin bán mới vào sổ |

**Bottleneck chính:** Bước 3 (Khâu tìm lại giá bán cũ và lịch sử giao dịch trong sổ sách thủ công tốn thời gian, dễ nhầm lẫn do ghi chép không đầy đủ và thông tin bị phân tán).

---

### 4.2. Quy trình tương lai (To-Be Process - Mức Workflow AI + Human-in-the-Loop)

Phân định rõ ràng vai trò **Rule**, **AI**, **Con người (Human)**, **Boundary** và **Phương án quay về (Fallback)**:

```text
[Khách hỏi thông tin sản phẩm / lịch sử mua]
       │
       ▼
(Rule) [Nhập liệu thông tin bán lẻ / quét mã QR chuẩn hóa vào CSDL]
       │
       ▼
(AI Workflow) [AI RAG truy xuất nhanh lịch sử giá, tồn kho & gợi ý báo giá]
       │
       ▼
(Con người - HITL) [Người bán xác nhận thông tin, duyệt giá & báo khách] ──▶ [Chốt đơn]
```

* **Bước 1 (Rule-based):** Chuẩn hóa khâu nhập liệu. Mỗi giao dịch nhập - xuất - bán hàng được nhập vào hệ thống CSDL tập trung theo biểu mẫu cố định (Rule-based Form / Quét mã SKU/QR).
* **Bước 2 (AI Workflow - RAG/Natural Language Query):** Khi người bán cần tìm thông tin, AI đóng vai trò Trợ lý tra cứu (dùng RAG/NL2SQL). Người bán chỉ cần gõ hoặc nói: *"Sản phẩm X tuần trước bán giá bao nhiêu?"* hoặc *"Tồn kho mã Y còn mấy cái?"*, AI sẽ truy xuất và trả kết quả chính xác trong 3 giây.
* **Bước 3 (Con người & Boundary):** Người bán trực tiếp đối soát và trả lời khách hàng. **Boundary (Ranh giới):** AI chỉ có quyền **tra cứu, tổng hợp và gợi ý** thông tin lịch sử giao dịch/tồn kho dựa trên dữ liệu đã ghi nhận, **tuyệt đối không** tự ý thay đổi giá bán chính thức, không tự tạo đơn hàng nếu chưa được con người xác nhận.
* **Bước 4 (Human-in-the-Loop):** Người bán là người chịu trách nhiệm kiểm tra lại thông tin gợi ý từ AI và đưa ra quyết định bán hàng cuối cùng.
* **Phương án quay về (Fallback):** Nếu hệ thống AI gặp sự cố hoặc dữ liệu đầu vào chưa kịp cập nhật, người bán chủ động chuyển về quy trình tra cứu bảng tính/sổ sách thủ công và kiểm tra trực tiếp tại kho để không làm gián đoạn việc bán hàng.

---

### 4.3. Before / after (So sánh trước và sau khi cải tiến)

| Chỉ số | Trước (As-Is) | Sau (Kỳ vọng To-Be) | Ghi chú |
|---|---:|---:|---|
| **Số bước** | 5 bước | 3 bước | Tinh gọn khâu tìm kiếm và đi đối chiếu kho thực tế |
| **Tổng thời gian** | ~13 - 23 phút/lượt tra cứu | ~1 - 3 phút/lượt tra cứu | Rút ngắn đáng kể thời gian khách hàng phải chờ đợi |
| **Số bước thủ công** | 5/5 bước | 1/3 bước (khâu xác nhận cuối) | AI tự động hóa hoàn toàn khâu tìm kiếm & tính toán tồn kho |
| **Bottleneck chính** | Tìm lại thông tin giá bán và giao dịch cũ trong sổ sách | Kiểm tra tính chính xác của dữ liệu đầu vào | Dịch chuyển từ "tìm kiếm thủ công" sang "chuẩn hóa dữ liệu" |
| **Rủi ro mới phát sinh** | Thiếu dữ liệu nếu người bán quên ghi nhận giao dịch mới | Khắc phục bằng giao diện nhập liệu siêu nhanh (Rule-based form/Mã QR) |

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Chủ cửa hàng điện tử và các thành viên trực tiếp ghi nhận, tra cứu và quản lý hàng hóa, giao dịch bán hàng |
| **Quy trình** | Khi cần kiểm tra một sản phẩm, người quản lý tìm thông tin trong sổ hoặc các nguồn ghi chép, đối chiếu lịch sử nhập và bán, kiểm tra hàng thực tế, tính số lượng còn lại rồi mới trả lời khách hoặc quyết định nhập thêm hàng |
| **Bottleneck** | Bước tìm và đối chiếu lịch sử giao dịch với hàng thực tế mất nhiều thời gian vì dữ liệu nhập, xuất, giá bán và số lượng chưa được ghi nhận đầy đủ, thống nhất và tập trung |
| **Impact** | Người quản lý mất thời gian tra cứu, khó xác định chính xác giá bán cũ và tồn kho, có nguy cơ trả lời khách sai, thiếu hàng bất ngờ hoặc ra quyết định nhập hàng dựa trên dữ liệu không đầy đủ |
| **Success Metric** (baseline → target, cách đo) | Baseline tạm ước lượng: 15–30 phút cho một lần tra cứu phức tạp → Target: dưới 5 phút/lần; đồng thời giảm số lần phải kiểm đếm lại hàng thực tế. Cách đo: ghi thời điểm bắt đầu và kết thúc của ít nhất 10 lượt tra cứu trước và sau pilot, đồng thời ghi số trường hợp dữ liệu hệ thống lệch với hàng thực tế |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không tự tạo hoặc sửa giao dịch, không tự điều chỉnh tồn kho, không quyết định giá bán và không suy đoán khi thiếu dữ liệu. Chủ cửa hàng hoặc người quản lý phải kiểm tra kết quả trước khi trả lời khách, báo giá, nhập hàng hoặc điều chỉnh tồn kho |

**Phản biện nhận được và cách nhóm xử lý:**

- Phản biện: Vấn đề cốt lõi có thể là dữ liệu chưa được ghi nhận đầy đủ chứ không phải thiếu công cụ AI.
- Nhóm đồng ý. Quy trình tương lai ưu tiên biểu mẫu chuẩn và Rule để ghi nhận, kiểm tra và cập nhật tồn kho. AI chỉ là khả năng bổ sung sau khi dữ liệu đủ và đáng tin cậy.
- Phản biện: Baseline 15–30 phút hiện mới là ước lượng.
- Nhóm đồng ý. Trước khi nộp bản cuối, nhóm cần thay bằng số liệu đo từ ít nhất 5–10 lần tra cứu thực tế hoặc từ kết quả phỏng vấn CP4.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: độ mơ hồ **thấp–trung bình** × độ phức tạp **trung bình** → phù hợp mức **Workflow**.

Vì sao:
- Độ mơ hồ thấp–trung bình: câu hỏi cần trả lời rõ ràng và kiểm chứng được (hàng X đã bán chưa, giá bao nhiêu, còn tồn bao nhiêu). Phần mơ hồ nằm ở dữ liệu đầu vào: ghi chép không đồng nhất, một sản phẩm có nhiều mức giá bán.
- Độ phức tạp trung bình: quy trình có nhiều bước nối nhau (ghi nhận → lưu → tra cứu → đối chiếu → tính tồn → kiểm hàng thực tế), nhưng mỗi bước có quy tắc khá rõ, không cần AI tự lập kế hoạch hay tự ra quyết định.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Dùng phần mềm bán hàng/kho hoặc bảng tính, ghi đầy đủ từng giao dịch nhập, xuất, số lượng, giá bán. | Gia đình ghi chép đều đặn và chỉ cần tra cứu theo bộ lọc cố định. | Phải nhập tay nhiều, dễ bỏ thói quen sau vài tuần; tra cứu vẫn phải thao tác thủ công. | Làm trước (nền bắt buộc) |
| **Rule** | Bảng tính có công thức tự tính tồn, cảnh báo khi tồn dưới ngưỡng, bộ lọc theo mã hàng. | Mã sản phẩm đã chuẩn hóa, câu hỏi lặp lại và cố định. | Cứng nhắc: không hiểu cùng một sản phẩm được gọi tên khác nhau, không đọc được ghi chú tự do. | Một phần |
| **Workflow** | Ghi chép/tin nhắn/ảnh hóa đơn → AI trích xuất thành bản ghi chuẩn → người xác nhận → lưu vào bảng → hỏi đáp tra cứu trên dữ liệu đã lưu. | Có dữ liệu giao dịch ở mức tối thiểu và có người xác nhận ở từng bước. | AI trích sai số lượng hoặc giá; người dùng lười xác nhận. | **Chọn** |
| **Agent** | AI tự theo dõi tồn, tự đề xuất nhập hàng, tự đối chiếu và điều chỉnh giá. | Dữ liệu đầy đủ, ổn định và có cơ chế kiểm soát chặt. | Sai tồn kho hoặc giá gây thiệt hại thật; dữ liệu hiện chưa đủ; quá nặng cho cửa hàng gia đình. | Không |

**Mức chọn:** Workflow, đặt trên nền No AI/Rule (chuẩn hóa ghi chép trước khi ứng dụng AI).

**Vì sao không chọn mức đơn giản hơn:** Rule thuần không xử lý được ghi chép không đồng nhất (tên sản phẩm viết nhiều kiểu, nhiều mức giá cho cùng một mặt hàng, ghi chú tự do). No AI giải quyết được việc ghi đầy đủ nhưng chưa giải quyết việc tra cứu nhanh bằng câu hỏi tự nhiên. Vì vậy giữ No AI/Rule làm bước 0 (chuẩn hóa dữ liệu), rồi thêm AI ở bước trích xuất và tra cứu.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Trích xuất ghi chép, tin nhắn, ảnh hóa đơn thành bản ghi có cấu trúc (sản phẩm, số lượng, giá, ngày, loại nhập/xuất); trả lời câu hỏi tra cứu: hàng đã bán chưa, giá bán từng lần, số lượng đã xuất, tồn dự tính. |
| **Judgment** — con người cân nhắc, quyết định gì? | Người trong gia đình xác nhận hoặc sửa bản ghi AI trích xuất; quyết định khi tồn trên sổ lệch với hàng thực tế; quyết định khi cùng một sản phẩm có nhiều mức giá. |
| **Action** — hành động cuối cùng là gì, ai làm? | Lưu bản ghi đã xác nhận vào bảng/phần mềm; kiểm hàng thực tế khi có lệch. Người làm: thành viên gia đình trực tiếp quản lý cửa hàng. |
| **Outcome** — đo kết quả bằng gì? | Thời gian tra cứu mỗi lần (baseline cần đo); % giao dịch được ghi đầy đủ; mức lệch tồn giữa sổ và hàng thực tế; % câu trả lời đúng khi kiểm tra lại. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Ghi chép/sổ sách giao dịch, danh mục sản phẩm, hóa đơn nhập hàng; mỗi lần hỏi cần tên sản phẩm và khoảng thời gian. Hiện chưa có đủ (ghi chép chưa đầy đủ từng giao dịch) nên phải bắt đầu ghi chuẩn trước. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Người dùng bấm đúng/sai hoặc sửa trực tiếp bản ghi; kiểm kê định kỳ so với số liệu AI trả về; nhật ký các câu hỏi AI không trả lời được hoặc trả lời sai. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? **Augment.** Bằng chứng: quy trình hiện tại luôn kết thúc bằng bước kiểm hàng thực tế tại cửa hàng/kho; giá bán thay đổi theo từng giao dịch nên cần người quyết định; dữ liệu chưa đầy đủ nên chưa thể giao hẳn việc cho AI.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? **Bỏ sót tệ hơn.** Vì nếu AI bỏ sót một giao dịch hoặc báo còn hàng trong khi đã bán, sổ sẽ lệch, có thể hứa hàng với khách rồi không có, hoặc mất tiền mà không biết; còn báo nhầm "có lệch" thì chỉ tốn công kiểm lại. Thiết kế đã xử lý: AI chỉ trả lời từ dữ liệu đã lưu và nói rõ "không tìm thấy/không chắc" thay vì đoán; mỗi câu trả lời kèm bản ghi gốc để đối chiếu; không tự ghi vào sổ khi chưa được xác nhận; ưu tiên cảnh báo thừa hơn bỏ sót; kiểm kê định kỳ để bắt các lệch AI không thấy.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Thành viên trong gia đình trực tiếp bán hàng và quản lý cửa hàng điện tử. |
| **Quy trình** | Ghi nhận hàng hóa/giao dịch → tìm lại trong sổ khi cần → đối chiếu hàng nhập và hàng đã bán → tính số lượng còn lại → kiểm hàng thực tế tại cửa hàng/kho. |
| **Bottleneck** | Bước tìm lại và đối chiếu thông tin, vì giao dịch ghi chưa đầy đủ, kết hợp nhiều cách quản lý và một sản phẩm có nhiều mức giá bán. Chưa có số phút cụ thể (cần đo). |
| **Impact** | Khó nắm chính xác hàng đã xuất, giá từng giao dịch và số lượng tồn; gây khó khăn trong kiểm soát hàng hóa và quản lý kinh doanh. |
| **Success Metric** (baseline → target, cách đo) | Baseline (cần đo trong 1–2 tuần): thời gian trung bình mỗi lần tra cứu; % giao dịch có bản ghi đầy đủ; mức lệch giữa tồn sổ và tồn thực tế khi kiểm kê. Target (đề xuất, chốt sau khi có baseline): giảm thời gian tra cứu ít nhất một nửa; ≥ 90% giao dịch mới được ghi đầy đủ; mức lệch tồn giảm so với baseline. Cách đo: bấm giờ vài lần tra cứu mẫu, kiểm kê định kỳ so với sổ, đếm bản ghi đủ/thiếu. |
| **Boundary** | Chỉ làm: tra cứu lịch sử bán, giá bán, số lượng đã xuất và tồn của sản phẩm tại cửa hàng này. Không làm: tự nhập hàng, tự đặt giá, kế toán/thuế, tự ghi sổ khi chưa được xác nhận. |
| **AI intervention point** | (1) Bước trích xuất ghi chép/hóa đơn thành bản ghi chuẩn. (2) Bước tra cứu và tổng hợp thông tin trên dữ liệu đã xác nhận. |
| **Mức chọn** | Workflow |
| **Rủi ro & người kiểm tra** | Rủi ro: AI trích sai số lượng/giá; AI "bịa" khi thiếu dữ liệu; lộ dữ liệu kinh doanh. Người kiểm tra: chủ cửa hàng/thành viên gia đình xác nhận bản ghi và kiểm kê định kỳ. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Success metric | Chưa có số liệu, chỉ ghi "tra cứu nhanh hơn" | Có 3 chỉ số cần đo baseline và target đề xuất | AI phản biện chỉ ra thiếu số liệu; đồng ý và không tự đặt số khi chưa đo. |
| Phạm vi AI | "Tìm kiếm, tổng hợp, trả lời câu hỏi" chung chung | Hai điểm can thiệp rõ: trích xuất và tra cứu, có người xác nhận | Tránh dùng AI cho toàn bộ quy trình quản lý. |
| Điều kiện dữ liệu | Giả định dữ liệu "đã được ghi nhận đầy đủ" | Thêm bước chuẩn hóa ghi chép trước khi ứng dụng AI | Dữ liệu thiếu thì AI không tra cứu chính xác được. |
| Boundary | Chưa có | Thêm danh sách làm / không làm | Giữ phạm vi vừa sức, tránh trượt sang Agent. |
| Mức can thiệp | "Cảm nhận nhanh: Workflow" | Workflow có lý do, so sánh với 3 mức còn lại | Chuyển từ cảm nhận sang quyết định có lập luận. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đúng dữ liệu | Số lượng, giá, ngày khớp bản ghi gốc trên bộ câu hỏi kiểm tra | Sai số lượng/giá so với bản ghi gốc |
| 2 | Trung thực khi thiếu dữ liệu | Nói rõ "không tìm thấy/không chắc" khi không có bản ghi | Tự suy đoán hoặc bịa thông tin |
| 3 | Truy vết được nguồn | Mỗi câu trả lời kèm bản ghi gốc để đối chiếu | Trả lời không có nguồn, người dùng không kiểm tra được |
| 4 | Dễ sửa | Người dùng sửa một bản ghi sai nhanh, không cần nhập lại từ đầu | Muốn sửa phải làm lại cả quy trình |
| 5 | Tiết kiệm thời gian | Thời gian tra cứu thấp hơn baseline đã đo | Không nhanh hơn cách tra sổ hiện tại |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | TB | Pain có thật (khó tra giá, số lượng đã xuất, tồn kho) và gia đình là người trực tiếp chịu. Nhưng chưa đo tần suất, chưa có số phút, chưa phỏng vấn người nhà nên chưa chắc họ sẽ chủ động dùng. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | TB | Thiết kế có bước xác nhận/sửa và dẫn nguồn bản ghi nên dễ kiểm tra. Rủi ro: người nhà không quen công nghệ, quen cách ghi cũ và có thể bỏ qua bước xác nhận. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Cao | Công cụ có sẵn (AI trích xuất, bảng tính), nhưng dữ liệu là điểm yếu nhất: giao dịch ghi chưa đầy đủ, nhiều cách ghi, chưa có danh mục sản phẩm chuẩn. Chưa chuẩn hóa dữ liệu thì AI không đạt độ chính xác. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | TB | Chi phí thấp với quy mô cửa hàng nhỏ. Cần cân nhắc việc đưa dữ liệu kinh doanh (giá nhập, doanh thu) lên dịch vụ AI và quy định hóa đơn/thuế nếu dùng làm sổ chính thức. Người vận hành hiện là bản thân bạn và gia đình nhập liệu, dễ phụ thuộc vào một người. |

### 8.2. Kết luận

**Quyết định:** Cải thiện thêm sau khi nghe nhận đóng góp

**Lý do:**
- Rủi ro Feasibility đang ở mức Cao: giao dịch ghi chưa đầy đủ, nhiều cách ghi chép, chưa có danh mục sản phẩm chuẩn. Nếu dựng AI ngay, kết quả tra cứu sẽ không đáng tin vì thiếu dữ liệu đầu vào.
- Chưa có baseline (thời gian tra cứu, tần suất lệch tồn, mức độ đầy đủ của dữ liệu) nên chưa chứng minh được vấn đề đủ lớn và chưa có mốc để biết AI có cải thiện hay không.
- Value mới chỉ dựa trên trải nghiệm của bản thân, chưa phỏng vấn hoặc quan sát người nhà, nên chưa biết họ có chịu ghi chép và xác nhận bản ghi hay không.
- Phương án No AI/Rule (chuẩn hóa ghi chép, bảng tính có công thức) rẻ, làm được ngay và là điều kiện bắt buộc cho Workflow, nên nên làm trước.

**Nếu Go — pilot nhỏ nhất:**
Chỉ làm với 1 nhóm hàng (ví dụ phụ kiện điện tử) trong 2 tuần. Gia đình ghi đầy đủ giao dịch nhập/xuất vào một bảng chuẩn. AI chỉ làm hai việc: trích xuất ghi chép/ảnh hóa đơn thành bản ghi và trả lời 3 loại câu hỏi (đã bán chưa, giá bán gần nhất, còn tồn bao nhiêu). Mọi bản ghi đều do người xác nhận. Cuối tuần 2 kiểm kê và đối chiếu với số liệu AI trả về.

**Nếu Not Yet — cần kiểm chứng gì trước:**
1. **Đo baseline** trong 1–2 tuần: bấm giờ các lần tra cứu, đếm số lần phải tìm lại sổ, ghi nhận số lần lệch tồn khi kiểm kê.
2. **Chuẩn hóa dữ liệu:** lập danh mục sản phẩm có mã thống nhất, mẫu ghi chép cố định cho nhập/xuất/bán, và kiểm tra gia đình có duy trì ghi đủ giao dịch không (đo % giao dịch có bản ghi đầy đủ).
3. **Phỏng vấn/quan sát người nhà:** họ thấy bước nào đau nhất, sẵn sàng nhập hoặc xác nhận bản ghi bằng cách nào (gõ, nhắn tin, chụp ảnh).
4. **Thử AI trên dữ liệu mẫu nhỏ** (khoảng 20–30 bản ghi thật) để xem AI trích xuất có đủ đúng không trước khi dựng cả luồng.

**Nếu No-Go — nên làm gì thay AI:**
Dùng phần mềm quản lý bán hàng và kho, hoặc bảng tính có công thức tự tính tồn và bộ lọc theo mã hàng. Đặt quy tắc ghi chép bắt buộc cho mỗi giao dịch (ngày, mã hàng, số lượng, giá, nhập/xuất) và kiểm kê định kỳ hằng tuần/tháng.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):
- Nếu sau **2 tuần** chuẩn hóa mà **dưới 70% giao dịch** được ghi đầy đủ → dừng việc dựng AI, quay về No AI (phần mềm/bảng tính) và tìm hiểu vì sao gia đình khó duy trì ghi chép.
- Nếu sau **2 tuần pilot** mà AI **trích xuất/tra cứu sai quá 10% số câu** trong bộ kiểm tra, hoặc **thời gian tra cứu không nhanh hơn baseline** → quay về Rule (bảng tính có công thức, bộ lọc cố định).

*(Các ngưỡng 70% và 10% là đề xuất ban đầu, cần chỉnh lại sau khi có baseline thực tế.)*

---

## 9. Hạn chế và hướng tiếp theo

- Bài chưa có số liệu đo thực tế (thời gian tra cứu, tần suất lệch tồn, % giao dịch ghi đủ); các target hiện chỉ là đề xuất.
- Value và Usability mới dựa trên trải nghiệm cá nhân, chưa phỏng vấn hay quan sát các thành viên khác trong gia đình.
- Chưa thử AI trên dữ liệu thật nên chưa biết độ chính xác khi trích xuất ghi chép viết tay hoặc ảnh hóa đơn.
- Chưa đánh giá kỹ vấn đề bảo mật dữ liệu kinh doanh (giá nhập, doanh thu) khi dùng dịch vụ AI bên ngoài, và quy định hóa đơn/thuế.
- Hướng tiếp theo: hỗ trợ nhập hàng từ nhiều nguồn ; dùng máy quét hình ảnh để AI hỗ trợ lưu trữ đầu vào của người dùng ; dùng AI để trích suất dữ liệu từ kho

## 10. Tài liệu tham khảo

- Repo nhóm: K5--L3A--DAY02-PhuongHoang-DiscoveryProblemFraming (https://github.com/MHuyHoat/K5--L3A--DAY02-PhuongHoang-DiscoveryProblemFraming)
- Template và hướng dẫn bài tập: docs/01-worksheet.md (trong repo nhóm)
- Google PAIR, *People + AI Guidebook* (augment vs automate, lỗi báo nhầm vs bỏ sót): https://pair.withgoogle.com/guidebook
- Agrawal, Gans, Goldfarb, *Prediction Machines* (khung Prediction – Judgment – Action – Outcome của AI Canvas)
- Marty Cagan, *Inspired* (bốn rủi ro sản phẩm: Value, Usability, Feasibility, Viability)
- Có sử dụng AI hỗ trợ gợi ý và phản biện nội dung; các nhận định cuối cùng do tôi tự kiểm tra và quyết định.
