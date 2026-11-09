# CP4 — Ghi chú phỏng vấn kiểm chứng (5 Interview Snapshots & Kết quả Khảo sát)

> Tài liệu phụ trợ cho Mục 3.2 của [group_report.md](../team/group_report.md).
> Tuân thủ quy tắc bảo mật ở `RULES.md`: không ghi họ tên thật, email hay số điện thoại của người được phỏng vấn; chỉ ghi theo vai trò và quy mô nhóm.
> Tuân thủ 3 nguyên tắc của **The Mom Test**: (1) Hỏi về công việc thực tế của họ, (2) Hỏi về lần gần nhất đã xảy ra và cách họ đang xử lý (workaround), (3) Không hỏi câu giả định *"Bạn có muốn dùng AI không?"*.

---

## 1. Danh sách câu hỏi khung đã dùng khi phỏng vấn (5–7 phút/người)

1. *"Lần gần nhất bạn phải tổng hợp tiến độ dự án của cả nhóm (để báo cáo cho giảng viên/mentor hoặc đồng bộ đầu tuần/cuối ngày) là khi nào?"*
2. *"Bạn có thể kể lại từng bước lúc đó bạn đã mở những công cụ nào và làm gì không?"*
3. *"Trong các bước đó, bước nào làm bạn mất nhiều thời gian hoặc thấy mệt nhất? Mất khoảng bao nhiêu phút?"*
4. *"Hiện tại nhóm bạn đang dùng cách nào (template, quy ước nhắn tin, bảng công việc...) để đỡ vất vả hơn? Cách đó có chỗ nào vẫn hay bị tắc không?"*
5. *"Người nhận báo cáo (giảng viên hướng dẫn / mentor / quản lý) thường đọc kỹ phần nào nhất và hay hỏi lại câu gì?"*

---

## 2. Chi tiết 5 Interview Snapshots

### Snapshot #1 — Nhóm trưởng đồ án môn học & dự án AI ứng dụng (Nhóm 5 người)

| Trường | Nội dung |
| --- | --- |
| **Người được hỏi** | Nhóm trưởng đồ án môn học & dự án AI ứng dụng (nhóm 5 sinh viên năm cuối, lịch học và thực tập lệch nhau) |
| **Thời điểm & hình thức hỏi** | Phỏng vấn trực tiếp 7 phút trong giờ giải lao buổi lab |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Code thì đẩy lên GitHub, lịch thì ở Google Sheets, nhưng lúc tắc ở đâu thì mấy bạn toàn chụp ảnh màn hình quăng vào Zalo lúc 11h đêm. Tối Chủ Nhật mình ngồi lội lại hơn trăm tin nhắn Zalo với lịch sử commit để viết báo cáo gửi thầy mà hoa cả mắt."* |
| **Lần gần nhất gặp vấn đề** | Tối Chủ Nhật tuần trước (trước buổi họp sáng thứ Hai với giảng viên). Mở 4 nhánh trên GitHub, 1 bảng Sheets và cuộn lại nhóm Zalo từ thứ Tư để tìm lý do vì sao phần tiền xử lý dữ liệu OCR bị chậm tiến độ. |
| **Workaround hiện tại** | Tối Chủ Nhật nhắn tag từng bạn vào Zalo bảo gửi 3 gạch đầu dòng tiến độ + khó khăn, nhưng thường sát giờ vẫn có 2 bạn bận chưa trả lời nên Nhóm trưởng phải tự vào GitHub xem commit và tự tóm tắt. |
| **Mất bao lâu, tần suất** | **65 phút/lần** mỗi tối Chủ Nhật + **15–20 phút/ngày** trong tuần để theo dõi tin nhắn nhóm. |
| **Insight rút ra** | Quy ước bắt mọi người tự nhắn báo cáo giờ cố định dễ thất bại khi làm lệch giờ; bước nghẽn nhất là **nối thông tin giữa commit GitHub và tin nhắn báo lỗi trên Zalo** để viết nhận định. |

---

### Snapshot #2 — Tech Lead nhóm phát triển sản phẩm (Nhóm 4 dev dùng AI coding)

