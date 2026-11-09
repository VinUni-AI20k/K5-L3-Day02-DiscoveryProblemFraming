# CP6 — Mức can thiệp, Problem Statement v1 và quyết định

Tôi tập trung vào việc tìm lại bằng chứng trong paper đã đọc để giải thích nhận định có căn cứ. Từ [CP4](https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming/blob/169d1927dce2f72cae879ac35dc90e8575901c3f/report/team/CP4.md) và [quy trình ở CP5](CP5.md), tôi so sánh các mức can thiệp, xác định tiêu chí đánh giá và chọn hướng tiếp tục.

**Nguồn số liệu:** Dữ liệu mô phỏng phục vụ bài lab, dựa trên CP1–CP5.

## 6. Mức can thiệp AI

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Tôi xếp bài toán vào ô **mơ hồ thấp, phức tạp thấp**. Paper đã được chọn, các bước tìm và kiểm tra nguồn tương đối rõ. Tôi có thể đối chiếu kết quả với PDF để biết bằng chứng có đúng vị trí và hỗ trợ nhận định hay không.

Điểm tôi cần giữ lại là bước đọc ngữ cảnh: mở đúng trang chưa có nghĩa là hiểu đúng kết quả.

### 6.2. So sánh No AI / Rule / Workflow / Agent

| Mức | Phương án | Đủ khi nào | Rủi ro | Lựa chọn của tôi |
|---|---|---|---|---|
| **No AI** | Ghi chú kèm nhận định, trang/hình/bảng, annotation và ngữ cảnh; mở lại bằng liên kết Zotero | Ghi chú dẫn về đúng nguồn, tôi kiểm tra được nội dung | Thiếu vị trí, liên kết hỏng, hiểu sai ngữ cảnh | Chọn |
| **Rule** | Script kiểm tra trường nguồn còn thiếu và tìm từ khóa theo quy tắc | Có nhiều thao tác lặp cần tự động hóa | Đủ trường nhưng sai nguồn; từ khóa không khớp nhận định | Chưa cần script riêng |
| **Workflow** | Nhận định + PDF → AI gợi ý đoạn kèm vị trí → tôi đối chiếu | Cách ghi chú và tìm kiếm đơn giản chưa đáp ứng nhu cầu | Đoạn liên quan nhưng không hỗ trợ nhận định | Chưa chọn |
| **Agent** | AI tự chọn công cụ, nguồn và bước tìm tiếp theo | Các bước tìm kiếm chưa xác định trước | Phạm vi rộng, thêm chi phí và khó kiểm tra nguồn | Không chọn |

**Tôi chọn No AI.** Tôi sẽ ghi vị trí nguồn ngay trong ghi chú và dùng liên kết Zotero để mở lại. Nếu liên kết thiếu hoặc hỏng, tôi tìm trong PDF rồi bổ sung vị trí vừa tìm được.

Lý do là cách này xử lý trực tiếp bước dò PDF trong CP2–CP5. CP4 cho thấy công cụ đã có tính năng phù hợp, còn tôi chưa có căn cứ để thêm AI. No AI cũng là mức đơn giản nhất để bắt đầu. Mốc 3 phút được giữ làm mục tiêu đánh giá từ CP5.

### 6.3. AI Canvas rút gọn

Tôi không dùng AI để dự đoán hoặc tạo nội dung trong phương án này, nên không điền AI Canvas theo hướng dẫn dành cho mức No AI. Việc xác nhận bằng chứng vẫn do tôi thực hiện.

### 6.4. Hai câu hỏi Google PAIR

Với mức No AI, tôi không cần điền phần này. Nếu chuyển sang Workflow/Agent, tôi sẽ làm rõ người dùng muốn được hỗ trợ hay giao việc, và kiểu sai nào gây hậu quả nặng hơn.

## 7. Problem Statement v1 và tiêu chí đánh giá

### 7.1. Problem Statement v1

| Trường | Nội dung |
|---|---|
| **Actor** | Tôi, trong vai sinh viên mới tham gia nhóm nghiên cứu, cần dùng lại nhận định từ paper đã đọc và có PDF gốc |
| **Quy trình** | Mở ghi chú → xác định paper → tìm bằng chứng → kiểm tra ngữ cảnh → ghi vị trí nguồn |
| **Bottleneck** | Dò PDF để tìm lại bằng chứng, với mốc 6 phút trong tổng 10 phút/lần ở Card #1 và CP5. Tôi giữ lưu ý từ CP4: cần phân biệt thiếu vị trí nguồn với khó hiểu ngữ cảnh. |
| **Impact** | Với mốc 3 lượt/tuần, tổng thời gian là 30 phút, trong đó dò PDF chiếm 18 phút. Khi thiếu nguồn, tôi khó giải thích nhận định với nhóm và mentor. |
| **Success Metric** | Từ mốc trung bình 10 phút/lần, ít nhất 9/10 tác vụ tìm đúng nguồn, đúng ngữ cảnh trong tối đa 3 phút. Khi áp dụng, tôi sẽ bấm giờ từ mở ghi chú đến xác minh và ghi nguồn, tính cả lượt thất bại; công bổ sung ghi chú được ghi riêng. |
| **Boundary** | Tôi đối chiếu nội dung và ngữ cảnh trong PDF trước khi dùng bằng chứng. Nếu nguồn sai hoặc mất, tôi quay về tìm thủ công; không kết luận chỉ từ annotation. |
| **AI intervention point** | Không có; tôi dùng ghi chú có vị trí nguồn và tính năng Zotero |
| **Mức chọn** | No AI |
| **Rủi ro & người kiểm tra** | Liên kết sai, thiếu ngữ cảnh, tăng công ghi chú. Tôi kiểm tra mỗi lần sử dụng; khi đánh giá, tôi nhờ một thành viên khác đối chiếu với PDF. |

