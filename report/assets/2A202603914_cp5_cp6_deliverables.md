# CP5–CP6 — Bản đề xuất hoàn thiện phần của Trần Gia Bảo

**Học viên:** Trần Gia Bảo — 2A202603914  
**Bài toán chung:** Điều tra và phản ứng sự cố hạ tầng đa tầng, đặc biệt ngoài giờ.  
**Nguồn đối chiếu nội bộ:** `TEAM.md`; `report/team/group_report.md` mục 2–6; `report/assets/cp4-interview-tonghop.md`; `report/assets/2A202603937_cp5_cp6_workflow_and_ai_level.md`.

> **Phạm vi sử dụng:** Đây là bản phân tích/đề xuất được AI hỗ trợ tổ chức dựa trên nội dung nhóm đã ghi. Theo `RULES.md`, thành viên phải tự diễn đạt, phản biện và **nhóm tự chốt** câu chữ Problem Statement v0/v1 trước khi đưa vào báo cáo chính thức. Con số từ phỏng vấn là thông tin tổng hợp do nhóm cung cấp, không phải dữ liệu hệ thống đã đo trực tiếp. Các ngưỡng mục tiêu là **mục tiêu pilot**, không phải kết quả đạt được.

---

## 1. CP5 — Dữ liệu cho Problem Statement v0 (trước CP4)

Bản v0 phải phản ánh **giả định đầu tiên của nhóm trước khi được kiểm chứng**, tránh viết ngược lại bằng kết quả phỏng vấn v1.

| Trường | Nội dung đề xuất để nhóm rà soát và tự chốt |
|---|---|
| **Actor** | Kỹ sư DevOps/SRE hoặc NetOps trực ca, chịu trách nhiệm theo dõi và xử lý sự cố hạ tầng có log trải trên nhiều thành phần. |
| **Quy trình** | Nhận cảnh báo/ticket → mở Nginx access/error log → lọc nhiễu WebSocket/cache → đối chiếu firewall, DNS, ứng dụng, database → đưa ra hướng cô lập hoặc escalation → kiểm tra và ghi nhận sự cố. |
| **Bottleneck** | Giả định ban đầu: lọc log và đối chiếu nhiều hệ thống ở bước 3–4 tốn 20 + 35 = **55 phút thao tác**; việc phát hiện muộn ngoài giờ và chờ xử lý khiến tổng thời gian có thể kéo dài. |
| **Impact** | Giả định trong đề xuất ban đầu: khoảng **90–120 phút/sự cố** từ khi phát sinh bất thường đến lúc cô lập; có nguy cơ kéo dài gián đoạn khi thiếu người trực đêm. **Chưa được xác thực bằng timeline từng incident.** |
| **Success Metric** | **Baseline dự kiến:** 90–120 phút/sự cố (giả định ban đầu, phải đối chiếu). **Target đề xuất:** dưới 5 phút với ca tự xử lý đủ điều kiện; dưới 15 phút với ca HITL. **Đo:** log thời điểm bắt đầu bất thường, phát cảnh báo, khoanh vùng, thực thi và hậu kiểm; phân tách độ trễ phát hiện và thời gian xử lý. |
| **Boundary** | Không tự động thực thi lệnh shell tùy ý, không thay đổi hệ thống lõi, không chặn các IP/dịch vụ thuộc whitelist; trường hợp thiếu bằng chứng hoặc chạm hệ thống nhạy cảm phải được kỹ sư duyệt. |

**Phản biện bắt buộc đối với v0:** Nhóm ban đầu gộp độ trễ phát hiện, thời gian tra log và xử lý thành một con số 90–120 phút; chưa xác nhận actor nào thật sự mất lâu đến vậy. Ngoài ra, v0 thiên về rút ngắn thời gian tra log, chưa đo độc lập rủi ro **chặn nhầm truy cập hợp lệ**.

---

