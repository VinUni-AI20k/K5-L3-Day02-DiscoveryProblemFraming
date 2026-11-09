# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: TEAMLAGI
- Candidate problem nhóm chọn (1 câu): Đối chiếu hồ sơ chào giá của các nhà thầu với yêu cầu/BOQ và giữa các nhà thầu để phát hiện chênh lệch.
- Quyết định cuối (Go / Not Yet / No-Go): nhóm xác nhận sau review; bản tổng hợp local đề xuất Not Yet cho triển khai/pilot, ưu tiên kiểm phương án Rule.
- Quy mô: 6 người; Nguyễn Trọng Hưởng xác nhận trong chat ngày 2026-11-09 rằng coach đã cho phép.
- Bản tổng hợp local đã review CP5 của Vinh và CP6 của Tuyên; đề xuất ưu tiên phần soát trên dữ liệu đã ghép đúng, với metric và điều kiện thử rõ. Nguồn kiểm chứng, quyền dữ liệu và quyết định chung được xác nhận riêng.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Nguyễn Trọng Hưởng | 202603607 | Trưởng nhóm, điều phối thời gian, ghi chép | trongjhuongwr |
| 2 | Nguyễn Văn Vinh | 2A202603672 | Quy trình, dữ liệu, bottleneck và before/after | VINH1811 |
| 3 | Đàm Tuấn Linh | 2A202603624 | Kiểm chứng, assumption map và snapshot | damlinh820 |
| 4 | Mai Đặng Khương | 2A202603627 | Research giải pháp hiện có, kiểm nguồn | dangkhuong14 |
| 5 | Phạm Ngọc Trung Quân | 2A202603626 | Eval, đáp án đối chiếu, phương án đơn giản | jadenphm29 |
| 6 | Giáp Mạnh Tuyên | 2A202603648 | Mức can thiệp, boundary và bốn rủi ro | Tanashi-Titus |

Nguồn họ tên/MSSV: báo cáo cá nhân của từng thành viên trên `origin/main` tại commit `4c402eb`; thông tin của Hưởng theo xác nhận trong chat. Vai trò được Hưởng xác nhận đã có sự đồng ý của các thành viên trong chat ngày 2026-11-09. Tài khoản GitHub được đối chiếu qua metadata tác giả commit trên GitHub: Vinh 2f96679, Linh a3e538b, Khương 8a05fa2, Quân 9f5410a, Tuyên b650c92; không suy từ tên nhánh.

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Hưởng điều phối/tổng hợp | Cả nhóm tự pitch, challenge và chốt | Báo cáo nhóm mục 2; thiếu ghi chép thực tế |
| CP4 — Kiểm chứng | Linh | Người hỗ trợ cụ thể chưa xác nhận | Linh đã cập nhật mục 3.1–3.2 tại main e278c07; bổ sung số người, thời điểm/cách hỏi và tín hiệu phản bác theo review |
| CP4 — Research | Khương | Người hỗ trợ cụ thể chưa xác nhận | Research mục 3.3 đã merge qua PR #5; file assets riêng là tùy chọn |
| CP5 — Quy trình trước/sau | Vinh | Hưởng tổng hợp | CP5 của Vinh đã merge qua PR #4; bản tổng hợp local giữ mục 4 từ main `314b6d8` |
| CP5 — Problem Statement v0 | Nhóm kiểm và tự chốt; Hưởng tổng hợp | Vinh cung cấp quy trình; Linh/Khương cung cấp bằng chứng | Báo cáo nhóm mục 5 có bản đề xuất local từ review; không ghi là nội dung nhóm đã chốt |
| CP6 — Eval | Quân | Hưởng tổng hợp | `report/assets/cp6-2A202603626-eval.md`; báo cáo nhóm mục 7 |
| CP6 — Mức can thiệp + Problem Statement v1 | Tuyên phân tích; nhóm kiểm/chốt; Hưởng tổng hợp | Quân cung cấp eval | CP6 của Tuyên đã merge qua PR #6; mục 7 local có bản đề xuất v1/eval để trao đổi |
| CP6 — Quyết định | Nhóm tự chốt; Hưởng ghi lại | Tuyên tổng hợp bốn rủi ro; Quân cung cấp eval | Mục 8 local có kết luận review Not Yet, điều kiện Go và ngưỡng dừng; chờ xác nhận chung |

