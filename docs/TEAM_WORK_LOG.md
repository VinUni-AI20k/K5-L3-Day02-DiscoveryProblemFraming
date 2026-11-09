# Điều phối công việc TEAMLAGI

**Trạng thái: phân công đã được các thành viên đồng ý, theo xác nhận của trưởng nhóm Nguyễn Trọng Hưởng trong chat ngày 2026-11-09. Trạng thái sản phẩm được theo dõi riêng; commit/PR chứa file này là bản công bố phân công.**

File điều phối được bổ sung theo hướng dẫn của LabCoach mà trưởng nhóm đã trao đổi. Các tài liệu đề bài trong repo giữ nguyên. Đây là hướng dẫn phối hợp; sản phẩm nộp chính vẫn là báo cáo cá nhân, báo cáo nhóm và `TEAM.md`.

## 1. Bài toán chung và bước hiện tại

- Nhóm đã trao đổi và chọn hướng đối chiếu chênh lệch hồ sơ của các nhà thầu.
- Phạm vi đề xuất để làm rõ: đối chiếu hồ sơ chào giá với yêu cầu/BOQ và giữa các nhà thầu; phát hiện chênh lệch khối lượng, đơn giá và mô tả hạng mục.
- Bản tổng hợp local đã review CP5 của Vinh và CP6 của Tuyên; đề xuất ưu tiên phần soát sau khi bảng đã ghép đúng. Tiếp tục ghi kết quả CP3, kiểm chứng CP4 và xác nhận phạm vi/đáp án trước thử.
- Việc chọn vấn đề không đồng nghĩa đã kiểm chứng pain, số liệu hoặc giải pháp.
- Quy mô nhóm: 6 người; trưởng nhóm xác nhận trong chat ngày 2026-11-09 rằng coach đã cho phép. Đây là thông tin do trưởng nhóm cung cấp, chưa kèm thông báo của coach trong repo.
- Phạm vi review đề xuất: so khối lượng/đơn giá trên bảng có mã, đơn vị và mapping đã kiểm; ghép file sai mẫu được tách riêng. Actor và baseline tham chiếu theo Vinh; quyền dùng dữ liệu, đáp án và xác nhận chung được kiểm trước pilot.

## 2. Phân công đã xác nhận và phụ thuộc

| Người | Nhánh cá nhân | Việc chính | Sản phẩm phụ trách | Phụ thuộc để tổng hợp/chốt | Trạng thái sản phẩm |
|---|---|---|---|---|---|
| Hưởng | `NguyenTrongHuong-branch` | Điều phối; tổng hợp kết quả CP3, phạm vi, Problem Statement và metric | `docs/TEAM_WORK_LOG.md`; `TEAM.md`; `report/team/group_report.md` | Ghi chép CP3 do nhóm cung cấp; sản phẩm của 5 thành viên; v0/v1 và quyết định do nhóm tự chốt | Đã có bản tổng hợp/review local, nguồn Vinh/Tuyên và research công cụ; nhóm kiểm/chốt trước công bố |
| Vinh | `vinh1811` | Mô tả quy trình thực tế, chuẩn bị dữ liệu được phép dùng, đo bottleneck và before/after | `report/assets/cp5-2A202603672-quy-trinh.md` | Phạm vi/actor được nhóm chốt; quyền dùng dữ liệu; tách số đo, ước lượng và target; đối chiếu kiểm chứng CP4 | CP5 đã merge qua PR #4; giữ nguyên trong bản tổng hợp local từ main `314b6d8` |
| Linh | `damlinh820` | Điều phối kiểm chứng, assumption map, snapshot và tổng hợp tín hiệu phản bác | `report/assets/cp4-2A202603624-kiem-chung.md` | Actor/phạm vi; người ngoài nhóm thực sự gặp vấn đề; ghi nguồn, khi nào và cách hỏi | Đã có assumption map và một snapshot tại main e278c07; cần bổ sung số người, thời điểm/cách hỏi và tín hiệu phản bác |
| Khương | `dangkhuong14` | Research giải pháp hiện có, kiểm nguồn, đối chiếu phần đã giải và khoảng trống | `report/assets/cp4-2A202603627-research.md` | Phạm vi bài toán và bước cần so sánh; link nguồn được mở và kiểm | Research nhà thầu mục 3.3 đã merge qua PR #5; liên kết chính thức đã mở kiểm |
| Quân | `quan-branch` | Tiêu chí đánh giá, tình huống kiểm tra, đáp án đối chiếu và phương án đơn giản làm mốc so sánh | `report/assets/cp6-2A202603626-eval.md` | Loại chênh lệch và ngưỡng do nhóm chốt; dữ liệu được phép dùng; đáp án có người domain kiểm; quy trình/boundary | Đã xác nhận phân công; chưa nhận sản phẩm CP6 |
| Tuyên | `titus` | So sánh mức can thiệp, dữ liệu, boundary, AI Canvas/PAIR nếu phù hợp và bốn rủi ro | `report/assets/cp6-2A202603648-muc-can-thiep.md` | Bằng chứng CP4; quy trình Vinh; đối chứng/eval Quân; nhóm tự chọn mức và quyết định | CP6 và rủi ro đã merge qua PR #6; bản local tách đề xuất cá nhân khỏi quyết định chung |