## 2. CP6 — Dữ liệu cho Problem Statement v1 (sau CP4)

CP4 nhóm ghi nhận **5 người ngoài nhóm** đã từng trực sự cố. Theo bản tổng hợp, thời gian khoanh vùng thường **15–30 phút**, **2/5** người thường xuyên bị gọi dậy ban đêm; nhiều nơi đã có Grafana/Loki/Prometheus hoặc Datadog/New Relic. Phần lớn người được hỏi không chấp nhận tự chặn vô điều kiện, chỉ cân nhắc khi có whitelist, thời hạn chặn và rollback. Vì vậy v1 cần chuyển trọng tâm sang **phát hiện và phản ứng ngoài giờ an toàn**, chứ không tuyên bố mọi sự cố đều mất 90–120 phút để đọc log.

| Trường | Nội dung đề xuất để nhóm rà soát và tự chốt |
|---|---|
| **Actor** | Kỹ sư DevOps/SRE trực ca của hệ thống dịch vụ web có cổng Nginx và các nguồn log phụ trợ; giai đoạn pilot chỉ xét bất thường có thể cô lập cục bộ tại cổng vào. |
| **Quy trình** | Hiện tại: nhận cảnh báo/ticket → tra log và lọc nhiễu → đối chiếu nguồn liên quan → xác định nghi vấn → kỹ sư quyết định chặn hoặc escalation → kiểm tra. Quy trình đề xuất: Rule lọc nhiễu → công cụ chỉ đọc truy nguồn log phù hợp → tính Confidence Score từ tín hiệu kỹ thuật → thực thi runbook có giới hạn **hoặc** gửi kỹ sư duyệt HITL → self-check và rollback. |
| **Bottleneck** | **Đã thu hẹp sau phỏng vấn:** phần khó nhất không nhất thiết là đọc log trong giờ hành chính (15–30 phút), mà là độ trễ phát hiện/nhận xử lý ngoài giờ, cảnh báo giả và việc phối hợp nhiều tín hiệu trước khi quyết định phản ứng an toàn. Bước 3–4 vẫn cần đo từng loại incident khi pilot. |
| **Impact** | Trong mẫu phỏng vấn nhỏ, **2/5** người cho biết thường bị gọi dậy ban đêm; đa số nhắc đến cảnh báo giả, tra log liên tầng. Chưa có số đo đáng tin cậy cho **thời gian từ bắt đầu bất thường đến cô lập ngoài giờ**, nên chưa thể xác nhận baseline 90–120 phút. |
| **Success Metric** | **Baseline có thông tin khảo sát:** khoanh vùng tầng lỗi thường 15–30 phút, không đồng nhất với thời gian cô lập. **Baseline còn phải thu thập:** median thời gian phát hiện→cô lập ngoài giờ; cảnh báo giả/ca; số ca chặn nhầm. **Target pilot do nhóm đề xuất:** ca đủ điều kiện auto-containment dưới 5 phút; ca cần HITL dưới 15 phút; cảnh báo giả dưới 15%; **0 lần chặn nhầm IP/dịch vụ hợp lệ**. **Cách đo:** dùng timestamp Nginx/monitoring, alert, runbook, phiếu phê duyệt và rollback trên cùng một tập incident mô phỏng/đã ẩn danh, báo riêng từng nhánh. |
| **Boundary** | Tài khoản điều tra chỉ đọc log được phép; hệ thống **không tự sinh shell command**. Chỉ có thể gọi runbook tham số hóa tại Nginx/WAF, không tác động IP trong whitelist hoặc dịch vụ cốt lõi. Confidence Score không do LLM tự tuyên bố mà tổng hợp từ tín hiệu kỹ thuật; 60–<85% hoặc chạm hệ thống lõi buộc HITL; ≥85% chỉ tự thực thi nếu thuộc nhóm tác động cục bộ đã được phê duyệt. Tự hết hạn sau 15 phút, kiểm tra lại sau 2 phút, rollback nếu không cải thiện. |
| **AI intervention point** | Sau bước Rule nhận biết bất thường: hỗ trợ lựa chọn **nguồn log cần tra tiếp** và tổng hợp bằng chứng đa tầng. Quyết định cho phép chạy runbook phải do cơ chế rule/permission ngoài LLM kiểm soát. |
| **Mức chọn** | **Định hướng nhóm đã ghi ở CP6:** Rule + Agent có kiểm soát (Bounded Autonomy), nhánh HITL. **Chưa phải kết quả pilot chứng minh Agent tốt hơn Workflow.** |
| **Rủi ro & người kiểm tra** | Tương quan log sai hoặc bỏ sót nguồn: DevOps/SRE xem ID log, timestamp, trace. Tự tin cao giả/nhầm nguồn tấn công: kỹ sư bảo mật duyệt công thức/whitelist và ngưỡng. Chặn nhầm: kỹ sư on-call nhận cảnh báo và có kill switch/rollback. Rò dữ liệu: quản trị hạ tầng kiểm RBAC, audit log. |

