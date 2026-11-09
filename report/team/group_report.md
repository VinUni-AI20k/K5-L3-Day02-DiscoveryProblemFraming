# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: CodeX
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
| **VS Code Dev Containers** | https://code.visualstudio.com/docs/devcontainers/containers | Bước 2 & 3: Cài đặt runtime, SDK, database và đồng bộ cấu hình IDE | Đóng gói sẵn toàn bộ môi trường chuẩn trong file `devcontainer.json`, bật lên là chạy ngay, triệt tiêu lỗi "chạy được trên máy anh nhưng lỗi máy em" | Đòi hỏi Techlead/Senior phải tốn công thiết lập chuẩn từ đầu. Các dự án outsource/maintain cũ thường chưa có sẵn, hoặc cấu hình cũ không tương thích kiến trúc chip mới | Giải pháp lý tưởng cho dự án mới, nhưng không giải quyết ngay được pain point khi Dev mới/Tester phải tiếp nhận một repo outsource/maintain cũ chưa được chuẩn hóa |
| **Docker Compose + `.env` (No-AI)** | https://docs.docker.com/compose/ | Bước 2 & 3: Container hóa môi trường (Dockerfile + docker-compose) kèm script kiểm tra biến `.env` | Cô lập môi trường tốt (runtime, DB), chuẩn hóa cấu hình qua script tự động kiểm tra `.env`, giảm thời gian cài đặt thủ công ở Bước 2 (45') và Bước 3 (30') | File `README.md`, `Dockerfile` hoặc `package.json`/`requirements.txt` ở dự án cũ thường lỗi thời. Khi sang Bước 4 (Build & run) bị crash do thư viện deprecated hoặc xung đột version với OS, Docker chỉ ném ra log lỗi dài mà không chỉ cách sửa | Phương án No-AI giải quyết tốt khâu tự động hóa khởi tạo (Bước 2–3), nhưng khi build fail ở Bước 4 (mất 180') và phải gọi Techlead ở Bước 5 (90') thì vẫn cần AI chẩn đoán |
| **GitHub Copilot CLI** | https://docs.github.com/en/copilot/github-copilot-in-the-cli | Bước 4: Giải thích thông báo lỗi (error log) và gợi ý lệnh sửa trên terminal | Tích hợp trực tiếp tại terminal (`gh copilot explain` / `suggest`), giải thích nhanh ý nghĩa lỗi và gợi ý cú pháp câu lệnh mà không cần rời màn hình đi tìm kiếm | Thiếu ngữ cảnh đối chiếu của dự án: chỉ đọc được đoạn lỗi ngắn trên terminal chứ không tự động đối chiếu chéo giữa `package.json` / `requirements.txt` với hệ điều hành thực tế của máy. Dễ gợi ý các lệnh ép cài đặt (`--force`, `sudo`) làm hỏng chuỗi dependency của dự án cũ | Không thể chỉ hỏi AI bằng đoạn log rời rạc. Cần một **Workflow** dùng script gom đủ bộ 3 đầu vào: `[Log lỗi khi build fail] + [package.json / requirements.txt] + [Thông tin OS/Runtime]` trước khi đưa vào AI |

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
| Số bước | 5 | 4 | Rút gọn bước cài đặt thủ công (nhờ Docker + script kiểm tra `.env`) và loại bỏ hoàn toàn Bước 5 (chờ Dev cũ/Techlead sang pair-debug 90') |
| Tổng thời gian |  360' | 40' | Giảm từ 6 tiếng (15' + 45' + 30' + 180' + 90') xuống 40 phút (25' chạy chuẩn hóa bước 1–3 + 15' xử lý lỗi build cùng AI) |
| Số bước thủ công | 5/5 | 2/4 | Bước kiểm tra `.env` và gom ngữ cảnh lỗi do Rule (script) chạy; Dev mới/Tester chỉ tự duyệt lệnh gợi ý của AI (HITL) và xác nhận chạy code |
| Bottleneck chính | Bước 4 & 5: Dò lỗi mâu thuẫn dependency (180') & gọi Dev cũ/Techlead pair-debug (90') = 270' | Dev mới / Tester kiểm tra lệnh gợi ý của AI và chạy thử (15') | Bottleneck chuyển thành bước kiểm soát an toàn có chủ đích, thời gian ngắn (15') và không làm gián đoạn người khác |
| Rủi ro mới phát sinh | - | AI chỉ sai version xung đột hoặc gợi ý lệnh can thiệp hệ thống (`sudo`, `--force`) làm hỏng môi trường máy cục bộ | Kiểm soát bằng Boundary (cấm AI tự thực thi lệnh trên máy) và 3 tiêu chí đánh giá đầu ra ở Mục 7 |

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
| **Actor** | Developer mới join dự án, Tester, và Techlead / Senior phụ trách dự án (trong bối cảnh ngày đầu tiếp nhận dự án outsource/maintain cũ hoặc onboard thành viên mới) |
| **Quy trình** | 1. Nhận quyền truy cập repo & đọc `README.md` cũ (15') → 2. Tải và cài đặt runtime, SDK, database theo docs cũ (45') → 3. Cài đặt dependencies & tạo file `.env` (30') → 4. Build và run project, gặp lỗi crash do xung đột thư viện/version (180') → 5. Nhờ Dev cũ hoặc Techlead sang pair-debug và sửa từng lỗi cấu hình (90') |
| **Bottleneck** | Bước 4 & 5: Dò lỗi mâu thuẫn dependency (180') và phải gọi Dev cũ/Techlead hỗ trợ pair-debug trực tiếp (90') — mất tổng cộng 270 phút / 360 phút |
| **Impact** | Lãng phí 4–8 tiếng của nhân sự mới (Dev/Tester); làm gián đoạn 1–2 tiếng của Senior/Techlead; chậm tiến độ kickoff sprint 1–2 ngày (xảy ra 5–6 lần/quý) |
| **Success Metric** (baseline → target, cách đo) | (1) Tổng thời gian setup giảm từ 360' xuống 40'; (2) Thời gian thao tác và gỡ lỗi cấu hình/dependency giảm từ 270' xuống 15' (vượt mục tiêu ban đầu là dưới 30'); (3) Số lần cần Dev cũ/Senior can thiệp trực tiếp giảm từ 3–4 lần xuống 0 lần |
| **Boundary** | AI không tự động thực thi lệnh trên terminal của người dùng, không gợi ý các lệnh can thiệp file hệ thống hoặc leo thang đặc quyền (`sudo`, `rm -rf`), không tự ý ghi đè file cấu hình gốc (`package.json`, `requirements.txt`, `.env`) khi người cài chưa duyệt |
| **AI intervention point** | Ngay tại Bước 4 khi lệnh build/run bị fail: Script (Rule) tự động kiểm tra biến môi trường `.env` và gom `[Log lỗi build] + [package.json / requirements.txt] + [Thông tin OS/Runtime]` gửi cho AI để chỉ ra đúng version xung đột và đề xuất lệnh sửa  |
| **Mức chọn** | Workflow |
| **Rủi ro & người kiểm tra** | AI chẩn đoán sai thư viện xung đột, bịa version không tồn tại hoặc đề xuất lệnh làm hỏng môi trường cục bộ → **Dev mới / Tester** trực tiếp kiểm tra lệnh gợi ý và chạy thử trong môi trường cô lập (Docker/venv); **Techlead** chỉ review PR cập nhật `README.md` sau khi code đã chạy thành công |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| **Success Metric** | Đặt mục tiêu giảm thời gian gỡ lỗi từ 270' xuống dưới 30' và giảm số lần gọi người khác từ 3–4 lần xuống 0 lần | Chốt cụ thể chỉ số tổng thời gian từ **360' → 40'**, thời gian gỡ lỗi từ **270' → 15'**, số lần làm phiền Senior từ **3 lần → 0 lần**, kèm bộ tiêu chí đánh giá chất lượng lệnh của AI | Cụ thể hóa cả thời gian tổng thể (bước 1–3 kết hợp No-AI/Rule giảm từ 90' xuống 25') lẫn thời gian debug (bước 4–5 dùng AI giảm từ 270' xuống 15') và đảm bảo lệnh gợi ý phải chạy được thực tế |
| **AI intervention point & Mức chọn** | Đang phân vân giữa "Rule hoặc Workflow"; dự kiến đưa log lỗi cho AI phân tích | Chốt mức **Workflow**: kết hợp **Rule** (script tự động kiểm tra `.env` và gom đủ 3 nguồn dữ liệu: log lỗi + `package.json`/`requirements.txt` + OS) trước khi đưa vào **AI** | Qua research ở Mục 3.3 (bài học từ Docker Compose và Copilot CLI), nếu thiếu Rule kiểm tra `.env` và gom ngữ cảnh file cấu hình thì AI sẽ đoán mò hoặc bỏ sót lỗi thiếu biến môi trường |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Chỉ đúng tên thư viện và version xung đột** | Chỉ ra chính xác tên package/thư viện đang gây crash khi build và nêu đúng phiên bản mâu thuẫn khớp với `error log`, file `package.json` / `requirements.txt` và hệ điều hành của người dùng | Đoán mò thư viện không có trong log lỗi, không phát hiện ra mâu thuẫn giữa file cấu hình với OS/SDK, hoặc bịa ra tên package/version không tồn tại |
| 2 | **An toàn hệ thống (Không can thiệp file hệ thống)** | Các câu lệnh đề xuất chỉ tác động trong phạm vi thư mục dự án hoặc môi trường ảo/container cục bộ (`venv`, `node_modules`, Docker) và giữ nguyên tính toàn vẹn của máy | Gợi ý các lệnh can thiệp vào file hệ thống của OS, yêu cầu quyền quản trị (`sudo`, `chmod 777`, `rm -rf` ngoài dự án) hoặc dùng cờ ép buộc (`--force`) phá vỡ các thư viện khác trên máy |
| 3 | **Lệnh phải chạy được và khắc phục được lỗi build** | Cú pháp câu lệnh chuẩn xác với OS và package manager của dự án; khi Dev mới/Tester copy chạy thử thì thực thi thành công ngay lần đầu và vượt qua được bước crash ở Bước 4 | Lệnh sai cú pháp (báo syntax error), gọi sai flag/tham số của công cụ, hoặc chạy xong nhưng khi build lại vẫn bị crash ở đúng lỗi xung đột cũ |

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
