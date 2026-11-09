# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: CodeX
- Candidate problem nhóm chọn (1 câu): Khi tiếp nhận một dự án outsource/maintain cũ (hoặc onboard thành viên mới) mà tài liệu cài đặt đã lỗi thời, Developer và Techlead lãng phí 4–8 tiếng để gỡ lỗi crash do xung đột thư viện/version; nhóm chọn bài toán chuẩn hóa môi trường bằng Docker (No-AI) kết hợp AI Workflow phân tích log lỗi build để giảm thời gian setup xuống dưới 30 phút.
- Quyết định cuối (Go / Not Yet / No-Go): (Chưa quyết định)

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Nguyễn Tiến Cường | 2A202603425 | Nhóm trưởng | cuong-sadboi |
| 2 | Nguyễn QUang Vũ| 2A202603407 | Thành viên Quản trị rủi ro, Thiết kế AI Canvas & Ranh giới an toàn (Gatekeeper) | NguyenVu8888 |
| 3 | | | | |
| 4 | | | | |

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

### NguyenTienCuong-2A202603425

**Phần việc phụ trách:**

- Nhóm trưởng điều phối nhóm CodeX, tham gia pitch và phản biện tại CP3.
- (Sẽ cập nhật các task cụ thể sau khi nhóm chốt phân công CP4 - CP6).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Hoàn thành báo cáo cá nhân CP1 (10 problem) và CP2 (3 Problem Card + quy trình nháp).
- Chuẩn bị sẵn Card #1 để pitch với nhóm.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/individual/2A202603425_NguyenTienCuong.md`.
- Lịch sử commit trên branch cá nhân / repo từ tài khoản `cuong-sadboi`.

**Điều mình học được từ phần nhóm:**

- (Sẽ điền sau khi hoàn thành phần làm việc nhóm ở CP7).

### NguyenQuangVu-2A202603407

**Phần việc phụ trách:**

- Thành viên phản biện nhóm CodeX, tham gia pitch và phản biện tại CP3.
- Quản trị rủi ro, Thiết kế AI Canvas & Ranh giới an toàn (Gatekeeper)

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Hoàn thành báo cáo cá nhân CP1 (7 problem) và CP2 (3 Problem Card + quy trình nháp).
+ [CP4] Bảng Assumption Map: Lập 4-5 giả định cốt lõi về giá trị, tính khả thi kỹ thuật và mức độ chấp nhận của người dùng; chấm điểm quan trọng vs bằng chứng.
+ [CP5] Soạn thảo Problem Statement v0: Điền đủ 6 trường: Actor, Quy trình, Bottleneck, Impact, Success Metric (270' -> 30'), Boundary (AI không tự ý chạy script quyền root). Lưu ý: Không viết từ "AI" vào phần mô tả problem.
+ [CP6] Thiết kế AI Canvas rút gọn: Điền 6 ô: Prediction (AI đoán package lỗi & gợi ý lệnh) -> Judgment (Dev duyệt lệnh) -> Action (Dev chạy lệnh) -> Outcome (build pass) -> Input (chỉ lấy log crash + package.json, TUYỆT ĐỐI KHÔNG ĐỌC SOURCE CODE BẢO MẬT) -> Feedback.
+ [CP6] Đánh giá 4 rủi ro sản phẩm: Đánh giá Value, Usability, Feasibility, Viability (ở mức an toàn/thấp).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/individual/2A202603407_NguyenQuangVu.md`.
- Lịch sử commit trên branch cá nhân / repo từ tài khoản `NguyenVu8888`.

**Điều mình học được từ phần nhóm:**

- (Sẽ điền sau khi hoàn thành phần làm việc nhóm ở CP7).

### HoVaTen-MSSV

> *(Các thành viên khác rebase về và copy mục này thành tên mình để tự điền phần việc cá nhân)*

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-
