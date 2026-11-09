# CP4 - Bộ câu hỏi Phỏng vấn & Khảo sát theo The Mom Test: Điều tra đa nguồn log và Cô lập sự cố ngoài giờ

**Người chuẩn bị câu hỏi chuyên môn (Domain Questions):** Bùi Đặng Nhật Nguyên (`2A202603937`) phối hợp cùng Đỗ Hoàng Vũ (`2A202603920`).
**Đối tượng hỏi:** Kỹ sư trực vận hành hệ thống (`IT / NetOps / DevOps / SRE On-call`) hoặc Lập trình viên Backend từng tham gia xử lý sự cố hạ tầng và đọc log nhiều tầng. *(Không phỏng vấn thành viên trong nhóm).*

**Nguyên tắc The Mom Test bắt buộc tuân thủ:**
1. Chỉ hỏi về **sự việc thật đã xảy ra trong quá khứ** (lần trực ca gần nhất, sự cố ngoài giờ gần nhất).
2. **Tuyệt đối không hỏi câu giả định hoặc dẫn dắt** kiểu *"Bạn có muốn có một AI Agent tự đọc log và tự chặn IP giúp bạn không?"* (vi phạm bị trừ 3 điểm tiêu chí `C7`).
3. Không giới thiệu ý tưởng `Agentic AI + Confidence Score + HITL` của nhóm trước khi người được hỏi kể xong quy trình và nỗi đau thực tế của họ.

---

## Phần A - Phỏng vấn sâu 2-3 Kỹ sư vận hành / DevOps / SRE (15 phút/người)

1. **Hỏi về sự cố thực tế gần nhất (Kiểm chứng Giả định #1 - Thời gian & Điểm nghẽn đa nguồn log):**
   - *"Anh/bạn có thể kể lại chi tiết lần gần nhất nhận được báo lỗi hệ thống hoặc lưu lượng bất thường (đặc biệt là vào buổi tối/đêm hoặc cuối tuần) không? Lần đó sự cố bắt đầu từ dấu hiệu gì và anh/bạn đã làm từng bước như thế nào?"*
2. **Đo lường số nguồn log và bước tốn thời gian nhất (Kiểm chứng Bottleneck):**
   - *"Trong lần xử lý đó, anh/bạn đã phải mở tổng cộng bao nhiêu nơi/công cụ để đọc log (ví dụ cổng proxy Nginx, tường lửa, ứng dụng, database)? Bước nào làm anh/bạn mất nhiều thời gian nhất và mất khoảng bao nhiêu phút?"*
3. **Hỏi về cảnh báo giả và nhiễu theo chu kỳ (Kiểm chứng Màng lọc đầu vào):**
   - *"Trong các ca trực tuần vừa qua, có bao nhiêu lần hệ thống báo động nhưng khi mở log ra kiểm tra thì chỉ là lưu lượng tăng tự nhiên (như đầu giờ sáng thứ Hai) hoặc kết nối giữ phiên? Mỗi lần xác minh như vậy mất bao lâu?"*
4. **Hỏi về hành động cô lập sự cố ban đêm và ranh giới an toàn (Kiểm chứng Giả định #2 - Ranh giới tự động vs Con người duyệt):**
   - *"Đã bao giờ nhóm của anh/bạn thử cài đặt quy tắc tự động chặn (auto-block IP / rate-limit / tự khởi động lại) khi có bất thường vào ban đêm chưa? Lần đó chuyện gì đã xảy ra, có từng chặn nhầm người dùng thật hay làm lỗi nặng hơn không?"*
   - *"Trong quy trình hiện tại của công ty, những thao tác xử lý nào người trực ca được phép quyết định chạy ngay lập tức, và những thao tác nào bắt buộc phải gom bằng chứng xin ý kiến cấp trên hoặc đội phát triển ứng dụng trước khi chạy?"*
5. **Hỏi về cách bàn giao bằng chứng liên tầng (Kiểm chứng Giả định #3 - Nhánh HITL):**
   - *"Lần gần nhất anh/bạn phải chuyển tiếp một sự cố phức tạp cho đội backend hoặc quản lý duyệt, anh/bạn phải chuẩn bị những thông tin gì từ log và mất bao lâu để bên nhận hiểu đúng nguyên nhân?"*

---

## Phần B - Khảo sát nhanh (5-10 người làm IT / Vận hành / Backend để lấy Baseline)

1. Vai trò hiện tại của bạn: Kỹ sư vận hành (IT/NetOps/SysAdmin) / Kỹ sư DevOps-SRE / Lập trình viên Backend / Khác.
2. Trong 1 tháng qua, bạn tham gia tra cứu log để điều tra sự cố khoảng bao nhiêu lần? (số lần).
3. Ở lần sự cố phức tạp gần nhất, bạn phải đối chiếu log từ bao nhiêu nguồn/máy chủ khác nhau? (số nguồn).
4. Trung bình mỗi lần điều tra sự cố liên tầng như vậy (từ lúc biết có lỗi đến lúc khoanh vùng xong nguyên nhân gốc và cô lập tạm thời), bạn mất khoảng bao nhiêu phút? (số phút).
5. Trong các cảnh báo bạn nhận được hàng tuần, ước tính khoảng bao nhiêu phần trăm là cảnh báo giả hoặc lưu lượng tăng bình thường theo chu kỳ? (0-100%).
6. Ở hệ thống bạn đang làm việc, thao tác nào hiện đã được phép tự động thực thi khi có bằng chứng rõ ràng mà không cần chờ người gõ lệnh tay? (Chặn/giới hạn tốc độ IP đơn lẻ / Không cho phép tự động bất kỳ lệnh nào / Khác).

---

*Lưu ý khi ghi chép kết quả: Mỗi buổi phỏng vấn lưu thành 1 bảng `Interview Snapshot` trong mục `3.2` của `report/team/group_report.md` hoặc file `report/assets/cp4-interview-snapshot-N.md`. Chỉ ghi vai trò, tuyệt đối không ghi tên thật, email, số điện thoại hay thông tin nội bộ của công ty người được hỏi.*
