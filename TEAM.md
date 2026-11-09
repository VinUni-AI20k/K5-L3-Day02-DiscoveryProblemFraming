# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: BDHH
- Candidate problem nhóm chọn (1 câu): Backend developer (sinh viên/junior) mất 20–40 phút mỗi lần dò stack trace dài, nhiều nhiễu để tìm nguyên nhân các lỗi khó phải truy qua nhiều file (lỗi kết nối CSDL, lỗi logic liên tầng).
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Trịnh Công Đức | 2A202603527 | Nhóm trưởng (tổ chức thảo luận nhóm, merge code); vẽ quy trình, viết Problem Statement v0 (CP5) | trinhcongduc112 |
| 2 | Dương Thanh Bình | 2A202603531 | Phụ trách chính CP4 (kiểm chứng, research) | BinhThanh313 |
| 3 | Nguyễn Quốc Hưng | 2A202603553 | Phụ trách CP6 (mức can thiệp AI, quyết định) | hung309911 |
| 4 | Trần Thái Hưng | 2A202603557 | Phụ trách CP6 (mức can thiệp AI, quyết định) | ghism137 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Cả nhóm thảo luận (Trịnh Công Đức tổ chức) | Dương Thanh Bình (gom cluster) | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Dương Thanh Bình | Cả nhóm thảo luận | Assumption map, snapshot hoặc survey |
| CP4 — Research | Dương Thanh Bình | Cả nhóm thảo luận | Bảng research có link |
| CP5 — Quy trình trước/sau | Trịnh Công Đức | Cả nhóm thảo luận | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Trịnh Công Đức | Cả nhóm thảo luận | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Trần Thái Hưng, Nguyễn Quốc Hưng | Cả nhóm thảo luận | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Trần Thái Hưng, Nguyễn Quốc Hưng | Cả nhóm thảo luận | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### HoVaTen-MSSV

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-

### TrinhCongDuc-2A202603527

**Phần việc phụ trách:**

- Nhóm trưởng: fork repo nhóm, mời các thành viên vào repo, tổ chức thảo luận nhóm và merge bài của các thành viên vào nhánh main.
- CP5: quy trình trước/sau và Problem Statement v0 (người chính).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch Problem Card "Debug lỗi runtime (ngoại lệ) từ file log", được nhóm chọn làm candidate problem.
- Tổ chức các buổi thảo luận nhóm, góp ý khi hội tụ và chốt bài toán.
- Vẽ quy trình hiện tại (5 bước, khoảng 43 phút/lần, bottleneck là bước đọc stack trace 20 phút) và quy trình tương lai (Rule lọc log → AI gợi ý vị trí lỗi → dev kiểm tra → dev sửa), kèm boundary, phương án quay về và bảng before/after.
- Viết Problem Statement v0: đối chiếu kết quả kiểm chứng CP4 để thu hẹp Actor và chỉnh baseline (20–40 phút/lần), ghi lại 4 phản biện và cách nhóm xử lý.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`: mục 4 (4.1–4.3) và mục 5.
- `report/individual/2A202603527_TrinhCongDuc.md`: Problem Card #1 ở mục 3, là nguồn của candidate problem.
- Commit `c39855e` trên nhánh `2A202603527-TrinhCongDuc`.
- Merge nhánh của các thành viên vào main: commit `15896eb`, `8e15bb9`, `22da565` (nhánh của Trần Thái Hưng được merge qua Pull Request #1, `c4d067c`).

**Điều mình học được từ phần nhóm:**

-
