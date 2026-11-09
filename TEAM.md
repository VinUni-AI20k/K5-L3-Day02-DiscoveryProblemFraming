# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm:
- Candidate problem nhóm chọn (1 câu):
- Quyết định cuối (Go / Not Yet / No-Go):

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | Lê Nguyễn Anh Khôi | 2A202603755 | Điều phối thời gian, chốt Problem Statement v1 | KN-16 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | | | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | | | Assumption map, snapshot hoặc survey |
| CP4 — Research | | | Bảng research có link |
| CP5 — Quy trình trước/sau | | | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | | | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | | | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | | | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### LeNguyenAnhKhoi-2A202603755

**Phần việc phụ trách:**
- Pitch 3 Problem Card cá nhân (Khiếu nại tài xế, Cứu hộ sạc pin khẩn cấp, Tiếp nhận xe xưởng dịch vụ); bảo vệ bài #3 để nhóm chọn làm bài toán chung.
- Điều phối tiến độ thảo luận của nhóm, hỗ trợ Cường gom nhóm Cluster và xây dựng cây Opportunity Solution Tree (OST) rút gọn.
- Phụ trách chính xây dựng Problem Statement v0 và phối hợp hoàn thiện Problem Statement v1 sau khi nhận phản biện.
- Phụ trách chính Mục 8 Quyết định: đánh giá 4 loại rủi ro (Value, Usability, Feasibility, Viability), xây dựng kịch bản thử nghiệm pilot 2 tuần và thiết lập 2 ngưỡng dừng.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Đóng góp candidate được chọn làm đề tài chính của nhóm (#3 — Đối chiếu khiếu nại tài xế với telemetry GPS và chat, đạt điểm cao nhất 32/35 điểm).
- Đặt câu hỏi phản biện cho 4 bài của các thành viên: Hiếu (#1 — *Hơn gì Google Maps*), Cường (#4 — *Phòng khám vắng ưu tiên ai*), Hải (#10 — *Phát hiện gian lận ảnh mờ*), Hiếu (#12 — *Phân biệt tin bài tập chính thức*).
- Tiếp thu phản biện của Hải để bổ sung cơ chế cờ đối chiếu chéo (Cross-check Flag) giữa telemetry GPS và log chat, ngăn chặn gian lận mẫu câu.
- Soạn thảo Problem Statement v0 và nâng cấp lên v1 (bổ sung 2 metric chặn: tỷ lệ xem lại log < 20% và tỷ lệ khiếu nại lần hai giảm ≥ 40%).
- Đánh giá 4 rủi ro, chốt quyết định Go phạm vi nhỏ (pilot 50 ticket) và đưa ra 2 ngưỡng dừng định lượng dứt khoát.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Bảng Pitch (candidate #3, #6, #7) và các câu hỏi phản biện trong Mục 2.1 `group_report.md`.
- Mục 2.4 Bảng chấm điểm shortlist (candidate #3 được chọn).
- Mục 5 Problem Statement v0 và Mục 7 Problem Statement v1 trong `group_report.md`.
- Mục 8.1 và 8.2 (Bốn rủi ro, Quyết định Go, Kịch bản pilot & Ngưỡng dừng) trong `group_report.md`.
- File cá nhân: `report/individual/2A202603755_LeNguyenAnhKhoi.md`.

**Điều mình học được từ phần nhóm:**
- Nhận thức rõ ràng ranh giới giữa một sự bất tiện thoáng qua (minor inconvenience) và một nỗi đau vận hành cấp tính (acute pain) có tác động tài chính trực tiếp đến con người.
- Thấu hiểu sâu sắc tư duy thiết kế AI hỗ trợ (Augmentation) thay vì tự động hóa hoàn toàn (Automation); trong các bài toán đối soát nghiệp vụ có nguy cơ gian lận, con người luôn phải là chốt chặn cuối cùng (Human-in-the-loop) để bảo đảm tính công bằng và an toàn ngân sách.
