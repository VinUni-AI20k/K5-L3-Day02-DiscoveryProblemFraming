# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm:H2
- Candidate problem nhóm chọn (1 câu):
- Quyết định cuối (Go / Not Yet / No-Go):

## Thành viên

|  STT | Họ và tên     | MSSV        | Vai trò trong nhóm                                                                                                 | Tài khoản GitHub             |
| ---: | ------------- | ----------- | ------------------------------------------------------------------------------------------------------------------ | ---------------------------- |
|    1 | Đỗ Minh Thanh | 2A202603793 | Đề xuất problem kỹ thuật; phản biện; tổng hợp khảo sát, xác định vấn đề; đối chiếu quy trình và Problem Statement. | https://github.com/thd050810 |
|    2 |               |             |                                                                                                                    |                              |
|    3 |               |             |                                                                                                                    |                              |
|    4 |               |             |                                                                                                                    |                              |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint                                 | Người chính | Người hỗ trợ | Sản phẩm                                       |
| ------------------------------------------ | ----------- | ------------ | ---------------------------------------------- |
| CP3 — Hội tụ nhóm                          |             |              | Cluster, cây OST, bảng chấm điểm               |
| CP4 — Kiểm chứng                           |             |              | Assumption map, snapshot hoặc survey           |
| CP4 — Research                             |             |              | Bảng research có link                          |
| CP5 — Quy trình trước/sau                  |             |              | Quy trình + bảng before/after                  |
| CP5 — Problem Statement v0                 |             |              | Problem Statement v0                           |
| CP6 — Mức can thiệp + Problem Statement v1 |             |              | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định                           |             |              | 4 rủi ro + Go/Not Yet/No-Go                    |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### DoMinhThanh-2A202603793

**Phần việc phụ trách:**

- Tự tìm ý tưởng, scan 10 problem và chọn 3 Problem Cards cá nhân để pitch.
- Phản biện các candidate của nhóm về độ chính xác dữ liệu, tính cá nhân hóa và công sức kiểm tra đầu ra.
- Tổng hợp khảo sát, xác định vấn đề và đối chiếu với quy trình, bottleneck, metric và boundary.
- Hoàn thiện báo cáo cá nhân và phần đóng góp của mình trong báo cáo nhóm; dùng AI hỗ trợ định dạng, chuyển sơ đồ và đối chiếu tài liệu. Tôi quyết định nội dung cá nhân cuối cùng; kết luận nhóm do cả nhóm thống nhất.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đưa ra 3 candidate: hiểu codebase có sẵn, tổng hợp tài liệu ôn thi và tổng hợp metrics experiment; tương ứng candidate #4, #5, #6 trong bảng pitch chung.
- Hỏi Hiếu liệu dữ liệu ngập có đủ mới để hỗ trợ chọn đường; hỏi Hải cách bảo đảm nhận xét đúng từng học sinh khi thời gian duyệt ngắn; hỏi Quân về nguy cơ AI bịa số liệu paper và công sức kiểm tra lại PDF.
- Tiếp nhận phản biện của Hiếu về việc chỉ đúng file/hàm trong codebase lớn, của Quân về tóm tắt tài liệu chính xác và của Hải về phương án dùng MLflow/Weights & Biases thay cho AI.
- Đối chiếu kết quả khảo sát nhóm để làm rõ nhu cầu giảm công soạn lời nhận xét, đồng thời giữ yêu cầu đúng dữ liệu và giáo viên duyệt. Phần đóng góp của tôi là tổng hợp và xác định vấn đề, không nhận toàn bộ hoạt động phỏng vấn là công việc cá nhân.
- Phân biệt thời gian soạn nhận xét 360 phút với tổng quy trình 480 phút/lớp; đối chiếu mục tiêu 45 phút và bước giáo viên rà soát trong quy trình tương lai.
- Đối chiếu phương án Workflow và ranh giới can thiệp: Rule xử lý bảng dữ liệu, AI gợi ý lời văn, giáo viên sửa/duyệt, rồi mới xuất file.
- Hoàn thiện 3 quy trình nháp cá nhân bằng Mermaid màu tối, thể hiện từng bước, thời gian và bottleneck.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603793_DoMinhThanh.md): mục 2 có 10 problem; mục 3 có top 3, Problem Cards và sơ đồ; mục 4 ghi đóng góp CP3–CP6; mục 5 ghi cách dùng AI; mục 6 là Reflection.


**Điều mình học được từ phần nhóm:**

- Pain có thật chưa đủ để kết luận cần AI: ghi và so sánh metrics có thể dùng công cụ thông thường trước khi cân nhắc LLM.
- Khi tổng hợp khảo sát, cần nối actor, bối cảnh, bottleneck và tác động để xác định một vấn đề cụ thể; không bắt đầu bằng tên giải pháp.
- Phải tính cả công sức kiểm tra và sửa đầu ra khi so sánh trước/sau. Bản nháp tạo nhanh chưa bảo đảm tổng thời gian công việc giảm.
- Với bài toán nhận xét học bạ, AI hỗ trợ diễn đạt; giáo viên kiểm tra dữ liệu, cân nhắc hoàn cảnh học sinh và quyết định nội dung cuối cùng.