| Trường | Nội dung |
| --- | --- |
| **Người được hỏi** | Tech Lead nhóm 4 lập trình viên trẻ đang xây dựng sản phẩm web/app có sử dụng công cụ AI hỗ trợ code (Cursor / Claude Code) |
| **Thời điểm & hình thức hỏi** | Phỏng vấn nhanh 6 phút qua cuộc gọi và trao đổi trực tiếp |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Từ hồi cả team dùng AI để code, một buổi chiều một ông push lên 15–20 files sửa đủ thứ. Không đọc lại diff với tóm tắt xem ông ấy vừa đổi logic gì thì hôm sau mình code đè lên hoặc họp hỏi nhau mất cả tiếng đồng hồ."* |
| **Lần gần nhất gặp vấn đề** | Chiều thứ Sáu tuần trước, 2 dev cùng sửa phần xác thực và API backend. Khi đồng bộ cuối ngày, cả nhóm mất 45 phút họp Discord chỉ để làm rõ ai đã sửa file nào và vì sao 1 API bị đổi dữ liệu trả về. |
| **Workaround hiện tại** | Quy ước mỗi lần push lớn phải nhắn 1 dòng tóm tắt vào Discord, nhưng khi đang gấp chạy tính năng thì dev chỉ viết commit message ngắn (`fix bug`, `update`). |
| **Mất bao lâu, tần suất** | **30–45 phút/ngày** (~3,5 giờ/tuần) để pull code, đọc diff và nhắn hỏi tiến độ qua lại. |
| **Insight rút ra** | Khi code cùng AI, tốc độ thay đổi code quá nhanh làm tăng mạnh nhu cầu tự động gom và tóm tắt thay đổi từ Git commit/PR kèm cảnh báo những chỗ đang xung đột hoặc chưa hoàn thiện. |

---

### Snapshot #3 — Nhóm trưởng nhóm đồ án 3 người (Tín hiệu phản bác)

| Trường | Nội dung |
| --- | --- |
| **Người được hỏi** | Nhóm trưởng nhóm đồ án 3 sinh viên ngồi học cùng nhau tại thư viện trường 4 buổi/tuần |
| **Thời điểm & hình thức hỏi** | Phỏng vấn trực tiếp 5 phút tại lớp (bàn khác) |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Nhóm mình có 3 người lại ngồi cạnh nhau suốt trên thư viện, có gì quay sang nói 5 phút là xong. Cuối tuần mình chỉ chụp ảnh bảng Trello kèm 3 gạch đầu dòng gửi thầy, mất tầm 10–15 phút thôi."* |
| **Lần gần nhất gặp vấn đề** | Sáng thứ Bảy tuần trước, cả 3 thành viên ngồi chung tại thư viện, kéo thẻ Trello sang cột *Done* và gửi link cho giảng viên. |
| **Workaround hiện tại** | Dùng 1 bảng Trello duy nhất và trao đổi trực tiếp tại bàn. |
| **Mất bao lâu, tần suất** | Chỉ **10–15 phút/tuần**. |
| **Insight rút ra** | **Tín hiệu phản bác giúp nhóm thu hẹp Actor:** Với nhóm 2–3 người ngồi làm việc trực tiếp cùng giờ và giảng viên chỉ xem bảng thẻ việc, phương án **No AI** (bảng Kanban + trao đổi trực tiếp) đã đủ 100%, không nên áp đặt công cụ phức tạp hay AI. |

---

### Snapshot #4 — Điều phối viên dự án nghiên cứu ứng dụng (Nhóm 6 người)

| Trường | Nội dung |
| --- | --- |
| **Người được hỏi** | Học viên phụ trách điều phối và viết báo cáo tuần cho nhóm nghiên cứu ứng dụng gồm 6 thành viên và 1 mentor doanh nghiệp |
| **Thời điểm & hình thức hỏi** | Phỏng vấn trực tiếp 6 phút tại lớp |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Mentor doanh nghiệp không có thời gian mở từng link GitHub hay bảng Sheets đâu. Anh ấy chỉ đọc đúng đoạn tóm tắt 200 chữ ở đầu email: tuần này đạt mốc gì, đang kẹt ở đâu cần anh ấy quyết, tuần sau làm gì. Viết đoạn đó sao cho chuẩn số liệu mà không sót ý của 6 người mới là bước lâu nhất."* |
| **Lần gần nhất gặp vấn đề** | Tối thứ Năm tuần trước, tổng hợp kết quả chạy thực nghiệm của 3 bạn làm mô hình và 2 bạn làm dữ liệu từ Google Sheets + nhóm chat Zalo để gửi mentor trước sáng thứ Sáu. |
| **Workaround hiện tại** | Dùng Google Form thu thập câu trả lời vào Sheets, sau đó mở Sheets đọc và tự viết lại thành đoạn nhận định điều hành (*executive summary*) trên Google Docs. |
| **Mất bao lâu, tần suất** | **50–60 phút/tuần** (riêng bước đọc gom từ Sheets/Zalo và viết đoạn nhận định 200 chữ mất **25–30 phút**). |
| **Insight rút ra** | Chứng minh rõ: kể cả khi đã dùng Form/Sheets (No AI/Rule) để gom thông tin, khâu **tổng hợp ngữ cảnh thành đoạn nhận định ngắn gọn (< 250 từ) nêu bật blocker cho mentor** vẫn là bước nghẽn chính cần hỗ trợ (Augment). |

