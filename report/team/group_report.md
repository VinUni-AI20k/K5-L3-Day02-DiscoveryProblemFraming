# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

Candidate tổng hợp từ CP2 của bốn báo cáo cá nhân, dùng mã truy vết ở mục 2.2. Chưa có biên bản pitch hoặc câu hỏi phản biện trực tiếp.

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Khoa | K1 — Khi chuẩn bị sprint, cần tìm và ghép thông tin dự án để hiểu bối cảnh công việc | Developer mới hoặc tham gia dự án có sẵn | Tìm, đọc và đối chiếu thông tin qua nhiều nguồn (bước 2–6 trong card) | |
| 2 | Khoa | K2 — Khi làm task trên hệ thống có sẵn, cần tìm kiến thức và quyết định kỹ thuật cũ để hiểu module | Developer làm việc với module chưa quen | Đọc code, tìm lịch sử và hỏi người từng phụ trách (bước 3–6) | |
| 3 | Khoa | K3 — Khi nhận backlog mới, cần hiểu yêu cầu và acceptance criteria để bắt đầu đúng phạm vi | Developer nhận task từ PO, PM hoặc Tech Lead | Làm rõ yêu cầu qua nhiều vòng trao đổi (bước 3–6) | |
| 4 | Dương | D1 — Khi review PR lớn, cần hiểu thay đổi và rủi ro để nhận xét có căn cứ | Developer được giao review PR | Giả thuyết: lần theo mã liên quan để hiểu tác động (bước 4) | |
| 5 | Dương | D2 — Khi điền nhiều biểu mẫu, cần xác định thông tin khách hàng để hoàn tất hồ sơ không bỏ sót | Nhân viên nhập thông tin khách hàng | Giả thuyết: nhập lại các trường trùng (bước 4) | |
| 6 | Dương | D3 — Khi nhận tiền điện, nước và dịch vụ, cần đối chiếu hợp đồng để kiểm khoản phải trả | Người thuê nhà | Giả thuyết: đối chiếu từng khoản với điều khoản và dữ liệu tính tiền (bước 4) | |
| 7 | Lam | L1 — Khi dùng lại nhận định trong paper đã đọc, cần tìm đúng bằng chứng để giải thích có căn cứ | Sinh viên mới tham gia nhóm nghiên cứu, bối cảnh giả định | Dò bằng chứng trong PDF (bước 3), chưa đo thực tế | |
| 8 | Lam | L2 — Khi có nhiều paper liên quan, cần xác định bài sát câu hỏi nghiên cứu để chọn bài đọc sâu | Sinh viên chọn paper, bối cảnh giả định | Đọc tiêu đề và abstract (bước 2), chưa đo thực tế | |
| 9 | Lam | L3 — Khi so điểm số giữa paper, cần kiểm điều kiện đánh giá để tránh kết luận thiếu căn cứ | Sinh viên lập bảng so sánh, bối cảnh giả định | Đối chiếu mô hình, dữ liệu và thiết lập (bước 4), chưa đo thực tế | |
| 10 | An | A1 — Khi rà soát biến thể tín hiệu, cần nhận biết khác biệt để chọn bước thử tiếp có căn cứ | Người nghiên cứu tín hiệu định lượng | Đối chiếu nhiều thay đổi và chỉ số (bước 3), thời gian phân rã là ước lượng | |
| 11 | An | A2 — Khi tiếp tục việc sau họp, cần rõ quyết định, người phụ trách và hạn để không bỏ sót cam kết | Người tổng hợp biên bản, bối cảnh giả định | Xác nhận người phụ trách và deadline (bước 3) | |
| 12 | An | A3 — Khi tra đề nghị mua vật tư, cần biết người đang xử lý và thông tin thiếu để bổ sung đúng chỗ | Nhân viên gửi đề nghị mua, bối cảnh giả định | Xác định người giữ hồ sơ và thông tin thiếu (bước 3) | |

### 2.2. Cluster

**[CHỜ NHÓM XÁC NHẬN]** Phân nhóm sơ bộ có hỗ trợ AI, từ CP1–CP2 của bốn báo cáo trên main tại commit 71f0e47. Pitch, phản biện trực tiếp và lựa chọn cuối do các thành viên thực hiện.

**Các candidate trong top 3 của từng thành viên**

Mã dưới đây dùng để truy vết card gốc. Cột ưu tiên pitch ghi lựa chọn trong báo cáo cá nhân, chưa phải kết quả pitch của nhóm.

