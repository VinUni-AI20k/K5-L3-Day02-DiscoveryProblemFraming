# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: **NEU65**
- Candidate problem nhóm chọn (1 câu): BA trong team phát triển AI Agent y tế mất nhiều thời gian đọc, trích xuất và đối chiếu thông tin từ tài liệu của các hệ thống HIS/EHR/AI Agent để lập bảng benchmarking.
- Quyết định cuối (Go / Not Yet / No-Go): **Not Yet**

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Vũ Quang Thái | 2A202603545 | Đề xuất candidate về sự kiện NEU; phản biện, tham gia phân tích quy trình và đánh giá quyết định | [vuThai05](https://github.com/vuThai05) |
| 2 | Nguyễn Thị Thùy Dung | 2A202603552 | Đề xuất candidate benchmarking; phụ trách chính phần research/kiểm chứng và xây dựng hướng workflow | [Dunnguyn](https://github.com/Dunnguyn) |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Thị Thùy Dung | Vũ Quang Thái | Cluster, cây OST, bảng chấm điểm; Thái đóng góp 3 candidate sự kiện NEU và tham gia đối chiếu shortlist |
| CP4 — Kiểm chứng | Vũ Quang Thái | Nguyễn Thị Thùy Dung | Assumption map, câu hỏi kiểm chứng và 2 interview snapshots; snapshots chỉ là mô phỏng/thăm dò, thời gian là ước lượng hồi tưởng |
| CP4 — Research | Nguyễn Thị Thùy Dung | Vũ Quang Thái | Bảng research G2, Elicit, Consensus và phân tích khoảng trống |
| CP5 — Quy trình trước/sau | Nguyễn Thị Thùy Dung | Vũ Quang Thái | AS-IS/TO-BE, bottleneck, Rule, AI Workflow, HITL và fallback |
| CP5 — Problem Statement v0 | Vũ Quang Thái | Nguyễn Thị Thùy Dung | Problem Statement v0: actor, quy trình, bottleneck, impact, metric, boundary |
| CP6 — Mức can thiệp + Problem Statement v1 | Vũ Quang Thái | Nguyễn Thị Thùy Dung | Ma trận, AI Canvas, tiêu chí đánh giá và Problem Statement v1 |
| CP6 — Quyết định | Cả hai | Cả hai | Đánh giá 4 rủi ro; thống nhất Not Yet và đề xuất pilot nhỏ |

## Cá nhân

### VuQuangThai-2A202603545

**Phần việc phụ trách:**

- Đề xuất và trình bày 3 candidate liên quan đến việc sinh viên NEU tìm kiếm, tổng hợp và theo dõi thông tin sự kiện.
- Phản biện candidate của thành viên còn lại; tham gia phân nhóm vấn đề, đối chiếu shortlist và thống nhất lựa chọn.
- Tham gia rà soát quy trình AS-IS/TO-BE, Problem Statement, mức can thiệp AI và quyết định cuối.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đưa vào nhóm 3 candidate về tìm sự kiện từ nhiều nguồn, tổng hợp thông tin để chọn sự kiện và theo dõi deadline/lịch.
- Đặt câu hỏi về tần suất, bằng chứng pain point và khả năng giải quyết bằng phương án không dùng AI.
- Cùng nhóm phân tích candidate benchmarking HIS/EHR/AI Agent; tham gia làm rõ bottleneck, metric, boundary và lựa chọn Workflow kết hợp Rule + HITL.
- Đồng thuận quyết định **Not Yet** vì baseline và pain point chưa được xác nhận bằng dữ liệu thực tế.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo cá nhân `2A202603545_VuQuangThai.md`: mục 2–6.
- `group_report.md`: mục 2.1 (candidate #1–#3), 2.2–2.4 (cluster, OST, shortlist và lựa chọn), mục 3–8 (kiểm chứng, quy trình, Problem Statement, AI intervention và quyết định).
- Commit: f341496 trên branch thai.

**Điều mình học được từ phần nhóm:**

- Kỹ năng điều phối nhóm, hợp nhất nhánh Git và lắng nghe các góc nhìn phản biện đa chiều về bài toán thực tế; hiểu chuỗi logic từ xác định vấn đề, phân tích quy trình, đo lường metric, thiết lập an toàn cho đến lựa chọn mức can thiệp AI phù hợp.

### NguyenThiThuyDung-2A202603552

**Phần việc phụ trách:**

- Đề xuất candidate benchmarking HIS/EHR/AI Agent và trình bày Problem Card.
- Phụ trách chính việc xác định giả định cần kiểm chứng, xây dựng câu hỏi/snapshot và research công cụ hiện có.
- Đóng góp chính vào phân tích quy trình, Problem Statement và lựa chọn mức can thiệp AI.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đề xuất candidate benchmarking đạt 32/35 điểm và được nhóm lựa chọn.
- Xác định hai giả định ưu tiên, xây dựng câu hỏi Mom Test và mẫu Interview Snapshot; nghiên cứu G2, Elicit, Consensus.
- Mô tả AS-IS/TO-BE; xác định điểm can thiệp AI tại bước đọc/trích xuất, kết hợp Rule, Human-in-the-loop và fallback.
- Tham gia xây dựng Problem Statement v0/v1, tiêu chí đánh giá, bốn rủi ro và đề xuất pilot; thống nhất quyết định **Not Yet**.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo cá nhân `2A202603552_NguyenThiThuyDung.md`: mục 3–6.
- `group_report.md`: mục 2.1–2.4 (candidate, cluster, OST, shortlist), mục 3 (assumption map, kiểm chứng, research), mục 4–8 (quy trình, Problem Statement, mức can thiệp và quyết định).
- Commit: dd9e42a, a6351ec, b41c374 trên branch dung.

**Điều mình học được từ phần nhóm:**

- Học hỏi được phương pháp khảo sát và đối chiếu các giải pháp có sẵn trên thị trường để tìm ra khoảng trống giá trị (value gap) cho bài toán của nhóm.

---