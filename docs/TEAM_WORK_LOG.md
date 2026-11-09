# Điều phối công việc TEAMLAGI

**Trạng thái: phân công đã được các thành viên đồng ý, theo xác nhận của trưởng nhóm Nguyễn Trọng Hưởng trong chat ngày 2026-11-09. Trạng thái sản phẩm được theo dõi riêng; commit/PR chứa file này là bản công bố phân công.**

File điều phối được bổ sung theo hướng dẫn của LabCoach mà trưởng nhóm đã trao đổi. Các tài liệu đề bài trong repo giữ nguyên. Đây là hướng dẫn phối hợp; sản phẩm nộp chính vẫn là báo cáo cá nhân, báo cáo nhóm và `TEAM.md`.

## 1. Bài toán chung và bước hiện tại

- Nhóm đã trao đổi và chọn hướng đối chiếu chênh lệch hồ sơ của các nhà thầu.
- Phạm vi đã chọn theo ủy quyền trưởng nhóm ngày 2026-11-09: soát khối lượng/đơn giá trên bảng đã ghép đúng mã, đơn vị và phiên bản BOQ; không gồm ghép sai mẫu, đọc PDF/scan hoặc đánh giá năng lực.
- Quyết định hiện tại: chọn Rule, **Not Yet cho triển khai/pilot**; target dưới 90 phút công/vòng gồm kiểm/sửa/ngoại lệ. Quyền dữ liệu, mapping, cấu hình và đáp án phải được xác nhận trước pilot.
- Việc chọn vấn đề không đồng nghĩa đã kiểm chứng pain, số liệu hoặc giải pháp.
- Quy mô nhóm: 6 người; trưởng nhóm xác nhận trong chat ngày 2026-11-09 rằng coach đã cho phép. Đây là thông tin do trưởng nhóm cung cấp, chưa kèm thông báo của coach trong repo.
- Bản tổng hợp và quyết định Rule/Not Yet đã công bố qua PR #8–#11. PR #16–#19 tiếp tục tích hợp Tuyên, Linh, Vinh và Quân; mốc main sau tích hợp là `2729d4b`. Các ghi nhận CP3/CP4 vẫn cần đúng nguồn hoạt động, không suy từ việc merge PR.

## 2. Phân công đã xác nhận và phụ thuộc

| Người | Nhánh cá nhân | Việc chính | Sản phẩm phụ trách | Phụ thuộc để tổng hợp/chốt | Trạng thái sản phẩm |
|---|---|---|---|---|---|
| Hưởng | `NguyenTrongHuong-branch` | Điều phối; tổng hợp CP3, phạm vi, Problem Statement và metric | `docs/TEAM_WORK_LOG.md`; `TEAM.md`; `report/team/group_report.md` | Ghi chép CP3 thực tế; dữ liệu/đáp án có người domain kiểm | Đã điều phối PR #16–#19, bảo toàn sáu báo cáo, đủ sáu mục đóng góp và bộ eval; rà soát nguồn, before/after và cấu trúc nộp |
| Vinh | `vinh1811` | Quy trình, dữ liệu, bottleneck và before/after | Báo cáo cá nhân; báo cáo nhóm mục 4 | Quyền dữ liệu, mapping, nguồn thời gian và đáp án | CP5 nguồn qua PR #4; cá nhân qua PR #12/#13; đóng góp TEAM và chuẩn hóa 6.7 qua PR #18, giữ đủ các báo cáo khác |
| Linh | `damlinh820` | Kiểm chứng, assumption map và snapshot | Báo cáo nhóm mục 3.1–3.2; báo cáo cá nhân | Nguồn vai trò, ngày/cách hỏi và hành vi từng người | Nhật ký và phần hiểu bài tích hợp PR #17; MSSV TEAM đã sửa. Vẫn một snapshot chi tiết cho tổng hợp ghi 3 người; bổ sung dữ liệu thực tế trước xác nhận pain |
| Khương | `dangkhuong14` | Research giải pháp và kiểm nguồn | Báo cáo nhóm mục 3.3; báo cáo cá nhân | Nguồn chính thức, giới hạn công cụ và phạm vi Rule | Research qua PR #5; báo cáo/đóng góp qua PR #14/#15; bảng dùng công cụ CP4 được đồng bộ theo nhật ký bàn giao |
| Quân | `quan-branch` | Tiêu chí, tình huống kiểm tra và đáp án thiết kế | `report/assets/cp6-2A202603626-eval.md`; báo cáo nhóm mục 7 | Dữ liệu được phép dùng, mapping/ngưỡng/đáp án domain | PR #19 đã khôi phục/sửa eval, tích hợp cá nhân và TEAM; 10 tình huống tổng hợp, chưa có kết quả pilot |
| Tuyên | `titus` | Mức can thiệp, boundary và bốn rủi ro | Báo cáo nhóm mục 6–8; báo cáo cá nhân | CP4; quy trình Vinh; eval Quân; dữ liệu/đáp án trước pilot | CP6 nguồn qua PR #6; cá nhân/đóng góp qua PR #16, thống nhất chọn Rule và Not Yet cho pilot |

