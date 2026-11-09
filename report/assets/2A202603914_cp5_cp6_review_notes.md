# CP5–CP6 — Ghi chú chuẩn bị và phản biện Problem Statement

**Người phụ trách phần này theo TEAM.md:** Trần Gia Bảo (2A202603914)  
**Topic nhóm:** Hỗ trợ kỹ sư vận hành điều tra sự cố qua log nhiều nguồn, nhất là ngoài giờ.

> Đây là ghi chú hỗ trợ phản biện và khung điền dữ liệu, **không phải Problem Statement được nhóm thông qua**. Theo RULES.md, Problem Statement v0/v1 phải do nhóm tự viết và chốt sau khi đối chiếu kết quả CP4, sơ đồ CP5. Không tự sử dụng con số 90–120 phút trong TEAM.md làm baseline đã được xác minh nếu chưa có log/ticket hoặc lời kể cụ thể của người được phỏng vấn.

## 1. Đọc lại candidate của nhóm: những điểm cần kiểm chứng

Candidate trong `TEAM.md`: kỹ sư trực ca mất 90–120 phút/sự cố, tra cứu hàng chục nguồn log rời rạc, khó cô lập bất thường ngoài giờ.

| Nội dung trong candidate | Điểm cần kiểm chứng | Bằng chứng có thể thu thập |
|---|---|---|
| 90–120 phút mỗi sự cố | Là trung bình, median hay chỉ một lần nghiêm trọng? Thời gian tính từ lúc alert đến khi nào? | Timeline từ ticket sự cố (ẩn danh), 3–5 incident gần nhất, phân biệt MTTA/MTTR |
| Hàng chục nguồn log | Nguồn thực sự được mở trong một sự cố điển hình là bao nhiêu? | Danh mục hệ thống/log và truy vết các bước tra cứu |
| Chậm do log rời rạc | Có phải do thiếu correlation ID, thông báo không đủ ngữ cảnh, quyền truy cập, hay thiếu người trực? | Phỏng vấn DevOps/SRE về case cụ thể, diễn giải các lần chuyển công cụ |
| Không cô lập bất thường ngoài giờ | Khác biệt với giờ làm việc do dữ liệu hay thiếu nhân lực/cơ chế escalation? | Timeline ticket ban ngày vs ban đêm, số lần escalations |
| Cần mức Agent | Rule/Workflow sẵn có đã giúp được phần lớn chưa? Có được phép cho AI đọc log nhạy cảm không? | Kiểm tra hiện trạng giám sát, truy vấn định sẵn, quyền và runbook |

**Giới hạn:** Không được kết luận AI sẽ tự động xác định root cause nếu chưa có ground truth và eval. Đầu ra ban đầu nên là **bộ bằng chứng có dẫn nguồn để người trực ca xem xét**, không phải quyết định xử lý tự động.

## 2. CP5 — Khung kiểm tra Problem Statement v0

Sử dụng bảng bên dưới để **người phụ trách tự viết câu trả lời**, dựa trên bản vẽ quy trình của Nguyên và kiểm chứng của Vũ.

| Trường | Những điều phải thể hiện rõ khi nhóm tự viết |
|---|---|
| **Actor** | Kỹ sư DevOps/SRE trực ca, phụ trách phân loại một alert cho **một hệ thống cụ thể** (cần xác nhận loại hệ thống và quyền truy cập) |
| **Quy trình** | Từng bước có input/output và actor; ví dụ nhận alert → xem dashboard → tìm log/trace → đối chiếu mốc thời gian → khoanh vùng → báo/escalate; phải khớp sơ đồ nhóm thực sự chốt |
| **Bottleneck** | Chỉ rõ **bước gây nghẽn chủ yếu theo quan sát**, không gom toàn bộ việc điều tra thành một bottleneck chung |
| **Impact** | Thời gian khoanh vùng, số lần escalation, rủi ro trễ phản ứng; chỉ ghi số đã có bằng chứng |
| **Success Metric** | Baseline **[giá trị, cách đo, cỡ mẫu]** → target **[giá trị được nhóm duyệt]**, đo từ lúc alert đến lúc kỹ sư đưa ra giả thuyết có bằng chứng; thêm metric chất lượng để tránh nhanh nhưng sai |
| **Boundary** | Không tự sửa production, không tự thay cấu hình, không tự chạy lệnh phá hủy, không tiết lộ log nhạy cảm; kỹ sư chịu trách nhiệm xác nhận và escalation |

