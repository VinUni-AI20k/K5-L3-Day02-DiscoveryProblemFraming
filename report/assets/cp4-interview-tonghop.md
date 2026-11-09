# CP4: Tổng hợp 5 buổi phỏng vấn

Bộ câu hỏi: [cp4-cauhoi-phongvan.md](cp4-cauhoi-phongvan.md)

| Trường | Nội dung |
|---|---|
| Người được hỏi | 5 người ngoài nhóm đã từng trực sự cố hệ thống: kỹ sư DevOps/SRE đang đi làm, quản trị hệ thống, lập trình viên backend. Không ghi tên, công ty |
| Hình thức | Gặp trực tiếp, gọi video/điện thoại, nhắn tin |
| Cách ghi | Các buổi không ghi âm và không có biên bản riêng; nội dung dưới đây là ý chính do người phỏng vấn tổng hợp lại |
| Lần gần nhất gặp vấn đề | Đa số đều gặp sự cố phải lần qua nhiều nguồn log để tìm tầng gây lỗi. **2/5 người thường xuyên bị gọi dậy giữa đêm** để xử lý sự cố |
| Workaround hiện tại | Xem dashboard và cảnh báo trên Grafana/Loki/Prometheus hoặc Datadog/New Relic; khi cần đào sâu thì ssh vào từng máy dùng grep/tail đọc log |
| Mất bao lâu | Thời gian từ lúc nhận cảnh báo đến lúc khoanh vùng được tầng lỗi phổ biến là 15–30 phút |
| Pain được nhắc nhiều nhất | Lần mò qua nhiều nguồn log; sự cố ban đêm không ai phản ứng kịp; cảnh báo giả |
| Thái độ với việc hệ thống tự chặn IP / giới hạn tốc độ | Đa số đồng ý có điều kiện: chỉ khi có whitelist, rollback và giới hạn thời gian chặn. Không chấp nhận tự chặn vô điều kiện |
| Insight / opportunity | Khoảng trống không nằm ở việc đọc log trong giờ hành chính (15–30 phút là chấp nhận được), mà ở phản ứng ngoài giờ: người trực bị gọi dậy giữa đêm cho cả sự cố thật lẫn cảnh báo giả. Hành động tự động chỉ được người dùng chấp nhận khi có ràng buộc an toàn rõ |
