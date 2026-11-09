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
| 4 | Mai Đăng Khương | 2A202603627 | Research giải pháp hiện có, kiểm nguồn | dangkhuong14 |
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

Các đường dẫn sản phẩm trong `report/assets/` là đầu ra dự kiến; Vinh và Tuyên viết trực tiếp trong `report/team/group_report.md`, đã tích hợp lên main qua PR #4/#6; Khương bổ sung mục 3.3 qua PR #5. Bản tổng hợp và quyết định Rule/Not Yet đã công bố qua PR #8–#10; nguồn baseline, target và kết quả thực nghiệm được phân biệt riêng. Phân công không thay thế bằng chứng đóng góp. Phụ thuộc và trạng thái chi tiết ở [nhật ký điều phối](docs/TEAM_WORK_LOG.md#2-phân-công-đã-xác-nhận-và-phụ-thuộc). Các quan hệ hỗ trợ phục vụ tổng hợp trong bảng là luồng bàn giao dự kiến, chưa ghi nhận là công việc đã diễn ra.

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenTrongHuong-202603607

**Phần việc phụ trách:**

- Điều phối sáu thành viên; quản lý phân công/log, review bàn giao và tổng hợp báo cáo nhóm, Problem Statement, metric; công bố phạm vi Rule và quyết định Not Yet qua PR #10 theo ủy quyền của tôi.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Điều phối tích hợp sáu báo cáo cá nhân qua PR #2; tiếp tục yêu cầu kiểm năm nhánh và merge PR #3–#7 của bốn thành viên. Không tạo PR trùng cho Quân vì nội dung đã có trên main; giữ các bản đang sửa trên nhánh cá nhân.
- Yêu cầu trợ lý đọc năm báo cáo, soạn mỗi người một câu hỏi bám vào card; lưu ở mục 4 báo cáo cá nhân như nội dung chuẩn bị trao đổi.
- Sử dụng trợ lý review CP5 của Vinh và CP6 của Tuyên, xử lý conflict/tên file, khôi phục template, kiểm phạm vi diff và merge qua PR #4/#6. Review sửa logic kiểm mapping và phân biệt baseline gom + soát 11–13 giờ/vòng với riêng soát 5–6 giờ/vòng. Bản tổng hợp đã tích hợp qua PR #8–#10, bổ sung v0/v1 và điều kiện trước pilot.
- Tổng hợp v0/v1, metric cùng phạm vi, năm tiêu chí, bốn rủi ro, điều kiện Go và ngưỡng dừng; bản trước đã merge qua PR #8/#9. Ngày 2026-11-09, tôi ủy quyền chốt hướng Rule cho phần soát và giữ Not Yet cho pilot, đồng bộ quyết định trong báo cáo nhóm và log.
- Yêu cầu review bản eval Quân tại `9ccefc8`; nhận xét được ghi trong báo cáo nhóm mục 7, gồm sửa trung vị TC-03, đơn vị tiền TC-09, tỷ lệ thiếu nguồn và phân biệt target với kết quả đã chạy. Đây là review tài liệu, không gán cho Quân câu trả lời chưa có.
- Kiểm research nhà thầu của Khương trong PR #5, sửa bốn tham chiếu thiếu đích thành link chính thức đã mở kiểm; giữ rõ tính năng công cụ với giả thuyết áp dụng. Phần research bổ trợ Microsoft trước đó được ghi đúng nguồn.
- Bảo toàn nội dung thành viên khi tích hợp; sửa tên file, khoảng trắng, dấu thừa và các điểm review đã nêu trong PR. Câu hỏi chuẩn bị không được ghi thành phỏng vấn/pitch đã xảy ra.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [PR #2](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/2), merge commit `4c402eb`: tập hợp báo cáo cá nhân trên main.
- [PR #3](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/3), [#4](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/4), [#5](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/5), [#6](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/6), [#7](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/7), main `314b6d8`: tích hợp mới và review.
- [Báo cáo cá nhân](report/individual/202603607_NguyenTrongHuong.md), mục 4–5: câu hỏi review và cách dùng AI.
- [Báo cáo nhóm](report/team/group_report.md), mục 3.3, 4–8 và 10: research, quy trình, v0/v1, quyết định đã công bố và commit nguồn.
- [PR #8](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/8) và [PR #9](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/9): bản tổng hợp và mục 2 đã tích hợp, main `90dcaa7`.
- [PR #10](https://github.com/trongjhuongwr/K5-L3A-DAY02-TEAMLAGI-DiscoveryProblemFraming/pull/10), nội dung `384850c`, merge `1ee80b3`: công bố quy trình Rule, metric dưới 90 phút công/vòng, quyết định Not Yet và review eval Quân.
- [Nhật ký điều phối](docs/TEAM_WORK_LOG.md): phân công, quyết định theo ủy quyền, review eval và sự kiện merge PR #10. Lượt rà soát ghi chú sau PR #10 được theo dõi riêng, không gán trước một commit cho thay đổi mới.

**Điều mình học được từ phần nhóm:**

- Khi tổng hợp phải giữ cùng phạm vi của baseline–target; số liệu trong báo cáo thành viên vẫn cần nguồn và quyền sử dụng được kiểm.
- Công thức đúng không bảo đảm so đúng hạng mục; kiểm tổng tiền cần đi cùng mapping, đơn vị và truy vết.
- Rule có thể phù hợp phần so số; hỗ trợ ghép ngữ nghĩa là bài toán mở rộng phải có đối chứng và người kiểm riêng.
### DamTuanLinh-2A20263624

**Phần việc phụ trách:**

- Tham gia xây dựng và phản biện Problem Card, đánh giá tính thực tiễn và mức độ phù hợp của các vấn đề được đề xuất.
- Tham gia phản biện chéo giữa các nhóm, tiếp nhận phản biện và đề xuất hướng cải thiện giải pháp AI.
- Thực hiện nghiên cứu, phỏng vấn 3 chuyên viên trong lĩnh vực đấu thầu xây dựng nhằm kiểm chứng nhu cầu thực tế và tính khả thi của giải pháp.
- Đóng góp vào việc điều chỉnh định hướng bài toán từ hệ thống AI tự động phát hiện sai lệch sang công cụ AI hỗ trợ đối soát hồ sơ, có sự kiểm chứng của con người.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- **Phản biện bài của nhóm khác:** Đặt câu hỏi cho nhóm phát triển nền tảng kết nối người kinh doanh đồ ăn và người mua trong khu dân cư: "Làm sao để xác nhận nhu cầu thực của người đăng bài?". Câu hỏi tập trung vào việc kiểm chứng nhu cầu người dùng trước khi phát triển giải pháp, tránh xây dựng sản phẩm dựa trên các giả định chưa được xác thực.

- **Tiếp nhận phản biện:** Nhận câu hỏi về khả năng nhận dạng giọng nói trong điều kiện có tiếng ồn, khác biệt giọng vùng miền và yêu cầu độ chính xác cao đối với các thông tin tài chính như khoản vay, số tiền trả nợ và dữ liệu khách hàng. Từ đó đề xuất hướng giải quyết không chỉ tập trung tối ưu một mô hình Speech-to-Text mà xây dựng pipeline xử lý gồm tiền xử lý âm thanh, nhận dạng giọng nói, fine-tuning theo dữ liệu đặc thù và kiểm chứng thông tin tài chính quan trọng.

- **Kiểm chứng nhu cầu thực tế:** Trực tiếp phỏng vấn 3 người có kinh nghiệm trong lĩnh vực đấu thầu xây dựng nhằm tìm hiểu khó khăn khi đối chiếu hồ sơ mời thầu và đánh giá khả năng ứng dụng AI vào quy trình làm việc.

- **Tổng hợp kết quả phỏng vấn:** Trong 3 người được phỏng vấn, 2 người xác nhận có nhu cầu sử dụng công cụ AI hỗ trợ rà soát hồ sơ. Một người bày tỏ lo ngại về tính phức tạp của việc đối chiếu, khả năng AI đưa ra kết quả sai và vấn đề trách nhiệm khi xảy ra sai sót. Kết quả cho thấy giải pháp có tín hiệu nhu cầu ban đầu nhưng vẫn tồn tại rủi ro đáng kể về độ tin cậy và trách nhiệm chuyên môn.

- **Đề xuất điều chỉnh định hướng giải pháp:** Từ kết quả kiểm chứng, đóng góp vào việc chuyển hướng bài toán từ hệ thống AI tự động phát hiện sai lệch và đưa ra kết luận sang công cụ AI hỗ trợ đối chiếu, rà soát hồ sơ (*AI-assisted Document Review*). Đề xuất áp dụng cơ chế *Human-in-the-loop*, trong đó AI hỗ trợ phát hiện chênh lệch, cung cấp thông tin để truy vết, còn chuyên viên chịu trách nhiệm xác minh và đưa ra quyết định cuối cùng.

- **Đóng góp vào việc xác định mức can thiệp AI:** Làm rõ ranh giới giữa chức năng hỗ trợ nghiệp vụ và chức năng ra quyết định. AI không thay thế chuyên viên đánh giá hồ sơ, đặc biệt đối với các trường hợp cần diễn giải ngữ nghĩa, xác minh thông tin hoặc chịu trách nhiệm pháp lý.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- **Hoạt động phản biện chéo:** Câu hỏi về xác nhận nhu cầu thực của người đăng bài trong dự án kết nối kinh doanh đồ ăn tại khu dân cư.
- **Hoạt động tiếp nhận phản biện:** Câu hỏi về nhận dạng giọng nói vùng miền, tiếng ồn và độ chính xác dữ liệu tài chính; đề xuất pipeline Speech-to-Text kết hợp kiểm chứng thông tin.
- **Hoạt động kiểm chứng:** Kết quả phỏng vấn 3 người làm trong lĩnh vực đấu thầu xây dựng, gồm 2 phản hồi tích cực về nhu cầu sử dụng và 1 phản hồi nêu rủi ro về độ chính xác, trách nhiệm.
- **Báo cáo nhóm `report/team/group_report.md`:** Các nội dung liên quan đến nghiên cứu người dùng, xác định vấn đề, phạm vi giải pháp, mức can thiệp AI và định hướng Human-in-the-loop.
- **Kết quả tác động:** Đóng góp bằng chứng thực tế để nhóm xem xét điều chỉnh định hướng từ AI tự động kết luận sang AI hỗ trợ đối soát hồ sơ.

*Lưu ý: Các bằng chứng trên được tổng hợp từ hoạt động cá nhân đã cung cấp; chưa xác định đường dẫn file minh chứng, số mục chính xác hoặc commit/PR riêng nên không gán mã commit chưa được kiểm chứng.*

**Điều mình học được từ phần nhóm:**

- Một vấn đề chỉ thực sự đáng giải quyết khi có bằng chứng về nhu cầu người dùng, không nên chỉ dựa trên giả định hoặc khả năng công nghệ.
- Phỏng vấn người dùng không chỉ nhằm xác nhận nhu cầu mà còn giúp phát hiện những rủi ro, giới hạn và điều kiện cần thiết để giải pháp được chấp nhận.
- Trong các nghiệp vụ đòi hỏi độ chính xác và trách nhiệm cao như đấu thầu xây dựng, AI không nhất thiết phải tự động hóa toàn bộ quy trình. Giải pháp hỗ trợ ra quyết định, có con người kiểm chứng, có thể phù hợp hơn.
- Cần phân biệt giữa độ chính xác kỹ thuật của mô hình và độ tin cậy của toàn bộ hệ thống. Một mô hình nhận dạng hoặc phát hiện tốt vẫn có thể gây sai sót nếu thiếu bước kiểm chứng, đối chiếu ngữ cảnh và truy vết nguồn.
- Kết quả nghiên cứu thực tế có thể làm thay đổi Problem Statement, phạm vi giải pháp và mức can thiệp AI. Việc điều chỉnh bài toán dựa trên bằng chứng là một phần quan trọng của quá trình Problem Discovery & Framing.
