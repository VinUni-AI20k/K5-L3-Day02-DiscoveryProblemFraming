# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: Nhom9999
- Candidate problem nhóm chọn (1 câu): (#7) Học viên học song song ở trường, khóa tiếng Anh và khóa AI mất khoảng 25 phút mỗi ngày để kiểm tra nhiệm vụ trên nhiều nền tảng và xếp thứ tự ưu tiên, nên khoảng 4 lần/tháng phải làm gấp sát deadline.
- Quyết định cuối (Go / Not Yet / No-Go): Go, phạm vi nhỏ: pilot 6 tuần ở mức Rule, không dùng AI; hai bước AI (gợi ý thứ tự, trích nhiệm vụ từ thông báo): Not Yet.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Vũ Quang Minh | 2A202603657 | Trưởng nhóm; điều phối thời gian, ghi chép, viết Problem Statement | Minh8246 |
| 2 | Hà Huy Thái | 2A202603682 | Phụ trách kiểm chứng (phỏng vấn); mức can thiệp AI + Problem Statement v1 | thailc0903 |
| 3 | Nguyễn Công Quân | 2A202603675 | Phụ trách research; vẽ quy trình | nguyencongquana2 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Vũ Quang Minh | Hà Huy Thái, Nguyễn Công Quân | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Hà Huy Thái | Vũ Quang Minh, Nguyễn Công Quân | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Công Quân | Vũ Quang Minh | Bảng research có link |
| CP5 — Quy trình trước/sau | Nguyễn Công Quân | Hà Huy Thái | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Vũ Quang Minh | Nguyễn Công Quân | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Hà Huy Thái | Vũ Quang Minh | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Vũ Quang Minh | Hà Huy Thái, Nguyễn Công Quân | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### HaHuyThai-2A202603682

**Phần việc phụ trách:**

-Phụ trách kiểm chứng CP4 (phỏng vấn), mức can thiệp AI và Problem Statement v1 (CP6); hỗ trợ quy trình trước/sau CP5 và quyết định CP6.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-Chuẩn bị và pitch ba candidate #4–#6 (kiểm tra file trước khi nộp, tìm lỗi Python, so sánh kết quả train); đặt câu hỏi phản biện cho các candidate #1, #3, #7 và #9.
- Phụ trách kiểm chứng CP4: xây dựng assumption map, tổng hợp các interview snapshot và xác định những giả định cần kiểm chứng thêm.
- Hỗ trợ xây dựng quy trình trước/sau CP5, xác định bước nghẽn, phần việc con người cần kiểm tra và phương án quay về khi AI sai.
- Thực hiện CP6 (mục 6): phân tích ma trận độ mơ hồ × độ phức tạp, so sánh No AI / Rule / Workflow / Agent, xây dựng AI Canvas và trả lời hai câu hỏi Google PAIR.
- Đề xuất Workflow có AI hỗ trợ xếp thứ tự ưu tiên, đồng thời phân tích hạn chế của Rule và rủi ro khi AI bỏ sót nhiệm vụ.
- Xây dựng Problem Statement v1 và các tiêu chí đánh giá đầu ra; phối hợp với nhóm rà soát để thống nhất với quyết định Go phạm vi nhỏ ở mức Rule, hai bước AI giữ ở Not Yet.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-report/team/group_report.md: mục 2.1 (candidate #4–#6 và các câu hỏi phản biện), mục 3 (kiểm chứng CP4), mục 4 (hỗ trợ quy trình), mục 6 (ma trận, bảng so sánh, AI Canvas, Google PAIR), mục 7 (Problem Statement v1, tiêu chí đánh giá).

- report/individual/2A202603682_HaHuyThai.md: CP1, CP2 và các phần nhật ký tham gia, sử dụng AI cần cập nhật theo công việc thực tế.

- Commit: bổ sung mã commit cá nhân sau khi push phần CP4(fbcc6b1) và CP6(77ffd18) lên GitHub.

**Điều mình học được từ phần nhóm:**

-Tôi hiểu rằng không phải vấn đề nào cũng cần dùng AI. Cần xác định rõ bước nghẽn, có số liệu kiểm chứng và thử giải pháp đơn giản trước. Qua CP6, tôi học được cách so sánh các mức can thiệp AI, đánh giá rủi ro và giữ con người kiểm tra những quyết định quan trọng.

### VuQuangMinh-2A202603657

**Phần việc phụ trách:**

- Trưởng nhóm: điều phối thời gian, ghi chép, review và merge PR của các thành viên.
- Người chính CP3 (hội tụ nhóm), Problem Statement v0 (CP5) và quyết định (CP6); hỗ trợ kiểm chứng và research CP4, mức can thiệp CP6.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch ba candidate #1–#3 (tìm bài nghe vừa trình độ, kiểm tra phát âm, soát lỗi ngữ pháp); đặt câu hỏi phản biện cho #4, #6 (Thái) và #8 (Quân).
- Viết cluster, cây OST, bảng chấm điểm shortlist và lý do chọn/loại; đề xuất chọn candidate #7, nhóm đồng ý.
- Điền thông tin nhóm, vai trò và phân công theo checkpoint trong `TEAM.md`.
- Rà soát mục 3 (CP4): mở lại link research, bổ sung nguồn trang giá Zapier, bổ sung thời gian và cách phỏng vấn cho các snapshot.
- Viết Problem Statement v0 (mục 5, CP5): 6 trường dựa trên quy trình nháp card #7 của Quân và 3 snapshot CP4; nhờ AI phản biện, sửa 3 điểm ngay ở v0 và chuyển 3 điểm (metric tỉ lệ, guardrail sót nhiệm vụ, phạm vi actor) sang v1 cho CP6; đối chiếu mục 5 với quy trình mục 4 của Quân và sửa 2 chỗ lệch.
- Viết quyết định CP6 (mục 8): chấm 4 rủi ro cho giải pháp mức Rule, quyết định Go phạm vi nhỏ (pilot 6 tuần), để hai bước AI (gợi ý thứ tự, trích nhiệm vụ) ở Not Yet với điều kiện cụ thể, đặt 4 ngưỡng dừng; viết mục 9 (hạn chế, hướng tiếp theo) và mục 10 (tài liệu tham khảo).
- Tổng kết báo cáo: ghép mục 6 của Thái (đề xuất Workflow có AI gợi ý thứ tự) với quyết định mức Rule ở mục 8: giữ lập luận ma trận, AI Canvas và câu trả lời PAIR của Thái, đưa phương án của Thái thành Workflow (a) ở Not Yet; viết mục 7 (Problem Statement v1, 5 tiêu chí đánh giá), đưa 3 điểm phản biện đã hoãn ở mục 5 vào v1; rà lại toàn bài cho thống nhất.
- Review và merge 15 PR của nhóm vào `main`.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`: mục 2.1 (candidate #1–#3, câu hỏi tại #4, #6, #8), mục 2.2–2.4 (cluster, OST, chấm điểm, lý do chọn/loại), mục 3 (rà soát CP4), mục 5 (Problem Statement v0 và bảng phản biện), mục 6 (ghép với phần của Thái), mục 7 (Problem Statement v1, tiêu chí đánh giá), mục 8 (4 rủi ro, quyết định, ngưỡng dừng), mục 9–10.
- `report/individual/2A202603657_VuQuangMinh.md`: CP1, CP2, mục 4 nhật ký tham gia CP3–CP6 và mục 5 dùng AI.
- Commit: `d0cc88c`, `557adc2` (thông tin nhóm, chốt #7, phân công), `1b2900f` (câu hỏi phản biện bảng 2.1), `7d01002` (cluster, OST, chấm điểm), `f348dd2` (sửa câu chữ báo cáo nhóm), `a1e4ca4` (rà soát CP4), `fef8440` (Problem Statement v0), `3be068d` (quyết định CP6).

**Điều mình học được từ phần nhóm:**

-

### NguyenCongQuan-2A202603675

**Phần việc phụ trách:**

- Phụ trách research CP4 và quy trình trước/sau CP5; hỗ trợ Problem Statement v0 và quyết định CP6.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Chuẩn bị và pitch ba candidate #7–#9; đặt câu hỏi phản biện cho candidate #2 và #5.
- Cung cấp candidate #7 cùng baseline khoảng 25 phút/ngày và khoảng 4 lần/tháng phải làm gấp; candidate này được nhóm chọn.
- Research ba hướng giải pháp hiện có: Todoist, workflow Zapier Discord–Todoist và Motion auto-scheduling; phân tích bước được giải, khoảng trống và bài học.
- Chi tiết hóa quy trình hiện tại thành bốn bước có thời gian và thiết kế quy trình tương lai giả thuyết gồm Rule/Workflow, AI hỗ trợ, bước con người kiểm tra, boundary và phương án quay về.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`: mục 2.1 (candidate #7–#9 và câu hỏi tại #2, #5), mục 2.4 (candidate được chọn), mục 3.3 (bảng research), mục 4 (quy trình trước/sau và bảng before/after).
- `report/individual/2A202603675_NguyenCongQuan.md`: CP1, CP2 và mục 4 nhật ký tham gia CP3–CP5.
- Commit cá nhân: `aba1090` (CP1), `7bae1df` (CP2), `4319ccd` (CP4 Research).

**Điều mình học được từ phần nhóm:**
- Tôi học được rằng nhóm không nên chọn vấn đề chỉ vì giải pháp nghe hấp dẫn, mà cần so sánh actor, quy trình, bottleneck và bằng chứng đo được trước khi quyết định.
