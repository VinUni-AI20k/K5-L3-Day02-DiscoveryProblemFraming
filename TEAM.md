# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm:
- Candidate problem nhóm chọn (1 câu):
- Quyết định cuối (Go / Not Yet / No-Go):

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | | | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | | | Assumption map, snapshot hoặc survey |
| CP4 — Research | | | Bảng research có link |
| CP5 — Quy trình trước/sau | | | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | | | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | | | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | | | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### HoangHaiNam-2A202603694

**Phần việc phụ trách:**

- Phản biện kỹ thuật (CP3), kiểm chứng & research giải pháp có sẵn (CP4), thiết kế quy trình trước/sau & Problem Statement (CP5–CP6), đánh giá mức can thiệp AI và rủi ro (CP6).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp 3 Problem Cards cá nhân từ thực tế làm việc của lập trình viên và tham gia phản biện chéo ở CP3 (nêu vấn đề AI bị hallucinate khi đọc context hàng trăm tin nhắn và đề xuất hướng cắt đoạn hội thoại có overlap).
- Cùng nhóm gom Cluster A, dựng cây OST, lập Assumption Map và trực tiếp research 3 công cụ (Zalo OA/GMF, Slack AI, n8n Information Extractor), chỉ ra giới hạn Zalo OA chỉ quản lý được nhóm do OA tạo.
- Tham gia thiết kế quy trình tương lai 6 bước (Rule + AI + Con người kiểm duyệt), hoàn thiện Problem Statement v0 → v1, bộ 3 tiêu chí đánh giá (eval) và đánh giá 4 rủi ro để chốt quyết định **Not Yet** kèm ngưỡng dừng.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- File cá nhân: `report/individual/2A202603694_HoangHaiNam.md`
- Phần nhóm trong `report/team/group_report.md`: Mục 2.1 (candidate #7, #8, #9), Mục 3.3 (bảng research Zalo OA/Slack AI/n8n), Mục 4 (quy trình trước/sau), Mục 5–8 (Problem Statement v0/v1, mức can thiệp AI, quyết định).

**Điều mình học được từ phần nhóm:**

- Học được cách đi từ nỗi đau thực tế đến kiểm chứng tính khả thi dữ liệu đầu vào trước khi xây AI: dù ý tưởng dùng AI tóm tắt nhóm Zalo nghe rất hấp dẫn, việc research kỹ giới hạn API/quyền truy cập của Zalo OA và rủi ro bảo mật dữ liệu giúp nhóm đưa ra quyết định thực tế và an toàn hơn thay vì vội vàng code ngay.


### PhamThanhTung-2A202603695

**Phần việc phụ trách:**

- Đề xuất và phân tích Candidate Problem cá nhân (CP3), tham gia phản biện và lựa chọn vấn đề của nhóm, tìm hiểu hướng kiểm chứng vấn đề (CP4), đề xuất quy trình xử lý và đánh giá mức can thiệp AI (CP5–CP6).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp 3 Candidate Problem cá nhân ở CP3 gồm: tổng hợp deadline từ LMS, tin nhắn nhóm và file bài tập (#10), tổng hợp tiến độ làm việc nhóm (#11), chuyển yêu cầu dài thành các đầu việc cụ thể (#12). Phân tích Actor, Bottleneck và tham gia phản biện để làm rõ các vấn đề.
- Ở CP4, tìm hiểu cách kiểm chứng thông tin từ nhiều nguồn khác nhau, xác định những trường hợp dễ bị bỏ sót hoặc nhầm lẫn deadline và xem xét tính khả thi của dữ liệu đầu vào trước khi áp dụng AI.
- Ở CP5–CP6, đề xuất hướng tổng hợp thông tin thành checklist công việc có deadline và nguồn tham chiếu để dễ kiểm tra. Tham gia đánh giá các mức can thiệp No AI, Rule, Workflow và Agent, đồng thời đề xuất cần có bước kiểm tra lại kết quả AI để hạn chế sai sót.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- File cá nhân: `report/individual/2A202603695_PhamThanhTung.md`
- Phần nhóm trong `report/team/group_report.md`: Mục 2.1 (Candidate #10, #11, #12 và nội dung phản biện), các phần CP3–CP6 liên quan đến kiểm chứng vấn đề, đề xuất quy trình và đánh giá mức can thiệp AI.

**Điều mình học được từ phần nhóm:**

- Qua quá trình làm việc nhóm, mình hiểu rõ hơn cách xác định một vấn đề thực tế và phân tích nguyên nhân trước khi đưa ra giải pháp. Mình học được cách đặt câu hỏi phản biện, kiểm chứng dữ liệu đầu vào và đánh giá tính khả thi của việc ứng dụng AI. Ngoài ra, mình nhận ra không phải vấn đề nào cũng cần dùng AI, mà cần lựa chọn giải pháp phù hợp để đảm bảo hiệu quả và hạn chế sai sót.
### HoVaTen-MSSV

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-
