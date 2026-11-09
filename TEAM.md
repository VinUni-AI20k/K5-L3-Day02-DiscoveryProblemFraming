# Team

## Thông tin nhóm

- Tên nhóm: 4Ward
- Candidate problem nhóm chọn (1 câu): Khi vừa kết thúc cuộc họp dài 1 tiếng, tôi muốn tổng hợp lại danh sách công việc (action items) kèm người phụ trách, để gửi cho từng người trong team xác nhận ngay.
- Quyết định cuối (Go / Not Yet / No-Go): Go (Pilot phạm vi nhỏ)

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Phùng Quang Trà | 2A202604094 |Nhóm  trưởng| https://github.com/phungtr|
| 2 | Nguyễn Tuấn Anh | 2A202604086 | Thành viên | TuanAnhNg131 |
| 3 | Vũ Nam Khánh | 2A202604112 | Thành viên | khanhvnm |
| 4 | Phạm Duy Thành| 2A202604075| Thành viên| https://github.com/thanhtey1234|

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Phùng Quang Trà | Nguyễn Tuấn Anh | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Phạm Duy Thành | Vũ Nam Khánh | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Tuấn Anh | Phạm Duy Thành | Bảng research có link |
| CP5 — Quy trình trước/sau | Vũ Nam Khánh | Phạm Duy Thành | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Phạm Duy Thành | Nguyễn Tuấn Anh | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Vũ Nam Khánh | Phạm Duy Thành | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Phùng Quang Trà | Vũ Nam Khánh, Nguyễn Tuấn Anh, Phạm Duy Thành | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.


### Phùng Quang Trà-2A202604094

**Phần việc phụ trách:**

- Nhóm trưởng: fork và quản lý repo nhóm, review và merge pull request của các thành viên.
- Phụ trách chính CP3 (hội tụ nhóm) và CP6 (quyết định) theo bảng phân công ở trên.
- Đại diện nhóm lên trình bày pitch và phản biện với các nhóm khác.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Scan 5 problem và viết 3 Problem Card kèm quy trình nháp (CP1–CP2); đưa 3 candidate vào bảng pitch của nhóm (#1–#3).
- Lên trình bày pitch card CRO (hồ sơ giải ngân online): actor là CRO nhập liệu, quy trình 6 bước, bottleneck ở bước đọc và nhập thông tin (ước lượng ~45 trong ~80 phút mỗi bộ, ~10 bộ/tháng), impact là khách phản hồi vì xử lý chậm và ~3/10 bộ bị trả về.
- Nhận và trả lời phản biện của lab coach khi trình bày: "Liên kết với VNeID vậy mà AI agent riêng thì xử lý như thế nào?" Hướng trả lời: agent nội bộ nhưng có liên kết VNeID, dữ liệu hồ sơ lấy về từ kho dữ liệu của nhà nước và tạo kho dữ liệu local riêng.
- Đặt câu hỏi phản biện cho nhóm trưởng nhóm 11 (bài AI hỗ trợ ghi note task): "Note của bạn có đặt sẵn lịch thông báo không?" Bạn ấy trả lời nhóm chưa tính tới trường hợp này.
- Cùng nhóm thống nhất lại chọn candidate #7 (tổng hợp action items sau họp) làm bài nhóm và chốt quyết định Go (Pilot phạm vi nhỏ).
- Review và merge 11 pull request (#1–#11) để gộp bài của cả 4 thành viên vào nhánh `main`.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md` mục 2.1: dòng 1–3 bảng pitch (commit `3b987d0`); mục 2.4 (candidate #7) và mục 8 (quyết định Go).
- `report/individual/2A202604094_PhungQuangTra.md`: mục 2–3 (bảng scan, 3 Problem Card, commit `0f7d4cf`) và mục 4 (nhật ký tham gia).
- Bảng phân công theo checkpoint trong `TEAM.md`; lịch sử pull request #1–#11 trên repo nhóm.

**Điều mình học được từ phần nhóm:**
-khả năng phản biện trước các câu hỏi về vấn đề ai nội bộ và đưa ra vấn đề giải quyết nhanh chóng
-hiêu rõ nỗi đau của người dùng và nhu cầu thật sự của người dùng để tạo ra giải pháp

### Vũ Nam Khánh - 2A202604112

**Phần việc phụ trách:**

- Phụ trách chính CP5 (Quy trình trước/sau) và CP6 (Mức can thiệp AI + Problem Statement v1).
- Hỗ trợ thực hiện CP6 (Quyết định 4 rủi ro).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đưa ra ý tưởng Candidate #7 (Tổng hợp action items sau họp 1h) và bảo vệ bài toán được chọn vào shortlist.
- Xây dựng sơ đồ Quy trình hiện tại (5 bước, 30 phút) và Quy trình tương lai (4 bước, 7 phút), xác định điểm nghẽn (bottleneck) ở bước trích xuất task/assignee.
- Phân tích Ma trận Độ mơ hồ x Độ phức tạp, hoàn thiện AI Canvas, trả lời 2 câu hỏi Google PAIR và nâng cấp Problem Statement từ v0 lên v1 (bổ sung metric chất lượng và boundary HITL).
- Hỗ trợ xây dựng bảng giả định Assumption Map và tham gia đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability) để chốt quyết định Go.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- File báo cáo cá nhân `2A202604112_VuNamKhanh.md`.

**Điều mình học được từ phần nhóm:**

- Biết cách hạ quy mô một bài toán AI quá rộng (từ bot tự ghi âm/gửi tin nhắn) xuống dạng Workflow đơn giản, tập trung đúng điểm nghẽn tốn thời gian nhất.
- Hiểu tầm quan trọng của Ranh giới (Boundary) và Human-in-the-loop (HITL) để tránh rủi ro AI đoán sai tên người làm hoặc tự bịa ra task làm trôi tin nhắn team.
