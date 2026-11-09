# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: Ban3
- Candidate problem nhóm chọn (1 câu): Hệ thống phát hiện tài xế ngâm cuốc và tự động phân loại khiếu nại hủy chuyến cho ứng dụng gọi xe Xanh SM.
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet (Chạy pilot 4 tuần trên môi trường Staging/Mock Sandbox trước khi xem xét tích hợp)

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Lý Thanh Lâm | 2A202603475 | | https://github.com/LysLama |
| 2 | Tô Minh Thành | 2A202603439 | | https://github.com/thanhtmhe186559 |
| 3 | Phạm Trung Kiên | 2A202603479 | | https://github.com/trungkienpham0607 |
| 4 | Nguyễn Thanh Tùng | 2A202603446 | | https://github.com/hunter2996 |
| 5 | Đoàn Gia Long | 2A202603443 | | https://github.com/DoanGiaLong |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Lý Thanh Lâm | Tô Minh Thành, Phạm Trung Kiên | Bảng pitch, Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Đoàn Gia Long | Tô Minh Thành | Assumption map, 5 interview snapshots (Bonus B2) |
| CP4 — Research | Phạm Trung Kiên | Lý Thanh Lâm | Bảng research 3 giải pháp có link đã kiểm chứng |
| CP5 — Quy trình trước/sau | Nguyễn Thanh Tùng | Phạm Trung Kiên | Sơ đồ Mermaid Trước/Sau + bảng before/after có HITL & Fallback |
| CP5 — Problem Statement v0 | Lý Thanh Lâm | Đoàn Gia Long | Problem Statement v0 (6 trường chuẩn) |
| CP6 — Mức can thiệp + Problem Statement v1 | Tô Minh Thành | Nguyễn Thanh Tùng | Ma trận, AI Canvas, PAIR, eval 10 pairs (Bonus B3), Problem Statement v1 |
| CP6 — Quyết định | Lý Thanh Lâm | Tô Minh Thành | Đánh giá 4 rủi ro + Quyết định Not Yet + Ngưỡng dừng đo được |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### LyThanhLam-2A202603475

**Phần việc phụ trách:**

- Nhóm trưởng điều phối tiến độ, quản trị repo GitHub chung của nhóm Bàn 3.
- Phụ trách chính CP3 (Hội tụ nhóm & Dựng cây Opportunity Solution Tree).
- Phụ trách CP5 (Problem Statement v0) và CP6 (Đánh giá 4 rủi ro, phân tích rào cản dữ liệu & đề xuất Quyết định Not Yet kèm ngưỡng dừng).
- Hỗ trợ CP4 (Research giải pháp Uber/Grab) và rà soát chất lượng tổng thể `group_report.md`.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Quản trị repo, phân công vai trò và checkpoint cho 5 thành viên trong `TEAM.md`.
- Đóng góp Card #1 về "Tài xế Xanh SM ngâm cuốc ép khách tự hủy", làm tiền đề then chốt kết hợp với bài gắn nhãn hủy chuyến của Kiên để nhóm hội tụ thành đề tài chung.
- Trực tiếp xây dựng cây Opportunity Solution Tree (OST) tách bạch giữa Outcome đo được, Opportunity (pain) và gạch bỏ các giải pháp đội lốt ở CP3.
- Soạn thảo Problem Statement v0 và v1, thiết lập Boundary nghiêm ngặt (không cho AI tự động phạt tài xế hoặc tự ý trừ/hoàn tiền ví hành khách).
- Phân tích 4 rủi ro lớn (Value, Usability, Feasibility, Viability) dưới góc độ bảo mật dữ liệu theo Nghị định 13/2023/NĐ-CP và ranh giới dữ liệu GSM, chốt quyết định Not Yet trung thực và khả thi.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`: Mục 1, Mục 2.3 (Cây OST), Mục 2.4 (Bảng chấm điểm & lý do chọn), Mục 5 (Problem Statement v0), Mục 7 (Problem Statement v1), Mục 8 (4 rủi ro & Quyết định Not Yet).
- `TEAM.md`: Bảng thành viên, phân công checkpoint và mục cá nhân.
- Commits trên branch `main` và `2A202603475-LyThanhLam`.

**Điều mình học được từ phần nhóm:**

- Chuyển từ tư duy "Solution-first" sang "Problem-first": ở bước cứu khách hàng đang đứng chờ xe, chỉ cần tập luật Rule-based đơn giản là đã giải quyết được 80% bức xúc mà không cần mô hình AI phức tạp.
- Nhận thức sâu sắc về ranh giới dữ liệu và pháp lý doanh nghiệp: một nhóm học viên làm lab bên ngoài không thể tự tiện tuyên bố có quyền can thiệp vào cơ sở dữ liệu nội bộ của GSM hay tự động ra lệnh bồi hoàn tiền; một quyết định "Not Yet" có cơ sở dữ liệu và lộ trình pilot staging 4 tuần giá trị và đáng tin cậy hơn nhiều so với một quyết định "Go" viển vông.

---

### HoVaTen-MSSV

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-