### 7.2. Tôi thay đổi gì so với v0

| Trường | v0 trong CP5 | v1 | Vì sao tôi đổi |
|---|---|---|---|
| Actor | Sinh viên đọc và so sánh paper | Giới hạn paper đã đọc, có PDF gốc | Giữ phạm vi tìm lại bằng chứng |
| Impact | 30–40 phút/tuần cho 3–4 lượt | Dùng mốc 30 phút/tuần cho 3 lượt | Thống nhất với CP1–CP2 và CP4 |
| Success Metric | 10 → tối đa 3 phút/lần, đúng đoạn và ngữ cảnh | Ít nhất 9/10 tác vụ đạt cả thời gian và chất lượng; tính ngoại lệ và công ghi chú | Đánh giá cả bộ tác vụ, không bỏ qua lượt phải tìm thủ công |
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

Tôi tính một lượt đạt khi đáp ứng tiêu chí 1–3 và 5. Nếu nguồn thiếu hoặc lỗi, tôi áp dụng tiêu chí 4; chỉ tính thành công sau khi xác minh được bằng chứng.

### 7.4. Tổng hợp dữ liệu đánh giá

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

## 8. Quyết định

### 8.1. Bốn rủi ro

Tôi đánh giá rủi ro ở phạm vi thiết kế pilot nhỏ:

| Rủi ro | Mức độ | Lý do |
|---|---|---|
| **Value** | Trung bình | Tôi mới dựa vào một trường hợp, chưa mở rộng kết luận sang người dùng khác |
| **Usability** | Trung bình | Tôi phải duy trì ghi chú, đọc ngữ cảnh và xử lý liên kết hỏng |
| **Feasibility** | Thấp | Tính năng cần dùng đã có; quy trình rõ, chưa cần xây mô hình hoặc hệ thống riêng |
| **Viability** | Thấp | Tôi dùng công cụ hiện có; tính cả công ghi chú, tổng thời gian trong bộ dữ liệu vẫn thấp hơn trước |

### 8.2. Kết luận

**Tôi chọn Go với thiết kế pilot nhỏ dùng No AI.** Phạm vi bài toán gọn, công cụ có sẵn và chưa có lý do tăng mức can thiệp. Tôi giữ việc kiểm tra PDF trước khi dùng bằng chứng.

**Pilot tôi đề xuất:** 10 tác vụ từ 5 paper đã đọc, gồm đoạn văn, hình và bảng. Tôi sẽ dùng mẫu ghi chú có nhận định, vị trí nguồn, annotation/liên kết và ngữ cảnh; ghi lại thời gian, đúng/sai, ngoại lệ và công chuẩn bị.

**Ngưỡng dừng:**

- Nếu dưới 9/10 tác vụ đạt đủ tiêu chí, tôi chưa mở rộng mà quay về tìm thủ công và sửa ghi chú.
- Nếu công chuẩn bị lớn hơn thời gian tiết kiệm, tôi thu hẹp các nhận định cần lưu nguồn.
- Nếu có bằng chứng sai được dùng trước khi đối chiếu PDF, tôi dừng để sửa bước kiểm tra.

## Tôi dùng AI ở đâu

Tôi dùng AI để đối chiếu CP1–CP5, tạo bộ dữ liệu, kiểm tra phép tính và phản biện lập luận. Phần phản biện tập trung vào ba điểm: mở đúng trang chưa đủ để hiểu đúng ngữ cảnh, phải tính công ghi chú và không bỏ qua lượt tìm quá ngưỡng thời gian.

## Tài liệu tham khảo

- [CP1–CP2](../individual/2A202604020_NguyenDucKhuongLam.md), [CP3](group_report.md), [shortlist](shortlist.md), [CP5](CP5.md).
- [CP4](https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming/blob/169d1927dce2f72cae879ac35dc90e8575901c3f/report/team/CP4.md).
- [Worksheet](../../docs/01-worksheet.md), [checklist](../../CHECKPOINTS.md), [rubric](../../RUBRIC.md).
- [Zotero PDF Reader](https://www.zotero.org/support/pdf_reader), [Zotero Notes](https://www.zotero.org/support/notes), [Adobe Searching PDFs](https://helpx.adobe.com/acrobat/using/searching-pdfs.html).