Các file phụ không bắt buộc tách riêng khi nội dung đã nằm trong báo cáo. Vinh/Tuyên/Khương viết phần nhóm trực tiếp; bộ eval Quân có tại `report/assets/cp6-2A202603626-eval.md` sau PR #19. Mỗi người còn chịu trách nhiệm xác nhận nhật ký thực tế và tự giải thích phần cá nhân. Sản phẩm thiết kế không thay cho dữ liệu/đáp án được duyệt hoặc kết quả pilot.

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
| 2026-11-09 | Theo yêu cầu Hưởng | Tích hợp cá nhân và đóng góp Tuyên qua PR #16; nhật ký, nguồn và phần hiểu bài Linh qua PR #17 | Giữ nguyên reflection 6.1–6.6 từ nhánh thành viên; sửa MSSV Linh, tách chọn Rule khỏi cho phép pilot |
| 2026-11-09 | Theo yêu cầu Hưởng | Xử lý nhánh Vinh có thao tác xóa báo cáo, giữ bản main và tích hợp riêng phần Vinh qua PR #18 | Đủ sáu báo cáo, giữ các nguồn tham khảo mới; TEAM chỉ thêm mục Vinh, 6.7 được chuẩn hóa |
| 2026-11-09 | Theo yêu cầu Hưởng | Tích hợp Quân và bộ eval sau review qua PR #19 | Sửa ba conflict, loại IDE files khỏi kết quả, khôi phục 10 tình huống tổng hợp và sửa phép tính/tiêu chí; không công bố hiệu quả chưa đo |
| 2026-11-09 | Theo yêu cầu Hưởng | Rà soát bản chung sau tích hợp | Dẫn ba câu hỏi theo nhật ký Vinh, bổ sung số bước before/after cùng phạm vi, đồng bộ nguồn/đóng góp và bảng dùng công cụ Khương; xóa template khi đủ sáu báo cáo riêng |

## 8. Danh sách cần bổ sung trước khi nộp

| Phần | Nội dung còn thiếu / việc cần kiểm | Người cung cấp hoặc chốt | Trạng thái |
|---|---|---|---|
| CP3 | Bổ sung hỏi–đáp thực tế và thay đổi sau phản biện; xác nhận điểm review khi thảo luận | Các thành viên; Hưởng tổng hợp | Đã có nguồn ba câu hỏi Vinh; câu hỏi đề xuất của các thành viên khác vẫn cần bản ghi, không tự điền thay |
| Phạm vi | Soát trên bảng đã ghép đúng; kiểm ngưỡng, dữ liệu và đáp án trước pilot | Hưởng quyết định theo ủy quyền; Vinh xác nhận đầu vào | Đã chọn Rule và phạm vi; quyền dữ liệu/ngưỡng không được suy từ quyết định này |
| CP4 | Bổ sung vai trò, ngày/cách hỏi và tình huống của ba người được ghi nhận; số phút/tần suất có nguồn | Linh; Khương hỗ trợ đối chiếu công cụ | Có một snapshot, tổng hợp 3 người và research; dữ liệu hành vi và nguồn định lượng còn thiếu |
| CP5 | Người domain kiểm mapping, quyền dữ liệu và nguồn baseline | Vinh; Hưởng tổng hợp | Đã có quy trình Rule, v0 và before/after cùng phạm vi, gồm số bước và bước có người tham gia; thời gian sau là ngân sách thiết kế |
| CP6 | Domain duyệt cấu hình/đáp án; bổ sung trường hợp biên và log khi pilot được phép | Quân, Vinh, Tuyên; Hưởng tổng hợp | Năm tiêu chí và 10 cặp dữ liệu tổng hợp/đáp án đã có; Rule/Not Yet và điều kiện chuyển Go giữ nguyên |
| Đóng góp | Mỗi người đối chiếu nội dung và giải thích sản phẩm của mình | Từng thành viên | Đủ sáu mục trong TEAM.md; có PR/commit hoặc đường dẫn sản phẩm làm nguồn, không gán công việc của người khác |
| Trình bày | Kiểm nguồn CP3/CP4, dữ liệu thời gian CP2 và yêu cầu tự viết reflection; nộp LMS cá nhân | Hưởng rà soát; từng người xác nhận | Đủ sáu báo cáo, mục 6.7 có 5–8 câu; template đã xóa sau kiểm đủ file. Việc nộp LMS nằm ngoài dữ liệu GitHub |
| Git | Review/merge các nhánh thành viên và bản rà soát cuối | Hưởng | PR #16–#19 đã merge; thay đổi rà soát cuối được công bố theo commit/PR chứa bản này. Không push hoặc xóa dữ liệu ngoài phạm vi |