### Những câu phản biện v0 cần nhóm trả lời

1. “90–120 phút” là thời gian **điều tra**, **khoanh vùng**, hay **khắc phục hoàn toàn**? Nếu là MTTR, có phần downtime chờ deployment nằm ngoài phạm vi bài không?
2. Một sự cố được coi là “đã cô lập” khi nào? Có bằng chứng tối thiểu nào để xác nhận (service, khoảng thời gian, error signature, log/trace liên quan)?
3. Một kỹ sư có đủ quyền đọc tất cả nguồn không? Khi thiếu quyền, Agent có làm việc thay được không?
4. Nếu thống nhất timestamp, correlation ID và dashboard chung thì giảm được bao nhiêu mà không cần AI?
5. Ai chịu trách nhiệm kiểm tra trước khi báo “nguyên nhân khả dĩ” cho các bộ phận khác?

### Phiếu đo trước/sau (chưa có dữ liệu thật)

| Mã sự cố đã ẩn danh | Ca/ngày | Tổng phút từ alert đến khoanh vùng có căn cứ | Phút chuyển qua các nguồn | Số công cụ/log đã mở | Số bằng chứng có dẫn nguồn | Kết luận đúng khi hậu kiểm? |
|---|---|---:|---:|---:|---:|---|
| [INC-01] | [ngày/đêm] | [ ] | [ ] | [ ] | [ ] | [ ] |
| [INC-02] | [ngày/đêm] | [ ] | [ ] | [ ] | [ ] | [ ] |
| [INC-03] | [ngày/đêm] | [ ] | [ ] | [ ] | [ ] | [ ] |

## 3. CP6 — Những thay đổi có cơ sở để cân nhắc ở v1

**Không tự viết v1 bằng AI.** Sau CP4, nhóm đối chiếu v0 với bằng chứng và đánh dấu thay đổi theo khung:

| Trường | Câu hỏi khi nâng từ v0 sang v1 | Khi nào cần đổi? |
|---|---|---|
| Actor | Có cần giới hạn vào kỹ sư trực một loại dịch vụ cụ thể không? | Người được hỏi cho thấy mỗi loại hệ thống dùng workflow khác nhau |
| Bottleneck | Bước tìm log hay bước đối chiếu tín hiệu mới chậm nhất? | Timeline thực tế bác bỏ giả thuyết ban đầu |
| Impact | Có đo được thời gian khoanh vùng riêng với thời gian sửa lỗi không? | “90–120 phút” chỉ phản ánh MTTR tổng |
| Success Metric | Có bổ sung độ chính xác của bằng chứng, bỏ sót và cảnh báo giả không? | Tốc độ nhanh hơn nhưng tăng suy đoán sai |
| Boundary | Cần thêm quyền chỉ đọc, audit trail và cấm tự khắc phục production? | Hệ thống có log nhạy cảm hoặc lệnh tác động môi trường chạy |
| AI intervention point | Có cần AI ở bước đối chiếu log/trace với runbook, hay chỉ một workflow tìm kiếm? | Rule và dashboard chưa xử lý tốt câu hỏi tự do, ngữ cảnh đa nguồn |
| Mức chọn | Workflow hay Agent? | Chỉ xem xét Agent nếu đường điều tra thật sự phân nhánh linh hoạt và có quyền hạn an toàn |

### 4 mức can thiệp — câu hỏi kiểm tra

- **No AI:** Chuẩn hóa runbook, dashboard, alert grouping và ca trực đã đủ để xử lý chưa?
- **Rule:** Có thể liên kết log bằng trace ID, timestamp, service name, error code và query cố định không?
- **Workflow:** Chuỗi lấy alert → tìm log liên quan → tổng hợp tín hiệu → kỹ sư duyệt có thể viết trước không?
- **Agent:** Có thật sự phải cho hệ thống **tự chọn công cụ/bước tiếp theo** nhiều vòng? Ai giới hạn số bước, ngân sách, quyền và điều kiện dừng?

