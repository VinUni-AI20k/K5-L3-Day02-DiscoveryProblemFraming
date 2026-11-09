# Điều phối công việc TEAMLAGI

**Trạng thái: phân công đã được các thành viên đồng ý, theo xác nhận của trưởng nhóm Nguyễn Trọng Hưởng trong chat ngày 2026-11-09. Trạng thái sản phẩm được theo dõi riêng; commit/PR chứa file này là bản công bố phân công.**

File điều phối được bổ sung theo hướng dẫn của LabCoach mà trưởng nhóm đã trao đổi. Các tài liệu đề bài trong repo giữ nguyên. Đây là hướng dẫn phối hợp; sản phẩm nộp chính vẫn là báo cáo cá nhân, báo cáo nhóm và `TEAM.md`.

## 1. Bài toán chung và bước hiện tại

- Nhóm đã trao đổi và chọn hướng đối chiếu chênh lệch hồ sơ của các nhà thầu.
- Phạm vi đã chọn theo ủy quyền trưởng nhóm ngày 2026-11-09: soát khối lượng/đơn giá trên bảng đã ghép đúng mã, đơn vị và phiên bản BOQ; không gồm ghép sai mẫu, đọc PDF/scan hoặc đánh giá năng lực.
- Quyết định hiện tại: chọn Rule, **Not Yet cho triển khai/pilot**; target dưới 90 phút công/vòng gồm kiểm/sửa/ngoại lệ. Quyền dữ liệu, mapping, cấu hình và đáp án phải được xác nhận trước pilot.
- Việc chọn vấn đề không đồng nghĩa đã kiểm chứng pain, số liệu hoặc giải pháp.
- Quy mô nhóm: 6 người; trưởng nhóm xác nhận trong chat ngày 2026-11-09 rằng coach đã cho phép. Đây là thông tin do trưởng nhóm cung cấp, chưa kèm thông báo của coach trong repo.
- Bản tổng hợp và mục 2 đã merge qua PR #8/#9; quy trình Rule, metric và quyết định hiện tại đã công bố qua PR #10, main `1ee80b3`. Đây là quyết định điều phối theo ủy quyền, không thay cho bản ghi pitch/challenge hoặc biểu quyết của sáu người.

## 2. Phân công đã xác nhận và phụ thuộc

| Người | Nhánh cá nhân | Việc chính | Sản phẩm phụ trách | Phụ thuộc để tổng hợp/chốt | Trạng thái sản phẩm |
|---|---|---|---|---|---|
| Hưởng | `NguyenTrongHuong-branch` | Điều phối; tổng hợp CP3, phạm vi, Problem Statement và metric | `docs/TEAM_WORK_LOG.md`; `TEAM.md`; `report/team/group_report.md` | Ghi chép CP3 thực tế; sản phẩm của 5 thành viên; dữ liệu và đáp án có người domain kiểm | Bản tổng hợp đã merge PR #8–#10; phạm vi Rule/Not Yet, metric và review eval đã công bố trên main `1ee80b3` |
| Vinh | `vinh1811` | Mô tả quy trình thực tế, chuẩn bị dữ liệu được phép dùng, đo bottleneck và before/after | `report/assets/cp5-2A202603672-quy-trinh.md` | Phạm vi Rule đã chọn; quyền dùng dữ liệu; tách số đo, ước lượng và target; đối chiếu CP4 | CP5 nguồn đã merge PR #4; quy trình hiện tại giữ ở mục 4.1, tương lai mục 4.2 được đồng bộ với phạm vi Rule |
| Linh | `damlinh820` | Điều phối kiểm chứng, assumption map, snapshot và tổng hợp tín hiệu phản bác | `report/assets/cp4-2A202603624-kiem-chung.md` | Actor/phạm vi; người ngoài nhóm thực sự gặp vấn đề; ghi nguồn, khi nào và cách hỏi | Main có một snapshot và tổng hợp 3 người tại `4efec2b`, gồm một lo ngại độ chính xác/trách nhiệm; bổ sung vai trò, ngày/cách hỏi và hành vi từng người |
| Khương | `dangkhuong14` | Research giải pháp hiện có, kiểm nguồn, đối chiếu phần đã giải và khoảng trống | `report/assets/cp4-2A202603627-research.md` | Phạm vi bài toán và bước cần so sánh; link nguồn được mở và kiểm | Research nhà thầu mục 3.3 đã merge qua PR #5; liên kết chính thức đã mở kiểm |
| Quân | `quan-branch` | Tiêu chí đánh giá, tình huống kiểm tra, đáp án đối chiếu và phương án đơn giản làm mốc so sánh | `report/assets/cp6-2A202603626-eval.md` | Phạm vi Rule; dữ liệu được phép dùng; đáp án và ngưỡng có người domain kiểm | Bản eval tại `9ccefc8` đã được review ở mục 7 và công bố nhận xét qua PR #10; đầu nhánh `70be730` đã xóa file eval. Cần khôi phục/sửa trước tích hợp; không coi bản cũ là kết quả test |
| Tuyên | `titus` | So sánh mức can thiệp, dữ liệu, boundary, AI Canvas/PAIR nếu phù hợp và bốn rủi ro | `report/assets/cp6-2A202603648-muc-can-thiep.md` | CP4; quy trình Vinh; đối chứng/eval Quân; quyết định Rule/Not Yet hiện tại | CP6 nguồn đã merge PR #6; rủi ro được nối với điều kiện chuyển Go, Canvas/PAIR chỉ áp dụng nhánh mở rộng |

