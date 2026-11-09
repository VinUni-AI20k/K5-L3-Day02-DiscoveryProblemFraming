# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: TamCa
- Candidate problem nhóm chọn (1 câu): Sinh viên IT năm cuối/mới ra trường mất nhiều thời gian (khoảng 16/30 phút mỗi CV) để đối chiếu và viết lại mô tả dự án trong CV cho khớp với từ khóa yêu cầu trong JD khi ứng tuyển Intern/Fresher.
- Quyết định cuối (Go / Not Yet / No-Go): **Go (pilot nhỏ, có điều kiện)**

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Trần Thị Nhài | 2A202603911 | Điều phối kiểm chứng/phỏng vấn · viết Problem Statement · vẽ quy trình | chanhochust |
| 2 | Ngô Ngọc Hải | 2A202603939 | Nhóm trưởng (repo owner) · điều phối chung · research giải pháp · mức can thiệp AI | NgoHai0804 |
| 3 | Trần Hữu Tài | 2A202603944 | Thư ký/ghi chép group_report · phản biện chính · phỏng vấn/survey · quyết định | taitran |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Ngô Ngọc Hải | Trần Thị Nhài, Trần Hữu Tài | Bảng pitch, cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng & Research | Trần Hữu Tài | Trần Thị Nhài, Ngô Ngọc Hải | Assumption map, interview snapshot / poll, bảng research có link |
| CP5 — Quy trình & Problem Statement v0 | Trần Thị Nhài | Trần Hữu Tài, Ngô Ngọc Hải | Quy trình hiện tại/tương lai, bảng before/after, Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Ngô Ngọc Hải | Trần Thị Nhài, Trần Hữu Tài | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Trần Hữu Tài | Ngô Ngọc Hải, Trần Thị Nhài | 4 rủi ro + Go/Not Yet/No-Go + ngưỡng dừng |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NgoNgocHai-2A202603939

**Phần việc phụ trách:**

- Nhóm trưởng (repo owner), điều phối chung. Người chính: CP3 Hội tụ nhóm, CP6 Mức can thiệp & PS v1. Người hỗ trợ: CP4 Kiểm chứng & Research, CP5 Quy trình, CP6 Quyết định.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch #4–#6; phản biện bài của Nhài (#1, #3) và Tài (#8, #9); đồng thuận loại bài #6 để chọn #1 (Chỉnh CV).
- Chủ trì phân 3 cluster, dựng cây OST với 1 outcome đo được; cùng nhóm chấm điểm shortlist (bài #1 đạt 34/35).
- Viết CP6: ma trận mơ hồ × phức tạp, bảng 4 mức (chọn Workflow, cấm Agent), AI Canvas rút gọn, 2 câu PAIR, 5 tiêu chí eval, Problem Statement v1; cùng Tài chốt mục 8 (Quyết định).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 1, 2.1–2.4, 6, 7, 8; commit `88e2e0b`, 17e8232, `d639625` (branch `202603939_NgoNgocHai`).

**Điều mình học được từ phần nhóm:**

- Phân biệt rõ bài toán Rule (tất định) và Workflow/AI (ngôn ngữ tự do); luôn giữ Human-in-the-loop và ngưỡng dừng đo được khi pilot.

### TranThiNhai-2A202603911

**Phần việc phụ trách:**

- Kiểm chứng, vẽ quy trình, viết Problem Statement. Chính: CP4 Kiểm chứng (phỏng vấn), CP5 Quy trình trước/sau, CP5 Problem Statement v0. Hỗ trợ: CP3 Hội tụ, CP4 research, CP6 Mức can thiệp. Bổ sung mục 9–10.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch #1–#3, card #1 "Chỉnh CV theo JD" được chọn (34/35); phản biện #4, #5 (Hải), #7 (Tài).
- Assumption map 6 giả định; bộ 5 câu hỏi The Mom Test; phỏng vấn 3 người (P1–P3), tổng hợp xác nhận/phản bác → nhóm thu hẹp problem về JD "lạ".
- Vẽ quy trình hiện tại/tương lai (Rule / AI / người, boundary, quay về) + bảng before/after.
- Viết Problem Statement v0 (metric ~40' → ≤ 20', ≥ 60% bullet chấp nhận, 0 kỹ năng bịa) + 4 phản biện; viết mục 9 (hạn chế) và 10 (tài liệu tham khảo).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1, 3.1–3.2, 4, 5, 9, 10; commit `02bd304`, `840e359`, `d9424b9` (branch `nhaichan`); nội dung mục 3.1–3.2 và 4 nằm trong commit `a2fe61b` (gộp chung phần CP4 của nhóm).

**Điều mình học được từ phần nhóm:**

- Tín hiệu phản bác quý hơn lời xác nhận: P3 cho thấy nhồi từ khóa không giúp qua vòng hồ sơ, khiến nhóm đổi metric từ "khớp từ khóa" sang "0 kỹ năng bịa" và giữ người duyệt từng dòng. Phương án No AI (CV master) cũng cần được kiểm thật trước khi kết luận cần AI.

### TranHuuTai-2A202603944

**Phần việc phụ trách:**

- Thư ký, phản biện chính. Người chính: CP4 Kiểm chứng & Research, CP6 Quyết định. Người hỗ trợ: CP3 Hội tụ nhóm, CP5 Quy trình & Problem Statement v0.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch #7–#9; phản biện #2, #6 (thành lý do loại).
- Chạy poll 8 người, tổng hợp kết quả CP4, tìm kiếm và tóm tắt research Jobscan/Teal.
- Đề xuất metric "0 kỹ năng bịa"; viết bảng 4 rủi ro + ngưỡng dừng ở CP6.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1, 3.2, 3.3, 8.1, 8.2; commit `7ebbef1`, `a2fe61b` (branch `taitran`).

**Điều mình học được từ phần nhóm:**

- Hỏi "No AI / Rule đã đủ chưa?" trước khi nghĩ đến AI; Go phải đi kèm ngưỡng dừng đo được.
