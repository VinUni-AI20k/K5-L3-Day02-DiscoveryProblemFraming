# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: TEAMLAGI
- Candidate problem nhóm chọn (1 câu): Đối chiếu hồ sơ chào giá của các nhà thầu với yêu cầu/BOQ và giữa các nhà thầu để phát hiện chênh lệch.
- Quyết định hiện tại (Go / Not Yet / No-Go): **Not Yet cho triển khai/pilot; chọn Rule cho phần soát số liệu**, theo ủy quyền trực tiếp của trưởng nhóm ngày 2026-11-09. Không ghi thành biên bản biểu quyết của sáu người.
- Quy mô: 6 người; Nguyễn Trọng Hưởng xác nhận trong chat ngày 2026-11-09 rằng coach đã cho phép.
- Phạm vi: soát khối lượng/đơn giá trên bảng đã ghép đúng mã, đơn vị và phiên bản; không gồm ghép file sai mẫu hoặc đánh giá năng lực. Target dưới 90 phút công/vòng gồm kiểm/sửa/ngoại lệ; chỉ pilot khi quyền dữ liệu, mapping và đáp án được xác nhận.

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
| CP4 — Kiểm chứng | Linh | Người hỗ trợ cụ thể chưa xác nhận | Mục 3.1–3.2 có assumption map, một snapshot và tổng hợp 3 người tại `4efec2b`; bổ sung ngày/cách hỏi và hành vi từng người |
| CP4 — Research | Khương | Người hỗ trợ cụ thể chưa xác nhận | Research mục 3.3 đã merge qua PR #5; file assets riêng là tùy chọn |
| CP5 — Quy trình trước/sau | Vinh | Hưởng tổng hợp | CP5 nguồn đã merge qua PR #4; mục 4.1 giữ bối cảnh, mục 4.2–4.3 cập nhật quy trình Rule đúng phạm vi đã chọn |
| CP5 — Problem Statement v0 | Hưởng tổng hợp theo ủy quyền trưởng nhóm | Vinh cung cấp quy trình; Linh/Khương cung cấp bằng chứng | Mục 5: phạm vi soát, baseline tham chiếu 300–360 phút và target dưới 90 phút; dữ liệu/ngưỡng được kiểm trước pilot |
| CP6 — Eval | Quân | Hưởng review | Bản eval và 10 tình huống trên nhánh Quân tại `9ccefc8`; nhận xét cần sửa ở mục 7 báo cáo nhóm; chưa tích hợp |
| CP6 — Mức can thiệp + Problem Statement v1 | Tuyên phân tích; Hưởng tổng hợp theo ủy quyền | Quân cung cấp eval | Mục 6–7: chọn Rule, AI mapping tách riêng; năm tiêu chí phải đạt đồng thời |
| CP6 — Quyết định | Hưởng, theo ủy quyền trực tiếp của trưởng nhóm | Tuyên cung cấp rủi ro; Quân cung cấp eval | Mục 8: Not Yet cho pilot, điều kiện chuyển Go, ngưỡng dừng và người phụ trách từng điều kiện |

Các đường dẫn sản phẩm trong `report/assets/` là đầu ra dự kiến; Vinh và Tuyên viết trực tiếp trong `report/team/group_report.md`, đã tích hợp lên main qua PR #4/#6; Khương bổ sung mục 3.3 qua PR #5. Bản tổng hợp local dẫn commit nguồn và phân biệt đề xuất với kết quả đã kiểm. Phân công không thay thế bằng chứng đóng góp. Phụ thuộc và trạng thái chi tiết ở [nhật ký điều phối](docs/TEAM_WORK_LOG.md#2-phân-công-đã-xác-nhận-và-phụ-thuộc). Các quan hệ hỗ trợ phục vụ tổng hợp trong bảng là luồng bàn giao dự kiến, chưa ghi nhận là công việc đã diễn ra.

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.


### NguyenVanVinh-2A202603672

**Phần việc phụ trách:**

