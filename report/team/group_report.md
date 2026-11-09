# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: hihihaha
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): #12 — Khi lập báo cáo tuần, kỹ sư sản phẩm tại nhà máy sản xuất mạch điện tử mất khoảng 70 phút mỗi tuần để tra số lượng sản xuất và đưa số liệu vào đúng mục trong biểu mẫu.
- Quyết định cuối: **Go — pilot nhỏ với mức Rule (Power Query + biểu mẫu Excel), không dùng AI.**

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

Bảng ghi các câu hỏi phản biện nhóm đã đặt trong lượt pitch, tập trung vào hành vi đã xảy ra và số liệu của từng card. Mỗi thành viên có ít nhất một câu hỏi.

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyen Tien Dat | Import Excel sổ quỹ: Khi làm task import Excel cho sổ quỹ tiền mặt, tôi muốn xác định đúng dữ liệu và cột ngay từ đầu, để không phải sửa lại file sau khi test | Thực tập sinh dev (MobifoneIT), mentor, BA | Map cột Excel (~40 phút/lần) | **Nguyễn Bá Thành:** Trong lần gần nhất, điều gì khiến bạn mất nhiều thời gian nhất khi map cột Excel? |
| 2 | Nguyen Tien Dat | Vẽ diagram đồ án: Khi vẽ diagram cho bài tập/đồ án, tôi muốn ra đúng cấu trúc ngay bản đầu, để không phải sửa nhiều vòng theo feedback | Sinh viên năm cuối, bạn cùng nhóm | Sửa diagram theo feedback (~20–25 phút/lần, 2 vòng) | **Phí Hoàng Nam:** Trong lần sửa diagram gần nhất, feedback nào khiến bạn phải sửa nhiều vòng nhất, và mỗi vòng mất bao lâu? |
| 3 | Nguyen Tien Dat | Đọc hiểu task Jira: Khi nhận task mới trên Jira, tôi muốn hiểu đúng yêu cầu và tài liệu liên quan trong một lần đọc, để không làm sai hướng rồi phải hỏi lại mentor | Thực tập sinh dev, mentor, BA | Đọc tài liệu nội bộ + đối chiếu (~35 phút/lần) | **Phí Hoàng Nam:** Trong lần gần nhất, phần lớn 35 phút mất ở bước tìm tài liệu hay ở bước đối chiếu yêu cầu trên Jira? |
| 4 | Phí Hoàng Nam | Tổng hợp đầu việc lab. Khi nhận bài lab, tôi muốn xác định các đầu việc, thứ tự thực hiện và yêu cầu nộp để bắt đầu làm mà không bỏ sót phần bắt buộc. | Học viên làm bài lab | Đọc checkpoint và tổng hợp yêu cầu từ nhiều tệp Markdown (ước tính 15 phút, cần đo lại). | **Nguyễn Văn Huy:** Trong 30 phút chuẩn bị bài Day 1, riêng việc đọc và tổng hợp yêu cầu mất bao lâu nếu tách thời gian tìm hiểu Colab? |
| 5 | Phí Hoàng Nam | Tìm link Phoenix. Khi chuẩn bị gửi stand-up buổi sáng, tôi muốn tìm được link Phoenix để gửi bài trước 10 giờ và nhận XP. | Học viên cần gửi stand-up | Tìm lại tin nhắn chứa link Phoenix (khoảng 2 phút ở lần gần nhất). | **Nguyễn Bá Thành:** Lần gần nhất tìm link Phoenix, bạn đã tìm ở đâu và mất khoảng bao lâu? |
| 6 | Phí Hoàng Nam | Theo dõi thông báo trên Outlook và Discord. Khi kiểm tra thông báo của chương trình, tôi muốn nhận ra những thông tin có việc cần làm để không bỏ lỡ yêu cầu hoặc thời hạn. | Học viên theo dõi thông báo của chương trình | Xác định thông báo nào có việc cần làm (ước tính 7 phút, cần kiểm tra xem có phải bước dẫn đến bỏ sót hay không). | **Nguyễn Tiến Đạt:** Lần gần nhất bỏ lỡ 2 workshop, bạn đã đọc thông báo trên kênh nào và bỏ sót ở bước nào? |
| 7 | Nguyễn Bá Thành | Sau họp nhóm, tôi muốn rõ việc, người phụ trách và hạn để không phải hỏi lại. | Thành viên nhóm; nhóm trưởng | Hỏi lại thông tin sau họp: 5 lần từ 3 thành viên; chưa rõ thuộc bao nhiêu buổi. | **Nguyễn Tiến Đạt:** Năm lượt hỏi lại xảy ra trong bao nhiêu buổi họp, và mọi người thường phải hỏi lại thông tin gì? |
| 8 | Nguyễn Bá Thành | Sau mỗi buổi LEC, tôi muốn tìm đủ link học tập để tiếp tục làm bài. | Học viên | Tìm lại link bài giảng, GitHub và nộp bài: khoảng 10 phút/buổi. | **Nguyễn Văn Huy:** Trong 10 phút mỗi buổi, thời gian tìm link bài giảng, GitHub và nộp bài chia ra bao nhiêu? |
| 9 | Nguyễn Bá Thành | Đầu ngày, tôi muốn nắm lịch và việc cần làm để chủ động sắp xếp. | Học viên; thành viên nhóm | Tổng hợp lịch học, việc nhóm, workshop/Office Hours: khoảng 10 phút/ngày. | **Phí Hoàng Nam:** 10 phút tổng hợp lịch mỗi ngày chủ yếu mất ở việc tìm thông tin hay sắp xếp thứ tự? |
| 10 | Nguyễn Văn Huy | Khi chuẩn bị weekly report, tôi muốn xác định 3 mã lỗi test xuất hiện nhiều nhất trong tuần, để tập trung báo cáo các lỗi chính | PE tại nhà máy sản xuất mạch điện tử | Tải file Excel từ phần mềm test và lọc, xếp hạng mã lỗi mất khoảng 60 phút mỗi tuần | **Nguyễn Bá Thành:** Trong 60 phút lọc và xếp hạng mã lỗi, bước nào mất nhiều thời gian nhất? |
| 11 | Nguyễn Văn Huy | Khi viết weekly report, tôi muốn xác định action phù hợp cho từng mã lỗi cũ và mới theo từng sản phẩm, để báo cáo có hướng xử lý rõ ràng | PE tại nhà máy sản xuất mạch điện tử | Viết action cho lỗi cũ mất khoảng 20 phút và lỗi mới khoảng 30 phút mỗi tuần | **Nguyễn Tiến Đạt:** Với lỗi cũ và lỗi mới, bạn dựa vào đâu để chọn action, và lần gần nhất phải sửa action mất bao lâu? |
| 12 | Nguyễn Văn Huy | Khi tổng hợp weekly report, tôi muốn tra cứu số lượng sản xuất của tuần trước và đưa dữ liệu vào đúng mục, để báo cáo đầy đủ và hạn chế nhập sai | PE tại nhà máy sản xuất mạch điện tử | Tra số lượng mất khoảng 20 phút và copy-paste dữ liệu vào form báo cáo mất khoảng 50 phút mỗi tuần | **Nguyễn Bá Thành:** Trong lần lập báo cáo tuần gần nhất, phần nào tốn thời gian nhất trong 50 phút điền form: tìm đúng mục, chép số liệu hay kiểm tra lại? |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Xử lý dữ liệu và hoàn thiện báo cáo | #1, #10, #11, #12 | Mất thời gian đối chiếu cột dữ liệu, lọc mã lỗi, xác định hướng xử lý hoặc điền số liệu vào đúng mục báo cáo. |
| B — Làm rõ yêu cầu và đầu việc | #2, #3, #4, #7 | Phải đọc lại tài liệu, hỏi thêm hoặc sửa qua nhiều vòng để hiểu yêu cầu, việc cần làm và ai phụ trách. |
| C — Tìm và theo dõi thông tin | #5, #6, #8, #9 | Link, lịch và thông báo nằm ở nhiều nơi, khiến người dùng mất thời gian tìm lại hoặc dễ bỏ sót việc cần làm. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME — Giảm số phút tìm, hiểu và tổng hợp thông tin cho mỗi đầu việc
├── Opportunity A — Mất thời gian đối chiếu, lọc và điền số liệu vào đúng chỗ
├── Opportunity B — Phải hỏi lại hoặc sửa nhiều vòng vì yêu cầu và trách nhiệm chưa rõ
└── Opportunity C — Mất thời gian tìm lại link, lịch và thông báo nằm rải rác
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- Form Excel dùng công thức tra cứu để tự điền số liệu (#12) là một phương án giải quyết. Vấn đề ở nhánh A là thời gian Huy mất để tra và điền số liệu.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #12 — Tra số liệu và điền báo cáo tuần (Huy) | 5 | 5 | 3 | 5 | 4 | 4 | 3 | **29** |
| #7 — Làm rõ đầu việc sau họp nhóm (Thành) | 5 | 3 | 3 | 3 | 4 | 4 | 5 | **27** |
| #8 — Tìm lại link sau buổi học (Thành) | 5 | 4 | 3 | 4 | 5 | 2 | 5 | **28** |

Mức điểm phản ánh dữ kiện hiện có. #12 có thể đo riêng thời gian tra số lượng và điền biểu mẫu. Nhóm quen bối cảnh của #7 và #8 hơn, còn số liệu hiện có của cả ba đề tài cần được kiểm chứng.

**Candidate được chọn** — #12 của Nguyễn Văn Huy, đạt 29/35 điểm.

**Vì sao chọn** — Công việc lặp lại hằng tuần và có số liệu ban đầu
cho hai bước cụ thể: khoảng 20 phút tra số lượng sản xuất và 50 phút
điền form. Nhóm có thể kiểm chứng thời gian từng bước ở CP4.

**Vì sao loại #7** — Có 5 lượt hỏi lại từ 3 thành viên, nhưng chưa rõ
xảy ra trong bao nhiêu buổi họp và làm mất thêm bao nhiêu thời gian.

**Vì sao loại #8** — Ước tính 10 phút mỗi buổi đang gộp việc tìm link
bài giảng, GitHub và nơi nộp bài. Chưa rõ bước nào chiếm nhiều thời
gian nhất để khoanh phạm vi kiểm chứng.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | PE khác trong nhà máy (không chỉ Huy) cũng mất ≥60 phút/tuần cho báo cáo tuần | Value | 5 | 2 | ✅ |
| 2 | Bước tốn thời gian nhất là chép số liệu vào form (50 phút), không phải tra số lượng (20 phút) | Value | 5 | 2 | ✅ |
| 3 | File số lượng xuất ra từ phần mềm test có cấu trúc cột ổn định giữa các tuần | Feasibility | 4 | 3 | ✅ (kiểm tra file thật của Huy) |
| 4 | Biểu mẫu báo cáo tuần dùng ô/mục cố định, map được từ cột dữ liệu | Feasibility | 4 | 3 | ✅ |
| 5 | Nhà máy cho phép chạy công cụ ngoài (Power Query/Python) trên máy và dùng dữ liệu nội bộ | Viability | 5 | 1 | Hỏi sau (quy định IT) |
| 6 | PE muốn tự kiểm số liệu trước khi nộp nên cần hỗ trợ (augment) hơn là giao hẳn (automate) | Usability | 4 | 2 | ✅ |

Giả định nhóm kiểm chứng trong buổi này: **#1, #2, #6** — đều nằm ở ô "quan trọng nhưng ít bằng chứng".

### 3.2. Kiểm chứng

Cách đã dùng: **Survey 5–10 người** (đồng nghiệp PE/QA cùng nhà máy và bạn học có lập báo cáo định kỳ).

Bộ câu hỏi survey — hỏi **hành vi đã xảy ra**, không hỏi giả định, không có câu dạng "Bạn có muốn…":

1. Công việc của bạn có phải lập báo cáo định kỳ (tuần/tháng) không? (Có / Không)
2. Lần gần nhất lập báo cáo tuần, bạn mất tổng bao nhiêu phút?
3. Trong đó bước nào tốn thời gian nhất? (tra/tìm số liệu · chép số liệu vào form · viết nhận xét/action · kiểm tra lại · khác)
4. Số liệu sản xuất bạn lấy từ đâu? (phần mềm test xuất Excel · MES/hệ thống · hỏi bộ phận khác · khác)
5. Bạn điền form bằng cách nào? (copy-paste tay · công thức Excel · macro · công cụ khác)
6. Bạn lập báo cáo bao nhiêu lần mỗi tuần/tháng?
7. Trong 4 tuần gần nhất, có tuần nào bạn nhập sai số hoặc nộp trễ không? Chuyện gì đã xảy ra?
8. Bạn từng dùng công cụ nào (Power Query, macro, phần mềm SPC/MES…) để giảm thời gian chưa? Kết quả ra sao?

Kết quả survey (hiện có **5 phản hồi** — đã đạt mốc tối thiểu 5; có thể thêm tới 10, hoặc 20 để đủ điều kiện bonus B2):

Phản hồi #1 — vai trò: người lập báo cáo định kỳ (không ghi tên thật):

| Câu hỏi | Trả lời |
|---|---|
| 1. Có lập báo cáo định kỳ? | Có |
| 2. Lần gần nhất mất bao lâu? | 170 phút |
| 3. Bước tốn thời gian nhất? | Chép số liệu vào form |
| 4. Số liệu lấy từ đâu? | Hệ thống test |
| 5. Điền form bằng cách nào? | Excel |
| 6. Tần suất lập báo cáo? | 4 lần/tháng |
| 7. 4 tuần gần nhất có sai/trễ không? | 1 lần nhập sai, 0 lần trễ |
| 8. Đã dùng công cụ nào để giảm thời gian? | Chưa dùng |

Phản hồi #2 — vai trò: người lập báo cáo định kỳ (không ghi tên thật):

| Câu hỏi | Trả lời |
|---|---|
| 1. Có lập báo cáo định kỳ? | Có |
| 2. Lần gần nhất mất bao lâu? | 200 phút |
| 3. Bước tốn thời gian nhất? | Chép số liệu vào form · viết nhận xét/action |
| 4. Số liệu lấy từ đâu? | Hệ thống test |
| 5. Điền form bằng cách nào? | Excel |
| 6. Tần suất lập báo cáo? | 4 lần/tháng |
| 7. 4 tuần gần nhất có sai/trễ không? | 1 lần sai, 0 lần trễ |
| 8. Đã dùng công cụ nào để giảm thời gian? | Chưa dùng |

Phản hồi #3 — vai trò: người lập báo cáo định kỳ (không ghi tên thật):

| Câu hỏi | Trả lời |
|---|---|
| 1. Có lập báo cáo định kỳ? | Có |
| 2. Lần gần nhất mất bao lâu? | 210 phút |
| 3. Bước tốn thời gian nhất? | Chép số liệu vào form · viết nhận xét/action |
| 4. Số liệu lấy từ đâu? | (không trả lời) |
| 5. Điền form bằng cách nào? | Excel |
| 6. Tần suất lập báo cáo? | 4 lần/tháng |
| 7. 4 tuần gần nhất có sai/trễ không? | 1 lần sai, 0 lần trễ |
| 8. Đã dùng công cụ nào để giảm thời gian? | Chưa dùng |

Phản hồi #4 — vai trò: người lập báo cáo định kỳ (không ghi tên thật):

| Câu hỏi | Trả lời |
|---|---|
| 1. Có lập báo cáo định kỳ? | Có |
| 2. Lần gần nhất mất bao lâu? | 170 phút |
| 3. Bước tốn thời gian nhất? | Chép số liệu vào form · viết nhận xét/action |
| 4. Số liệu lấy từ đâu? | (không trả lời) |
| 5. Điền form bằng cách nào? | Excel |
| 6. Tần suất lập báo cáo? | 4 lần/tháng |
| 7. 4 tuần gần nhất có sai/trễ không? | 0 lần sai, 0 lần trễ |
| 8. Đã dùng công cụ nào để giảm thời gian? | Chưa dùng |

Phản hồi #5 — vai trò: người lập báo cáo định kỳ (không ghi tên thật):

| Câu hỏi | Trả lời |
|---|---|
| 1. Có lập báo cáo định kỳ? | Có |
| 2. Lần gần nhất mất bao lâu? | 140 phút |
| 3. Bước tốn thời gian nhất? | Chép số liệu vào form · viết nhận xét/action |
| 4. Số liệu lấy từ đâu? | (không trả lời) |
| 5. Điền form bằng cách nào? | Excel |
| 6. Tần suất lập báo cáo? | 4 lần/tháng |
| 7. 4 tuần gần nhất có sai/trễ không? | 1 lần sai, 0 lần trễ |
| 8. Đã dùng công cụ nào để giảm thời gian? | Chưa dùng |

*Nếu bổ sung phỏng vấn, mỗi buổi ghi một Interview Snapshot theo bảng dưới (hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):*

Interview Snapshot #1:

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | QA |
| Câu nói đáng nhớ nhất (nguyên văn) | "Mất thời gian khi phải tổng hợp những thông tin có sẵn." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Bị sai thông số nên số liệu không khớp |
| Hiện đang xử lý bằng cách nào (workaround)? | Phải rà soát lại số liệu |
| Mất bao lâu, bao lần? | Khoảng 60 phút để kiểm tra |
| Insight / opportunity rút ra | Pain nằm ở bước tổng hợp/đối chiếu thông tin có sẵn và rà soát lại khi số liệu lệch. Người được hỏi tự đề xuất "AI agent quản lý dữ liệu" — đây là **solution**, không đưa vào tầng opportunity. |

Interview Snapshot #2:

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | PM (Project Manager) |
| Câu nói đáng nhớ nhất (nguyên văn) | "Bị khách hàng phàn nàn về sai số liệu." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Cách đây 3 tuần |
| Hiện đang xử lý bằng cách nào (workaround)? | Xin lỗi khách hàng, rà soát lại dữ liệu |
| Mất bao lâu, bao lần? | Khoảng 3 tháng sai 1 lần |
| Insight / opportunity rút ra | Sai số liệu không chỉ tốn thời gian nội bộ mà còn ảnh hưởng bên ngoài (khách hàng phàn nàn). Người được hỏi tự đề xuất "cần một tool quản lý dữ liệu" — đây là **solution**, không đưa vào tầng opportunity. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Survey (đồng nghiệp PE/QA) | 5 | 5/5 nói bước tốn thời gian nhất là chép số liệu vào form (4 người thêm "viết nhận xét/action"); 5/5 điền form thủ công bằng Excel; 5/5 chưa dùng công cụ hỗ trợ; 4/5 từng nhập sai số (1 lần/4 tuần), 0/5 trễ hạn; thời gian 170, 200, 210, 170 và 140 phút (trung vị 170) | **Tín hiệu phản bác nhỏ:** 1/5 nói 0 lần sai trong 4 tuần; 1/5 chỉ mất 140 phút; 3/5 không nêu nguồn số liệu. Cả năm đều cao hơn baseline 70 phút của #12 → baseline 70 phút chỉ là phần tra + điền, không phải toàn báo cáo |
| Phỏng vấn | 2 | QA: mất ~60 phút rà soát lại vì sai thông số làm số liệu không khớp, nói mất thời gian khi tổng hợp thông tin đã có sẵn. PM: bị khách hàng phàn nàn về sai số liệu (cách đây 3 tuần), phải xin lỗi khách hàng và rà soát lại dữ liệu; tần suất sai ~3 tháng/lần | Chưa có phản bác |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** 5 survey + 2 phỏng vấn đều xác nhận pain nằm ở bước tổng hợp/đối chiếu số liệu (chép vào form, rà soát lại khi lệch). Phỏng vấn PM mở rộng hệ quả ra bên ngoài: sai số liệu từng khiến khách hàng phàn nàn. Nhóm đã sửa ba điểm: (1) tách baseline **70 phút** cho phần tra + điền (ước tính của Huy) khỏi baseline **170 phút** cho toàn báo cáo (trung vị 5 survey); (2) thêm tiêu chí **0 lỗi số liệu sau khi nộp trong 4 tuần** thay vì chỉ đo thời gian; (3) giữ phạm vi giải pháp ở mức **Rule**, vì 4/5 survey vẫn dùng Excel thủ công và bước tốn thời gian nhất là thao tác cơ học. Tín hiệu phản bác nhỏ (1/5 không sai lần nào, 1/5 chỉ 140 phút) được ghi nhận nhưng không đủ để đổi hướng.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Excel Power Query — connector Folder (gộp nhiều file tự động) | https://learn.microsoft.com/en-us/power-query/connectors/folder | Bước tra/gom số lượng sản xuất (~20 phút): tự đọc mọi file cùng cấu trúc trong một thư mục, Refresh khi có file mới | Có sẵn trong Excel; "Combine & Load/Transform" gộp file không cần code | File nguồn phải cùng định dạng/cấu trúc (sheet/table, header); phần mềm test đổi layout là query lỗi; không tự quyết số liệu thuộc mục nào của form | Dùng tốt cho bước gom số liệu nếu file export ổn định; vẫn cần rule map sang đúng mục + người kiểm |
| xlwings Reports (template → Excel/PDF) | https://docs.xlwings.org/en/0.24.4/reports.html | Bước điền form báo cáo (~50 phút): ghi DataFrame vào ô/bảng template có sẵn, xuất Excel/PDF | Tách code xử lý và template; người dùng tự sửa layout; hỗ trợ bảng, chart, ảnh, PDF | Tính năng Reports cần xlwings **PRO** (trả phí); cần Python + setup; có thể bị chặn script trên máy văn phòng | Pattern "template + engine điền" đúng hướng, nhưng phải kiểm chi phí/quy định IT; có thể thay bằng Excel-native (Power Query + công thức) |
| InfinityQS ProFicient (SPC real-time) | https://help.infinityqs.com/help/en/ProFicient/ | Thu thập dữ liệu chất lượng tự động + kho dữ liệu tập trung: thay việc lọc/xếp hạng mã lỗi thủ công (#10) và nhập tay | Kết nối nhiều nguồn nhà máy (OPC, file phẳng, DB…), thu thập tự động, báo cáo/dashboard real-time | Giải pháp cấp nhà máy, chi phí & triển khai lớn; cần tích hợp MES/ERP; quá tầm cho báo cáo tuần của một PE | Thế giới đã có giải pháp mạnh nhưng đắt; phạm vi lab nên chọn mức nhẹ (Rule/Power Query) thay vì mua SPC |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Tần suất: mỗi tuần, khi PE lập báo cáo tuần. 

```text
[PE] Tra số lượng sản xuất tuần trước từ dữ liệu nguồn (20')
  Input: dữ liệu sản xuất của tuần trước
  Output: số lượng cần đưa vào báo cáo
  → [PE] Mở biểu mẫu báo cáo và copy-paste số liệu vào đúng mục (50')
      Input: số lượng đã tra + biểu mẫu báo cáo tuần
      Output: biểu mẫu có số liệu sản xuất
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Handoff |
|---:|---|---|---|---|---|
| 1. Tra số lượng sản xuất tuần trước | PE | Dữ liệu sản xuất của tuần trước | Số lượng sản xuất cần báo cáo | Khoảng 20 phút / tuần (ước tính Huy, CP3) | PE chuyển số liệu sang bước điền biểu mẫu |
| 2. Điền số liệu vào đúng mục | PE | Số lượng đã tra và biểu mẫu báo cáo tuần | Biểu mẫu có số liệu sản xuất | Khoảng 50 phút / tuần (ước tính Huy, CP3) | PE hoàn thiện biểu mẫu để tiếp tục quy trình báo cáo hiện có |

**Bottleneck chính:** Bước 2 — copy-paste số liệu vào đúng mục của biểu mẫu, khoảng 50 phút mỗi tuần theo ước tính của Huy. Chưa có log bấm giờ hoặc dữ liệu kiểm chứng độc lập; cần xác nhận trong pilot.

### 4.2. Quy trình tương lai

Đề xuất thử trước bằng quy tắc/Excel (Power Query và biểu mẫu), không cần AI để tra hay tính số liệu. Thời gian từng bước là mục tiêu giả thuyết để kiểm tra, không phải kết quả đã đo.

```text
[PE] Đưa file nguồn đúng kỳ vào thư mục đã thống nhất (3')       ← CON NGƯỜI
  → [Power Query / rule] Refresh và gom số lượng (5')            ← RULE
  → [Rule / biểu mẫu] Ánh xạ số lượng vào các mục báo cáo (5')    ← RULE
  → [PE] Đối chiếu số trong biểu mẫu với nguồn và sửa nếu cần (12') ← CON NGƯỜI / HITL
  → [PE] Hoàn tất và gửi theo quy trình hiện tại (5')              ← CON NGƯỜI

BOUNDARY: Rule chỉ đọc file nguồn đã chọn và điền theo mapping đã xác nhận;
không tự suy đoán số thiếu, không ghi đè dữ liệu nguồn, không tự gửi báo cáo.
Nếu sau này thêm AI, AI không được tự tạo/sửa số liệu hay tự gửi; PE phải đối chiếu
mọi số liệu với nguồn trước khi đầu ra được dùng.
PHƯƠNG ÁN QUAY VỀ: Nếu file đổi cấu trúc, mapping sai hoặc kết quả không khớp,
dừng dùng kết quả tự động; PE tra và điền thủ công theo quy trình hiện tại,
đồng thời ghi nhận lỗi để sửa mapping trước lần chạy sau.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 2 | 5 | Tương lai tách riêng nạp file, gom số, ánh xạ, kiểm tra và gửi |
| Tổng thời gian | Khoảng 70 phút / tuần | Mục tiêu khoảng 30 phút / tuần | Baseline = 20' + 50' theo ước tính ở CP3; thời gian tương lai là giả thuyết cần pilot |
| Số bước thủ công | 2/2 | 3/5 | PE nạp file, kiểm tra kết quả và gửi; 2 bước xử lý bằng rule |
| Bottleneck chính | Điền biểu mẫu (khoảng 50') | Đối chiếu số liệu (mục tiêu 12') | Dành thời gian cho kiểm soát chất lượng; phải đo lại khi pilot |
| Rủi ro mới phát sinh | — | File đổi cấu trúc hoặc mapping sai làm điền nhầm mục/số | Đối chiếu với file nguồn; dừng và quay về quy trình thủ công nếu không khớp |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | PE tại nhà máy sản xuất mạch điện tử, phụ trách tổng hợp số lượng sản xuất vào báo cáo tuần. |
| **Quy trình** | Mỗi tuần, PE tra số lượng sản xuất của tuần trước từ dữ liệu nguồn rồi điền số liệu vào đúng mục trong biểu mẫu báo cáo. |
| **Bottleneck** | Điền/copy-paste số liệu vào đúng mục của biểu mẫu, ước tính khoảng 50 phút mỗi tuần theo thông tin Huy nêu ở CP3 và là bước tốn thời gian nhất theo 5/5 survey; bước tra số lượng khoảng 20 phút. Toàn bộ báo cáo tuần có trung vị 170 phút (5 survey). Chưa được bấm giờ độc lập. |
| **Impact** | Quy trình tra và điền số liệu chiếm khoảng 70 phút mỗi tuần theo ước tính ban đầu (20 phút tra + 50 phút điền); toàn bộ báo cáo tuần có trung vị 170 phút (5 survey). CP4 xác nhận 4/5 người từng nhập sai ít nhất 1 lần trong 4 tuần, 0/5 trễ hạn; PM bị khách hàng phàn nàn về sai số cách đây 3 tuần; QA mất khoảng 60 phút rà soát lại khi số liệu lệch. |
| **Success Metric** (baseline → target, cách đo) | **Baseline:** 70 phút/tuần cho phần tra + điền (ước tính CP3, sẽ đo lại) và 170 phút/tuần cho toàn báo cáo (trung vị 5 survey). **Target:** không quá 30 phút/tuần cho phần tra + điền; chưa đặt target riêng cho toàn báo cáo. Trong 4 tuần lập báo cáo, PE bấm giờ từ lúc bắt đầu tra dữ liệu đến khi hoàn tất phần số liệu; ghi riêng thời gian từng bước, số lần sửa và số mục sai/thiếu khi đối chiếu với nguồn. Chỉ đạt mục tiêu nếu giảm thời gian mà không tăng lỗi; xác nhận baseline bằng lần đo đầu tiên. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | CP5 chưa đề xuất dùng AI để xử lý số liệu. Rule chỉ gom và ánh xạ dữ liệu theo nguồn/mapping đã xác nhận; không suy đoán hoặc sửa số liệu nguồn, không tự gửi báo cáo. PE phải đối chiếu số và mục trong biểu mẫu với nguồn trước khi hoàn tất. Nếu sau này dùng AI, AI không được tự tạo/sửa số liệu hay tự gửi; đầu ra phải được PE kiểm tra. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- Phản biện: Baseline khoảng 70 phút hiện là ước tính tự báo cáo, chưa phải số đo; target thời gian đơn lẻ có thể khuyến khích điền nhanh nhưng kém chính xác. Cần đo baseline bằng bấm giờ và theo dõi lỗi/sửa trong pilot.
- Trạng thái: Nhóm đã cập nhật Impact và Success Metric v0 theo CP4 (5 survey + 2 phỏng vấn): tách baseline 70 phút cho phần tra + điền và 170 phút cho toàn báo cáo, đồng thời bổ sung số liệu lỗi. Cần xác nhận lại bằng bấm giờ trong pilot. Chưa ghi nhận phản biện từ nhóm khác.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **độ mơ hồ thấp – độ phức tạp trung bình**.

Vì sao:

- **Độ mơ hồ thấp:** actor, quy trình, input và output đã rõ. 5/5 người được survey xác nhận bước tốn thời gian nhất là chép số liệu vào form; dữ liệu là số lượng sản xuất xuất ra từ phần mềm test nên có cấu trúc cột.
- **Độ phức tạp trung bình:** mỗi tuần có thể có nhiều file nguồn, biểu mẫu có nhiều mục và cấu trúc file có thể thay đổi; nhưng việc ánh xạ số liệu là quy tắc xác định, không cần hiểu ngôn ngữ hay tự ra quyết định.
- **Kết luận:** bài toán phù hợp với **Rule** — tự động hóa các bước cơ học theo quy tắc đã xác nhận, con người vẫn kiểm tra.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Chuẩn hóa quy trình: đặt tên file theo kỳ, checklist mục báo cáo, khóa biểu mẫu và giao đúng người. | Lỗi do thiếu quy trình, không phải do thao tác lặp. | Vẫn mất khoảng 50 phút copy-paste mỗi tuần; không tác động vào bước tốn thời gian nhất. | Không (chỉ dùng như bổ trợ) |
| **Rule** | Power Query đọc/gộp file nguồn trong thư mục; công thức/template ánh xạ số lượng vào đúng mục; PE refresh và đối chiếu. | File nguồn có cấu trúc ổn định, mapping xác định và người dùng đang dùng Excel. | File đổi layout làm query lỗi; mapping sai làm điền nhầm mục; vẫn cần người kiểm tra. | **Có — mức chọn** |
| **Workflow** | AI đọc file/email, trích số và đề xuất điền vào form theo các bước định sẵn; PE duyệt từng kết quả. | Dữ liệu phi cấu trúc hoặc cần hiểu nội dung chữ để xác định mục báo cáo. | AI có thể tạo số không có trong nguồn, khó truy vết; cần bộ eval và kiểm tra từng ô. | Không — dữ liệu đã có cấu trúc |
| **Agent** | Agent tự tải file, tự quyết mục, tự điền và có thể tự gửi báo cáo. | Cần tự vận hành nhiều bước, có giám sát và audit đầy đủ. | Tự quyết hoặc tự gửi số sai; chi phí kiểm soát và trách nhiệm cao. | Không |

**Mức chọn:** **Rule** — Power Query + biểu mẫu Excel, không dùng AI.

**Vì sao không chọn mức đơn giản hơn:** No AI không xử lý được bước tốn thời gian nhất. 5/5 người được survey vẫn chép số liệu thủ công bằng Excel và 4/5 từng nhập sai; chỉ đổi quy trình thì vẫn giữ nguyên khoảng 50 phút copy-paste mỗi tuần. Rule tự động hóa đúng phần cơ học này mà không cần thêm công cụ mới.

**Vì sao không chọn mức cao hơn:** Workflow/Agent chỉ đáng dùng khi bước cần phán đoán nội dung hoặc tự quyết định bước tiếp theo. Ở bài này, số liệu có cấu trúc và mapping xác định; thêm AI làm tăng rủi ro tạo/sửa số không có trong nguồn, khó kiểm tra hơn so với Rule. Nếu sau pilot bước “viết nhận xét/action” (4/5 survey đề cập) vẫn là nút thắt, nhóm sẽ đánh giá riêng một Workflow cho bước đó, kèm eval và HITL — không mở rộng lên Agent.

### 6.3. AI Canvas rút gọn — áp dụng cho mức Rule (không có AI)

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | **Không có AI.** Rule gom số từ file nguồn và ánh xạ vào các mục theo bảng mapping đã xác nhận. |
| **Judgment** — con người cân nhắc, quyết định gì? | PE quyết định file nguồn đúng kỳ, kiểm tra số liệu có khớp nguồn không, quyết định sửa hay không sửa và nội dung nhận xét. |
| **Action** — hành động cuối cùng là gì, ai làm? | PE là người hoàn tất và gửi báo cáo; Rule chỉ tạo bản nháp số liệu. |
| **Outcome** — đo kết quả bằng gì? | Thời gian tra + điền ≤30 phút/tuần; 0 lỗi số liệu sau khi nộp; 0 lần phải làm lại toàn bộ. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | File export của phần mềm test theo tuần, biểu mẫu báo cáo và bảng mapping. Các file đã có trong quy trình hiện tại; cần xác nhận cấu trúc ổn định qua 4–8 tuần. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Log lỗi mapping/file, thời gian đo từng tuần và ý kiến PE sau mỗi kỳ báo cáo; dùng để sửa mapping trước kỳ sau. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: **Augment.** 5/5 người được survey vẫn điền form thủ công bằng Excel và 4/5 từng nhập sai; QA phải rà lại khoảng 60 phút khi số liệu lệch; PM từng phải xin lỗi khách vì sai số. PE cần giữ quyền quyết định số cuối cùng, nên Rule chỉ tạo bản nháp và PE đối chiếu trước khi gửi.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: **Báo nhầm tệ hơn.** Một số sai trông hợp lệ có thể lọt tới khách hàng (PM đã gặp), khó phát hiện hơn một ô trống. Thiết kế xử lý bằng bước PE đối chiếu 100% ô với nguồn, đánh dấu các ô thay đổi, so tổng và chặn gửi nếu chưa xác nhận; nếu mapping/file lỗi thì quay về quy trình thủ công.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | PE tại nhà máy sản xuất mạch điện tử, phụ trách tổng hợp số lượng sản xuất vào báo cáo tuần. |
| **Quy trình** | Hằng tuần, PE đưa file nguồn đúng kỳ vào thư mục đã thống nhất, refresh Power Query để gom số lượng, Rule ánh xạ số liệu vào các mục của biểu mẫu, PE đối chiếu với nguồn rồi hoàn tất và gửi theo quy trình hiện tại. |
| **Bottleneck** | Bước điền/copy-paste số liệu vào đúng mục của biểu mẫu, khoảng 50 phút/tuần theo ước tính của Huy và là bước tốn thời gian nhất theo 5/5 survey; bước tra số lượng khoảng 20 phút. Toàn bộ báo cáo tuần có trung vị 170 phút (5 survey). |
| **Impact** | 5/5 survey nói chép số liệu vào form là bước tốn thời gian nhất; 4/5 từng nhập sai ít nhất 1 lần trong 4 tuần; 0/5 trễ hạn. PM bị khách hàng phàn nàn về sai số cách đây 3 tuần; QA mất khoảng 60 phút rà soát lại khi số liệu lệch. |
| **Success Metric** (baseline → target, cách đo) | **Baseline:** 70 phút/tuần cho phần tra + điền số liệu (ước tính CP3, sẽ đo lại) và 170 phút/tuần cho toàn báo cáo (trung vị 5 survey). **Target:** ≤30 phút/tuần cho phần tra + điền; ≤130 phút/tuần cho toàn báo cáo; 0 lỗi số liệu được phát hiện sau khi nộp trong 4 tuần. **Cách đo:** PE bấm giờ từng bước trong 4 kỳ báo cáo, ghi log lỗi/mapping và đối chiếu 100% ô với file nguồn trước khi gửi; so sánh trung vị 4 tuần trước và sau pilot. |
| **Boundary** | Rule chỉ đọc file trong thư mục đã chọn và điền theo bảng mapping đã xác nhận; **không** tự suy đoán hoặc điền số thiếu, **không** sửa/ghi đè file nguồn, **không** đổi mục/công thức ngoài mapping, **không** tự gửi báo cáo. Vì mức chọn là Rule nên không có thành phần AI; nếu sau này thêm AI, AI **không được** tự tạo/sửa số liệu, tự chọn mục ngoài mapping hoặc tự gửi báo cáo. PE phải đối chiếu 100% số liệu với nguồn và xác nhận trước khi gửi. Nếu file đổi cấu trúc, mapping sai hoặc tổng không khớp: dừng và quay về quy trình thủ công. |
| **AI intervention point** | **Không có.** Bài toán là biến đổi số liệu có cấu trúc theo mapping xác định; dùng AI không giải thêm bước nào mà còn tạo rủi ro tạo/sửa số không có trong nguồn. Nhóm chỉ xem xét Workflow cho bước viết nhận xét/action nếu pilot cho thấy đây là nút thắt mới. |
| **Mức chọn** | **Rule** |
| **Rủi ro & người kiểm tra** | File đổi cấu trúc: PE phát hiện khi refresh và kiểm tra đầu vào. Mapping sai: PE đối chiếu với nguồn trước khi gửi. Quy định IT: IT/quản lý nhà máy xác nhận trước pilot. Số liệu cuối: PE chịu trách nhiệm xác nhận trước khi gửi. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| **Quy trình** | 2 bước: tra số (20') → copy-paste vào form (50'). | 5 bước: nạp file (3') → Power Query gom số (5') → Rule ánh xạ (5') → PE đối chiếu (12') → PE hoàn tất/gửi (5'). | Tách riêng bước kiểm tra và phương án quay về; thời gian tương lai là mục tiêu giả thuyết cần pilot. |
| **Success Metric** | Baseline 70 phút cho phần tra + điền và 170 phút cho toàn báo cáo; target 30 phút cho phần tra + điền; chưa có target cho toàn báo cáo và chưa có tiêu chí lỗi riêng. | Target 30 phút cho phần tra + điền và 130 phút cho toàn báo cáo; thêm 0 lỗi số liệu sau nộp trong 4 tuần. | Tách đúng phạm vi đo và thêm tiêu chí chất lượng để tránh tăng tốc nhưng tăng sai. |
| **Boundary** | Rule không suy đoán/sửa số, không tự gửi; PE kiểm tra. | Giữ nguyên, bổ sung: không đổi mục/công thức ngoài mapping; dừng và quay về thủ công khi file/mapping lỗi. | Chốt mức Rule và phương án quay về ở CP6. |
| **Mức chọn** | Chưa chốt mức can thiệp; v0 mới đề xuất Rule ở mục 4.2. | **Rule** — Power Query + biểu mẫu Excel, không dùng AI. | Chốt mức sau khi so sánh 4 mức ở CP6. |
| **AI intervention point** | Chưa có. | Không có; lý do: dữ liệu có cấu trúc, mapping xác định. | Chọn mức Rule, không cần AI. |
| **Rủi ro & người kiểm tra** | Chưa có. | 4 rủi ro và người kiểm tra: PE, IT/quản lý nhà máy. | Yêu cầu của CP6. |

**Tiêu chí đánh giá đầu ra của giải pháp Rule (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Đúng số liệu nguồn** | 100% ô số liệu khớp file nguồn sau đối chiếu; 0 sai lệch. | Có ≥1 ô lệch hoặc không đối chiếu được với nguồn. |
| 2 | **Đúng vị trí/mục** | 100% số liệu nằm đúng mục theo mapping; 0 ô điền nhầm. | Có ≥1 ô sai mục hoặc sai kỳ báo cáo. |
| 3 | **Thời gian** | Trung vị thời gian tra + điền ≤30 phút/tuần trong 4 tuần pilot. | Trung vị >30 phút/tuần, hoặc 2 tuần liên tiếp >40 phút. |
| 4 | **Không tăng lỗi** | 0 lỗi số liệu được phát hiện sau khi nộp trong 4 tuần pilot. | Có ≥1 lỗi số liệu lọt vào báo cáo đã gửi. |
| 5 | **Quay về an toàn** | 100% lần file đổi cấu trúc/mapping lỗi được phát hiện trước khi gửi và xử lý thủ công trong cùng ngày. | Có báo cáo nộp từ dữ liệu chưa đối chiếu, hoặc phải làm lại toàn bộ >1 tuần. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** | 5/5 survey xác nhận chép số liệu vào form là bước tốn thời gian nhất; 4/5 từng nhập sai trong 4 tuần; 2 phỏng vấn (QA, PM) xác nhận hệ quả; pain lặp lại hằng tuần. Mẫu còn nhỏ (5 survey + 2 phỏng vấn, chủ yếu cùng nhà máy) nên cần mở rộng khi pilot. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của giải pháp Rule không? | **Thấp** | 5/5 đã dùng Excel; Power Query có sẵn trong Excel; quy trình mới chỉ thêm thao tác refresh và đối chiếu; PE vẫn giữ quyền sửa. Cần training ngắn và bảng mapping rõ ràng. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Trung bình** | File export có cấu trúc nhưng mới kiểm tra trên file thật của Huy (giả định #3 mới có 3/5 bằng chứng); mapping chưa được xây; chưa test qua nhiều tuần; Power Query phụ thuộc layout file nguồn. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Trung bình** | Chi phí thấp vì dùng Excel sẵn có, không mua giải pháp SPC; nhưng chưa xác nhận quy định IT cho Power Query/macro (giả định #5 mới có 1/5 bằng chứng). Cần một người duy trì mapping (PE/Huy) và thời gian kiểm tra mỗi tuần. |

### 8.2. Kết luận

**Quyết định:** **Go — pilot nhỏ với mức Rule (Power Query + biểu mẫu Excel), không dùng AI.**

**Lý do:** Value và Usability có rủi ro thấp; Feasibility và Viability ở mức trung bình nhưng có thể kiểm chứng trong 4 tuần với chi phí thấp và phương án quay về rõ. Pain đã được xác nhận bằng 5 survey + 2 phỏng vấn; bước tốn thời gian nhất là thao tác cơ học nên Rule phù hợp hơn AI. Không chọn Not Yet vì đã đủ bằng chứng để thử; không chọn No-Go vì No AI không xử lý được bước copy-paste.

**Nếu Go — pilot nhỏ nhất:** 1 PE (Huy), 1 dòng sản phẩm, 4 kỳ báo cáo tuần. Dùng Power Query đọc file nguồn và template Excel; chạy song song quy trình hiện tại: bản tự động chỉ là bản nháp, PE đối chiếu 100% và vẫn dùng file hiện tại để gửi. Trước pilot: xác nhận quy định IT, kiểm tra cấu trúc file 4–8 tuần và xây bảng mapping. Trong pilot: bấm giờ từng bước, ghi log lỗi/mapping và số lần phải quay về thủ công.

**Nếu Not Yet — cần kiểm chứng gì trước:** xác nhận quy định IT cho Power Query/macro; đo baseline 4 tuần bằng bấm giờ; kiểm tra cấu trúc file nguồn qua 4–8 tuần và xây mapping trước khi chạy.

**Nếu No-Go — nên làm gì thay AI:** giữ quy trình thủ công có checklist và biểu mẫu Excel chuẩn hóa; chỉ chuẩn hóa tên file, mục báo cáo và người kiểm tra, không tự động hóa.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …): Sau 4 tuần pilot, nếu trung vị thời gian tra + điền >50 phút/tuần, hoặc có ≥1 lỗi số liệu lọt vào báo cáo đã gửi, hoặc phải quay về thủ công >2/4 tuần do file/mapping lỗi → dừng, quay về quy trình thủ công. Chỉ xem lại khi cấu trúc file ổn định và mapping đã được sửa.

---

## 9. Hạn chế và hướng tiếp theo

- Mẫu survey gồm 5 người và 2 phỏng vấn, chủ yếu là đồng nghiệp cùng nhà máy; thời gian là tự báo cáo, chưa được bấm giờ độc lập.
- Baseline đang có hai phạm vi: 70 phút cho phần tra + điền (ước tính) và 170 phút cho toàn báo cáo (trung vị survey). Pilot phải đo cùng một phạm vi để so sánh.
- Chưa xác nhận quy định IT cho Power Query/macro; chưa xây bảng mapping; chưa chạy thử trên file thật qua nhiều tuần.
- Chưa có dữ liệu pilot; các target 30/130 phút và 0 lỗi là giả thuyết cần kiểm chứng.
- Bước viết nhận xét/action được 4/5 survey nhắc đến nhưng nằm ngoài phạm vi Rule hiện tại. Nếu sau pilot đây là nút thắt mới, nhóm sẽ đánh giá riêng một Workflow cho bước đó.

Hướng tiếp theo:

- Chạy pilot 4 tuần với 1 PE và 1 dòng sản phẩm; đo thời gian từng bước và ghi log lỗi.
- Mở rộng survey lên 10–20 người hoặc thêm 3 phỏng vấn PE để tăng độ tin cậy (bonus B2 cần ≥20 survey hoặc ≥5 phỏng vấn).
- Kiểm tra cấu trúc file nguồn qua 4–8 tuần và xây bảng mapping.
- Xác nhận quy định IT và người duy trì mapping.
- Sau pilot, quyết định giữ Rule, mở rộng phạm vi, hay thử Workflow cho riêng bước viết nhận xét/action.

## 10. Tài liệu tham khảo

- Microsoft Learn — Excel Power Query, connector Folder: https://learn.microsoft.com/en-us/power-query/connectors/folder
- xlwings — Reports (template → Excel/PDF): https://docs.xlwings.org/en/0.24.4/reports.html
- InfinityQS — ProFicient (SPC real-time): https://help.infinityqs.com/help/en/ProFicient/
- Google PAIR — People + AI Guidebook: https://pair.withgoogle.com/guidebook/
- Rob Fitzpatrick — *The Mom Test* (nguyên tắc hỏi về hành vi đã xảy ra).
- Anthropic — *Building effective agents* (phân biệt workflow và agent): https://www.anthropic.com/research/building-effective-agents