Các đường dẫn `report/assets/cp...` là đầu ra dự kiến. Khi kiểm tra ngày 2026-11-09, thư mục assets vẫn chỉ có README; Vinh/Tuyên viết phần nhóm trực tiếp, đã merge qua PR #4/#6; research Khương đã merge qua PR #5. Có sản phẩm trên nhánh riêng không đồng nghĩa đã merge hoặc đã có kết quả pilot. Các phụ thuộc là thứ cần có để tổng hợp/chốt; có thể chuẩn bị song song. Người phụ trách chịu trách nhiệm nội dung và giải thích được lập luận. Mỗi người còn thực hiện đầy đủ phần cá nhân của mình.

Hưởng phụ trách tổng hợp v0/v1, metric và quyết định; cách sử dụng công cụ được ghi ở báo cáo cá nhân mục 5. Quyết định điều phối theo ủy quyền trực tiếp của trưởng nhóm đã công bố qua PR #10; nguồn baseline, target thiết kế và kết quả thực nghiệm được giữ riêng. Quyết định này không xác nhận rằng đã có buổi phản biện hoặc cả sáu người đã biểu quyết.

## 3. Quy tắc sửa file

1. Hưởng duy trì file điều phối này và tổng hợp báo cáo nhóm. Các thành viên gửi tình trạng công việc để Hưởng cập nhật.
2. Mỗi người chỉ sửa báo cáo cá nhân của mình và file sản phẩm được giao trong bảng. Nếu cần đổi phạm vi, thống nhất với Hưởng trước.
3. Hưởng lấy các sản phẩm đã được người phụ trách kiểm tra để tổng hợp vào các mục tương ứng của báo cáo nhóm, giữ dẫn nguồn và bằng chứng đóng góp.
4. Với `TEAM.md`, Hưởng cập nhật danh sách/phân công; mỗi người tự điền mục đóng góp mang tên mình. Các PR sửa file này được xử lý lần lượt.
5. Người sửa file chung cần dùng bản mới nhất từ `main` và kiểm tra diff trước khi tạo PR. Các nhánh cá nhân cũ có thể còn thay đổi ngoài phạm vi; cần kiểm cả diff của PR.
6. File điều phối trên `main` là bản phân công đã công bố. Thay đổi chưa push/merge trên nhánh cá nhân chưa phải thông tin mà mọi thành viên đã nhận được. File log không phải cơ chế khóa file tự động.

## 4. Báo cáo cá nhân của từng người

| Người | File trên `main` |
|---|---|
| Hưởng | `report/individual/202603607_NguyenTrongHuong.md` |
| Linh | `report/individual/2A202603624_DamTuanLinh.md` |
| Quân | `report/individual/2A202603626_PhamNgocTrungQuan.md` |
| Khương | `report/individual/2A202603627_MaiDangKhuong.md` |
| Tuyên | `report/individual/2A202603648_GiapManhTuyen.md` |
| Vinh | `report/individual/2A202603672_NguyenVanVinh.md` |

