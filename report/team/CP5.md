# CP5 — Quy trình trước/sau và Problem Statement v0

Phụ trách: Đồng Hữu Nguyên Khoa.

## 4. Quy trình trước/sau (CP5)

Quy trình dưới đây là mô tả ban đầu từ Problem Card. Cần đối chiếu với một lượt tìm dẫn chứng thực tế; báo cáo hiện chưa có số đo từng bước.

### 4.1. Quy trình hiện tại

```text
HIỆN TẠI — GIẢ THUYẾT, 5 bước chính

[1 Ghi chú] → [2 Xác định paper] → [3 Dò PDF] → [4 Đọc ngữ cảnh]
                                      ↑                 ↓
                          BOTTLENECK GIẢ THUYẾT   [5 Lưu vị trí nguồn]

Thời gian từng bước: [CẦN ĐO]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên | Nhận định cần kiểm chứng, ghi chú đã có | Ghi chú liên quan được mở | [CẦN ĐO] | Có thể thiếu vị trí nguồn. |
| 2 | Sinh viên | Ghi chú, tên bài hoặc citation | Paper/PDF cần đối chiếu | [CẦN ĐO] | Phạm vi là paper đã đọc. |
| 3 | Sinh viên | Nhận định và PDF | Đoạn, hình hoặc bảng có thể chứa bằng chứng | [CẦN ĐO] | Bottleneck giả thuyết; chưa chứng minh là bước lâu nhất. |
| 4 | Sinh viên | Bằng chứng ứng viên và phần xung quanh | Xác nhận hoặc bác bỏ nhận định theo ngữ cảnh | [CẦN ĐO] | Giữ đúng điều kiện và giới hạn của kết quả. |
| 5 | Sinh viên | Kết quả đã đối chiếu PDF | Bằng chứng và vị trí nguồn được lưu | [CẦN ĐO] | Chưa đủ căn cứ thì ghi chưa xác minh, không dùng làm bằng chứng. |

**Bottleneck chính cần kiểm chứng:** bước 3 — tìm đúng đoạn, hình hoặc bảng khi ghi chú không lưu vị trí nguồn. Khó định vị và khó hiểu ngữ cảnh cần được đo riêng.

### 4.2. Quy trình tương lai

**No AI đề xuất:** ghi chú có cấu trúc và Zotero; người học thao tác và giữ quyền xác nhận bằng chứng. Công tạo ghi chú/liên kết khi đọc cũng phải được đo, dù diễn ra trước lượt tìm lại.

```text
NO AI ĐỀ XUẤT — CHƯA TRIỂN KHAI, 5 bước chính

[1 Nhận định cần kiểm chứng]
               ↓
[2 Structured notes / Zotero]
               ↓
[3 Mở liên kết nguồn] ── thiếu / sai ──> [Tìm thủ công trong PDF]
               │                                    │
               └──────────────────┬─────────────────┘
                                  ↓
                  [4 Sinh viên kiểm tra ngữ cảnh] ← HITL
                                  ↓
                  [5 Lưu bằng chứng đúng vị trí]

Không đủ căn cứ: ghi chưa tìm thấy/chưa xác minh, không chấp nhận nhận định.
Thời gian từng bước và công chuẩn bị: [CẦN ĐO]
```

**Boundary:** người học mở PDF gốc để kiểm nguồn, nội dung và ngữ cảnh trước khi lưu. AI không được tự tạo trích dẫn, bịa nguồn/số trang hoặc tự xác nhận bằng chứng đúng. Liên kết thiếu/sai thì tìm thủ công và vẫn qua bước kiểm tra.

**OPTIONAL — CHƯA TRIỂN KHAI:** chỉ cân nhắc khi No AI và tìm kiếm theo quy tắc chưa đủ.

```text
[Nhận định + paper] → [Retrieval] → [AI gợi ý đoạn và vị trí nguồn]
                                                    ↓
                       [Người học mở PDF gốc để xác minh] → [Lưu kết quả]
```

Vị trí nguồn phải đến từ PDF/metadata truy xuất, không để mô hình tạo số trang. Nếu không tìm đủ căn cứ, báo chưa tìm thấy và quay về kiểm thủ công. Rule (keyword search/BM25) có thể được thử trước Workflow; Agent chưa có cơ sở để chọn.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---|---|---|
| Số bước chính | 5 | 5 | Theo hai pipeline trên slide; nhánh ngoại lệ và công chuẩn bị được ghi riêng. |
| Tổng thời gian | Chưa có baseline thực nghiệm [CẦN ĐO] | Mục tiêu đề xuất giảm ít nhất 30% | Tính cả chuẩn bị, tìm kiếm và kiểm chứng cho cùng bộ tác vụ. |
| Số bước thủ công | 5/5 bước do người học thao tác | 5/5 bước do người học thao tác, có Zotero hỗ trợ | Chưa triển khai script/AI tự động; không suy hiệu quả chỉ từ số bước. |
| Bottleneck | Giả thuyết: dò PDF để tìm đúng bằng chứng | Kỳ vọng giảm dò lại nhờ liên kết nguồn | Chưa biết công kiểm ngữ cảnh và tạo ghi chú có triệt tiêu lợi ích không. |
| Rủi ro mới phát sinh | Ghi chú thiếu vị trí nguồn, phải dò lại | Liên kết sai/hỏng, công chuẩn bị tăng, hiểu sai ngữ cảnh | Luôn kiểm PDF, có fallback thủ công và tính cả ngoại lệ. |
| Chất lượng | [CẦN ĐO] | Không giảm so với baseline | Đánh giá riêng evidence hit rate, citation accuracy và context correctness. |

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên đang đọc và tổng hợp paper nghiên cứu, cần dùng lại nhận định từ paper đã đọc. |
| **Quy trình** | Ghi chú → xác định paper → dò PDF → đọc ngữ cảnh → lưu vị trí nguồn. |
| **Bottleneck** | Giả thuyết: ghi chú thiếu vị trí khiến người học phải dò lại đúng đoạn, hình hoặc bảng; cần quan sát để xác nhận bước nghẽn. |
| **Impact** | Có thể tốn thời gian đọc lại và diễn giải sai điều kiện/giới hạn của kết quả; chưa đo mức độ hay tần suất. |
| **Success Metric** (baseline → target, cách đo) | Baseline: chưa có số đo thực nghiệm. Target đề xuất: giảm ít nhất 30% tổng thời gian, không giảm độ đúng của nguồn và ngữ cảnh. Đo cách tìm hiện tại và No AI trên bộ tác vụ có đối chiếu PDF, tính cả chuẩn bị và xác minh. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Ưu tiên ghi chú có cấu trúc/Zotero. Người học kiểm PDF trước khi dùng bằng chứng; thiếu/sai liên kết thì tìm thủ công. Nếu thử AI sau này, chỉ gợi ý đoạn và vị trí từ nguồn thật, không tự tạo citation hoặc xác nhận độ đúng. |

**Phản biện AI đã ghi nhận:** đo tốc độ chưa đủ; tìm đúng vị trí nhưng sai ngữ cảnh vẫn không đạt. Cần tính cả công tạo ghi chú, lượt thất bại và quay về thủ công để tránh chuyển công sức sang bước khác.

**Điều chỉnh sau phản biện:** tách thời gian tìm khỏi tổng công chuẩn bị và kiểm chứng; kiểm riêng độ đúng của nguồn và ngữ cảnh. Cách đo được trình bày ở mục 7.
