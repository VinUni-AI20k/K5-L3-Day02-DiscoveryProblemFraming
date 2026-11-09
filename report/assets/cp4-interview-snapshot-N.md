
# Interview Snapshot — CP4: Problem Validation

**Problem:** Đọc, trích xuất và đối chiếu thông tin chức năng từ tài liệu công khai của các hệ thống HIS/EHR/AI Agent.

**Interview ID:** P1  
**Trạng thái:** Chưa thực hiện — kế hoạch phỏng vấn  
**Phương pháp:** User Interview (Mom Test) kết hợp quan sát tác vụ thực tế.

## Interview snapshot — P1

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | **Chưa thực hiện/chưa cung cấp.** Đối tượng dự kiến: BA từng tham gia nghiên cứu hoặc so sánh hệ thống HIS/EHR/AI Agent. |
| Câu nói đáng nhớ nhất (nguyên văn) | Chưa có — chỉ ghi câu nói nguyên văn sau khi phỏng vấn thực tế. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Chưa xác minh. Cần hỏi về lần benchmarking gần nhất: hệ thống được nghiên cứu, số tài liệu, tiêu chí so sánh và kết quả đầu ra. |
| Hiện đang xử lý bằng cách nào (workaround)? | Chưa xác minh. Giả thuyết: tìm kiếm website/tài liệu nhà cung cấp, đọc thủ công, ghi chú và lập bảng so sánh. |
| Mất bao lâu, bao lần? | Ước lượng từ Problem Card: **150 phút/hệ thống**, trong đó **60 phút đọc và trích xuất**. Chưa có dữ liệu đo thực tế hoặc tần suất được xác nhận. |
| Insight / opportunity rút ra | Chưa kết luận. Cần xác định bottleneck thực sự nằm ở tìm tài liệu, đọc/trích xuất thông tin, chuẩn hóa tiêu chí hay xác minh nhận định. |

## Câu hỏi phỏng vấn — Mom Test

1. Lần gần nhất bạn phải so sánh hai hoặc nhiều hệ thống HIS/EHR/AI Agent là khi nào? Bạn đã thực hiện những bước gì?
2. Bạn sử dụng những nguồn tài liệu nào? Có phải chuyển qua nhiều website, brochure, tài liệu kỹ thuật hoặc demo không?
3. Bước nào mất nhiều thời gian nhất? Bạn có ghi nhận thời gian cho từng bước không?
4. Bạn ghi nhận chức năng và bằng chứng vào đâu? Đã từng phải quay lại tìm nguồn để xác minh chưa?
5. Lần gần nhất bạn không tìm được thông tin cần thiết là khi nào? Bạn đã xử lý như thế nào?
6. Khi hoàn thành bảng so sánh, những nhận định nào cần được kiểm chứng lại trước khi gửi cho PO/PM?

## Kế hoạch quan sát và đo lường

| Chỉ số | Cách đo |
|---|---|
| Thời gian thực hiện | Ghi nhận số phút cho từng bước trong quy trình AS-IS. |
| Số nguồn đã mở | Đếm số website, brochure, tài liệu kỹ thuật và nguồn khác đã sử dụng. |
| Tỷ lệ tiêu chí có bằng chứng | Số tiêu chí có nguồn kiểm chứng / tổng số tiêu chí được đánh giá. |
| Số nhận định phải chỉnh sửa | Ghi nhận số kết luận bị sửa sau khi review. |
| Bottleneck thực tế | Xác định bước chiếm nhiều thời gian nhất và nguyên nhân. |

**Thiết kế quan sát:** Chọn 2 hệ thống HIS/EHR/AI Agent và bộ 8–12 tiêu chí chung. Yêu cầu BA thực hiện quy trình hiện tại, ghi nhận thời gian và kết quả trước khi thử nghiệm bất kỳ phương án hỗ trợ nào.

## Tổng hợp tình trạng bằng chứng

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---|---|---|
| Báo cáo cá nhân BA | 1 báo cáo | Có quy trình 6 bước, ước lượng 150 phút/hệ thống và 60 phút đọc/trích xuất. | Chưa có log đo thực tế và chưa xác minh tần suất. |
| Tài liệu sản phẩm công khai: G2, Elicit, Consensus | 3 nguồn tham khảo | Có những công cụ hỗ trợ nghiên cứu, tìm kiếm và so sánh thông tin. | Chưa chứng minh các công cụ giải quyết đầy đủ workflow benchmarking HIS/EHR. |
| Phỏng vấn / quan sát tác vụ | 0 | Chưa có. | Chưa có. |

## Kết luận kiểm chứng

**Trạng thái:** Chưa đủ bằng chứng xác nhận problem.

Phạm vi tạm thời được thu hẹp từ "nghiên cứu thị trường hệ thống y tế" thành:

> Đọc, trích xuất và đối chiếu thông tin chức năng từ tài liệu công khai của một số hệ thống HIS/EHR/AI Agent theo bộ tiêu chí cố định.

**Việc cần thực hiện tiếp:** Phỏng vấn BA, quan sát một tác vụ benchmarking thực tế, đo baseline và cập nhật problem statement dựa trên bằng chứng thu thập được.

**Lưu ý:** Các số liệu thời gian hiện tại là ước lượng, không phải kết quả phỏng vấn hoặc quan sát đã hoàn thành.
