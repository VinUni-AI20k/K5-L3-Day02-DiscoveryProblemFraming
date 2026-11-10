# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: I3
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Phạm vi phát triển hướng tới: Tất cả các tuyến xe buýt và các khung giờ di chuyển.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Nhật Minh | Khi chờ xe buýt, tôi muốn biết mức đông của các chuyến phù hợp với hành trình để chủ động chọn chuyến trong thời gian có thể chờ. | Hành khách trên các tuyến xe buýt, trong đó có Minh. | Bước chờ xe chưa có thông tin về mức đông của các chuyến. Trong trải nghiệm của Minh trên E03, thời gian chờ khoảng 20 phút; chưa tách được thời gian phát sinh do lựa chọn chuyến. | Bạn đã từng bỏ chuyến đông để chờ chuyến sau chưa? Nếu có thông tin về độ đông, bạn sẵn sàng chờ thêm bao lâu? **Người hỏi:**  Nguyễn Minh Quang |
| 2 | Nguyễn Nhật Minh | Khi cân nhắc 2 phòng trọ đã biết giá và các khoản phí, tôi muốn so sánh tổng chi phí hằng tháng để chọn phòng phù hợp ngân sách. | Người tìm phòng trọ, trong đó có Minh. | Bước ước tính và quy đổi các khoản phí thành tổng chi phí có thể so sánh; toàn bộ quá trình khoảng 5 phút, chưa đo riêng bước này. | Bước nào khiến bạn khó tính nhất? **Người hỏi:** Nguyễn Minh Quang |
| 3 | Nguyễn Nhật Minh | Khi thu quỹ lớp qua chuyển khoản, tôi muốn xác định đúng người đóng từng khoản để ghi nhận chính xác và hạn chế hỏi lại. | Thủ quỹ lớp và các thành viên đóng quỹ. | Bước tìm và xác minh tên người đóng khi giao dịch thiếu họ tên. Lần thu của Minh mất khoảng 120 phút tổng cộng; phần dò tên/hỏi lại nằm trong khoảng 60 phút cuối, chưa tách thời gian riêng. | Trong lần thu gần nhất, có bao nhiêu khoản thiếu tên và bạn đã xác minh người gửi như thế nào để tránh ghi nhầm? **Người hỏi:**  Hoàng Đức An |
| 4 | Nguyễn Minh Quang | Khi nhận tài liệu môn học hoặc requirement đồ án dài, tôi muốn nắm ý chính và các phần việc cần làm để hiểu yêu cầu và phân công công việc. | Sinh viên CNTT hoặc trưởng nhóm đồ án. | Bước đọc chi tiết và trích xuất yêu cầu từ tài liệu dài 10–20 trang, khoảng 45 phút. | Bạn kiểm tra thế nào để không bỏ sót yêu cầu? **Người hỏi:** Nguyễn Nhật Minh |
| 5 | Nguyễn Minh Quang | Khi xử lý lỗi liên quan đến luồng dữ liệu realtime, tôi muốn đối chiếu log backend từ nhiều nguồn để tìm nguyên nhân nhanh hơn. | Lập trình viên backend. | Bước dò timestamp và so khớp sự kiện giữa các nguồn log thủ công, khoảng 25 phút. | Gom log theo timestamp đã đủ để tìm lỗi chưa? **Người hỏi:** Hoàng Đức An |
| 6 | Nguyễn Minh Quang | Khi nghe podcast về System Design trên đường đi, tôi muốn ghi lại các từ khóa và kiến trúc chính để ôn tập mà không phải tua lại nhiều lần. | Sinh viên CNTT tự học qua podcast. | Bước nhớ lại nội dung và tua lại đoạn audio đã quên, khoảng 25 phút. | Bạn làm sao để ghi đủ các ý quan trọng? **Người hỏi:** Nguyễn Nhật Minh |
| 7 | Hoàng Đức An | Khi kết thúc buổi họp, tôi muốn nắm các nội dung chính và đầu việc để không quên nội dung và giảm thời gian xem lại. | CEO và nhân viên văn phòng tham gia cuộc họp. | Bước nghe lại bản ghi, đọc ghi chú và xác định đầu việc sau họp, ước tính khoảng 30–60 phút/cuộc họp. | Ai kiểm tra lại các đầu việc sau họp? **Người hỏi:** Nguyễn Minh Quang |
| 8 | Hoàng Đức An | Khi khách hàng gửi yêu cầu hỗ trợ, tôi muốn xác định đúng loại yêu cầu và bộ phận phụ trách để giảm thời gian xử lý thủ công. | Nhân viên chăm sóc khách hàng và quản lý dịch vụ. | Bước đọc, xác định vấn đề và phân loại yêu cầu, khoảng 5 phút/yêu cầu theo Problem Card. | Có bao nhiêu ticket bị chuyển sai bộ phận? **Người hỏi:** Nguyễn Nhật Minh |
| 9 | Hoàng Đức An | Khi cần mua hoặc thuê căn hộ, tôi muốn tìm những căn phù hợp ngân sách, vị trí, diện tích và tiện ích để giảm công sức tìm kiếm và so sánh. | Người tìm mua hoặc thuê căn hộ. | Bước lọc căn hộ và kiểm tra tình trạng còn bán hoặc cho thuê, khoảng 5 phút/lần theo phần bottleneck của Problem Card. | Mốc 5 phút và 20–45 phút khác nhau thế nào? **Người hỏi:** Nguyễn Minh Quang |