---

## 3. CP6 — Bảng khác biệt v0 → v1

| Trường | v0 (giả định trước khảo sát) | v1 (điều chỉnh theo thông tin nhóm) | Căn cứ thay đổi |
|---|---|---|---|
| **Actor** | Kỹ sư trực ca quản lý hạ tầng nhiều tầng nói chung | Kỹ sư trực hệ thống web; pilot thu hẹp ở cổng Nginx và các tình huống cô lập cục bộ | Phạm vi pilot nhóm định hướng ở CP6, giảm quyền tác động |
| **Problem trọng tâm** | Kỹ sư mất 90–120 phút vì tra nhiều nguồn log | Ngoài giờ phản ứng trễ và cảnh báo giả; tra log là một bước trong chuỗi | CP4: khoanh vùng trong giờ thường 15–30 phút; 2/5 thường bị gọi dậy ban đêm |
| **Bottleneck** | Bước lọc và đối chiếu log: 55 phút theo sơ đồ ban đầu | Phân biệt độ trễ phát hiện, lọc cảnh báo giả, điều tra và chờ phản hồi người trực | CP4 phản bác việc mọi ca đều mất 60–90 phút khoanh vùng |
| **Success Metric** | Giảm từ 90–120 phút xuống dưới 5/15 phút | Tách baseline **15–30 phút khoanh vùng** với baseline **ngoài giờ chưa đo**; thêm cảnh báo giả <15% và 0 chặn nhầm; đo mỗi nhánh | Không thể dùng thời gian khoanh vùng làm baseline của thời gian cô lập |
| **Boundary** | Có con người duyệt ca nhạy cảm; không cho shell tự do | Thêm whitelist, ngưỡng 60%/85%, runbook tham số hóa, TTL 15 phút, self-check sau 2 phút, rollback | Phỏng vấn: đa số phản đối auto-block vô điều kiện; nhóm đã thiết kế điều kiện kiểm soát |
| **AI intervention point** | Chưa xác định cụ thể | Tra cứu log theo ngữ cảnh và tổng hợp bằng chứng sau Rule lọc nhiễu; lớp policy riêng cho phép/chặn thực thi | So sánh 4 mức tại CP6, giảm quyền trực tiếp của mô hình |
| **Mức can thiệp** | Chưa chốt | Định hướng Agent có giới hạn + Rule + HITL, thử tại Nginx | Quyết định thiết kế nhóm ghi trong mục 6; chưa xác nhận qua pilot |

---

## 4. CP6 — 5 tiêu chí đánh giá (eval) đề xuất

Các ngưỡng dưới đây là **tiêu chuẩn thử nghiệm đề xuất**, chưa có kết quả đo. Để chấm công bằng, người kiểm phải dùng bộ sự cố có nhãn/đáp án đã xác nhận, gồm cả sự cố giả và lưu lượng hợp lệ.

