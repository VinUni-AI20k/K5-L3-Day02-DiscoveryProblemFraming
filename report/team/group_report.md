# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: xyz
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Phạm Quỳnh Anh | Khi khách hàng nhắn tin hỏi thông tin sản phẩm (giá, kích thước, tình trạng còn hàng) ngoài giờ hành chính (22h–7h), tôi muốn cung cấp thông tin chính xác và tư vấn tức thì cho khách, để giữ chân khách mua hàng mà tôi không phải thức đêm trực page. | Chủ cửa hàng online, nhân viên trực page, khách mua ban đêm | Độ trễ phản hồi qua đêm 6–8 tiếng khiến khách chuyển sang shop khác (tỷ lệ rớt đơn ban đêm 40%). | "Nếu khách chỉ hỏi dạo lúc 2h sáng rồi không mua thì có tốn công không? Giải pháp Rule tự động gửi tin nhắn mẫu có sẵn của Facebook có giải quyết được không?" (Vũ Đức Minh hỏi) |
| 2 | Phạm Quỳnh Anh | Khi phát sinh các khoản chi tiêu nhỏ lẻ trong ngày (tiền ăn, gửi xe, tiền mua đồ), tôi muốn ghi nhận lại số tiền và phân loại vào các khoản mục, để kiểm soát chi tiêu hàng tháng mà không phải nhớ lại và cộng trừ lại vào cuối ngày. | Cá nhân, sinh viên | Bước nhớ lại và gõ tay từng dòng vào Excel/app mỗi tối (15–20 phút), dễ bỏ cuộc sau 1 tuần. | "Tại sao không dùng app như Money Lover hay kiểm tra lịch sử biến động số dư ngân hàng? Rào cản lớn nhất là do bạn lười nhập liệu hay do app hiện tại khó dùng?" (Nguyễn Văn Nhi hỏi) |
| 3 | Phạm Quỳnh Anh | Khi ôn thi cuối kỳ với hơn 200 trang slide bài giảng, tôi muốn trích xuất các công thức và kiến thức cốt lõi thành bản tóm tắt, để có thể ghi nhớ nhanh chóng mà không mất 4–5 tiếng lật giở từng trang slide. | Sinh viên đại học | Bước đọc lướt và gõ lại công thức/định nghĩa sang file Word (mất 4–5 tiếng/môn). | "Dữ liệu slide bài giảng có nhiều hình vẽ, công thức toán dạng ảnh chụp và không có cấu trúc cố định thì hệ thống có đọc được không? Đã thử xin tóm tắt của khóa trên chưa?" (Vũ Đức Minh hỏi) |
| 4 | Vũ Đức Minh | Khi một nhân viên mới bắt đầu làm việc, tôi muốn được cấp đầy đủ tài khoản và quyền truy cập vào các hệ thống cần thiết theo vị trí công việc, để có thể bắt đầu thực hiện nhiệm vụ mà không phải chờ đợi các bộ phận liên quan thiết lập tài khoản. | Nhân viên mới, HR, IT/System Admin, quản lý trực tiếp | Bước xác định hệ thống cần cấp quyền, gửi yêu cầu, chờ phê duyệt từ nhiều đầu mối và thiết lập tài khoản trên từng hệ thống (mất vài ngày). | "Việc cấp quyền truy cập hệ thống công ty có chính sách bảo mật nghiêm ngặt và cần người chịu trách nhiệm, liệu có rủi ro bảo mật nào nếu tự động hóa khâu phân quyền này không?" (Phạm Quỳnh Anh hỏi) |
| 5 | Vũ Đức Minh | Khi người dân đến hỏi về một thủ tục hành chính, tôi muốn xác định đầy đủ hoàn cảnh và điều kiện của họ để hướng dẫn chính xác các giấy tờ, bước thực hiện cần thiết, nhằm hạn chế việc người dân phải đi lại nhiều lần do thiếu hồ sơ. | Cán bộ tiếp nhận hồ sơ, cán bộ tư vấn, người dân, cơ quan hành chính | Cán bộ phải khai thác thông tin, tra cứu quy định và đối chiếu điều kiện; cán bộ ít kinh nghiệm dễ bỏ sót câu hỏi hoặc trường hợp ngoại lệ. | "Quy định pháp luật và thủ tục hành chính thay đổi thường xuyên theo thông tư mới, làm sao đảm bảo thông tin tra cứu luôn được cập nhật chính xác và có giá trị pháp lý?" (Nguyễn Văn Nhi hỏi) |
| 6 | Vũ Đức Minh | Khi nhận được đơn đặt hàng cho mặt hàng công ty không còn tồn kho, tôi muốn nhanh chóng tìm được các nhà cung cấp thay thế có hàng sẵn, giá nhập và thời gian giao phù hợp, để đáp ứng đơn hàng và hạn chế mất doanh thu. | Nhân viên kinh doanh, nhân viên mua hàng, nhà cung cấp, khách hàng | Tìm kiếm và liên hệ nhiều nhà cung cấp, chờ phản hồi rồi tổng hợp thông tin so sánh giá và thời gian giao. | "Các nhà cung cấp bên ngoài thường không công khai tồn kho real-time qua API, vậy làm sao thu thập được dữ liệu tồn kho của họ mà không phải gọi điện thoại hỏi tay?" (Phạm Quỳnh Anh hỏi) |
| 7 | Nguyễn Văn Nhi | Khi bắt đầu thực hiện một bài tập Lab, tôi muốn nhanh chóng xác định được các yêu cầu, hướng dẫn thực hiện và quy định nộp bài từ những tài liệu liên quan, để hiểu đúng nhiệm vụ và bắt đầu triển khai mà không mất quá nhiều thời gian tìm kiếm thông tin. | Học viên thực hiện bài Lab (cá nhân và nhóm), Mentor hỗ trợ | Dò tìm và đối chiếu chéo yêu cầu/rule/rubric giữa 5–6 file tài liệu rời rạc (`Slide`, `README`, `RULES`, `CHECKPOINTS`, `RUBRIC`) mất 15–20 phút/lần. | "Tại sao không chỉ cần ban tổ chức gộp các yêu cầu thành 1 bảng checklist duy nhất ngay đầu file CHECKPOINTS (No AI/Rule) thay vì phải xây dựng giải pháp công nghệ phức tạp?" (Vũ Đức Minh hỏi) |
| 8 | Nguyễn Văn Nhi | Khi viết báo cáo nghiên cứu khoa học hoặc luận văn, tôi muốn đảm bảo mỗi nội dung, số liệu và nhận định trong bài viết đều được đối chiếu chính xác với nguồn tài liệu gốc, đồng thời duy trì đúng thứ tự trích dẫn, để tránh sai lệch thông tin và đáp ứng yêu cầu học thuật. | Sinh viên làm khóa luận/NCKH, Giảng viên hướng dẫn, Người phản biện | Mở lại từng paper PDF gốc để đối chiếu thủ công độ khớp giữa nhận định/số liệu trong bài viết với nội dung bài báo gốc (mất 25 phút/lần rà soát chương). | "Đã có các phần mềm quản lý trích dẫn như Zotero hay BibTeX giải quyết việc đánh số và định dạng, việc kiểm tra độ khớp ngữ nghĩa giữa câu viết và paper gốc có thực sự làm được bằng AI với chi phí token hợp lý không?" (Phạm Quỳnh Anh hỏi) |
| 9 | Nguyễn Văn Nhi | Khi thực hiện các thí nghiệm Ablation trong quá trình nghiên cứu, tôi muốn xác định chính xác cấu hình mô hình, phiên bản dữ liệu và các thay đổi được áp dụng cho từng lần chạy, để có thể truy vết, đối chiếu và sử dụng đúng kết quả thực nghiệm khi phân tích và viết luận văn. | Sinh viên/NCS làm Machine Learning, Thành viên nhóm nghiên cứu | Dò tìm lại cấu hình từ các file log rời rạc (30 phút) và phải chạy lại thí nghiệm khi không truy vết được (mất 4–6 tiếng GPU/lần chạy). | "Vấn đề này đã có các công cụ MLOps chuyên dụng như Weights & Biases (W&B) hoặc MLflow giải quyết rất tốt bằng việc lưu log tự động, liệu có cần can thiệp AI vào đây không hay chỉ là vấn đề kỷ luật dùng công cụ?" (Vũ Đức Minh hỏi) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung (Bản chất công việc) |
|---|---|---|
| **A — Hỗ trợ và khai thác thông tin** | `#1` Trả lời khách hàng ngoài giờ; `#3` Tóm tắt tài liệu học tập; `#5` Hướng dẫn thủ tục hành chính; `#7` Tra cứu hướng dẫn và quy định trong Lab | Tiếp nhận yêu cầu bằng ngôn ngữ tự nhiên, tìm kiếm, tổng hợp và trình bày thông tin phù hợp với ngữ cảnh |
| **B — Tìm kiếm và kiểm chứng thông tin** | `#6` Tìm nhà cung cấp thay thế; `#8` Kiểm chứng trích dẫn trong bài nghiên cứu; `#9` Truy xuất cấu hình và lịch sử thí nghiệm ML | Tìm thông tin từ nhiều nguồn, so sánh, kiểm tra tính chính xác và truy xuất nguồn gốc |
| **C — Vận hành lặp lại theo quy trình** | `#2` Ghi nhận chi tiêu cá nhân; `#4` Cấp tài khoản và phân quyền nhân viên mới | Thực hiện các bước lặp lại theo quy tắc, biểu mẫu và điều kiện đã xác định |


### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian xử lý thủ công và giảm sai sót trong các tác vụ tra cứu, kiểm chứng thông tin và vận hành lặp lại
├── Opportunity A (từ Cluster A - #1, #3, #5, #7): Thông tin hướng dẫn/quy định dài và phân tán ở nhiều nơi, khiến người cần thông tin mất nhiều thời gian tự dò tìm hoặc phải chờ hỏi lại người phụ trách
├── Opportunity B (từ Cluster B - #6, #8, #9): Phải đối chiếu chéo thủ công giữa nội dung/kết quả đang làm với nhiều nguồn dữ liệu gốc (paper PDF, file log thí nghiệm, hồ sơ nhà cung cấp) nên tốn thời gian và dễ nhầm lẫn nguồn
└── Opportunity C (từ Cluster C - #2, #4): Các thao tác nhập liệu và cấp quyền theo quy tắc cố định phải làm tay lặp đi lặp lại qua nhiều bước, gây tốn thời gian và dễ bỏ sót bước
     ✗ "Chatbot trả lời khách hàng ngoài giờ / Chatbot hỏi đáp Lab" ← solution, gạch bỏ khỏi tầng này
     ✗ "Tool tự động kiểm tra trích dẫn / Hệ thống quản lý thí nghiệm" ← solution, gạch bỏ khỏi tầng này
     ✗ "Script tự động cấp tài khoản và phân quyền" ← solution, gạch bỏ khỏi tầng này 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "Cần một Chatbot trực fanpage ngoài giờ (#1) hoặc trợ lý ảo hỏi đáp quy định Lab (#7)": Đã gạch bỏ vì đây là giải pháp công nghệ; pain thật sự là người dùng không tra cứu nhanh được câu trả lời đúng ngữ cảnh từ tài liệu sẵn có.
- "Làm công cụ tự động kiểm tra trích dẫn (#8) / Dashboard quản lý thí nghiệm (#9)": Đã gạch bỏ vì đây là tính năng sản phẩm; pain thật sự là việc mất hàng chục phút đối chiếu thủ công số liệu/cấu hình với nguồn gốc để tránh sai lệch.
- "Tự động hóa quy trình cấp tài khoản (#4)": Đã gạch bỏ vì "tự động hóa" là cách giải quyết; pain thật sự là thao tác tay lặp lại trên nhiều hệ thống theo một biểu mẫu cố định.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **#3 — Tóm tắt tài liệu học tập (200 trang slide ôn thi)** | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| **#2 — Ghi nhận và phân loại chi tiêu cá nhân** | 5 | 5 | 4 | 4 | 5 | 3 | 5 | **31** |
| **#5 — Hướng dẫn thủ tục hành chính cho người dân** | 4 | 4 | 4 | 3 | 2 | 5 | 3 | **25** |
| **#6 — Tìm nhà cung cấp thay thế khi hết tồn kho** | 4 | 4 | 3 | 4 | 2 | 4 | 3 | **24** |

**Candidate được chọn:** **`#3` — Tóm tắt tài liệu học tập (Trích xuất công thức và kiến thức cốt lõi từ slide bài giảng khi ôn thi cuối kỳ)** *(hoặc `#2` nếu nhóm chốt chọn bài toán chi tiêu cá nhân).*

**Vì sao chọn:**
- **Actor và Domain sát sườn 100% thành viên:** Cả nhóm đều là sinh viên/học viên trực tiếp trải qua nỗi đau đọc hàng trăm trang slide trước kỳ thi; quy trình hiện tại rất rõ từng bước và có sẵn dữ liệu thật (các bộ slide môn học).
- **Thuận lợi kiểm chứng thực tế ngay ở CP4:** Dễ dàng phỏng vấn trực tiếp người thật (các bạn học viên ở nhóm khác trong lớp theo đúng luật *The Mom Test*) và thu thập survey nhanh ngay trong 30 phút của buổi Lab mà không phải giả định.
- **Phân tầng rõ rệt giữa No AI / Rule / Workflow / Agent:** Dễ dàng đặt lên bàn cân giữa giải pháp không dùng AI (dùng bản tóm tắt khóa trên, mục lục chuẩn), Rule (script gom text từ PDF/PPTX), và Workflow AI (trích xuất khái niệm/công thức theo chương + con người kiểm tra lại công thức toán/hình vẽ).

**Vì sao loại các candidate còn lại:**
- **Loại `#5` (Hướng dẫn thủ tục hành chính):** Dù pain point xã hội rất lớn và rất hay để so sánh giữa Decision Tree (Rule) với AI, nhưng trong khuôn khổ 4 tiếng của buổi Lab, nhóm không thể tiếp cận phỏng vấn trực tiếp "cán bộ tiếp nhận hồ sơ" thật ở CP4. Ngoài ra, bài toán có rủi ro pháp lý cao (Viability) khi văn bản pháp luật thay đổi liên tục.
- **Loại `#6` (Tìm nhà cung cấp thay thế khi hết hàng):** Quy trình phụ thuộc nhiều vào yếu tố bên ngoài (các nhà cung cấp truyền thống không mở API tồn kho thời gian thực mà phải gọi điện/nhắn Zalo hỏi tay). Nhóm cũng khó tìm được nhân viên thu mua (Procurement) thực tế để phỏng vấn kiểm chứng ngay trong giờ Lab.
- **Loại `#2` (Ghi nhận chi tiêu cá nhân):** Đạt điểm rất cao (32/35) và dễ kiểm chứng, nhưng trên thị trường đã có quá nhiều ứng dụng giải quyết tốt bằng Rule/tích hợp biến động số dư ngân hàng (Money Lover, MISA, app ngân hàng). Phần bottleneck thực sự còn lại chủ yếu nằm ở thói quen/động lực duy trì của người dùng hơn là bài toán kỹ thuật cần tới AI.

**Xử lý bất đồng (nếu có):**
- Một số thành viên ấn tượng với tính thực tiễn doanh nghiệp/xã hội của **`#5` (Thủ tục hành chính)** và **`#6` (Nhà cung cấp thay thế)**, trong khi thành viên khác nghiêng về **`#2` (Chi tiêu cá nhân)** và **`#3` (Tóm tắt tài liệu học tập)** vì có thể phỏng vấn người thật ngay tại lớp ở CP4. Nhóm đã thống nhất chấm điểm khách quan trên 7 tiêu chí, ưu tiên tiêu chí *"Vừa sức lab"* và *"Có thể kiểm chứng bằng hành vi người thật ngay tại lớp (CP4)"* để chốt chọn **`#3`** (và giữ `#2` làm phương án dự phòng sát nhất).

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

[Interview snapshot](report/assets/cp4-interview-snapshot.md):

| Nguồn                                                             | Số người / số mẫu | Tín hiệu xác nhận                                                                                                                                                   | Tín hiệu phản bác                                                                                                                                                                      |
| ----------------------------------------------------------------- | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Phỏng vấn 1 – Sinh viên gặp khó khăn về thuật ngữ song ngữ        | 1                 | Giáo trình tiếng Anh và slide tiếng Việt sử dụng cách diễn giải khác nhau; sinh viên khó thống nhất thuật ngữ và tổng hợp kiến thức để ôn thi.                      | Chưa chứng minh nhu cầu tóm tắt tự động; vấn đề cốt lõi có thể là chuẩn hóa thuật ngữ và cách diễn giải.                                                                               |
| Phỏng vấn 2 – Sinh viên không nhận biết được lỗ hổng kiến thức    | 1                 | Đọc bản tóm tắt tạo cảm giác hiểu bài nhưng không thể vận dụng khi thi; sinh viên không biết mình còn yếu ở đâu.                                                    | Tóm tắt tài liệu đơn thuần không giải quyết được vấn đề; nhu cầu thực tế nghiêng về kiểm tra mức độ hiểu và phát hiện lỗ hổng kiến thức.                                               |
| Phỏng vấn 3 – Sinh viên khó vận dụng công thức vào bài tập        | 1                 | Tóm tắt chỉ liệt kê công thức chưa đủ để giải bài; sinh viên cần dạng bài mẫu và hướng dẫn cách lựa chọn, áp dụng công thức.                                        | Nhu cầu có thể nằm ở luyện tập theo dạng bài và hướng dẫn giải, không phải tổng hợp tài liệu.                                                                                          |
| Phỏng vấn 4 – Sinh viên cần tổng hợp công thức toán học chính xác | 1                 | Mất 4,5–5 giờ tổng hợp công thức cho một môn; phải chụp và nhập lại công thức thủ công. Có nhu cầu rõ về độ chính xác ký hiệu và khả năng đối chiếu số trang nguồn. | Không dám tin bản tóm tắt trên mạng vì sợ sai dấu trừ, chỉ số dưới. Nếu không bảo đảm độ chính xác, người học vẫn chọn làm thủ công.                                                   |
| Phỏng vấn 5 – Sinh viên chỉ cần tự tổng hợp khi tài liệu thay đổi | 1                 | Mất khoảng 3 giờ tự làm đề cương khi giảng viên đổi giáo trình hoặc slide mới.                                                                                      | Khi có đề cương tốt từ khóa trước, sinh viên ưu tiên dùng lại thay vì tự tổng hợp. Nhu cầu không xuất hiện ở mọi môn học; giải pháp phải tạo giá trị vượt trội so với tài liệu có sẵn. |

**Nhận định sau kiểm chứng**

Tín hiệu xác nhận:

- Sinh viên thực sự mất thời gian trong việc tổng hợp và hệ thống hóa tài liệu, đặc biệt với môn có nhiều công thức hoặc tài liệu mới.
- Việc tóm tắt đơn thuần chưa đáp ứng đầy đủ nhu cầu ôn thi.
- Độ chính xác, khả năng truy xuất về tài liệu gốc và khả năng hỗ trợ vận dụng kiến thức là những yêu cầu quan trọng.

Tín hiệu phản bác:

- Không phải sinh viên nào cũng cần tự tổng hợp tài liệu; đề cương từ khóa trước có thể giải quyết vấn đề với chi phí gần như bằng 0.
- Một số pain liên quan đến kiểm tra kiến thức, luyện tập dạng bài hoặc chuẩn hóa thuật ngữ, không trực tiếp thuộc bài toán tóm tắt.
- Sinh viên không sẵn sàng tin tưởng kết quả tự động nếu không thể kiểm chứng độ chính xác.

**Nhóm đã sửa problem thế nào sau kiểm chứng?**

Nhóm thu hẹp problem từ “Sinh viên mất nhiều thời gian tóm tắt tài liệu học tập trước kỳ thi” thành:

> Sinh viên gặp khó khăn trong việc tự tổng hợp và hệ thống hóa kiến thức ôn thi từ các tài liệu dài, phân tán hoặc mới cập nhật, đặc biệt khi cần bảo đảm tính chính xác của công thức, thuật ngữ và khả năng đối chiếu với tài liệu gốc.

Đồng thời, nhóm xác định rõ phạm vi:

1. Đối tượng ưu tiên: Sinh viên có môn học sử dụng nhiều tài liệu, công thức hoặc giáo trình/slide mới mà chưa có đề cương đáng tin cậy từ khóa trước.
2. Pain trọng tâm: Tốn thời gian tự tổng hợp kiến thức và khó bảo đảm bản tổng hợp chính xác, đầy đủ.
3. Điều kiện để giải pháp có giá trị: Kết quả phải giữ đúng ký hiệu, thuật ngữ, có nguồn và số trang để đối chiếu.
4. Chưa gộp vào problem chính: Kiểm tra lỗ hổng kiến thức và luyện tập dạng bài. Đây là những opportunity liên quan nhưng cần kiểm chứng riêng, vì có thể đòi hỏi một bài toán khác với tổng hợp tài liệu.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