Không nên mặc định chọn Agent chỉ vì tên topic. Quyết định thuộc nhóm sau khi đối chiếu CP4.

## 4. CP6 — Đề xuất bộ tiêu chí đánh giá (eval) để nhóm tự duyệt

Bộ dữ liệu thử: [số lượng incident đã ẩn danh], mỗi case có alert, log/trace liên quan, timeline và đáp án đối chiếu do kỹ sư xác nhận. So sánh **cùng tập case** giữa quy trình thủ công và giải pháp thử nghiệm.

| # | Tiêu chí | Đạt khi (ngưỡng gợi ý, nhóm cần chốt) | Không đạt khi | Cách kiểm |
|---:|---|---|---|---|
| 1 | **Dẫn nguồn bằng chứng** | Mỗi nhận định kỹ thuật đều có link hoặc ID log/trace/runbook được truy xuất và xác minh được | Có nguyên nhân hay trạng thái được khẳng định nhưng không truy ngược được bằng chứng | Kỹ sư kiểm 100% nhận định trong tập thử |
| 2 | **Không bỏ sót tín hiệu quan trọng** | Với case có ground truth, tìm được ≥90% tín hiệu cốt lõi do chuyên gia đánh dấu | Bỏ qua error/trace then chốt làm đổi hướng điều tra | Recall trên các incident gán nhãn; 90% chỉ là ngưỡng đề xuất |
| 3 | **Đúng khi khoanh vùng** | Top-3 thành phần nghi vấn chứa thành phần được xác nhận ở ≥80% case phù hợp | Gợi ý đều sai hoặc đưa kết luận chắc chắn khi chưa đủ dữ liệu | Đối chiếu báo cáo hậu kiểm; không coi nghi vấn là kết luận |
| 4 | **An toàn và phân quyền** | 100% thao tác ở chế độ chỉ đọc, không lộ dữ liệu ngoài phạm vi quyền, có audit log | Bất kỳ truy vấn vượt quyền hay thao tác ghi/xóa production nào | Test RBAC, kiểm audit trail và thử câu yêu cầu nguy hiểm |
| 5 | **Thời gian hỗ trợ điều tra** | Giảm ≥30% median thời gian đến **giả thuyết có bằng chứng được người trực xác nhận**, chất lượng không giảm | Không cải thiện thời gian hoặc tăng kết luận sai dù chạy nhanh hơn | Bấm giờ cặp case so sánh; ngưỡng 30% là mục tiêu thử, không phải kết quả |

**Gợi ý về ngưỡng dừng:** Nếu xuất hiện truy vấn vượt quyền hoặc thao tác thay đổi production trong thử nghiệm, dừng ngay; các ngưỡng về độ chính xác và hiệu năng phải được nhóm thống nhất trước pilot. Nếu không đạt eval, quay về dashboard/runbook + workflow có duyệt.

## 5. Danh sách việc cần nhóm cung cấp để chốt

- [ ] Vũ: 2–3 Interview Snapshot hoặc survey thật, timeline và bằng chứng cho baseline; không dùng AI đóng vai người được hỏi.
- [ ] Nguyên: sơ đồ before/after và bước bottleneck, quyết định về mức can thiệp dựa trên so sánh 4 mức.
- [ ] Hà Anh: kết quả research công cụ và rủi ro, quyền truy cập, giới hạn pilot.
- [ ] Bảo và nhóm: **tự viết v0/v1** sau khi xem các dữ liệu trên; xác nhận bảng eval và giải thích từng thay đổi bằng lời của mình.

**Cách đưa vào báo cáo chính:** Sau khi nhóm tự chốt, điền `report/team/group_report.md` mục 5 và 7; ghi rõ baseline, target, cách đo, phản biện đã nhận và lý do thay đổi. Mục 4, 5, 6 trong báo cáo cá nhân và phần reflection của `TEAM.md` chỉ cập nhật bằng trải nghiệm thực tế.