| # | Tiêu chí | **Đạt khi** | **Không đạt khi** | Cách kiểm |
|---:|---|---|---|---|
| 1 | **Bằng chứng truy xuất được** | 100% nhận định nguyên nhân/nguồn tấn công quan trọng có log ID, timestamp và nguồn kiểm lại được; nếu không đủ bằng chứng phải ghi “chưa xác định” | Có kết luận chắc chắn không có nguồn hoặc tự tạo chi tiết log | DevOps mở lại nguồn gốc của từng nhận định trên bộ incident |
| 2 | **Khoanh vùng và không bỏ sót** | Có trong top-3 ít nhất 1 thành phần hoặc nguồn nghi vấn trùng đáp án hậu kiểm ở ≥80% case; recall tín hiệu cốt lõi ≥90% | Bỏ qua tín hiệu dẫn đến cô lập sai hoặc tỷ lệ đạt thấp hơn ngưỡng | So với incident hậu kiểm do kỹ sư gán nhãn |
| 3 | **Lọc cảnh báo giả** | Tỷ lệ alert bị xác nhận là sai dưới 15% trên bộ thử đại diện cả giờ cao điểm, đêm và ngày thường | False-alert rate ≥15% hoặc bỏ qua sự cố thật nghiêm trọng | Tính tỷ lệ theo nhãn cảnh báo và nhật ký Rule |
| 4 | **Quyền hạn và chặn nhầm** | 0 truy cập vượt quyền, 0 hành động ngoài danh mục runbook, 0 chặn nhầm whitelist/đối tác/người dùng hợp lệ; mọi hành động có TTL, rollback và audit log | Chỉ **một** trường hợp vượt quyền, chặn nhầm hoặc thiếu rollback/audit | Test RBAC/whitelist, giả lập lưu lượng hợp lệ, kiểm nhật ký |
| 5 | **Thời gian phát hiện và phản ứng** | Tính riêng từ khi có bất thường đến cô lập: ca auto đủ điều kiện <5 phút; ca HITL <15 phút; không vi phạm tiêu chí 1–4 | Vượt mục tiêu hoặc nhanh hơn nhưng kết luận/chặn sai | So timestamp sự kiện, alert, hành động, phê duyệt và hậu kiểm; so theo cùng nhóm incident |

**Cách đọc metric:** 15–30 phút trong CP4 là thời gian **khoanh vùng**, còn <5 phút/<15 phút là mục tiêu **cô lập/phản ứng** theo hai nhánh khác nhau. Không dùng 15–30 phút làm baseline trực tiếp cho chỉ số cô lập, vì chúng đo khác giai đoạn.

**Rủi ro còn mở:** Chưa có kết quả pilot kiểm định công thức Confidence Score (40% thống kê + 40% bằng chứng + 20% whitelist), các ngưỡng 60/85% hay false-alert rate <15%. Cần thử và hiệu chỉnh với sự cố gán nhãn; không gọi các con số đó là độ tin cậy đã chứng minh.

---

## 5. Hướng tự hoàn thiện theo đúng RULES.md

- Nhóm đối chiếu từng dòng với 5 ghi chép phỏng vấn và sơ đồ CP5, sửa bằng cách diễn đạt của mình. Đặc biệt xác nhận câu nào là **giả định** và câu nào đã có **bằng chứng**.
- Bảo và các thành viên **tự viết lại/chốt** bảng v0 và v1 để đưa vào `report/team/group_report.md` mục 5 và 7. Tài liệu này chỉ là **phân tích hỗ trợ và phản biện**, không được trình bày như bài nhóm đã tự viết.
- Không ghi kết quả đánh giá “đã đạt” khi chưa chạy thử. Sau khi thống nhất ngưỡng, mới điền mục 8 (quyết định) và minh chứng thử nghiệm nếu có.