- Người chính CP5 — Quy trình trước/sau: vẽ quy trình hiện tại, quy trình tương lai và bảng before/after (mục 4 báo cáo nhóm).
- Người cung cấp domain và dữ liệu cho candidate được chọn (V1 — soát chênh khối lượng/đơn giá): actor, quy trình thực tế, số liệu gói thầu và baseline thời gian.
- Hỗ trợ CP5 — Problem Statement v0: cung cấp quy trình, bottleneck và baseline cho bản tổng hợp.
- Việc được giao trước pilot (mục 8): xác nhận phạm vi, nhật ký thời gian và dữ liệu được phép dùng.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- **CP1 — Scan:** 8 problem theo đủ 4 lăng kính, lấy từ quy trình đánh giá chào giá gói cơ điện (BOQ ~4.100 dòng, 4 nhà thầu, 7 hạng mục); mỗi dòng có số đo thời gian, số dòng hoặc số lần.
- **CP2 — Problem Card:** 3 card kèm quy trình nháp (Mermaid): V1 soát chênh lệch (5–6 giờ/vòng), V2 gom bảng chào giá (6–7 giờ/vòng), V3 chấm năng lực (3 giờ công/nhà thầu, tổng của 2 người). Dùng AI phản biện; sửa V1 từ "Rule hoặc Workflow" thành Rule.
- **CP3 — Hội tụ:** pitch 3 card; V1 vào shortlist với 30/35 điểm, cao nhất (L1 và T1 cùng 24 điểm) và được chọn. Đặt câu hỏi phản biện cho card của Hưởng (H1), Linh (L2), Quân (Q3).
- **CP4 — Kiểm chứng / research:** cung cấp số liệu domain bổ trợ cho mục 3. Research thêm 3 nguồn và tự mở kiểm link: Power Query (Microsoft yêu cầu các file cùng schema, nên không gom được file sai mẫu), Archdesk và Corten (công cụ bid leveling có sẵn); loại 1 link chết.
- **CP5 — Quy trình trước/sau:** viết mục 4 báo cáo nhóm:
  - 4.1: quy trình hiện tại 8 bước, có actor / input / output / thời gian, tổng 11–13 giờ/vòng; bottleneck chính là bước dò ~16.000 dòng (~4 giờ/vòng), bottleneck phụ là ghép file sai mẫu (2,5 giờ).
  - 4.2: quy trình tương lai 9 bước tách Rule / AI / con người; 5 điều boundary, HITL ở 3 bước, 3 phương án quay về.
  - 4.3: bảng before/after — từ 8/8 bước thủ công xuống 4/9; thời gian kỳ vọng ~2–2,5 giờ/vòng (ước, chưa pilot); 5 rủi ro mới kèm cách xử lý.
- **Sau review CP5:** chấp nhận hai điểm sửa — bước duyệt phải kiểm mọi dòng AI ghép (tổng tiền khớp không chứng minh ghép đúng) và tách baseline riêng phần soát (300–360 phút/vòng) khỏi thời gian gom.
- **CP5–CP6 — Problem Statement, mức can thiệp:** baseline 300–360 phút/vòng và target dưới 90 phút/vòng (từ mục tiêu 1,5 giờ ở Card #1) được dùng cho v0/v1; kết luận Rule của Card #1 được nhóm giữ ở CP6, AI mapping tách thành hướng mở rộng.
- **CP7:** hoàn thành báo cáo cá nhân mục 4–6 và phần này trong `TEAM.md`.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo nhóm](report/team/group_report.md):
  - Mục 2.1, dòng 4–6: card V1, V2, V3; mục 2.4: bảng chấm điểm V1 30/35.
  - Mục 4: quy trình trước/sau (4.1–4.3) do Vinh viết.
  - Mục 5 và 7: baseline phần soát ghi nguồn "theo Vinh".
  - Mục 8.2: việc được giao trước pilot; mục 10: nguồn [V-CP5].
- [PR #4](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/4), merge commit `270bb22`; các commit của Vinh: `a295e96`, `cd91790`, `2f96679`.
- [Báo cáo cá nhân](report/individual/2A202603672_NguyenVanVinh.md): mục 2 (scan), mục 3 (3 card + quy trình nháp), mục 4 (tham gia nhóm), mục 5 (dùng AI).
- Không có file trong `report/assets/`: sơ đồ viết trực tiếp bằng Mermaid trong báo cáo.

**Điều mình học được từ phần nhóm:**

- Nên thử Rule làm mốc đối chứng trước, chỉ dùng AI khi chứng minh được Rule không đủ.
- Phải tách bước gom khỏi bước soát; gộp lại thì baseline và target không cùng phạm vi.
- Tổng tiền khớp không chứng minh các dòng đã được ghép đúng; cần kiểm cả mã, đơn vị và dòng nguồn.
- Số liệu từ một gói thầu chỉ là điểm bắt đầu; cần bấm giờ từng bước và có bộ đáp án trước khi kết luận.
