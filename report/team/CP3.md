# Hội tụ nhóm — Opportunity Solution Tree và chấm điểm candidate

## 1. Các candidate problem của nhóm

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

## 2. Opportunity Solution Tree (OST)

### Outcome khi hội tụ

Nhóm không cố gộp cả 6 candidate vào một sản phẩm chung. OST được sử dụng để phân biệt:

- **Outcome:** kết quả muốn cải thiện.
- **Opportunity:** pain hoặc nhu cầu của người dùng.
- **Solution:** những cách có thể can thiệp để giải quyết opportunity.

Candidate được chọn để tiếp tục discovery là **quản lý kho cho hộ kinh doanh nhỏ**.

### OST của candidate được chọn

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

## 3. Tiêu chí chấm điểm candidate

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

## 4. Bảng chấm điểm candidate

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

## 5. Lý do chấm điểm

### Rank 1 — Quản lý kho cho hộ kinh doanh nhỏ — 34/35

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

### Rank 2 — Camera hỗ trợ điểm danh — 32/35

**Điểm mạnh:**

- Actor rõ: giảng viên/giáo viên và học sinh, sinh viên.
- Quy trình điểm danh hiện tại dễ quan sát.
- Impact dễ đo bằng thời gian điểm danh và tỷ lệ sai sót.
- Nhóm dễ tiếp cận người dùng để khảo sát.

**Điểm chưa chắc:**

- Có nhiều giải pháp đơn giản hơn như QR, mã lớp, NFC hoặc thẻ sinh viên.
- Camera AI có rủi ro về ánh sáng, góc camera, nhận diện nhầm, dữ liệu khuôn mặt và quyền riêng tư.
- Cần chứng minh camera tạo giá trị đủ lớn so với Rule đơn giản.

### Rank 3 — Lọc và so sánh phòng/căn hộ — 32/35

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

### Rank 4 — Chẩn đoán hình ảnh xe tại gara — 27/35

**Điểm mạnh:**

- Impact có thể lớn vì liên quan trực tiếp tới kiểm tra và sửa xe.
- Có use case rõ cho Computer Vision.

**Điểm yếu:**

- Cần dữ liệu ảnh lỗi xe có nhãn.
- Cần chuyên gia kỹ thuật xác minh kết quả.
- AI chẩn đoán sai có thể dẫn đến kiểm tra hoặc sửa chữa sai hướng.
- Nhóm khó tiếp cận dữ liệu và chuyên môn hơn ba candidate phía trên.

### Rank 5 — Đối chiếu JD và sửa CV — 27/35

**Điểm mạnh:**

- Actor rõ: sinh viên năm 3/4 chuẩn bị xin việc.
- Dễ tìm người dùng khảo sát và pilot bằng JD, CV.

**Điểm yếu:**

- Thị trường đã có nhiều công cụ ATS, keyword matching, CV review.
- Một phần problem có thể giải bằng Rule hoặc checklist.
- Nếu không kiểm soát phạm vi, AI dễ chuyển thành viết lại CV hoặc tạo kinh nghiệm không có thật.
- Cần xác định pain chính là thiếu keyword, khó viết bullet hay chưa hiểu JD.

### Rank 6 — Tìm tài liệu học tập và hướng dẫn LAB — 26/35

**Điểm mạnh:**

- Actor rất dễ tiếp cận; pain quen thuộc với sinh viên.
- Quy trình dễ khảo sát.

**Điểm yếu:**

- Root cause rộng: tài liệu rải rác, không biết từ khóa, chưa tổ chức tài liệu hoặc tài liệu thực sự chưa tồn tại.
- Tổ chức tài liệu và search thông thường có thể đã giải quyết phần lớn problem.
- Impact khó đo rõ hơn các candidate khác.
- Khó chứng minh AI tạo thêm giá trị nếu nguồn tài liệu chưa chuẩn hóa.

---

## 6. Candidate được nhóm chọn

Nhóm thống nhất chọn hướng đề tài:

> **AI Agent hỗ trợ quản lý kho hàng dành cho người dùng lớn tuổi tại các hộ kinh doanh nhỏ.**

Tuy nhiên, sau phản biện, nhóm **không mặc định phải xây AI Agent ngay từ đầu**.

**Problem được giữ lại để tiếp tục discovery:**

> **Người quản lý tại các hộ kinh doanh nhỏ gặp khó khăn trong việc ghi nhận, tra cứu và đối chiếu thông tin nhập – xuất – tồn kho, đặc biệt khi dữ liệu đang được quản lý thủ công hoặc phân tán.**

Việc có cần AI hay không và mức can thiệp Rule, Workflow hay Agent sẽ được quyết định sau bước validation.

---

## 7. Vì sao chọn candidate quản lý kho

### 7.1. Có người dùng thật để tiếp cận

Một thành viên có thể trực tiếp quan sát và phỏng vấn người đang quản lý cửa hàng/hộ kinh doanh.

### 7.2. Pain có tác động thực tế

Sai lệch tồn kho có thể ảnh hưởng trực tiếp tới nhập hàng, bán hàng, kiểm kê, doanh thu và quản lý vốn.

### 7.3. Quy trình hiện tại tương đối rõ

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

### 7.4. Có bottleneck đáng kiểm chứng

Khâu ghi nhận và tìm lại dữ liệu có thể thiếu đầy đủ hoặc nhất quán, khiến việc kiểm tra tồn kho phải đối chiếu nhiều nguồn. Đây vẫn là **giả thuyết**, chưa phải kết luận sau khảo sát.

### 7.5. Có thể so sánh nhiều mức giải pháp

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

## 8. Vì sao không chọn các candidate còn lại

### Camera hỗ trợ điểm danh

- Có nhiều phương án đơn giản hơn camera AI như QR hoặc NFC.
- Phải xử lý dữ liệu khuôn mặt, quyền riêng tư và nguy cơ nhận diện sai.
- Nếu pain chủ yếu là thời gian điểm danh thì Rule đơn giản có thể đủ tốt.

**Kết luận:** Nguy cơ sử dụng công nghệ phức tạp hơn mức problem yêu cầu (**over-engineering**).

### Lọc và so sánh phòng/căn hộ

- Dữ liệu phụ thuộc sale/chủ nhà và các nền tảng bên ngoài.
- Tin đăng có thể sai hoặc lỗi thời; khó kiểm soát trạng thái còn phòng theo thời gian thực.
- Việc phát hiện listing trùng có nhiều trường hợp khó xác định.
- Nhóm kiểm soát được ít phần của data pipeline hơn bài quản lý kho.

**Kết luận:** Pain có thật và actor rõ nhưng Feasibility Risk cao hơn candidate được chọn.

### Chẩn đoán hình ảnh xe tại gara

- Cần dữ liệu chuyên ngành và người có chuyên môn xác nhận kết quả.
- Sai sót có hậu quả cao hơn.
- Phạm vi Computer Vision tương đối lớn.

### Đối chiếu JD và sửa CV

- Có nhiều sản phẩm tương tự trên thị trường.
- Một phần problem có thể giải bằng keyword matching.
- Cần nghiên cứu thêm để xác định khoảng trống thực sự.

### Tìm tài liệu học tập và hướng dẫn LAB

- Problem còn rộng và root cause chưa rõ.
- Có khả năng chỉ cần tổ chức lại tài liệu và cải thiện search.
- Impact khó định lượng hơn các candidate khác.

---

## 9. Kết luận hội tụ

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