---

### Snapshot #5 — Lập trình viên Backend từng dùng bot tự động gửi báo cáo

| Trường | Nội dung |
| --- | --- |
| **Người được hỏi** | Lập trình viên Backend (1 năm kinh nghiệm, từng tham gia dự án dùng bot tự động lấy commit/ticket gửi báo cáo thẳng lên kênh Slack) |
| **Thời điểm & hình thức hỏi** | Phỏng vấn trực tiếp 6 phút tại lớp |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Đợt trước team mình từng cài một con bot tự động lấy commit với ticket rồi tự post báo cáo ngày lên kênh chung. Được 1 tuần là không ai đọc nữa vì nó viết dài dòng và có lần nó báo 'Đã hoàn thành tính năng thanh toán' trong khi mới chỉ push code khung chưa chạy được, làm sếp hiểu nhầm."* |
| **Lần gần nhất gặp vấn đề** | Cách đây 2 tháng, bot tự đọc commit message rồi đăng thẳng báo cáo lên kênh có quản lý mà không qua Tech Lead duyệt, dẫn đến báo cáo sai trạng thái hoàn thành của module. |
| **Workaround hiện tại** | Tắt chế độ tự động đăng của bot; chỉ dùng script gom danh sách PR rồi Tech Lead đọc duyệt và sửa lại 3–4 gạch đầu dòng trước khi gửi. |
| **Mất bao lâu, tần suất** | Giảm từ 45 phút xuống **15 phút/lần**, loại bỏ hoàn toàn sự cố hiểu nhầm tiến độ. |
| **Insight rút ra** | Củng cố ranh giới **Boundary & HITL**: Không bao giờ để AI tự gửi báo cáo (Automate) hoặc tự suy diễn trạng thái "Đã hoàn thành" chỉ từ commit message; con người bắt buộc phải kiểm duyệt bản nháp trước khi gửi. |

---

## 3. Kết quả Khảo sát nhanh (Micro-survey 8 học viên các bàn khác)

| Câu hỏi khảo sát | Kết quả (n = 8) | Ghi chú chi tiết |
| --- | --- | --- |
| **1. Khi tổng hợp tiến độ nhóm, bạn phải mở mấy công cụ?** | - **3–4 công cụ:** 6/8 người (75%)<br>- **1–2 công cụ:** 2/8 người (25%) | Phổ biến nhất là bộ ba: GitHub + Google Sheets/Notion + Zalo/Discord. |
| **2. Tổng thời gian mỗi lần làm báo cáo tiến độ tuần / đồng bộ lớn?** | - **45–75 phút:** 5/8 người (62,5%)<br>- **25–45 phút:** 1/8 người (12,5%)<br>- **Dưới 20 phút:** 2/8 người (25%) | 2 người mất dưới 20 phút đều thuộc nhóm chỉ có 2–3 thành viên làm chung 1 bài nhỏ. |
| **3. Bước nào làm bạn tốn thời gian nhất?** | - **Đọc lại chat/commit tìm lý do nghẽn & viết nhận định:** 6/8 người (75%)<br>- **Đếm và cập nhật trạng thái thẻ việc:** 1/8 người (12,5%)<br>- **Format văn bản:** 1/8 người (12,5%) | Khớp với giả định Bottleneck nằm ở Bước 3 và Bước 5. |
| **4. Bạn đã từng gặp lỗi bỏ sót blocker của thành viên hoặc gửi trễ báo cáo chưa?** | - **Đã từng (ít nhất 1–2 lần/tháng):** 6/8 người (75%)<br>- **Chưa từng:** 2/8 người (25%) | Nguyên nhân chính là tin nhắn báo lỗi bị trôi trong nhóm chat Zalo. |

