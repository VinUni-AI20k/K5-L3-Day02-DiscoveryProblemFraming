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
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

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

### 7.1. Problem Statement v1

| Trường | Nội dung |
|---|---|
| **Actor** | Chuyên viên phụ trách đánh giá thầu (Phó kiến trúc sư / KTKT); Lãnh đạo dự án |
| **Quy trình** | 1. Tiếp nhận 4 file chào giá. 2. Kiểm mẫu (file đúng/sai). 3. Gom 3 file đúng mẫu (copy × 7 sheet). 4. Ghép 1 file sai mẫu vào mã dòng BOQ. 5. Kiểm tổng tiền khớp file gốc. **[Phần gom: 6–7h]** 6. Dò từng dòng: so khối lượng chào ≠ BOQ; so đơn giá chênh >30% vs trung vị 4 nhà thầu; tô màu dòng bất thường (~4h trên ~16.000 dòng). **[Phần soát: 5–6h]** 7. Cộng phát sinh, ghi chú lý do chênh lệch. 8. Trình lãnh đạo. |
| **Bottleneck** | **Chính (Bước 6):** Dò ~16.000 dòng (4.100 BOQ × 4 nhà thầu) bằng mắt → ~4h/vòng; rủi ro sót 1–2 dòng = sai lệch giá hàng tỷ. **Phụ (Bước 4):** Ghép file sai mẫu → ~2.5h nếu có. **Tổng:** 11–13h/vòng, 2 vòng/gói = 22–26h/gói. |
| **Impact** | Chuyên viên mất nhiều thời gian soát thủ công; nguy cơ bỏ sót chênh lệch (sót dòng = sai hàng tỷ VND); lãnh đạo không có cơ sở dữ liệu đầy đủ để so sánh công bằng; khi phát hiện sai ở vòng 2, phải làm lại toàn bộ. |
| **Success Metric** (baseline → target, cách đo) | **(1) Thời gian soát:** 5–6h/vòng → < 1.5h/vòng (giảm ≥75%). Cách đo: bấm giờ mở file → chạy tool → đọc output → ghi chú. **(2) Phát hiện chênh khối lượng:** ~70–80% (sót 1–2 dòng/4.100) → 100% (0 sót). Cách đo: chạy tool trên file test 100 dòng (20 chênh thật); recall = detected/20. **(3) Không báo nhầm:** 0% → ≤2% FP. Cách đo: FP / 80 dòng bình thường. **(4) Phát hiện bất thường đơn giá:** ~60–70% → ≥90%. Cách đo: detect / ground_truth. **(5) Ghi chú đầy đủ:** Mọi dòng tô màu phải có ghi chú không trống. |
| **Boundary** | **AI/Rule KHÔNG được:** (1) Sửa khối lượng, đơn giá hay bất kỳ số liệu. (2) Tự xóa/bỏ qua dòng. (3) Kết luận nhà thầu nào đạt/rẻ/bị loại. (4) Tự gửi file. (5) Nhận dữ liệu chào giá qua công cụ chưa được cấp phép. **Con người PHẢI kiểm tra:** (a) Mọi mapping AI gợi ý (PC#2). (b) Tổng tiền phải khớp 100% file gốc. (c) Mọi dòng tô màu phải xem + ghi lý do trước khi trình. |
| **AI intervention point** | **Bước 2 (Rule):** Kiểm mẫu tự động. **Bước 3 (Rule):** Gom Power Query. **Bước 4 (AI, tùy chọn):** Gợi ý ghép dòng sai mẫu theo ý nghĩa (PC#2, Not Yet). **Bước 7 (Rule):** Công thức tính chênh, tô màu. **Bước 8 (Con người):** HITL xem + ghi chú. |
| **Mức chọn** | **Rule-based** cho PC#1 (soát chênh). **Not Yet** cho PC#2 (ghép sai mẫu) và AI. **No-Go** cho PC#3 (đánh giá năng lực). |
| **Rủi ro & người kiểm tra** | **(Value Risk):** Chưa đo hiệu quả phương án mới. Xử lý: pilot trên gói cũ. **(Usability Risk):** Chuyên viên quen Excel. Xử lý: giữ định dạng quen. **(Feasibility Risk):** File sai mẫu, mã khác nhau. Xử lý: tách bước kiểm/ghép/phát hiện. **(Viability Risk):** Chi phí triển khai, bảo mật. Xử lý: ưu tiên công cụ sẵn có, phân quyền. |

### 7.2. So sánh v0 (CP5) vs v1 (CP6)

| Trường | v0 (CP5) | v1 (CP6) | Thay đổi / Lý do |
|---|---|---|---|
| **Phạm vi** | Chưa rõ scope PC#1 vs PC#2 | PC#1 = bài toán chính (Rule). PC#2 = Not Yet (Workflow+AI). PC#3 = No-Go (Agent). | Làm rõ sau kiểm chứng CP4; phân tách rủi ro. |
| **Bottleneck** | "Bước 6 dò 16.000 dòng" (chung chung) | Rõ: bước 6 (~4h) chính, bước 4 (~2.5h) phụ. Tác động: 4h/(16h) = 25% soát. | Tính toán thời gian từng bước ở CP5. |
| **Impact** | "Khó so sánh giá công bằng" | Cụ thể: sót dòng = sai ~3 tỷ VND ở gói gần nhất. | Dữ liệu thực tế từ chuyên viên KTKT (Vinh). |
| **Success Metric** | "Giảm ≥50%, precision ≥90%" (mơ hồ) | 5 metric rõ: thời gian <1.5h, detect 100%, FP ≤2%, ≥90% bất thường, 100% ghi chú. | Xây dựng eval framework 8 section, mỗi metric có "cách đo". |
| **Boundary** | "Không sửa số, cần HITL" (tóm lại) | Chi tiết 5 điều AI không được + 3 khi con người phải kiểm. | Phản biện nhóm mạnh hơn về HITL ở từng bước. |
| **Quyết định** | v0 template chưa điền | Rõ: Go (Rule-based), Not Yet (PC#2), No-Go (PC#3). | Kết quả bỏ phiếu nhóm sau CP6. |

### 7.3. Tiêu chí đánh giá (5 criteria)

#### **C1: Độ chính xác phát hiện chênh khối lượng**
| Đạt | Không đạt |
|---|---|
| ✅ Phát hiện **100%** dòng có khối lượng chào ≠ BOQ | ❌ Sót >5% |
| ✅ Không báo nhầm (FP ≤2% trên dòng bình thường) | ❌ Báo nhầm >2% |
| ✅ Ghi rõ: khối lượng chào, BOQ, chênh lệch (%, tuyệt đối) | ❌ Ghi chú mơ hồ |
| ✅ Trace back được vị trí ở file gốc (sheet, dòng, cột) | ❌ Không ghi vị trí |

#### **C2: Chính xác phát hiện bất thường đơn giá**
| Đạt | Không đạt |
|---|---|
| ✅ Phát hiện **≥90%** dòng chênh >30% vs trung vị | ❌ Phát hiện <70% |
| ✅ Ghi: đơn giá từng nhà, trung vị, %, nhà nào chênh | ❌ Ghi chung chung |
| ✅ Mức cảnh báo rõ (CRITICAL >50%, WARNING >30%) | ❌ Không có cấp độ |
| ✅ Ngưỡng 30% được confirm lãnh đạo | ❌ Ngưỡng chỉ ước lượng |

#### **C3: Xử lý dữ liệu thiếu & định dạng sai**
| Đạt | Không đạt |
|---|---|
| ✅ Phát hiện **100%** ô trống (khối lượng, đơn giá) | ❌ Bỏ sót ô trống |
| ✅ Flag ô có ký tự không cần (khoảng trắng, tiền tệ, dấu) | ❌ Chấp nhận định dạng sai |
| ✅ Tất cả ô flag có ghi chú giải thích | ❌ Ghi chú mơ hồ |
| ✅ Chuyên viên sửa/skip được mà không ảnh output | ❌ Tool crash khi lỗi |

#### **C4: Truy nguồn & kiểm chứng**
| Đạt | Không đạt |
|---|---|
| ✅ Trace back cụ thể (sheet, row, col) trong file input | ❌ Output không ghi vị trí |
| ✅ Ghi rõ công thức (ví dụ: Chênh% = ABS(chào−BOQ)/BOQ) | ❌ Không ghi công thức |
| ✅ Kiểm chéo bằng tay được (input không bị thay đổi) | ❌ Tool thay input |
| ✅ Có phương án quay về (Rule fail → ghép tay) | ❌ Không phương án B |

#### **C5: Giảm thời gian + khả năng sử dụng**
| Đạt | Không đạt |
|---|---|
| ✅ Thời gian ≤1.5h/vòng hoặc ≥75% giảm | ❌ Giảm <50% hoặc không đo |
| ✅ Output xuất Excel/CSV (không format lại) | ❌ Output khó đọc |
| ✅ Chuyên viên chạy được không cần đào tạo lâu | ❌ Cách dùng phức tạp |
| ✅ Tool chạy máy thường (Excel, Power Query, macro) | ❌ Cần server/kỹ sư bảo trì |
| ✅ Chuyên viên hiểu giới hạn (không tin tuyệt đối) | ❌ Tin máy, soát lơ là |

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