| Mã | Thành viên / nguồn | Candidate CP2 và mã CP1 | Ưu tiên pitch |
|---|---|---|---|
| K1 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #1: Tìm kiếm và tổng hợp thông tin dự án; CP1 #1, #5 | Có |
| K2 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #2: Truy xuất kiến thức kỹ thuật và quyết định cũ; CP1 #4, #9 | — |
| K3 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #3: Hiểu backlog và làm rõ yêu cầu; CP1 #2, #7 | — |
| D1 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #1: Đọc Pull Request lớn; CP1 #6 | Có |
| D2 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #2: Nhập lại thông tin khách hàng; CP1 #12 | — |
| D3 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #3: Đối chiếu chi phí thuê nhà; CP1 #19 | — |
| L1 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #1: Tìm lại bằng chứng trong paper đã đọc; CP1 #1 | Có |
| L2 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #2: Sàng lọc paper sát câu hỏi nghiên cứu; CP1 #3 | — |
| L3 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #3: Đối chiếu điều kiện đánh giá giữa các paper; CP1 #7 | — |
| A1 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #1: So sánh các biến thể tín hiệu định lượng; CP1 #2 | Có |
| A2 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #2: Xác định quyết định, người phụ trách và deadline sau cuộc họp; CP1 #9 | — |
| A3 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #3: Xác định trạng thái và thông tin thiếu của đề nghị mua vật tư; CP1 #8 | — |

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm và hiểu thông tin theo ngữ cảnh | K1, K2, D1, L1, L2 | Phải tìm, đọc và nối thông tin liên quan trước khi sử dụng: bối cảnh dự án, mã nguồn hoặc tài liệu nghiên cứu. Tìm lại nguồn đã biết và sàng lọc nguồn mới là các bước khác nhau, cần giữ riêng khi phân tích từng card. |
| B — Đối chiếu kết quả nghiên cứu | L3, A1 | Nhiều chỉ số và điều kiện thử nghiệm cần được đối chiếu trước khi diễn giải khác biệt; chỉ nhìn kết quả có thể dẫn đến so sánh thiếu căn cứ. |
| C — Làm rõ thông tin và trách nhiệm trong phối hợp | K3, A2, A3 | Thông tin để tiếp tục công việc còn thiếu hoặc mơ hồ; phải tìm đầu mối và xác nhận lại yêu cầu, trách nhiệm hoặc trạng thái xử lý. |
| D — Nhập lặp dữ liệu khách hàng | D2 | Cùng thông tin phải điền qua nhiều biểu mẫu, sau đó kiểm tra sự nhất quán. |
| E — Đối chiếu khoản thu với hợp đồng thuê | D3 | Người thuê phải kiểm các khoản thu bằng điều khoản và chứng từ liên quan. |

A và C gom theo pattern, chưa đồng nghĩa các card là cùng một problem. D và E tạm đứng riêng vì chưa có card khác đủ gần về pain và quy trình. Nhóm cần xác nhận ranh giới cluster, nhất là việc tìm lại thông tin so với sàng lọc thông tin mới ở A.

**Dữ liệu còn thiếu:** Dương chưa có số đo; Khoa chưa có baseline thực đo và các target còn là giả thuyết. Báo cáo của Lam dùng bối cảnh và số liệu giả định. An tự báo cáo tổng thời gian ở Card #1, còn thời gian phân rã và bối cảnh Card #2–#3 là ước lượng hoặc giả định. Chưa dùng các số này làm baseline chung hay bằng chứng đồng thuận của nhóm.

### 2.3. Opportunity Solution Tree rút gọn

Phạm vi: tìm lại bằng chứng trong paper đã đọc, theo candidate L1 của Lam và [shortlist](shortlist.md).

~~~text
OUTCOME: Giảm thời gian tìm lại bằng chứng từ paper,
         đồng thời giữ đúng ngữ cảnh và truy xuất được nguồn.
├── Opportunity 1: Ghi chú thiếu vị trí cụ thể của bằng chứng
│                 như số trang, hình, bảng hoặc đoạn văn.
├── Opportunity 2: Mất thời gian dò lại PDF để tìm đúng
│                 đoạn, hình hoặc bảng cần dùng.
├── Opportunity 3: Khó xác nhận ngữ cảnh của bằng chứng
│                 để diễn giải nhận định đúng phạm vi.
└── Opportunity 4: Vị trí nguồn được ghi không nhất quán
                  giữa các paper, gây khó khi tìm lại.
~~~