Linh dùng tên file có dấu `_` như bản đã chuẩn hóa trên `main`. Mỗi người tự ghi đóng góp, cách dùng AI và reflection đúng với việc mình thực hiện.

## 5. Quy trình làm việc cho thành viên và trợ lý AI

1. Kiểm tra nhánh, trạng thái Git, nội dung mới nhất của file điều phối và yêu cầu checkpoint.
2. Xác định file/phần được giao và dữ liệu hiện có. Thống nhất nội dung với người phụ trách trước khi viết.
3. Làm trên nhánh cá nhân. Phân biệt thông tin quan sát được, ước lượng theo trí nhớ, benchmark, giả định và target.
4. Gửi người phụ trách phần thay đổi và những mục còn thiếu để kiểm tra.
5. Chỉ commit/push khi người phụ trách yêu cầu. Tạo PR vào `main` của repo TEAMLAGI khi có yêu cầu; kiểm diff chỉ chứa các file đã thống nhất.
6. Hưởng review, merge lần lượt và cập nhật trạng thái trong file điều phối. Sau khi merge, thành viên kiểm tra phần mình trên `main`.

Yêu cầu có thể gửi cho từng trợ lý:

> Đọc `docs/TEAM_WORK_LOG.md` và yêu cầu checkpoint liên quan. Tôi là [tên], làm trên branch [nhánh]. Xác định phạm vi được giao, trao đổi nội dung với tôi trước khi sửa, rồi chỉ sửa các file thuộc phạm vi đó. Báo rõ thay đổi và dữ liệu còn thiếu. Chờ tôi yêu cầu trước khi commit/push hoặc tạo PR.

## 6. Đầu ra cần có để hoàn thành phần nhóm

- CP3: kết quả pitch/phản biện thực sự đã diễn ra, cluster, cây OST, bảng chấm điểm, lý do chọn và loại.
- CP4: 4–6 giả định; phỏng vấn 2–3 người ngoài nhóm hoặc survey 5–10 người đúng actor; tín hiệu phản bác; research 2–3 giải pháp có nguồn; điều nhóm sửa sau kiểm chứng.
- CP5: quy trình trước/sau, thời gian, baseline–target–cách đo, human review, phương án quay về và Problem Statement v0.
- CP6: so sánh bốn mức, AI Canvas/PAIR nếu phù hợp, 3–5 tiêu chí đánh giá, Problem Statement v1, bốn rủi ro, quyết định và ngưỡng dừng.
- Mục tiêu nâng chất lượng đề xuất: từ 5 interview snapshot hoặc survey từ 20 người và có thay đổi bài; bộ 10 input/đầu ra mong đợi cho bước AI nếu có. Các mục tiêu này chưa phải kết quả đã thực hiện.

Việc phỏng vấn do người thật thực hiện với người thật. CP3 pitch/phản biện và CP7 reflection thực hiện theo `RULES.md`. AI hỗ trợ đúng phạm vi được đề bài cho phép; các nhận định cuối cùng do thành viên và nhóm kiểm tra.

## 7. Nhật ký điều phối

Hưởng bổ sung dòng khi có sự kiện thực tế. Trạng thái nhiệm vụ: chờ xác nhận, chưa bắt đầu, đang làm, chờ review, cần sửa, đã merge.

Ngày trong nhật ký dưới đây là ngày ghi nhận trong chat/kiểm tra repo, không phải ngày suy đoán nhóm đã họp hoặc coach đã cho phép. Chỉ ghi “đã merge” khi có PR/commit kiểm tra được.