Các đường dẫn sản phẩm trong `report/assets/` là đầu ra dự kiến; Vinh và Tuyên viết trực tiếp trong `report/team/group_report.md`, đã tích hợp lên main qua PR #4/#6; Khương bổ sung mục 3.3 qua PR #5. Bản tổng hợp local dẫn commit nguồn và phân biệt đề xuất với kết quả đã kiểm. Phân công không thay thế bằng chứng đóng góp. Phụ thuộc và trạng thái chi tiết ở [nhật ký điều phối](docs/TEAM_WORK_LOG.md#2-phân-công-đã-xác-nhận-và-phụ-thuộc). Các quan hệ hỗ trợ phục vụ tổng hợp trong bảng là luồng bàn giao dự kiến, chưa ghi nhận là công việc đã diễn ra.

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenTrongHuong-202603607

**Phần việc phụ trách:**

- Điều phối sáu thành viên; quản lý phân công/log, review bàn giao và tổng hợp báo cáo nhóm, Problem Statement, metric và quyết định để nhóm kiểm/chốt.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Điều phối tích hợp sáu báo cáo cá nhân qua PR #2; tiếp tục yêu cầu kiểm năm nhánh và merge PR #3–#7 của bốn thành viên. Không tạo PR trùng cho Quân vì nội dung đã có trên main; giữ các bản đang sửa trên nhánh cá nhân.
- Yêu cầu trợ lý đọc năm báo cáo, soạn mỗi người một câu hỏi bám vào card; lưu ở mục 4 báo cáo cá nhân như nội dung chuẩn bị trao đổi.
- Sử dụng trợ lý review CP5 của Vinh và CP6 của Tuyên, xử lý conflict/tên file, khôi phục template, kiểm phạm vi diff và merge qua PR #4/#6. Review sửa logic kiểm mapping và phân biệt baseline gom + soát 11–13 giờ/vòng với riêng soát 5–6 giờ/vòng. Bản tổng hợp local giữ nội dung đã merge, bổ sung v0/v1 và điều kiện review.
- Có bản đề xuất v0/v1, metric cùng phạm vi, năm tiêu chí đánh giá, bốn rủi ro, điều kiện Go và ngưỡng dừng. Các nội dung này là sản phẩm tổng hợp/review; quyết định cuối do nhóm tự xác nhận.
- Kiểm research nhà thầu của Khương trong PR #5, sửa bốn tham chiếu thiếu đích thành link chính thức đã mở kiểm; giữ rõ tính năng công cụ với giả thuyết áp dụng. Phần research bổ trợ Microsoft trước đó được ghi đúng nguồn.
- Bảo toàn nội dung thành viên khi tích hợp; sửa tên file, khoảng trắng, dấu thừa và các điểm review đã nêu trong PR. Câu hỏi chuẩn bị không được ghi thành phỏng vấn/pitch đã xảy ra.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [PR #2](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/2), merge commit `4c402eb`: tập hợp báo cáo cá nhân trên main.
- [PR #3](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/3), [#4](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/4), [#5](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/5), [#6](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/6), [#7](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/7), main `314b6d8`: tích hợp mới và review.
- [Báo cáo cá nhân](report/individual/202603607_NguyenTrongHuong.md), mục 4–5: câu hỏi review và cách dùng AI.
- [Báo cáo nhóm](report/team/group_report.md), mục 3.3, 4–8 và 10: research, bản tổng hợp đề xuất và commit nguồn.
- [Nhật ký điều phối](docs/TEAM_WORK_LOG.md): phân công và sự kiện review. Bản mới của các file này ở local, không gán một commit công bố cho phần còn đang sửa.

**Điều mình học được từ phần nhóm:**

- Khi tổng hợp phải giữ cùng phạm vi của baseline–target; số liệu trong báo cáo thành viên vẫn cần nguồn và quyền sử dụng được kiểm.
- Công thức đúng không bảo đảm so đúng hạng mục; kiểm tổng tiền cần đi cùng mapping, đơn vị và truy vết.
- Rule có thể phù hợp phần so số; hỗ trợ ghép ngữ nghĩa là bài toán mở rộng phải có đối chứng và người kiểm riêng.
