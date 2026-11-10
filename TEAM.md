# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: BacHo
- Candidate problem nhóm chọn (1 câu): Sinh viên phụ trách ghép report nhóm mất khoảng 3–4 tiếng sát deadline để thu bài, đọc đối chiếu, hỏi lại thành viên và sửa các phần mâu thuẫn (số liệu, insight) thành một report thống nhất.
- Quyết định cuối (Go / Not Yet / No-Go): Go, phạm vi nhỏ

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Trần Hải Long | 202603891 | Nhóm trưởng | longhtr028 |
| 2 | Lê Danh Giang | 202603912 | Người phản biện chính, viết Problem Statement | giangj |
| 3 | Nguyễn Đức Hải | 2A202603899 | | hainguyen312 |
| 4 | Trần Tuấn Anh | 2A202603909 | Phụ trách kiểm chứng | Tanh0406 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Trần Hải Long | Lê Danh Giang | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Trần Tuấn Anh | Lê Danh Giang | Assumption map, snapshot hoặc survey |
| CP4 — Research | Lê Danh Giang | | Bảng research có link |
| CP5 — Quy trình trước/sau | | Lê Danh Giang | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | | Lê Danh Giang | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Lê Danh Giang | | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | | Lê Danh Giang | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### LeDanhGiang-202603912

**Phần việc phụ trách:**

- Tham gia pitch ý tưởng và lập 3 Problem Cards ban đầu (theo dõi chi phí API, lộ trình giao thông, kiểm tra xe máy).
- Phản biện bài toán của các thành viên khác để lọc danh sách, tham gia gom cluster và chấm điểm 12 Candidate Problems.
- Tìm hiểu các công cụ hỗ trợ ghép report sẵn có (Google Docs tabs, Gemini Notebook) ở CP4.
- Rà soát, bổ sung metric chất lượng cho Problem Statement v1 và đề xuất ngưỡng dừng ở CP6.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đưa ra được 3 bài toán vào danh sách 12 candidate; góp phần loại sớm các bài toán thiếu dữ liệu hoặc không phỏng vấn được.
- Đóng góp vào việc thiết kế quy trình Before/After: chỉ ra được "nút thắt" lớn nhất là đồng bộ số liệu và nối logic insight, qua đó giới hạn Boundary là AI chỉ quét mâu thuẫn (bước 3) thay vì tự động viết insight.
- Đánh giá rủi ro và thống nhất kế hoạch "Go, phạm vi nhỏ", tạo Rule kiểm số liệu cứng chạy trước AI để tránh bỏ sót lỗi.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Các mục 2.1, 2.3, 2.4 (Gom cluster & Chấm điểm shortlist) trong `group_report.md`.
- Mục 3.3 (Research giải pháp đã có) và 4.3 (Bảng Before/after) trong `group_report.md`.
- Mục 6 và 7 (Mức can thiệp AI, Problem Statement v1) trong `group_report.md`.
- *(Điền thêm link commit cá nhân của bạn tại đây sau khi push code)*

**Điều mình học được từ phần nhóm:**

- Học được cách dùng những con số thực tế (bao nhiêu giờ, bao nhiêu lần) để đo lường vấn đề thay vì chỉ nói chung chung là "mất thời gian".
- Nhận ra nỗi đau thực sự của người dùng khi ứng dụng AI đôi khi không phải là thiếu công cụ, mà là rủi ro về hallucination (sợ AI bịa thông tin). Do đó, việc xác định Boundary và để người dùng duyệt (Human-in-the-loop) là cực kỳ quan trọng.