| Ngày | Người cập nhật | Sự kiện | Bằng chứng / bước tiếp theo |
|---|---|---|---|
| 2026-11-09 | Hưởng / trợ lý | Chuẩn bị bản nháp điều phối theo trao đổi trong chat; phân công chưa được xác nhận | Trưởng nhóm kiểm tra bảng mục 2; sau khi thống nhất mới công bố trên `main` |
| 2026-11-09 | Trợ lý, theo xác nhận của Hưởng | Trưởng nhóm xác nhận các thành viên đã đồng ý phân công tại mục 2 | Nguồn: phản hồi trong chat; cập nhật bản local, chưa có commit công bố trên `main` |
| 2026-11-09 | Trợ lý, theo xác nhận của Hưởng | Trưởng nhóm xác nhận coach đã cho phép nhóm 6 người | Nguồn: phản hồi trong chat; chưa kèm thông báo coach trong repo |
| 2026-11-09 | Trợ lý | Kiểm tra nguồn: chưa thấy đầu ra CP4–CP6 trong `report/assets/`; log điều phối chưa có trên `origin/main` | `origin/main` tại `4c402eb`; `vinh1811` tại `cd91790`, `damlinh820` tại `8a584a0`, `dangkhuong14` tại `90d25d1`, `quan-branch` tại `9f5410a`, `titus` tại `4abb76e` |
| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Soạn bản tham khảo CP3 từ các candidate trong báo cáo cá nhân, gồm câu hỏi gợi ý, cluster, OST, shortlist và lập luận đề xuất | `report/team/group_report.md` mục 2.5; ghi rõ AI đề xuất, chưa phải kết quả CP3. Không tạo điểm số hoặc ghi nhận buổi pitch/challenge chưa có nguồn |
| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Fetch GitHub, fast-forward main local tới `7aa2e9c`, merge nội dung main vào worktree nhánh Hưởng và khôi phục bản đang sửa | Merge đang chờ commit; HEAD cá nhân `e967785` giữ nguyên; backup stash `e7653d3`; không push |
| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Đọc năm báo cáo ở các nhánh mới nhất, soạn năm câu hỏi review vào báo cáo Hưởng | Vinh `2f96679`, Linh `6f3fe68`, Khương `90d25d1`, Quân `9f5410a`, Tuyên `b650c92`; không ghi là hỏi–đáp đã diễn ra |
| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Review và tổng hợp CP5/CP6; soạn v0/v1, metric, năm tiêu chí, bốn rủi ro và kết luận review Not Yet | Báo cáo nhóm mục 4–8: tách gom/soát, kiểm mapping ngoài tổng tiền, Rule là hướng đề xuất; nhóm xác nhận riêng |
| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Mở kiểm ba tài liệu Microsoft về Append, Merge và Conditional Formatting; bổ sung research và đóng góp Hưởng | Báo cáo nhóm mục 3.3/10, TEAM mục cá nhân; research tính năng không thay baseline hay kết quả pilot |

| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Review, chuẩn hóa và merge năm PR từ bốn thành viên; main/local main tới `314b6d8` | PR #3/#7 Linh, #4 Vinh, #5 Khương, #6 Tuyên. Nhánh Quân không có nội dung mới; các bản local của Hưởng giữ nguyên trong lượt merge |
| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Hoàn thiện bằng chứng CP1 từ tình huống điều phối/tích hợp đang diễn ra, cập nhật đóng góp thật và đối chiếu bản tổng hợp local với main mới | CP1 giữ ba trải nghiệm đời sống; hai vấn đề còn lại có số đếm nhánh/báo cáo/PR. Mục 3.3/4/6 báo cáo nhóm giữ nội dung các thành viên đã merge; v0/v1 và eval là đề xuất local |