Các opportunity trên lấy từ shortlist và [Card #1 của Lam](../individual/2A202604020_NguyenDucKhuongLam.md); cần được kiểm chứng bằng trường hợp thực tế. Hướng đo là thời gian tìm được bằng chứng, độ đúng của vị trí nguồn và ngữ cảnh. Baseline và target chưa chốt bằng số đo thực tế.

**Các ý là solution, không đặt ở tầng Opportunity:**

- AI chatbot đọc paper.
- RAG-based paper assistant.
- Tự động tóm tắt PDF.
- Ghi chú có cấu trúc, Zotero annotation và liên kết đến trang PDF.

### 2.4. Chấm điểm shortlist (1–5)

Nguồn: [shortlist.md](shortlist.md). Điểm được giữ nguyên từ bảng shortlist.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| L1 — Tìm lại bằng chứng từ paper | 5 | 5 | 4 | 5 | 5 | 5 | 4 | **33** |
| A1 — So sánh biến thể tín hiệu | 5 | 5 | 4 | 4 | 4 | 5 | 3 | **30** |
| K1 — Tổng hợp thông tin trước Sprint Planning | 5 | 4 | 2 | 3 | 3 | 4 | 4 | **25** |

Mốc 10 phút/lần, trong đó 6 phút dò PDF, là số liệu giả định trong báo cáo của Lam, chưa phải baseline đã đo. Điểm ở cột “Pain có bằng chứng” là đánh giá được ghi trong shortlist, chưa thay thế việc kiểm chứng thực tế.

**Candidate được chọn:** L1 — Tìm lại bằng chứng từ paper.

**Job Story:** Khi cần dùng lại một nhận định từ paper đã đọc, tôi muốn tìm đúng đoạn, hình hoặc bảng chứa bằng chứng, để giải thích có căn cứ mà không phải đọc lại cả bài.

**Vì sao chọn:**

- Phạm vi gọn trong một tác vụ: tìm đúng bằng chứng trong paper đã đọc.
- Có thể đo thời gian tìm và kiểm tra trực tiếp vị trí nguồn, ngữ cảnh trong PDF.
- Có phương án không dùng AI để đối chiếu: ghi số trang/hình/bảng, annotation và liên kết PDF trong Zotero.
- Không cần tích hợp nhiều nguồn dữ liệu dự án. Candidate đạt 33 điểm, cao nhất trong shortlist.

**Vì sao loại các candidate còn lại:**

- **A1 — So sánh biến thể tín hiệu:** domain quant research đặc thù; cần kiểm tra điều kiện thử nghiệm và phân biệt mô tả chênh lệch với kết luận nhân quả.
- **K1 — Tổng hợp thông tin trước Sprint Planning:** phạm vi rộng, liên quan nhiều nguồn và quyền truy cập; chưa có baseline thực nghiệm để xác định bước nghẽn chính.

**Xử lý bất đồng (nếu có):** Chưa có ghi nhận trong tài liệu nguồn.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

**[CHƯA KIỂM CHỨNG]** CP4 hiện là bản draft: phần 3.2 rà soát một Problem Card, chưa có mẫu phỏng vấn hoặc survey thật. Các mốc thời gian và tần suất trong card là giả định, không phải baseline thực nghiệm. Nguồn: [CP4.md](CP4.md) và [Card #1 của Lam](../individual/2A202604020_NguyenDucKhuongLam.md).

### 3.1. Assumption Map

Thang điểm: 1 = thấp, 5 = cao; ưu tiên giả định quan trọng cao nhưng ít bằng chứng.

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Việc tìm lại bằng chứng xảy ra khoảng 3 lần/tuần, ảnh hưởng đến viết bảng so sánh và trả lời mentor. | Value | 5 | 2 | Có — đối chiếu các lần tìm trong tuần gần nhất. |
| 2 | Thiếu vị trí nguồn trong ghi chú là nguyên nhân chính khiến bước dò PDF mất khoảng 6 phút. | Value | 5 | 2 | Có — xem ghi chú và thao tác tìm thực tế. |
| 3 | Ghi chú kèm trang/hình/bảng và liên kết nguồn giúp hoàn tất một lượt trong tối đa 3 phút, vẫn đúng ngữ cảnh. | Usability | 5 | 1 | Có — đo thử cả thời gian và độ đúng. |
| 4 | Zotero hỗ trợ nối annotation trong ghi chú về trang PDF. | Feasibility | 4 | 4 | Đã đối chiếu tài liệu [Zotero PDF Reader](https://www.zotero.org/support/pdf_reader); cần thử với PDF đang dùng. |
| 5 | Công sức ghi nguồn ngay khi đọc thấp hơn thời gian tiết kiệm khi tìm lại. | Viability | 4 | 1 | Có — ghi thêm thời gian tạo ghi chú. |

**Ưu tiên kiểm chứng:** #2 và #3; nếu nghẽn ở hiểu ngữ cảnh thay vì định vị nguồn, liên kết trang chưa đủ giải quyết problem.

### 3.2. Kiểm chứng

| Nội dung rà soát | Ghi nhận từ Problem Card #1 |
|---|---|
| Actor / bối cảnh | Rachal, sinh viên mới tham gia nhóm nghiên cứu; cần dùng lại nhận định khi viết bảng so sánh hoặc trả lời nhóm/mentor. |
| Quy trình / workaround | Mở ghi chú → xác định paper → dò PDF → kiểm tra ngữ cảnh → ghi vị trí nguồn; đang dò lại vì ghi chú thiếu vị trí. |
| Thời gian / tần suất | Khoảng 10 phút/lần × 3 lần/tuần = 30 phút/tuần; riêng dò PDF khoảng 6 phút/lần = 18 phút/tuần. |
| Opportunity | Giúp đi từ nhận định đã ghi đến đúng bằng chứng trong paper, giữ được ngữ cảnh để giải thích. |

**Câu hỏi kiểm chứng hành vi:**

1. Lần gần nhất cần tìm lại bằng chứng để viết bảng so sánh hoặc trả lời mentor là khi nào? Hãy mở ghi chú và PDF đã dùng, kể lại từng bước.
2. Khi đó ghi chú có trang, số hình/bảng hoặc liên kết không? Bước nào mất lâu nhất, có lịch sử thao tác hay ghi nhận thời gian không?
3. Trong tuần gần nhất đã tìm lại bao nhiêu lần? Lần nào tìm nhanh hoặc không tìm được, khác nhau ở điểm gì?
4. Đã dùng annotation hoặc liên kết PDF lần nào? Hãy chỉ một ghi chú cụ thể và cách kiểm tra bằng chứng có thực sự hỗ trợ nhận định.

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác / cần kiểm tra |
|---|---|---|---|
| Problem Card #1 | 1 card; chưa có mẫu phỏng vấn | Mô tả bước dò PDF chiếm 6/10 phút và thiếu vị trí nguồn. | Chưa đủ để kết luận thiếu vị trí là nguyên nhân chính hoặc mức 10 phút đại diện cho người khác. |
| Tài liệu Zotero tại mục 3.3 | 2 trang tài liệu; không phải mẫu người dùng | Có sẵn cách gắn ghi chú với paper và quay lại trang PDF. | Phản bác nhu cầu phải xây công cụ AI mới; chưa chứng minh người dùng đạt mục tiêu 3 phút. |

### 3.3. Research giải pháp đã có

Các nguồn chính thức đã mở kiểm tra ngày 09/11/2026. Khoảng trống và bài học là nhận định của nhóm cho quy trình đang xét.

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Zotero — annotation → note → trang PDF | [PDF Reader and Note Editor](https://www.zotero.org/support/pdf_reader) | Bước 3, 5: annotation đưa vào note có liên kết về trang PDF và trích dẫn. | Giữ đường dẫn từ ghi chú về bằng chứng, không cần AI. | Ghi chú cũ thiếu annotation cần bổ sung; mở đúng trang chưa đảm bảo hiểu đúng điều kiện của kết quả. | Thử mẫu: nhận định + annotation + trang/hình/bảng + ngữ cảnh; vẫn giữ bước 4 do người đọc thực hiện. |
| Zotero — ghi chú gắn với paper | [Notes](https://www.zotero.org/support/notes) | Bước 1, 2: child note thuộc một tài liệu; nội dung note tìm được qua tìm kiếm Zotero. | Giữ ghi chú cùng paper, hỗ trợ xác định nguồn. | Chỉ gắn note với paper chưa chỉ ra đoạn bằng chứng. | Kết hợp child note với annotation; tên paper hoặc citation đơn lẻ chưa đủ. |
| Adobe Acrobat — tìm kiếm PDF | [Searching PDFs](https://helpx.adobe.com/acrobat/using/searching-pdfs.html) | Bước 3: tìm từ/cụm từ trong PDF để định vị nội dung. | Tận dụng công cụ tìm kiếm sẵn có khi nhớ từ khóa. | Nhận định diễn đạt lại có thể không khớp từ khóa; vẫn phải đọc kết quả và ngữ cảnh. | Dùng tìm kiếm khi ghi chú chưa có liên kết; tìm thấy thì lưu ngay vị trí để dùng lần sau. |

---

## 4. Quy trình trước/sau (CP5)

**[CHƯA KIỂM CHỨNG]** Nội dung từ [CP5.md](CP5.md). Thời gian hiện tại là mốc giả định từ card; phương án tương lai và mốc 3 phút là kỳ vọng, chưa phải kết quả đo.

### 4.1. Quy trình hiện tại

```text
HIỆN TẠI — 5 bước, khoảng 10 phút, 5/5 bước thủ công

[1 Mở ghi chú: 1'] → [2 Xác định paper: 1']
→ [3 Dò bằng chứng trong PDF: 6'] ← BOTTLENECK
→ [4 Kiểm tra ngữ cảnh: 1'] → [5 Ghi lại vị trí nguồn: 1']
```

**Bottleneck chính:** Dò bằng chứng trong PDF, 6 phút/lần theo mốc giả định trong CP5.

CP5.md chưa có bảng actor/input/output/handoff cho từng bước; cần nhóm bổ sung bằng mô tả quy trình đã kiểm tra thực tế.

### 4.2. Quy trình tương lai

```text
TƯƠNG LAI — 4 bước, khoảng 3 phút, 2/4 bước thủ công

[1 Mở ghi chú có liên kết paper + từ khóa: 0.5']  ← CON NGƯỜI
→ [2 Mở đúng trang/annotation trong Zotero: 0.5'] ← RULE (annotation + page link)
→ [3 Kiểm tra bằng chứng và ngữ cảnh: 1.5']       ← CON NGƯỜI
→ [4 Ghi lại vị trí nguồn vào bảng so sánh: 0.5'] ← CON NGƯỜI

BOUNDARY: Không tự động kết luận paper chứng minh điều gì. Người đọc phải kiểm tra
đoạn trích, ngữ cảnh và đối chiếu với PDF gốc trước khi sử dụng bằng chứng.

PHƯƠNG ÁN QUAY VỀ: Nếu annotation hoặc liên kết sai/mất,
mở PDF gốc và tìm thủ công bằng Ctrl+F hoặc dò theo số trang.
```

**[CẦN NHÓM XÁC NHẬN]** CP5 ghi “2/4 bước thủ công”, nhưng sơ đồ gắn nhãn CON NGƯỜI ở bước 1, 3 và 4. CP5 gọi thao tác annotation/page link là RULE, trong khi CP6 chọn No AI và dành Rule cho script riêng. Các nhãn và số đếm được giữ theo nguồn, chưa tự điều chỉnh.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 4 | Gộp thao tác xác định paper và truy cập vị trí nguồn |
| Tổng thời gian | 10' | 3' | Target chính: tối đa 3 phút/lần |
| Bước thủ công | 5/5 | 2/4 | Hai bước chính được hỗ trợ bởi annotation và liên kết nguồn |
| Bottleneck | Dò bằng chứng trong PDF (6') | Kiểm tra bằng chứng và ngữ cảnh (1.5') | Bottleneck mới được giữ lại có chủ đích để đảm bảo độ chính xác |
| Rủi ro mới | Ghi chú thiếu vị trí nguồn | Annotation sai, liên kết hỏng hoặc ghi nhầm trang | Xử lý bằng kiểm tra PDF gốc |
| Chất lượng | Phụ thuộc vào trí nhớ và khả năng tìm kiếm | Phải tìm đúng đoạn và giữ nguyên ngữ cảnh | Không đánh đổi độ chính xác lấy tốc độ |

---

## 5. Problem Statement v0 (CP5)

**[CHƯA KIỂM CHỨNG]** Giữ nguyên v0 và phần phản biện được ghi trong CP5. Các mốc 10 phút, 6 phút và 30–40 phút/tuần chưa có baseline thực nghiệm đính kèm.

| Trường | Nội dung |
|---|---|
| **Actor** | Lam, sinh viên mới tham gia nhóm nghiên cứu, thường xuyên đọc và so sánh các paper |
| **Quy trình** | Khi cần sử dụng lại một nhận định từ paper đã đọc: mở ghi chú, xác định paper, dò bằng chứng trong PDF, kiểm tra ngữ cảnh và ghi lại vị trí nguồn |
| **Bottleneck** | Dò bằng chứng trong PDF mất khoảng 6 phút/lần vì ghi chú thiếu số trang, hình hoặc bảng tham chiếu |
| **Impact** | Khoảng 30–40 phút/tuần cho 3–4 lần tìm kiếm; khó bảo vệ nhận định khi không tìm lại được bằng chứng gốc |
| **Success Metric** | Giảm thời gian tìm bằng chứng từ khoảng 10 phút xuống tối đa 3 phút/lần. Đo bằng cách bấm giờ trong các tác vụ tìm kiếm thực tế. Đồng thời yêu cầu tìm đúng đoạn, đúng trang và giữ được ngữ cảnh |
| **Boundary** | Ưu tiên Zotero annotation, liên kết PDF và ghi chú có cấu trúc. AI (nếu thử nghiệm sau này) chỉ gợi ý vị trí bằng chứng, không tự kết luận hoặc tạo trích dẫn chưa được kiểm chứng. Người dùng phải đối chiếu PDF gốc |

**Phản biện nhận được:** AI chỉ ra rằng metric hiện tại chủ yếu đo tốc độ tìm kiếm, chưa chứng minh người dùng tìm được bằng chứng chính xác. Tìm nhanh nhưng sai đoạn hoặc mất ngữ cảnh có thể dẫn đến trích dẫn sai trong nghiên cứu.

**Nhóm đồng ý và bổ sung:** ngoài thời gian tìm kiếm, cần đo tỷ lệ tìm đúng bằng chứng (đúng đoạn, trang/hình/bảng) và khả năng giữ nguyên ngữ cảnh. Chỉ tính một lần tìm kiếm là thành công khi người dùng xác định được nguồn và xác minh được nội dung trong PDF gốc.

---

## 6. Mức can thiệp AI (CP6)

Nguồn: [CP6.md](CP6.md), do Lam chuẩn bị. Giữ ngôi xưng “tôi” của tác giả ở các mục 6–8; lựa chọn cá nhân trong nguồn chưa được đổi thành tuyên bố đồng thuận của cả nhóm.

Tôi tập trung vào việc tìm lại bằng chứng trong paper đã đọc để giải thích nhận định có căn cứ. Từ [CP4](https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming/blob/169d1927dce2f72cae879ac35dc90e8575901c3f/report/team/CP4.md) và [quy trình ở CP5](CP5.md), tôi so sánh các mức can thiệp, xác định tiêu chí đánh giá và chọn hướng tiếp tục.

**Nguồn số liệu:** Dữ liệu mô phỏng phục vụ bài lab, dựa trên CP1–CP5.

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Tôi xếp bài toán vào ô **mơ hồ thấp, phức tạp thấp** trong phạm vi tìm lại một bằng chứng ở paper đã đọc. Tôi chỉ cần đối chiếu ghi chú với PDF đã chọn, không tổng hợp nhiều nguồn hoặc tìm paper mới. Các bước đã rõ; kết quả được kiểm tra bằng vị trí nguồn và nội dung hỗ trợ nhận định.

Điểm tôi cần giữ lại là bước đọc ngữ cảnh: mở đúng trang chưa có nghĩa là hiểu đúng kết quả.

### 6.2. So sánh 4 mức

| Mức | Phương án | Đủ khi nào | Rủi ro | Lựa chọn của tôi |
|---|---|---|---|---|
| **No AI** | Ghi chú kèm nhận định, trang/hình/bảng, annotation và ngữ cảnh; mở lại bằng liên kết Zotero | Ghi chú dẫn về đúng nguồn, tôi kiểm tra được nội dung | Thiếu vị trí, liên kết hỏng, hiểu sai ngữ cảnh | Chọn |
| **Rule** | Script kiểm tra trường nguồn còn thiếu và tìm từ khóa theo quy tắc | Có nhiều thao tác lặp cần tự động hóa | Đủ trường nhưng sai nguồn; từ khóa không khớp nhận định | Chưa cần script riêng |
| **Workflow** | Các bước cố định: nhận định + PDF → AI gợi ý đoạn kèm vị trí → tôi đối chiếu | Cách ghi chú và tìm kiếm đơn giản chưa đáp ứng nhu cầu | Đoạn liên quan nhưng không hỗ trợ nhận định | Chưa chọn |
| **Agent** | AI tự chọn công cụ, nguồn và bước tìm tiếp theo | Các bước tìm kiếm chưa xác định trước | Phạm vi rộng, thêm chi phí và khó kiểm tra nguồn | Không chọn |

**Tôi chọn No AI.** Tôi sẽ ghi vị trí nguồn ngay trong ghi chú và dùng liên kết Zotero để mở lại. Nếu liên kết thiếu hoặc hỏng, tôi tìm trong PDF rồi bổ sung vị trí vừa tìm được.

Lý do là cách này xử lý trực tiếp bước dò PDF trong CP2–CP5. CP4 cho thấy công cụ đã có tính năng phù hợp, còn tôi chưa có căn cứ để thêm AI. Tôi chủ yếu sửa cách ghi chú và dùng tính năng sẵn có; chưa cần script tự động, AI tạo nội dung hoặc tự quyết bước tìm kiếm. No AI là mức đơn giản nhất để bắt đầu. Mốc 3 phút được giữ làm mục tiêu đánh giá từ CP5.

### 6.3. AI Canvas rút gọn

Tôi không dùng AI để dự đoán hoặc tạo nội dung trong phương án này, nên không điền AI Canvas theo hướng dẫn dành cho mức No AI. Việc xác nhận bằng chứng vẫn do tôi thực hiện.

### 6.4. Hai câu hỏi Google PAIR

Với mức No AI, tôi không cần điền phần này. Nếu chuyển sang Workflow/Agent, tôi sẽ làm rõ người dùng muốn được hỗ trợ hay giao việc, và kiểu sai nào gây hậu quả nặng hơn.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

### 7.1. Problem Statement v1

| Trường | Nội dung |
|---|---|
| **Actor** | Tôi, trong vai sinh viên mới tham gia nhóm nghiên cứu, cần dùng lại nhận định từ paper đã đọc và có PDF gốc |
| **Quy trình** | Mở ghi chú → xác định paper → tìm bằng chứng → kiểm tra ngữ cảnh → ghi vị trí nguồn |
| **Bottleneck** | Dò PDF để tìm lại bằng chứng, với mốc 6 phút trong tổng 10 phút/lần ở Card #1 và CP5. Tôi giữ lưu ý từ CP4: cần phân biệt thiếu vị trí nguồn với khó hiểu ngữ cảnh. |
| **Impact** | Với mốc 3 lượt/tuần, tổng thời gian là 30 phút, trong đó dò PDF chiếm 18 phút. Khi thiếu nguồn, tôi khó giải thích nhận định với nhóm và mentor. |
| **Success Metric** | Từ mốc trung bình 10 phút/lần, ít nhất 9/10 tác vụ tìm đúng nguồn, đúng ngữ cảnh trong tối đa 3 phút. Trong pilot 4 tuần với 10 tác vụ, tôi sẽ bấm giờ từ mở ghi chú đến xác minh và ghi nguồn, tính cả lượt thất bại. Tôi ghi riêng công bổ sung ghi chú; tổng thời gian gồm chuẩn bị phải thấp hơn tổng thời gian tìm thủ công cho cùng bộ tác vụ. |
| **Boundary** | Tôi đối chiếu nội dung và ngữ cảnh trong PDF trước khi dùng bằng chứng; không dùng AI tạo trích dẫn hoặc tự kết luận paper chứng minh điều gì. Nếu nguồn sai hoặc mất, tôi quay về tìm thủ công; chưa xác minh được thì ghi rõ và không dùng nhận định đó. |
| **AI intervention point** | Không có; tôi dùng ghi chú có vị trí nguồn và tính năng Zotero |
| **Mức chọn** | No AI |
| **Rủi ro & người kiểm tra** | Liên kết sai, thiếu ngữ cảnh, tăng công ghi chú. Tôi kiểm tra mỗi lần sử dụng; khi đánh giá, tôi nhờ một thành viên khác đối chiếu với PDF. |

### 7.2. Tôi thay đổi gì so với v0

| Trường | v0 trong CP5 | v1 | Vì sao tôi đổi |
|---|---|---|---|
| Actor | Sinh viên đọc và so sánh paper | Giới hạn paper đã đọc, có PDF gốc | Giữ phạm vi tìm lại bằng chứng |
| Impact | 30–40 phút/tuần cho 3–4 lượt | Dùng mốc 30 phút/tuần cho 3 lượt | Thống nhất với CP1–CP2 và CP4 |
| Success Metric | 10 → tối đa 3 phút/lần, đúng đoạn và ngữ cảnh | Ít nhất 9/10 tác vụ đạt trong pilot 4 tuần; tính ngoại lệ và tổng công ghi chú | Đánh giá cả bộ tác vụ, không bỏ qua lượt tìm thủ công hoặc công chuẩn bị |
| Boundary | Ưu tiên Zotero; AI có thể thử sau | Chọn No AI, giữ kiểm tra PDF và cách quay về | Phù hợp với phương án tôi chọn |

### 7.3. Tiêu chí đánh giá

Tôi dùng 5 tiêu chí cho phương án ghi chú và truy xuất nguồn:

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đúng nguồn | Đúng paper và vị trí trang/hình/bảng/đoạn | Nhầm paper, phiên bản hoặc vị trí |
| 2 | Đúng bằng chứng | Nội dung thực sự hỗ trợ nhận định | Chỉ trùng từ khóa hoặc không hỗ trợ nhận định |
| 3 | Giữ đúng ngữ cảnh | Giữ đúng đối tượng, điều kiện và giới hạn | Bỏ điều kiện hoặc khái quát vượt bằng chứng |
| 4 | Xử lý nguồn thiếu/lỗi | Ghi rõ chưa xác minh, quay về PDF gốc | Dùng nguồn chưa kiểm tra hoặc tự tạo nguồn |
| 5 | Thời gian | Tìm và xác minh đúng trong tối đa 3 phút | Quá 3 phút hoặc chưa xác minh được |

Tôi tính một lượt đạt khi đáp ứng tiêu chí 1–3 và 5. Nếu nguồn thiếu hoặc lỗi, tôi áp dụng thêm tiêu chí 4. Lượt chưa xác minh được vẫn tính vào tổng 10 tác vụ và không được tính là thành công.

### 7.4. Tổng hợp dữ liệu đánh giá

**[DỮ LIỆU MÔ PHỎNG — CHƯA KIỂM CHỨNG]** Bảng này là dữ liệu mô phỏng do CP6 khai báo, không phải kết quả pilot đã thực hiện. Pilot 4 tuần ở mục 8.2 vẫn là kế hoạch. Các giá trị 3,06 phút, 9/10, 10/10 và 40,6 phút được giữ nguyên theo nguồn.

| Chỉ số | Giá trị |
|---|---|
| Trung bình trước cải thiện | 10 phút/tác vụ; trong đó dò PDF 6 phút |
| Trung bình sau cải thiện, gồm kiểm tra ngữ cảnh và ngoại lệ | 3,06 phút/tác vụ |
| Đúng nguồn, đúng ngữ cảnh và tối đa 3 phút | 9/10 tác vụ |
| Đúng nguồn/ngữ cảnh sau cả bước quay về thủ công | 10/10 tác vụ |
| Công bổ sung ghi chú | 10 phút cho 10 tác vụ |
| Tổng thời gian tìm | 100 → 30,6 phút |
| Tổng sau cải thiện, gồm công bổ sung ghi chú | 40,6 phút |

Tôi tính cả lượt mất 4,5 phút do liên kết hỏng. Vì vậy, trung bình là 3,06 phút, còn tỷ lệ đạt ngưỡng 3 phút là 9/10. Với các lượt đã có vị trí nguồn, tôi vẫn tính thời gian đọc lại ngữ cảnh.

Tính cả 10 phút bổ sung ghi chú, tổng thời gian là 40,6 phút so với 100 phút ban đầu.

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

Tôi đánh giá rủi ro ở phạm vi thiết kế pilot nhỏ:

| Rủi ro | Mức độ | Lý do |
|---|---|---|
| **Value** | Trung bình | Tôi mới dựa vào một trường hợp, chưa mở rộng kết luận sang người dùng khác |
| **Usability** | Trung bình | Tôi phải duy trì ghi chú, đọc ngữ cảnh và xử lý liên kết hỏng |
| **Feasibility** | Thấp | Tính năng cần dùng đã có; quy trình rõ, chưa cần xây mô hình hoặc hệ thống riêng |
| **Viability** | Thấp | Tôi dùng công cụ hiện có; tính cả công ghi chú, tổng thời gian trong bộ dữ liệu vẫn thấp hơn trước |

### 8.2. Kết luận

**[CẦN NHÓM XÁC NHẬN]** CP6 ghi lựa chọn của tác giả là Go cho pilot nhỏ dùng No AI, không phải Go triển khai AI. Chưa có biên bản xác nhận quyết định chung trong ba file nguồn. Giữ nguyên kết luận và pilot của CP6 bên dưới.

**Tôi chọn Go với thiết kế pilot nhỏ dùng No AI.** Ở phạm vi này, hai rủi ro Trung bình là giá trị sử dụng và khả năng duy trì ghi chú; tôi sẽ đánh giá chúng trong pilot. Phương án dùng công cụ có sẵn, chưa cần xây hệ thống mới. Tôi giữ việc kiểm tra PDF trước khi dùng bằng chứng và chưa mở rộng sang người dùng khác.

**Pilot tôi đề xuất:** Trong 4 tuần, tôi chọn 10 tác vụ từ 5 paper đã đọc, gồm đoạn văn, hình và bảng. Tôi sẽ dùng mẫu ghi chú có nhận định, vị trí nguồn, annotation/liên kết và ngữ cảnh; ghi lại thời gian, đúng/sai, ngoại lệ và công chuẩn bị. Một thành viên khác đối chiếu bằng chứng với PDF theo 5 tiêu chí; tôi so sánh tổng thời gian với cách tìm thủ công trên cùng bộ tác vụ.

**Ngưỡng dừng:**

- Sau 4 tuần, nếu chưa đủ 10 tác vụ hoặc dưới 9/10 tác vụ đạt đủ tiêu chí, tôi chưa mở rộng mà quay về tìm thủ công và sửa ghi chú.
- Nếu công chuẩn bị lớn hơn hoặc bằng thời gian tiết kiệm, tôi thu hẹp các nhận định cần lưu nguồn.
- Nếu có bằng chứng sai được dùng trước khi đối chiếu PDF, tôi dừng để sửa bước kiểm tra.

---

## 9. Hạn chế và hướng tiếp theo

### 9.1. Những điểm cần nhóm xác nhận

| Nội dung | Ghi nhận từ nguồn | Việc còn thiếu / cần xác nhận |
|---|---|---|
| Kiểm chứng người dùng (C7) | CP4 rà soát một card và có bộ câu hỏi; chưa có mẫu phỏng vấn hoặc survey. | **[CHƯA KIỂM CHỨNG]** Cần dữ liệu người thật, nguồn và cách thu thập; ghi cả tín hiệu phản bác và thay đổi problem sau kiểm chứng. |
| Baseline và dữ liệu đánh giá (C7, C9) | CP3 nêu thời gian trong card là giả định. CP6 khai báo dữ liệu mô phỏng; pilot 4 tuần mới được đề xuất. | Không dùng các bảng mô phỏng làm bằng chứng thực nghiệm. Chưa có log đo từng tác vụ hoặc bộ 10 tác vụ/đáp án tham chiếu đính kèm. |
| Actor (C8, C9) | CP4 dùng Rachal; v0 của CP5 dùng Lam; v1 của CP6 dùng “tôi”. | **[CẦN NHÓM XÁC NHẬN]** Thống nhất actor và bối cảnh; chưa xác định đây là cùng một trường hợp thực tế. |
| Bước thủ công và mức can thiệp (C8, C10) | CP5 ghi 2/4 bước thủ công nhưng gắn nhãn CON NGƯỜI ở ba bước; annotation/page link được ghi RULE. CP6 gọi phương án dùng Zotero là No AI. | **[CẦN NHÓM XÁC NHẬN]** Làm rõ cách đếm bước và phân loại mức can thiệp, không tự sửa số liệu nguồn. |
| Quy trình chi tiết (C8) | CP5 có sơ đồ ASCII, thời gian giả định, boundary, fallback và bảng before/after. | Chưa có bảng actor/input/output/handoff cho từng bước và quan sát xác nhận quy trình. |
| Độ phức tạp (C10) | CP6 chọn “mơ hồ thấp, phức tạp thấp”; quy trình có 4–5 bước. Worksheet có gợi ý 3+ bước nối tiếp khi xét độ phức tạp cao. | **[CẦN NHÓM XÁC NHẬN]** Giải thích cách áp dụng tiêu chí độ phức tạp cho phạm vi này; chưa tự đổi ô ma trận. |
| Phạm vi và metric v0 → v1 (C9) | CP5 dùng 3–4 lượt, 30–40 phút/tuần; CP6 thu về 3 lượt, 30 phút/tuần và ghi lý do tại mục 7.2. | Giữ cả hai phiên bản để truy vết; nhóm cần xác nhận phạm vi và đo baseline thật trước khi đánh giá target. |
| Quyết định và pilot (C11) | CP6 ghi Go cho pilot No AI, có bốn rủi ro và ngưỡng dừng. | **[CẦN NHÓM XÁC NHẬN]** Chốt quyết định chung, người thực hiện và người đối chiếu PDF; không coi pilot là đã chạy hoặc lựa chọn cá nhân là đồng thuận của nhóm. |

### 9.2. Ghi nhận sử dụng AI trong CP6

Tôi dùng AI để đối chiếu CP1–CP5, tạo bộ dữ liệu, kiểm tra phép tính và phản biện lập luận. Phần phản biện tập trung vào ba điểm: mở đúng trang chưa đủ để hiểu đúng ngữ cảnh, phải tính công ghi chú và không bỏ qua lượt tìm quá ngưỡng thời gian.

---

## 10. Tài liệu tham khảo

- [CP1–CP2](../individual/2A202604020_NguyenDucKhuongLam.md), [CP3](group_report.md), [shortlist](shortlist.md), [CP5](CP5.md).
- [CP4](https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming/blob/169d1927dce2f72cae879ac35dc90e8575901c3f/report/team/CP4.md).
- [Worksheet](../../docs/01-worksheet.md), [checklist](../../CHECKPOINTS.md), [rubric](../../RUBRIC.md).
- [Zotero PDF Reader](https://www.zotero.org/support/pdf_reader), [Zotero Notes](https://www.zotero.org/support/notes), [Adobe Searching PDFs](https://helpx.adobe.com/acrobat/using/searching-pdfs.html).
- File nguồn tích hợp: [CP4.md](CP4.md), [CP5.md](CP5.md), [CP6.md](CP6.md).