### 2.2. Cluster

### Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tóm tắt & Rút trích thông tin | Tóm tắt tài liệu môn học (#4), Tóm tắt kiến thức từ Podcast (#6), Tóm tắt nội dung họp (#7) | Cần xử lý một lượng thông tin dài (text/audio), rút ra các ý chính và action items để tiết kiệm thời gian đọc/nghe. |
| B — Đưa ra quyết định & So sánh | Khó chọn chuyến buýt E03 (#1), Khó so sánh chi phí 2 phòng trọ (#2), Tìm căn hộ theo tiêu chí (#9) | Cần đối chiếu nhiều biến số (độ đông đúc, thời gian, chi phí, tiện ích) để đưa ra lựa chọn hoặc đề xuất tối ưu nhất. |
| C — Đối chiếu & Phân loại dữ liệu | Thủ quỹ đối chiếu chuyển khoản (#3), Gom log realtime tra cứu bug (#5), Phân loại ticket CSKH (#8) | Xử lý dữ liệu nhiễu hoặc rời rạc (tên viết tắt, log rác, yêu cầu khách hàng) để khớp đúng người, đúng chỗ hoặc gom về một nơi. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Tăng tỷ lệ lượt đi xe buýt mà hành khách chọn được chuyến có mức đông phù hợp trong thời gian có thể chờ.
├── Opportunity: Hành khách chưa biết mức đông của chuyến xe trước khi xe đến điểm đón.
├── Opportunity: Khó cân nhắc lên chuyến hiện tại hay chờ chuyến sau khi chưa biết mức đông của chuyến sau.
└── Opportunity: Hành khách cần chọn chuyến phù hợp với khoảng thời gian có thể chờ.
```

Baseline cần được ghi nhận theo tuyến và khung giờ; mức đông được xem là phù hợp cần được làm rõ khi kiểm chứng.

Ví dụ giải pháp không đưa vào các nhánh opportunity: ứng dụng hiển thị độ đông, AI dự báo số hành khách.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **1. Khó chọn chuyến xe buýt E03 theo độ đông** | 5 | 5 | 5 | 5 | 4 | 5 | 5 | **34** |
| **2. Khó so sánh chi phí của 2 phòng trọ**  | 3 | 5 | 4 | 2 | 5 | 4 | 5 | **28** |
| **3. Thủ quỹ đối chiếu chuyển khoản thiếu tên**  | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| **4. Tóm tắt tài liệu môn học / requirement**  | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| **5. Gom log realtime tra cứu bug**  | 5 | 4 | 4 | 4 | 3 | 4 | 4 | **28** |
| **6. Tóm tắt kiến thức từ Podcast**  | 3 | 4 | 3 | 3 | 4 | 4 | 5 | **26** |
| **7. Tóm tắt Nội dung họp**  | 5 | 3 | 5 | 4 | 4 | 4 | 5 | **30** |
| **8. CSKH: Phân loại và chuyển đúng bộ phận**  | 3 | 3 | 4 | 4 | 3 | 4 | 3 | **24** |
| **9. Tìm căn hộ theo tiêu chí khách hàng**  | 4 | 3 | 3 | 3 | 3 | 4 | 3 | **23** |

---

**Candidate được chọn:**
**#1. Khó chọn chuyến xe buýt E03 theo mức độ đông** (của Minh).

**Vì sao chọn:**
- **Nỗi đau thật, tần suất cao:** Hầu hết sinh viên trong nhóm đều gặp cảnh chờ 20 phút rồi phải chen chúc trên tuyến E03 khung 7h-8h sáng. Impact (thời gian chờ, sự mệt mỏi) là rất rõ ràng và dễ phỏng vấn user.
- **Có đất để so sánh các mức AI:** Bài toán này rất tuyệt vời để so sánh: No AI (nhìn app GPS thường), Rule (đặt ngưỡng Fix: >40 người là đông), và AI/ML (Mô hình dự đoán độ đông theo thời gian, trạm, thời tiết).
- **Rủi ro dữ liệu đã có lời giải:** Nhóm chọn phương án dùng *Dữ liệu giả lập (Mock Data)* dựa trên quan sát thực tế và đóng vai là team Product nội bộ của hãng xe buýt. Điều này biến ý tưởng từ "bất khả thi" thành một bài toán Data/ML cực kỳ vừa sức cho thời gian làm lab.

**Vì sao loại các candidate còn lại:**
- Bài *Tóm tắt tài liệu (#4)* và *Thủ quỹ (#3)* có số điểm tương đương (34 điểm). Tuy nhiên, bài "Thủ quỹ" có tần suất diễn ra ít (1-2 lần/kỳ), còn bài "Tóm tắt tài liệu" lại hơi cá nhân. Nhóm muốn chọn bài toán Xe buýt (#1) vì nó mang tính cộng đồng cao, có chứa thách thức về mặt Xử lý Dữ liệu (Data Pipeline) và Machine Learning dự đoán - cực kỳ phù hợp với một đồ án ứng dụng AI.

**Xử lý bất đồng (nếu có):**
Ban đầu nhóm e ngại bài E03 bị thiếu API dữ liệu số lượng khách thật (Feasibility rủi ro cao). Tuy nhiên, sau khi thống nhất hướng pivot: sử dụng thuật toán ML để dự đoán dựa trên dữ liệu quét thẻ giả lập (Mock Data tap-in), cả nhóm đều đồng ý đây là bài toán hay nhất, đủ chiều sâu để trình bày.

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Hành khách trên các tuyến xe buýt thường gặp chuyến đông và xem đây là khó khăn đáng giải quyết. | Value | 5 | 2 | Có — hỏi thêm hành khách ở nhiều tuyến, khung giờ và ghi nhận số lần gặp xe đông. |
| 2 | Biết mức đông trước có thể giúp hành khách điều chỉnh giờ đi hoặc cân nhắc chuyến khác trong thời gian có thể chờ. | Value | 5 | 2 | Có — kiểm tra hành vi thực tế, không chỉ hỏi ý định. |
| 3 | Có thể tiếp cận dữ liệu mức đông của từng chuyến trên các tuyến xe buýt trước khi xe đến điểm đón. | Feasibility | 5 | 1 | Có — kiểm tra ứng dụng hiện có, nguồn dữ liệu từ các đơn vị vận hành và mức độ bao phủ tuyến. |
| 4 | Thông tin mức đông có thể đủ chính xác và cập nhật kịp thời để hành khách lựa chọn. | Feasibility | 5 | 1 | Có — so sánh thông tin hiển thị với quan sát trên các chuyến thực tế. |
| 5 | Hành khách hiểu và sử dụng được các mức đông/vắng trước khi quyết định lên xe. | Usability | 3 | 1 | Kiểm tra sau khi có cách trình bày thông tin để thử. |
| 6 | Việc thu thập, chia sẻ và duy trì dữ liệu có thể thực hiện phù hợp với quyền truy cập và chi phí. | Viability | 4 | 1 | Có — xác minh quyền sử dụng dữ liệu và cách vận hành với nguồn cung cấp. |

*Điểm quan trọng và bằng chứng là đánh giá sơ bộ để nhóm thảo luận: 1 = thấp/ít bằng chứng, 5 = cao/nhiều bằng chứng.*

**Giả định đã thăm dò:** #1 và #2 qua quan sát của một thành viên đi E03 và trao đổi với 2 sinh viên đi xe buýt. Chưa ghi rõ tuyến của hai sinh viên; một người nêu ý định đi sớm, chưa có bằng chứng đã thực sự đổi giờ đi. Các giả định #3–#6 chưa được kiểm chứng trên các tuyến xe buýt trong phạm vi hướng tới.

### 3.2. Kiểm chứng

**Cách kiểm chứng:** Ngày 09/11/2026, nhóm hỏi trực tiếp trên lớp 2 sinh viên ngoài nhóm thường đi xe buýt đến trường. Nhóm cũng ghi nhận trải nghiệm đi E03 của một thành viên.

**Interview Snapshot 1**

| Trường | Nội dung |
|---|---|
| Người được hỏi | Sinh viên ngoài nhóm, đi xe buýt đến trường; chưa ghi rõ tuyến xe. |
| Thời điểm và cách hỏi | Ngày 09/11/2026, hỏi trực tiếp trên lớp. |
| Lần gần nhất | Chuyến xe bạn đi rất đông. |
| Cách xử lý | Vẫn lên xe vì không chắc chuyến sau có vắng hơn. Bạn chủ động căn thời gian ra điểm đón để không phải đợi lâu. |
| Ý chính | Bạn không biết chuyến sau có đông hay không.  |
| Insight | Thiếu thông tin về chuyến sau khiến bạn khó cân nhắc giữa lên xe đông và tiếp tục chờ. |

**Interview Snapshot 2**

| Trường | Nội dung |
|---|---|
| Người được hỏi | Sinh viên ngoài nhóm, đi xe buýt đến trường; chưa ghi rõ tuyến xe. |
| Thời điểm và cách hỏi | Ngày 09/11/2026, hỏi trực tiếp trên lớp. |
| Mức độ quan tâm | Bạn quan tâm xe có đông hay không và muốn biết trước mức độ đông. |
| Ý kiến | Bạn nói sẵn sàng đi sớm nếu biết có chuyến vắng hơn. |
| Lần gần nhất / thời gian chờ | Đi sáng nay/không cần đợi vì căn được giờ. |
| Insight | Thông tin về độ đông có thể giúp hành khách cân nhắc điều chỉnh giờ đi. |

**Tổng hợp:**

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Quan sát của thành viên đi E03 | 1 thành viên | Có chuyến đông và chuyến sau vắng hơn; chưa biết trước mức đông khi chờ xe. Thời gian chờ thường khoảng 20 phút theo ước lượng. | Chưa đủ bằng chứng kết luận thời gian chờ là do thiếu thông tin về độ đông. |
| Phỏng vấn trực tiếp trên lớp | 2 sinh viên ngoài nhóm | Một bạn không biết chuyến sau có vắng hơn không; bạn còn lại quan tâm độ đông và muốn biết trước. | Một bạn vẫn lên xe đông; bạn còn lại căn được giờ nên không phải đợi. Đây là tín hiệu cần xem lại mục tiêu giảm thời gian chờ; chưa đủ cơ sở kết luận họ sẽ chờ thêm để đi chuyến vắng. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Nhóm tập trung vào việc hành khách chưa biết trước mức đông của các chuyến xe buýt phù hợp với hành trình, nên khó chủ động chọn chuyến trong thời gian có thể chờ. Bài toán hướng tới tất cả các tuyến xe buýt. Phản hồi cho thấy cần xem xét cả việc điều chỉnh giờ đi, bên cạnh quyết định lên xe hay chờ chuyến sau.

**Cần hoàn thiện:** Bổ sung kiểm chứng ở nhiều tuyến và khung giờ, ghi rõ tuyến xe, thời gian chờ và tần suất gặp chuyến đông của từng người. Cần kiểm chứng thêm hành vi lựa chọn chuyến, điều chỉnh giờ đi và ghi tín hiệu phản bác nếu có. Dữ liệu hiện tại là bằng chứng ban đầu, chưa đủ để kết luận mức độ phổ biến của vấn đề trên tất cả các tuyến.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| BusMap | [Các tính năng](https://busmap.vn/tinh-nang/); [FAQ](https://busmap.vn/faq/) | Tra cứu tuyến và thời gian xe đến trước khi lên xe. | Trang tính năng mô tả lịch tuyến và thời gian chờ dựa trên GPS; FAQ nêu cách xem xe tại trạm. | Các trang đã đọc chưa mô tả mức đông theo từng chuyến; chưa kiểm tra trực tiếp mức độ hỗ trợ các tuyến xe trên ứng dụng. FAQ lưu ý dữ liệu Hà Nội phụ thuộc kết nối với các đơn vị vận hành. | Thử thông tin giờ đến sẵn có trên các tuyến trước; giờ xe đến không tự cho biết xe đông hay vắng. |
| Google Maps — dự báo độ đông | [Dự báo từ đóng góp hành khách](https://support.google.com/transitpartners/answer/9551309?hl=en); [Nguồn dữ liệu độ đông](https://support.google.com/transitpartners/answer/10106342?hl=en) | Hỗ trợ hành khách cân nhắc độ đông khi tra cứu chuyến đi, tùy nơi có dữ liệu. | Google mô tả dự báo từ phản hồi của người dùng; dữ liệu độ đông cũng có thể đến từ đơn vị vận tải hoặc dự báo nội bộ. | Dự báo không mặc nhiên là số đo thời gian thực; chưa kiểm tra các tuyến và khung giờ nào có hiển thị độ đông. | Kiểm tra mức độ bao phủ các tuyến trên công cụ có sẵn và đối chiếu với quan sát thực tế trước khi đề xuất xây mới. |
| Transit — thông tin độ đông chuyến sắp đến | [Hướng dẫn theo dõi chuyến](https://help.transitapp.com/article/445-how-to-track-departures-on-your-transit-line) | Hiển thị thời gian đến và mức đông của chuyến sắp đến tại khu vực được hỗ trợ. | Theo tài liệu Transit, dữ liệu độ đông có thể đến từ cảm biến của đơn vị vận tải hoặc phản hồi người đi xe. | Phụ thuộc khu vực và nguồn dữ liệu; chưa xác minh mức độ bao phủ các tuyến hoặc độ chính xác tại các điểm đón. | Tham khảo cách kết hợp nguồn dữ liệu và phản hồi hành khách; cần xác minh khả năng tiếp cận dữ liệu từ các tuyến và đơn vị vận hành. |

**Kết luận research:** Đã có công cụ hỗ trợ một phần việc xem giờ đến hoặc mức đông tại nơi có dữ liệu. Với mục tiêu hỗ trợ hành khách trên tất cả các tuyến xe buýt, nhóm cần kiểm tra mức độ bao phủ tuyến, nguồn dữ liệu độ đông và độ chính xác theo tuyến, khung giờ trước khi kết luận nên dùng công cụ sẵn có hay phát triển thêm.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

```text
    HIỆN TẠI — riêng thời gian chờ khoảng 20 phút/lượt (ước lượng)

    [1 Đến điểm đón E03: ? phút]

    → [2 Chờ xe, lướt điện thoại: khoảng 20 phút] ← BOTTLENECK: chưa biết mức đông
    
    → [3 Quan sát khi xe đến và lên xe: ? phút]

    ? phút = chưa đo riêng; 20 phút không phải tổng thời gian của toàn bộ hành trình.
    Chưa xác nhận việc bỏ chuyến đông để chờ chuyến sau.
```

| Bước | Actor                    | Input                                              | Output                                    | Thời gian / tần suất | Ghi chú                                                       |
| ---- | ------------------------ | -------------------------------------------------- | ----------------------------------------- | -------------------- | ------------------------------------------------------------- |
| 1    | Hành khách               | Đến điểm đón E03                                   | Có mặt tại điểm đón, sẵn sàng chờ xe      | Ngay khi đến         | Cần xác định đúng vị trí đón                                  |
| 2    | Hành khách               | Thời gian chờ xe, điện thoại cá nhân               | Tiếp tục chờ xe, theo dõi thời gian       | Khoảng 20 phút       | Bottleneck: Chưa biết mức độ đông đúc và thời gian xe đến     |
| 3    | Hành khách               | Xe đã đến, xác nhận đúng tuyến                     | Lên xe thành công                         | ? phút               | Phụ thuộc vào số lượng người lên xe và tình trạng xếp hàng    |

**Bottleneck**: Hành khách thiếu thông tin theo thời gian thực về thời gian xe đến và mức độ đông đúc tại điểm đón E03, dẫn đến thời gian chờ không chắc chắn và trải nghiệm di chuyển kém thuận tiện.

### 4.2. Quy trình tương lai

```text
    TƯƠNG LAI — 5 bước, khoảng 5 phút, 2/5 bước thủ công

    [1 Hành khách mở ứng dụng, chọn điểm đón E03: 1 phút] ← RULE (GPS / định vị)

    → [2 AI dự đoán thời gian xe đến (ETA): 5 giây] ← AI (GPS + dữ liệu giao thông)

    → [3 AI dự đoán mức độ đông đúc tại điểm đón: 2 phút] ← AI (dữ liệu hành khách + lịch sử)

    → [4 Ứng dụng hiển thị ETA, mức độ đông đúc và gửi thông báo: 1 phút] ← AI + RULE (cập nhật thông tin, thông báo tự động)

    → [5 Hành khách xác nhận đúng xe và lên xe: ? phút] ← CON NGƯỜI

    BOUNDARY: AI chỉ dự đoán thời gian xe đến và mức độ đông đúc dựa trên dữ liệu được cung cấp. AI không điều khiển xe, không đảm bảo còn chỗ và không tự quyết định việc lên xe thay hành khách.

    PHƯƠNG ÁN QUAY VỀ: Nếu AI không dự đoán được hoặc dữ liệu không chính xác → Ứng dụng hiển thị lịch trình xe và thông tin thời gian dự kiến theo phương pháp truyền thống; hành khách tự quan sát và chờ xe.

    Lưu ý: Tổng thời gian trên là mục tiêu thiết kế sơ bộ, chưa phải số liệu đo lường thực tế.
```

### 4.3. Before / after

| Chỉ số               | Trước                                                     | Sau (kỳ vọng)                                                        | Ghi chú                                                               |
| -------------------- | --------------------------------------------------------- | -------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Số bước              | 3                                                         | 5                                                                    | Quy trình được bổ sung các bước dự đoán và cung cấp thông tin bằng AI |
| Tổng thời gian       | Khoảng 20 phút chờ xe + thời gian di chuyển đến và lên xe | Khoảng 6 phút xử lý trên ứng dụng + thời gian di chuyển và lên xe    | Thời gian chờ thực tế có thể giảm nhờ chủ động lựa chọn thời điểm     |
| Số bước thủ công     | 3/3                                                       | 1/5                                                                  | Hành khách vẫn tự xác nhận xe và lên xe                               |
| Bottleneck chính     | Không biết thời gian xe đến và mức độ đông đúc            | Độ chính xác của dữ liệu GPS và mô hình dự đoán                      | Phụ thuộc vào chất lượng và tính cập nhật của dữ liệu                 |
| Rủi ro mới phát sinh | Chờ xe lâu, không biết tình trạng đông đúc                | AI dự đoán sai ETA hoặc mức độ đông đúc, dữ liệu GPS không chính xác | Cần có phương án dự phòng khi AI hoạt động không hiệu quả             |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Hành khách đi E03 buổi sáng |
| **Quy trình** | [1 Đến điểm đón E03: ? phút] → [2 Chờ xe, lướt điện thoại: khoảng 20 phút] ← BOTTLENECK: chưa biết mức đông → [3 Quan sát khi xe đến và lên xe: ? phút] |
| **Bottleneck** | Không biết thời gian xe đến và mức độ đông đúc |
| **Impact** | Đứng chờ xe mất 20 phút |
| **Success Metric** (baseline → target, cách đo) | Thời gian chờ 20 phút, mong muốn đạt 5 phút, đo bằng cách bắt đầu từ thời điểm chờ xe |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ dự đoán thời gian xe đến và mức độ đông đúc dựa trên dữ liệu được cung cấp. AI không điều khiển xe, không đảm bảo còn chỗ và không tự quyết định việc lên xe thay hành khách. |

**Phản biện nhận được**: Tại sao phải sử dụng AI thay vì thuật toán tính toán ETA thông thường? Nhóm không đồng ý, AI có thể xem được rất nhiều yếu tố để có thể đưa ra tính toán gần chính xác hơn

---

# 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ thấp, Độ phức tạp trung bình – cao**.

**Vì sao:**
- Độ mơ hồ thấp: Dầu vào (data tap-in, timestamp, trạm) rất rõ ràng, đầu ra cần một con số/phân loại cụ thể (Xanh/Vàng/Đỏ).
- Độ phức tạp trung bình – cao: Có quy luật nhưng đan xen nhiều biến số (người lên thì quẹt thẻ, người xuống không quẹt thẻ, phụ thuộc thời tiết, điểm kẹt xe, trạm trường học...). Không thể tính bằng công thức toán cộng trừ đơn giản.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Chỉ hiển thị vị trí GPS của xe trên app (như hiện tại). | Người dùng chỉ cần biết xe sắp tới chưa để chạy ra bến. | Không giải quyết được nỗi đau "lên xe bị nhồi nhét". | Không |
| **Rule** | Số người = Tổng số lượt tap-in trong chuyến. Đặt rule: >40 lượt là Đỏ (Đông). | Khi mọi người đều tap-out lúc xuống xe (ở VN gần như không có). | Số người chỉ tăng lên chứ không giảm xuống, xe đã trống nhưng app vẫn báo Đỏ. | Không |
| **Workflow (có ML)** | Rule gom log tap-in → ML dự đoán số người xuống để nội suy số người trên xe → Hiện cảnh báo màu trên app → Sinh viên tự quyết định. | Khi cần cân bằng giữa chi phí hệ thống và tính thực tiễn của dữ liệu (không cần camera). | Mô hình ML đoán sai lượng người xuống ở các trạm lớn. | **Chọn** |
| **Agent** | AI phân tích độ đông, tự động điều phối thêm xe buýt dự phòng từ trạm điều hành, hoặc tự book Grab cho khách. | Cần tự động hóa toàn bộ hệ thống giao thông công cộng. | Quá xa vời, chi phí khổng lồ, ngoài tầm kiểm soát của PM/User. | Không |

**Mức chọn:** Workflow (kết hợp Machine Learning / Predictive AI).

**Vì sao không chọn mức đơn giản hơn:** Mức Rule không thể giải bài toán khách xuống xe không quẹt thẻ. Bắt buộc phải có thuật toán Machine Learning học dữ liệu lịch sử để "nội suy" (ước lượng) lượng người xuống tại các trạm trọng điểm (VD: trạm Bách Kinh Xây).


### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Ước lượng số khách đang có trên xe và gán nhãn độ đông: Thoải mái (Xanh), Kín chỗ (Vàng), Quá tải (Đỏ). |
| **Judgment** — con người cân nhắc, quyết định gì? | Sinh viên nhìn nhãn màu, kết hợp với hoàn cảnh (có sắp muộn học không) để quyết định đi chuyến này hay đợi chuyến sau. |
| **Action** — hành động cuối cùng là gì, ai làm? | Sinh viên bước lên xe hoặc ở lại trạm (Người dùng làm). |
| **Outcome** — đo kết quả bằng gì? | Tỉ lệ sinh viên bị nhồi nhét giảm; Trải nghiệm đi xe buýt E03 thoải mái hơn. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Real-time log tap-in từ máy POS, Vị trí trạm hiện tại, Thời gian, Thứ trong tuần. (Giả định: Có sẵn từ Data Warehouse của VinBus). |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Nút report nhanh trên app: "Thực tế xe có đông không?" để người dùng feedback (Crowdsourcing phụ trợ). |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? 
  * Bằng chứng: Augment (Hỗ trợ). Sinh viên vẫn muốn tự ra quyết định. Nếu họ sắp thi cuối kỳ thì xe "Đỏ" cỡ nào họ cũng phải đu lên, AI không được quyền cấm họ lên xe hay tự ý hủy chuyến của họ.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
  * **Báo sót (App báo Xanh/Vắng, nhưng xe Đỏ/Đông) là tệ nhất.** Nếu báo vắng, sinh viên đợi chuyến sau, nhưng lên xe lại bị nhồi nhét, họ sẽ cảm thấy bị lừa và xóa app ngay.
  * Thiết kế xử lý: Mô hình ML sẽ được tinh chỉnh thiên về "An toàn" (tăng độ nhạy với dự đoán số người ở lại trên xe). Thà báo Vàng hơi lố một chút, còn hơn báo Xanh sai sự thật.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên NEU đi xe buýt E03 trong khung giờ cao điểm (7h - 8h sáng). |
| **Quy trình** | Mở app → Xem vị trí xe → (Mới) Xem độ đông đúc → Quyết định ra bến/lên xe/đợi chuyến sau. |
| **Bottleneck** | Quyết định mù mờ vì chỉ thấy vị trí GPS, dẫn đến việc thường xuyên bị kẹt trên những chuyến xe quá tải (mất 20 phút chịu đựng). |
| **Impact** | Trải nghiệm mệt mỏi, stress trước giờ học; không phân bổ được thời gian chờ hợp lý. |
| **Success Metric** (baseline → target, cách đo) | (1) Độ chính xác của phân loại độ đông đạt >80% so với thực tế (đo bằng log đối chiếu). (2) User đánh giá tính hữu ích >4/5 sao qua in-app survey. |
| **Boundary** | AI chỉ gợi ý mức độ đông đúc (Xanh/Vàng/Đỏ), không ép buộc hành vi người dùng, không can thiệp lộ trình xe. |
| **AI intervention point** | Tại màn hình hiển thị thông tin chuyến xe E03 đang đến gần trạm. |
| **Mức chọn** | Workflow (tích hợp ML Prediction). |
| **Rủi ro & người kiểm tra** | Model nội suy sai lượng người xuống dẫn đến sai lệch tích lũy. → Kỹ sư/PM kiểm tra lại model định kỳ bằng đối chiếu camera quay lén hoặc chốt kiểm tra thực tế. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Quy trình | Chỉ xem GPS rồi ra bến | Xem GPS + Độ đông rồi mới ra quyết định | Cập nhật bước can thiệp của AI vào hành trình người dùng. |
| Success Metric | Giảm thời gian chờ xe | Độ chính xác thuật toán >80% | Phản biện: Mục tiêu không phải là "chờ ít đi" (chờ chuyến vắng có khi lâu hơn), mà là "chủ động được quyết định dựa trên thông tin đúng". |

**Tiêu chí đánh giá đầu ra của AI (3 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Tính logic của con số | Số lượng người ước tính trên xe luôn ≥ 0 và ≤ 80 (sức chứa max của xe buýt). | Thuật toán trừ sai dẫn đến số người trên xe bị âm (-5). |
| 2 | Độ trễ hiển thị (Latency) | App cập nhật trạng thái màu trong dưới 3 giây kể từ khi xe rời trạm trước. | App load quá lâu (quay vòng vòng) do ML tính toán chậm. |
| 3 | Mức độ an toàn của dự đoán | Hạn chế tối đa False Negative (Thực tế đông mà báo vắng). | Tỉ lệ báo Xanh nhưng thực tế xe Đỏ vượt quá 10%. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Thấp (An toàn) | 100% sinh viên đi xe buýt đều sợ cảnh chen chúc, thông tin độ đông là tính năng họ khao khát nhất. |
| **Usability** | Người dùng có dùng được, có hiểu được đầu ra không? | Thấp (An toàn) | Giao diện hiển thị theo thang màu giao thông (Xanh/Vàng/Đỏ) hoặc icon hình người, ai cũng hiểu. |
| **Feasibility** | Có đủ dữ liệu, công cụ để làm không? | Trung bình | Có thể dùng Mock Data (dữ liệu giả lập) để train model trong phạm vi lab. Cần kiến thức cơ bản về Machine Learning Regression. |
| **Viability** | Có hợp chi phí, pháp lý không? Ai vận hành? | Trung bình | Trong thực tế, cần được VinBus/Tramoc mở API log POS. Chi phí huấn luyện model rẻ vì dữ liệu tabular (dạng bảng), không tốn GPU như LLM. |

### 8.2. Kết luận

**Quyết định:** Go (Phạm vi nhỏ / Pilot)

**Lý do:** Không có rủi ro nào ở mức CAO (Nguy hiểm). Bài toán có Value rất lớn, giải quyết được pain point có thật. Vấn đề Feasibility có thể xử lý bằng cách giới hạn phạm vi làm Pilot trên một tập dữ liệu giả lập.

**Nếu Go — pilot nhỏ nhất:**
- Tập trung DUY NHẤT vào tuyến E03, chỉ trong khung giờ 7h-9h sáng.
- Xây dựng tập Mock Data gồm 5000 dòng log tap-in giả lập.
- Train một model RandomForest/XGBoost đơn giản để test độ chính xác trước khi tích hợp vào UI.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):
Nếu test trên Mock Data mà model liên tục dự đoán ra số âm hoặc sai lệch tích lũy quá 30% (so với thực tế quan sát) → Dừng pilot AI, quay về hướng dùng Rule cứng (chỉ đếm số tap-in và cảnh báo nếu vượt ngưỡng).

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế:** Tập Mock Data do nhóm tạo ra có thể chưa phản ánh hết những biến động bất thường (như mưa lớn đột xuất, tắc đường sự cố).
- **Hướng tiếp theo:** 
  1. Tổ chức một chiến dịch thu thập Data thật trong 3 ngày (nhóm cử người đứng tại trạm Bách Kinh Xây ghi nhận lượng người lên/xuống) để đối chiếu với model.
  2. Bổ sung tính năng "Crowdsourcing": Cho phép sinh viên bấm nút báo cáo "Đông quá" ngay trên app để model ML tự động cập nhật lại trọng số.

## 10. Tài liệu tham khảo

- Google Maps Help - Hướng dẫn tính năng Độ đông đúc phương tiện công cộng (Transit Crowding).
- [Alighting Estimation for Smart Card Data] Các bài báo nghiên cứu về việc dùng Machine Learning nội suy số người xuống xe từ dữ liệu Tap-in.