Các đường dẫn `report/assets/cp...` là đầu ra dự kiến. Khi kiểm tra ngày 2026-11-09, thư mục assets vẫn chỉ có README; Vinh/Tuyên viết phần nhóm trực tiếp, đã merge qua PR #4/#6; research Khương đã merge qua PR #5. Có sản phẩm trên nhánh riêng không đồng nghĩa đã merge hoặc đã có kết quả pilot. Các phụ thuộc là thứ cần có để tổng hợp/chốt; có thể chuẩn bị song song. Người phụ trách chịu trách nhiệm nội dung và giải thích được lập luận. Mỗi người còn thực hiện đầy đủ phần cá nhân của mình.

Hưởng tổng hợp và phản biện v0/v1, metric và quyết định. Theo yêu cầu mới trong chat, trợ lý đã soạn bản tổng hợp đề xuất từ nguồn thành viên; cách dùng này được ghi rõ để không coi là phần nhóm đã tự viết/chốt. Nhóm tự kiểm, sửa và xác nhận nội dung theo yêu cầu repo.

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

## 8. Danh sách cần bổ sung trước khi nộp

| Phần | Nội dung còn thiếu / việc cần kiểm | Người cung cấp hoặc chốt | Trạng thái |
|---|---|---|---|
| CP3 | Pitch thực tế, câu hỏi và người hỏi/nhận, cluster, outcome/OST, shortlist 3 candidate, điểm 7 tiêu chí, lý do chọn và loại ít nhất 2 candidate, bất đồng nếu có | Cả nhóm; Hưởng tổng hợp | Chưa có ghi chép được cung cấp; chỉ xác nhận hướng đã chọn |
| Phạm vi | Actor, hạng mục, loại chênh lệch, tiêu chí/ngưỡng, dữ liệu được phép dùng | Cả nhóm, đối chiếu với Vinh | Chưa chốt |
| CP4 | Kiểm sáu giả định đề xuất, bổ sung kiểm chứng người thật và đối chiếu research công cụ | Linh, Khương; nhóm xác nhận điều chỉnh | Có assumption map/research đề xuất ở bản tổng hợp local; kiểm chứng ngoài nhóm và bàn giao theo phân công được bổ sung từ nguồn thực tế |
| CP5 | Kiểm phạm vi/timing nguồn Vinh và bản review; xác nhận mapping, quyền dữ liệu và v0 | Vinh; nhóm kiểm/chốt, Hưởng tổng hợp | Có CP5 nguồn và v0 đề xuất local; cần phản hồi người phụ trách |
| CP6 | Hoàn thiện eval cùng đáp án, kiểm bản review v1/bốn rủi ro và lựa chọn | Quân, Tuyên; nhóm kiểm/chốt | Có CP6 của Tuyên, năm tiêu chí và kết luận review local; không coi là test đã đạt |
| Đóng góp | Mỗi thành viên tự ghi phần mình, dẫn sản phẩm và nguồn | Từng thành viên | Đã cập nhật phần Hưởng theo PR và sản phẩm tổng hợp local; các thành viên tự ghi phần mình |
| Trình bày | Đủ mục 1–10; link nguồn/file và hình hiển thị; tên báo cáo đúng; CP7 do từng người tự viết | Hưởng rà soát; từng người kiểm phần mình | Báo cáo có khung 1–10, nội dung chưa đủ để nộp |
| Git | Nhánh Hưởng được đồng bộ với main e278c07 trước khi commit/push bản tổng hợp | Hưởng duyệt trước commit/push | Kiểm diff chỉ bốn file của Hưởng; giữ báo cáo thành viên và nguồn CP4 mới |
