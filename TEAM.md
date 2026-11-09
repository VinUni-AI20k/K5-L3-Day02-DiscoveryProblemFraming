# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: Nhomabc404
- Candidate problem nhóm chọn (1 câu): Người được hỏi phải giải thích lại cùng một câu hỏi cho đồng nghiệp, bạn học, khoảng 2 lần/tuần và khoảng 15–30 phút mỗi lần (survey 10 người, ước lượng). *(Bản nháp, chờ nhóm xác nhận.)*
- Quyết định cuối (Go / Not Yet / No-Go): Go, phạm vi nhỏ (pilot FAQ, No AI) *(bản nháp, chờ nhóm xác nhận)*

## Thành viên

| STT | Họ và tên           | MSSV        | Vai trò trong nhóm                                    | Tài khoản GitHub |
| --: | ------------------- | ----------- | ----------------------------------------------------- | ---------------- |
| 1   | Nguyễn Quang Đạo    | 2A202603614 | Phụ trách Research, Phụ trách Mức can thiệp AI & PS v1 | NguyenQuangDao   |
| 2   | Đỗ Cao Cường        | 2A202603612 | Vẽ quy trình trước/sau, Viết Problem Statement v0     | cuongdc03        |
| 3   | Hồ Sỹ Tùng          | 2A202603650 | Ghi chép, Phụ trách Hội tụ nhóm (Cluster & OST)       | SyxTun9          |
| 4   | Trần Quốc Đông      | 2A202603643 | Nhóm trưởng, Điều phối thời gian, Phản biện chính     | dongtranquoc951  |
| 5   | Trần Đức Mạnh       | 2A202603615 | Phụ trách Kiểm chứng (Assumption Map & Survey)        | trmanh204        |
| 6   | Nguyễn Văn Ngọc Sơn | 2A202603600 | Phụ trách Đánh giá rủi ro & Quyết định CP6            | kynnnS           |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Hồ Sỹ Tùng | Trần Quốc Đông | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Trần Đức Mạnh | Đỗ Cao Cường | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Quang Đạo | Nguyễn Văn Ngọc Sơn | Bảng research có link |
| CP5 — Quy trình trước/sau | Đỗ Cao Cường | Trần Đức Mạnh | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Đỗ Cao Cường | Hồ Sỹ Tùng, Trần Quốc Đông | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Quang Đạo | Nguyễn Văn Ngọc Sơn | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Nguyễn Văn Ngọc Sơn | Trần Quốc Đông | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenQuangDao-2A202603614

**Phần việc phụ trách:**