| 2026-11-09 | Trợ lý, theo yêu cầu Hưởng | Chuẩn bị commit/push và PR cho bản tổng hợp Hưởng trên main e278c07 | Giữ CP4 Linh mới bổ sung; kiểm bốn file, nguồn giả định/đề xuất và metadata tác giả; không ghi nhận đồng thuận hoặc phỏng vấn thay nhóm |
| 2026-11-09 | Theo yêu cầu Hưởng | Xác nhận bản tổng hợp và mục 2 đã merge qua PR #8/#9 | Main `90dcaa7`; cập nhật các trạng thái lịch sử “local” trong phần theo dõi hiện tại |
| 2026-11-09 | Theo ủy quyền trực tiếp của Hưởng | Ghi quyết định điều phối: Rule cho soát trên bảng đã ghép đúng; Not Yet cho pilot; target dưới 90 phút công/vòng | Báo cáo nhóm mục 1, 4–8 và TEAM.md; không gán thành biểu quyết sáu người. Điều kiện chuyển Go/ngưỡng dừng giữ rõ ở mục 8 |
| 2026-11-09 | Theo yêu cầu Hưởng | Fetch và review eval mới trên nhánh Quân | `9ccefc8`: 10 tình huống tổng hợp; lỗi trung vị TC-03, đơn vị tiền TC-09, baseline thiếu nguồn và target bị ghi thành kết quả; nhận xét ở mục 7, chưa merge |
| 2026-11-09 | Theo yêu cầu Hưởng | Commit/push nhánh Hưởng, tạo và merge PR #10 sau kiểm tra; đồng bộ main và nhánh cá nhân | [PR #10](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/10): nội dung `384850c`, merge `1ee80b3`; bốn file, không conflict; công bố Rule/Not Yet và metric dưới 90 phút công/vòng |
| 2026-11-09 | Theo yêu cầu Hưởng | Rà soát phần Hưởng sau PR #10, đối chiếu nguồn review và cập nhật trạng thái công bố | Mục 4/6.7/7 báo cáo cá nhân, TEAM.md và báo cáo nhóm được đồng bộ với `1ee80b3`; mô tả PR là nguồn review tài liệu, không gán thêm người hỏi/đáp. Đầu nhánh Quân `70be730` không còn file eval của `9ccefc8` |

## 8. Danh sách cần bổ sung trước khi nộp

| Phần | Nội dung còn thiếu / việc cần kiểm | Người cung cấp hoặc chốt | Trạng thái |
|---|---|---|---|
| CP3 | Bổ sung bản ghi pitch/challenge thực tế; đối chiếu cluster/OST, điểm và lý do chọn/loại | Cả nhóm; Hưởng tổng hợp | Mục 2 đã tổng hợp 18 card, cluster/OST và điểm review; hỏi–đáp giữa các thành viên cần nguồn thực tế |
| Phạm vi | Soát trên bảng đã ghép đúng; kiểm ngưỡng, dữ liệu và đáp án trước pilot | Hưởng quyết định theo ủy quyền; Vinh xác nhận đầu vào | Đã chọn Rule và phạm vi; quyền dữ liệu/ngưỡng không được suy từ quyết định này |
| CP4 | Kiểm sáu giả định, bổ sung kiểm chứng người thật và đối chiếu research công cụ | Linh, Khương; nhóm xác nhận điều chỉnh | Assumption map/research đã có trên main; repo có một snapshot và tổng hợp 3 người, cần bổ sung nguồn hành vi, vai trò, ngày và cách hỏi từng người |
| CP5 | Đối chiếu timing nguồn Vinh; kiểm mapping và quyền dữ liệu | Vinh; Hưởng tổng hợp | v0 và quy trình tương lai đã đồng bộ phạm vi Rule; phút tương lai là ngân sách thiết kế, không phải số đo |
| CP6 | Sửa eval, có đáp án domain; đối chiếu năm tiêu chí, bốn rủi ro và điều kiện chuyển Go | Quân, Vinh, Tuyên; Hưởng tổng hợp | Đã có quyết định Rule/Not Yet; eval nhánh Quân cần sửa theo review, không coi là test đã đạt |
| Đóng góp | Mỗi thành viên tự ghi phần mình, dẫn sản phẩm và nguồn | Từng thành viên | Phần Hưởng có bằng chứng PR #2–#10 và sản phẩm trên main; các thành viên tự ghi phần mình |
| Trình bày | Đủ mục 1–10; link nguồn/file và hình hiển thị; tên báo cáo đúng; CP7 do từng người tự viết | Hưởng rà soát; từng người kiểm phần mình | Báo cáo có khung 1–10, nội dung chưa đủ để nộp |
| Git | PR #10 đã merge; rà soát ghi chú và nguồn của Hưởng trên nền main `1ee80b3` | Hưởng kiểm tra trước commit/push lượt mới | Cập nhật mới ở local, chỉ bốn file hiện có; không tự merge nhánh Quân hoặc push lượt rà soát này |
