# CP5–CP6 — Phần việc Trần Gia Bảo (2A202603914)

**Topic nhóm:** Hỗ trợ kỹ sư DevOps/SRE trực ca điều tra sự cố từ nhiều nguồn log.  
**Trạng thái:** Khung hoàn thiện trước buổi chốt nhóm. Những trường đánh dấu `[...]` cần điền từ CP4 và sơ đồ CP5; không phải kết quả đã kiểm chứng.

## CP5 — Problem Statement v0

> Nhóm tự hoàn thiện câu chữ chính thức từ kết quả phỏng vấn và quy trình đã thống nhất. Bảng này chỉ nhắc đúng 6 thành phần cần có.

| Trường | Dữ liệu cần nhóm điền |
|---|---|
| **Actor** | [Vai trò kỹ sư trực ca cụ thể, loại hệ thống, quyền truy cập] |
| **Quy trình** | [Chuỗi 5–7 bước đúng theo sơ đồ CP5 của Nguyên, bắt đầu từ alert và kết thúc tại mốc khoanh vùng/escalate] |
| **Bottleneck** | [Một bước chậm nhất, lý do và thời gian đo từ sự cố thực tế] |
| **Impact** | [Ảnh hưởng đến thời gian khoanh vùng/escalation; bằng chứng CP4] |
| **Success Metric** | Baseline: [giá trị + đơn vị + cỡ mẫu]; Target: [ngưỡng nhóm thống nhất]; Cách đo: [mốc bắt đầu/kết thúc, log/ticket, so sánh trước–sau] |
| **Boundary** | [Việc công cụ không được tự làm; quyền chỉ đọc; bước kỹ sư xác nhận] |

**Cần kiểm tra trước khi chốt v0:**

1. “90–120 phút” trong `TEAM.md` đã có chứng cứ hay mới là ước lượng? Có phải thời gian điều tra, hay gồm cả khắc phục?
2. Bottleneck thật sự là **tìm log**, **liên kết các sự kiện**, hay **chờ người hỗ trợ**?
3. Nếu chỉ đưa toàn bộ log vào một dashboard và chuẩn hóa trace ID, pain còn bao nhiêu?
4. “Khoanh vùng thành công” được xác nhận bằng tiêu chí nào?

## CP6 — Problem Statement v1

> Chỉ hoàn thiện sau khi nhóm so sánh No AI, Rule, Workflow và Agent, rồi quyết định điểm can thiệp. Không mặc định chọn Agent vì tên topic.

| Trường | Nhóm cần xác nhận trong bản v1 |
|---|---|
| **Actor** | [Nhóm kỹ sư và loại sự cố sau kiểm chứng; có thu hẹp so với v0 không?] |
| **Quy trình** | [Các bước thực tế được xác nhận tại CP4–CP5] |
| **Bottleneck** | [Bước nghẽn thực tế và bằng chứng] |
| **Impact** | [Tác động đo được; không đồng nhất MTTR với thời gian tìm bằng chứng] |
| **Success Metric** | [Baseline → target → cách đo]; bổ sung thước đo chất lượng để tránh “nhanh nhưng sai” |
| **Boundary** | [Quyền truy cập tối thiểu; kỹ sư duyệt; cấm thao tác thay đổi production nếu chưa cho phép] |
| **AI intervention point** | [Bước cụ thể cần AI, hoặc “không có” nếu Rule đã đủ] |
| **Mức chọn** | [No AI / Rule / Workflow / Agent — do nhóm chốt kèm lý do] |
| **Rủi ro & người kiểm tra** | [Sai liên kết log, gán nhầm nguyên nhân, rò rỉ dữ liệu; người phụ trách kiểm từng loại] |

## CP6 — Bảng thay đổi v0 → v1

Chỉ ghi **thay đổi thực sự đã diễn ra** sau phản biện/kiểm chứng, không điền giả rằng nhóm đã đổi.

| Trường | v0 | v1 | Lý do thay đổi/bằng chứng |
|---|---|---|---|
| Actor | [ ] | [ ] | [Từ kết quả CP4, nếu có] |
| Bottleneck | [ ] | [ ] | [Từ timeline sự cố, nếu có] |
| Success Metric | [ ] | [ ] | [Từ đánh giá về tốc độ và chất lượng, nếu có] |
| Boundary | [ ] | [ ] | [Từ rủi ro vận hành và quyền hạn, nếu có] |
| AI intervention point | Chưa xác định ở v0 | [ ] | [Từ so sánh 4 mức ở CP6] |

## CP6 — Đề xuất 5 tiêu chí đánh giá đầu ra

**Các ngưỡng số dưới đây là target đề xuất để nhóm thảo luận, không phải kết quả thử nghiệm.** Cần thống nhất bộ incident đã ẩn danh và đáp án hậu kiểm trước khi đo.

| # | Tiêu chí | Đạt khi | Không đạt khi | Phương pháp kiểm |
|---:|---|---|---|---|
| 1 | Có bằng chứng truy vết | 100% nhận định kỹ thuật quan trọng kèm ID/link log, trace hoặc runbook kiểm tra được | Có kết luận không truy ra nguồn | Kỹ sư đối chiếu từng nhận định |
| 2 | Không bỏ sót tín hiệu chính | Recall ≥ 90% với những tín hiệu đã được chuyên gia gán nhãn | Bỏ sót lỗi/trace then chốt làm lệch hướng điều tra | So kết quả với ground truth của tập case |
| 3 | Khoanh vùng đúng thành phần nghi vấn | Top-3 thành phần nghi vấn có thành phần được xác nhận ở ≥ 80% case phù hợp | Gợi ý sai toàn bộ hoặc coi nghi vấn là nguyên nhân đã xác nhận | So với incident postmortem đã duyệt |
| 4 | An toàn vận hành | 100% truy cập chỉ đọc, đúng quyền; mọi lần truy xuất có audit log | Có bất kỳ hành động sửa/xóa production hoặc truy cập vượt quyền | Test quyền, audit và tình huống prompt độc hại |
| 5 | Hiệu quả thời gian | Median thời gian từ alert đến giả thuyết **được kỹ sư xác nhận** giảm ≥ 30%, và tiêu chí chất lượng không giảm | Không giảm thời gian hoặc tạo kết luận sai dù nhanh hơn | Bấm giờ các case tương đương, so trước/sau |

**Nguyên tắc đánh giá:** không tính là thành công nếu rút ngắn thời gian nhưng làm tăng bỏ sót tín hiệu, gán nhầm root cause hoặc vi phạm phân quyền.

## Việc còn thiếu để chốt và đưa vào group_report.md

- **Vũ (CP4):** Kết quả phỏng vấn và số liệu sự cố có thể trích dẫn, cả tín hiệu phản bác.
- **Nguyên (CP5/CP6):** Sơ đồ trước/sau, bước nghẽn được nhóm xác nhận và mức AI sau so sánh 4 mức.
- **Bảo + nhóm:** Tự viết và duyệt Problem Statement v0/v1; xác nhận baseline, target, các ngưỡng eval và lý do đổi.
- **Hà Anh:** Xác nhận rủi ro/điều kiện dừng trước khi chốt quyết định cuối.

**Vị trí nhập bản đã thống nhất:** `report/team/group_report.md` mục 5 và mục 7. Ghi rõ nguồn số liệu, không đánh dấu bài nhóm hoàn thành khi CP4 chưa có bằng chứng.