- Phụ trách chính **CP4 — Research** (nghiên cứu các giải pháp/công cụ có sẵn giải quyết bài toán hỏi đáp lặp lại).
- Phụ trách chính **CP6 — Mức can thiệp AI + Problem Statement v1** (phân tích ma trận độ mơ hồ × độ phức tạp, so sánh 4 mức can thiệp, lập AI Canvas rút gọn, viết Problem Statement v1 và bộ tiêu chí đánh giá).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp 3 candidate problem cá nhân (#1, #2, #3) vào bảng Pitch ở CP3.
- Tìm hiểu, mở kiểm tra thực tế và tổng hợp bảng đối chiếu 3 giải pháp có sẵn (Slack Workflow Builder trả lời FAQ bằng emoji, Notion Q&A / Notion Agent, Slack AI) để rút ra bài học cốt lõi: dù có AI hay không thì điều kiện tiên quyết vẫn phải có tài liệu FAQ nguồn chuẩn xác.
- Xác định vị trí bài toán trên ma trận (mơ hồ thấp × vận hành đơn giản), lập bảng so sánh 4 mức (`No AI` / `Rule` / `Workflow` / `Agent`) và lập luận chọn mức **No AI** (trang FAQ dùng chung).
- Điền AI Canvas rút gọn, trả lời 2 câu hỏi của Google PAIR và xây dựng 5 tiêu chí đánh giá (eval) kèm ngưỡng đạt/không đạt.
- Cập nhật **Problem Statement v1** từ bản v0 dựa trên dữ liệu survey 10 người (điều chỉnh baseline từ `30–60 phút/lần` về mức phổ biến `15–30 phút/lần`, bổ sung chỉ số tần suất và làm rõ boundary/người kiểm tra).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo nhóm `report/team/group_report.md`: Mục 2.1 (candidate #1–#3), Mục 3.3 (Research giải pháp đã có), Mục 6 (Mức can thiệp AI: 6.1, 6.2, 6.3, 6.4) và Mục 7 (Problem Statement v1 + tiêu chí đánh giá).
- Báo cáo cá nhân: `report/individual/2A202603614_NguyenQuangDao.md`.

**Điều mình học được từ phần nhóm:**

- Khi đối chiếu các công cụ lớn như Slack hay Notion ở bước Research, mình nhận ra công cụ AI hỏi đáp chỉ phát huy tác dụng khi nhóm đã có sẵn tài liệu chuẩn và được duy trì đều đặn; nếu chưa có FAQ mà nhảy ngay lên làm chatbot/agent thì vừa tốn công vừa dễ sinh câu trả lời sai (báo nhầm với giọng chắc chắn). Nhờ kết hợp kết quả survey 10 người với research thực tế, việc chọn mức **No AI** (pilot FAQ trong 2 tuần) trở nên thuyết phục và tiết kiệm hơn rất nhiều.

### DoCaoCuong-2A202603612

**Phần việc phụ trách:**

- Phụ trách chính **CP5 — Quy trình trước/sau** (vẽ sơ đồ quy trình hiện tại và tương lai, lập bảng đối chiếu Before/After).
- Phụ trách chính **CP5 — Problem Statement v0** (viết bản đặc tả bài toán đầu tiên gồm 6 trường trước khi đưa vào kiểm chứng mức can thiệp).
- Hỗ trợ **CP4 — Kiểm chứng** (đối chiếu giả định ban đầu của candidate #5 với kết quả khảo sát).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp 3 candidate problem (#4, #5, #6) ở CP3, trong đó candidate #5 (*Giải thích lại cùng một câu hỏi cho đồng nghiệp, bạn học*) được cả nhóm chấm cao nhất (30/35 điểm) và chọn làm bài toán chung; ghi phiếu chấm điểm và câu hỏi phản biện cho candidate #8.
- Phác thảo sơ đồ quy trình hiện tại (4 bước, xác định bottleneck ở bước 3 — giải thích lại từ đầu) và quy trình tương lai theo hướng **No AI** (tự tra FAQ/tin ghim trước khi hỏi trực tiếp, kèm bước cập nhật câu mới và phương án quay về).
- Lập bảng so sánh **Before / After** về số bước, tổng thời gian, số bước thủ công và các rủi ro mới phát sinh (FAQ lỗi thời, người hỏi không đọc, thiếu người duy trì).
- Soạn **Problem Statement v0** đầy đủ 6 trường (*Actor, Quy trình, Bottleneck, Impact, Success Metric, Boundary*) và ghi nhận các điểm phản biện ban đầu.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo nhóm `report/team/group_report.md`: Mục 2.1 (candidate #4–#6), Mục 2.4 (phiếu chấm điểm cá nhân và dữ kiện gốc của candidate #5), Mục 4 (Quy trình trước/sau: 4.1, 4.2, 4.3) và Mục 5 (Problem Statement v0).
- Báo cáo cá nhân: `report/individual/2A202603612_DoCaoCuong.md`.

**Điều mình học được từ phần nhóm:**

- Con số ước lượng cảm tính ban đầu của cá nhân mình (`30–60 phút/lần`) khi đem ra khảo sát 10 người ở CP4 đã được hiệu chỉnh lại sát thực tế hơn (`15–30 phút/lần` là phổ biến nhất, chỉ 3/10 người rơi vào mức `30–60 phút`). Việc vẽ rõ quy trình hiện tại và tương lai giúp nhóm thấy ngay nút thắt nằm ở chỗ thiếu một nơi lưu câu trả lời chuẩn chứ chưa cần tới công cụ AI phức tạp.

### HoSyTung-2A202603650

**Phần việc phụ trách:**

- Phụ trách chính **CP3 — Hội tụ nhóm** (tổng hợp 18 candidate từ 6 thành viên, gom nhóm Cluster, vẽ cây Opportunity Solution Tree rút gọn và lập bảng chấm điểm shortlist).
- Hỗ trợ **CP5 — Problem Statement v0** (rà soát tính nhất quán giữa nhánh Opportunity B trên cây OST và bản Problem Statement v0).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp 3 candidate problem (#7, #8, #9) vào bảng Pitch của nhóm, trong đó candidate #8 được đưa vào shortlist 3 bài toán để chấm điểm chi tiết.
- Phân loại 18 candidate của cả nhóm thành 4 nhóm có cùng quy luật (Cluster A: Gom và đọc thông tin rải ở nhiều nguồn; Cluster B: Câu hỏi/yêu cầu lặp lại xử lý bằng tay; Cluster C: Kiểm tra, phát hiện lỗi hoặc sai lệch; Cluster D: Việc nhỏ hằng ngày thiếu tín hiệu nhắc đúng lúc).
- Vẽ cây **Opportunity Solution Tree (OST)** rút gọn từ 1 Outcome gốc ra 4 nhánh Opportunity, đồng thời rà soát và gạch bỏ 4 ý bị viết theo kiểu "solution đội lốt opportunity" (#3, #7, #14, #15) để viết lại thành pain thật của người dùng.
- Tổng hợp bảng chấm điểm 7 tiêu chí cho 3 candidate trong shortlist (#5, #8, #15) và ghi rõ lý do chọn #5 cũng như lý do loại các candidate còn lại.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo nhóm `report/team/group_report.md`: Mục 2.1 (candidate #7–#9), Mục 2.2 (Bảng Cluster), Mục 2.3 (Cây Opportunity Solution Tree rút gọn & danh sách các solution đội lốt opportunity đã sửa), Mục 2.4 (Bảng chấm điểm shortlist).
- Báo cáo cá nhân: `report/individual/2A202603650_HoSyTung.md`.

**Điều mình học được từ phần nhóm:**

- Lỗi phổ biến nhất khi mới nêu vấn đề là đưa luôn tính năng hoặc cách giải vào câu mô tả (như candidate #7 của mình "Tìm kiếm ảnh chụp màn hình theo nội dung" thực chất là tính năng, còn nỗi đau thật là "không tìm lại được ảnh chụp màn hình khi cần dùng"). Nhờ bước vẽ cây OST và nhận câu hỏi phản biện từ nhóm cho candidate #8, mình hiểu rõ vì sao một bài toán phải có Actor, nguồn dữ liệu và số phút đo đếm được thì mới đủ điều kiện đi tiếp.

### TranQuocDong-2A202603643

**Phần việc phụ trách:**

- **Nhóm trưởng & Điều phối thời gian:** quản lý repo chung của nhóm, phân bổ thời gian qua các checkpoint (CP3 → CP6) và kiểm tra chất lượng tổng thể của báo cáo nhóm.
- **Người phản biện chính:** đặt câu hỏi phản biện trong phiên Pitch (CP3), kiểm tra chéo các giả định ở CP4 và phản biện Problem Statement v0/v1 (CP5–CP6).
- Hỗ trợ **CP3 — Hội tụ nhóm**, **CP5 — Problem Statement v0** và **CP6 — Quyết định**.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Khởi tạo, quản lý cấu trúc repo nhóm và tổng hợp thông tin chung tại Mục 1 `group_report.md` cùng `TEAM.md`.
- Đóng góp 3 candidate problem (#10, #11, #12) vào bảng Pitch ở CP3.
- Đóng vai trò phản biện chính ở các bước chuyển tiếp: chất vấn các candidate chưa rõ actor/bottleneck ở CP3, chỉ ra hạn chế của khảo sát ở CP4 (câu hỏi "Sẵn sàng dùng FAQ" mới chỉ là ý định tương lai theo *The Mom Test* chứ chưa phải hành vi thật), và yêu cầu làm rõ ai là người duy trì FAQ hàng tuần.
- Cùng phụ trách CP6 rà soát mục 8 (4 rủi ro + ngưỡng dừng) và biên tập Mục 9 (*Hạn chế và hướng tiếp theo*) để đảm bảo báo cáo nhóm trung thực, không phóng đại số liệu.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo nhóm `report/team/group_report.md`: Mục 1 (Thông tin nhóm), Mục 2.1 (candidate #10–#12), Mục 3.2 (phần Hạn chế của survey theo *The Mom Test*), Mục 5 (phần phản biện PS v0), Mục 8.2 & Mục 9 (Hạn chế và hướng tiếp theo).
- Quản lý và rà soát file `TEAM.md`, `report/individual/2A202603643_TranQuocDong.md`.

**Điều mình học được từ phần nhóm:**

- Điều phối một buổi Discovery hiệu quả không nằm ở việc cố chọn một bài toán nghe thật kêu để gắn AI vào, mà là giữ cho cả nhóm bám sát bằng chứng thực tế ở từng checkpoint. Khi đóng vai người phản biện theo nguyên tắc *The Mom Test*, mình học được cách phân biệt giữa lời đồng tình xã giao ("7/10 sẵn sàng dùng FAQ") với cam kết hành vi thật, từ đó giúp nhóm chọn phương án **Go phạm vi nhỏ (pilot 2 tuần)** kèm ngưỡng dừng rõ ràng.

### TranDucManh-2A202603615

**Phần việc phụ trách:**

- Phụ trách chính **CP4 — Kiểm chứng** (lập bảng Assumption Map và thiết kế, thu thập, phân tích kết quả Survey 10 người).
- Hỗ trợ **CP5 — Quy trình trước/sau** (cung cấp số liệu baseline thực tế từ khảo sát để cập nhật vào sơ đồ quy trình và bảng Before/After).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp 3 candidate problem (#13, #14, #15) vào bảng Pitch ở CP3, trong đó candidate #15 (*Đọc paper PDF dài để lấy phương pháp và dataset*) lọt vào shortlist 3 bài toán và đạt 24/35 điểm.
- Xây dựng **Assumption Map** gồm 6 giả định cốt lõi của bài toán #5 (phân loại theo 4 nhóm *Value, Usability, Feasibility, Viability* và chấm điểm mức độ quan trọng × mức độ bằng chứng từ 1–5) để chọn ra 4 giả định ưu tiên kiểm chứng ngay (#1, #2, #3, #4).
- Thiết kế và tổng hợp dữ liệu thô từ **Survey 10 người** (R1 → R10 gồm Kỹ sư phần mềm, Trưởng nhóm, Nhân viên văn phòng, Sinh viên) trên 4 chỉ số: tần suất bị hỏi lại trong 2 tuần, thời gian mỗi lần, mức độ giống nhau của câu hỏi và mức sẵn sàng dùng FAQ.
- Phân tích tín hiệu xác nhận & **phản bác một phần** (chỉ 3/10 mất 30–60 phút, còn phổ biến là 15–30 phút; ước lượng trung bình ~65 phút/tuần/người), từ đó đề xuất nhóm sửa lại baseline và đổi quyết định sang Go phạm vi nhỏ.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo nhóm `report/team/group_report.md`: Mục 2.1 (candidate #13–#15), Mục 3.1 (Assumption Map), Mục 3.2 (Bảng dữ liệu thô R1–R10, bảng tổng hợp chỉ số và mục "Nhóm đã sửa problem thế nào sau kiểm chứng").
- Báo cáo cá nhân: `report/individual/2A202603615_TranDucManh.md`.

**Điều mình học được từ phần nhóm:**

- Kiểm chứng thực tế giúp nhóm thoát khỏi cái bẫy tự suy diễn từ trải nghiệm của 1 người: giả định ban đầu nghĩ rằng mỗi lần giải thích mất tới 30–60 phút, nhưng dữ liệu khảo sát 10 người đã phản bác một phần con số đó và chỉ ra mức 30–60 phút chỉ xảy ra ở nhóm Trưởng nhóm và Kỹ sư phần mềm bị hỏi dồn nhiều lần. Chính những tín hiệu phản bác một phần này lại làm cho bài toán và chỉ số Success Metric của nhóm trở nên đáng tin cậy hơn.

### NguyenVanNgocSon-2A202603600

**Phần việc phụ trách:**

- Phụ trách chính **CP6 — Quyết định** (đánh giá 4 nhóm rủi ro *Value, Usability, Feasibility, Viability*, lập luận quyết định *Go / Not Yet / No-Go*, thiết kế kế hoạch pilot nhỏ nhất và ngưỡng dừng).
- Hỗ trợ **CP4 — Research** và **CP6 — Mức can thiệp AI + Problem Statement v1** (cùng đối chiếu công cụ và xây dựng bộ 5 tiêu chí đánh giá đầu ra).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp 3 candidate problem (#16, #17, #18) về kiểm soát lỗi chất lượng mô hình và hệ thống vào bảng Pitch ở CP3 (thuộc Cluster C).
- Phối hợp ở CP4 Research và CP6 để xây dựng 5 tiêu chí đánh giá (eval) cho FAQ / AI (*Đúng nội dung, Tìm thấy nhanh ≤ 2 phút, Không bịa ngoài FAQ, Chuyển người khi không chắc, Cập nhật câu hỏi lặp lại ≥ 2 lần trong 1 tuần*).
- Phân tích và chấm mức độ cho **4 rủi ro** tại Mục 8.1: *Value* (Thấp), *Usability* (Trung bình — vì ý định dùng FAQ chưa phải hành vi thật), *Feasibility* (Thấp — FAQ viết tay không đòi hỏi kỹ thuật phức tạp), *Viability* (Trung bình — cần chỉ định người duy trì FAQ hàng tuần).
- Viết kết luận quyết định **Go, phạm vi nhỏ (pilot FAQ, mức No AI)** tại Mục 8.2, xác định quy mô pilot 2 tuần cho 5 câu hỏi phổ biến nhất và đặt **ngưỡng dừng định lượng** sau 2 tuần và 4 tuần.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo nhóm `report/team/group_report.md`: Mục 2.1 (candidate #16–#18), hỗ trợ Mục 3.3 & Mục 7 (bảng 5 tiêu chí đánh giá), phụ trách chính Mục 8 (8.1 Bốn rủi ro, 8.2 Kết luận Go/Not Yet/No-Go và Ngưỡng dừng).
- Báo cáo cá nhân: `report/individual/2A202603600_NguyenVanNgocSon.md`.

**Điều mình học được từ phần nhóm:**

- Trước buổi lab, mình thường nghĩ các bài toán trong khóa AI đều phải kết thúc bằng việc xây một workflow hay agent tự động. Tuy nhiên, khi đặt 4 rủi ro (*Value, Usability, Feasibility, Viability*) lên bàn cân cùng ngưỡng dừng đo đếm được, mình thấy rõ rủi ro lớn nhất hiện tại nằm ở *Usability* (liệu đồng nghiệp có chịu tự tra FAQ không) và *Viability* (ai cập nhật FAQ hàng tuần), chứ không phải bài toán kỹ thuật AI. Một quyết định **Go phạm vi nhỏ với No AI** giúp kiểm chứng đúng rủi ro cốt lõi với chi phí bằng 0 trước khi quyết định có đầu tư công nghệ hay không.
