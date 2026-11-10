# Interview Snapshot #3 — Trải nghiệm sử dụng ứng dụng nhắc việc & to-do list

> **Mã tài liệu:** `cp4-interview-snapshot-3`  
> **Phương pháp:** Phỏng vấn sâu 1-1 theo chuẩn **The Mom Test**.  
> **Người thực hiện phỏng vấn:** Nguyễn Văn Minh (phụ trách CP4 Kiểm chứng).  
> **Tuân thủ quy định bảo mật:** Thông tin cá nhân đã được ẩn danh theo quy định bảo mật.

---

## 1. Thông tin đối tượng phỏng vấn

| Trường | Nội dung |
|---|---|
| **Mã định danh** | Sinh viên C |
| **Vai trò** | Sinh viên năm 2 ngành Kỹ thuật Hệ thống / Khoa học Dữ liệu, thường xuyên thực hành bài lab kỹ thuật và dự án nhóm |
| **Kênh tiếp nhận bài** | Canvas LMS, Zalo nhóm lớp, Google Classroom |
| **Thời gian phỏng vấn** | 10 phút, phỏng vấn trực tiếp |

---

## 2. Trích dẫn đắt giá nhất (Verbatim Quote)

> *"Mình muốn có một công cụ nhìn vào là biết tối nay và ngày mai phải nộp bài gì ngay lập tức, chứ không muốn mất thời gian tự tay ngồi gõ từng đầu việc vào ứng dụng nhắc việc."*

---

## 3. Diễn biến sự việc cụ thể gần nhất (Critical Incident)

- **Thời điểm xảy ra:** Thứ Sáu tuần trước (khoảng 23h45).
- **Chuyện gì đã diễn ra:**
  - Sinh viên C ngồi tập trung viết code và sửa lỗi cho bài tập lớn lập trình từ 19h tối đến tận 1h sáng hôm sau.
  - Do quá tập trung vào bài code khó, C quên bẵng mất rằng trước 23h59 tối hôm đó có một bài quiz trắc nghiệm kiểm tra kiến thức tuần trên Canvas LMS (chiếm 5% tổng điểm quá trình).
  - Kết quả là hệ thống LMS tự động đóng cổng nộp bài lúc 00h00, C bị điểm 0 cho bài trắc nghiệm đó mà không được làm lại.

---

## 4. Hành vi thực tế và giải pháp thay thế hiện tại (Workarounds)

- **Cách đang làm:**
  - C đã từng cài đặt các ứng dụng nhắc việc phổ biến như Apple Reminders, Google Tasks và Notion.
  - Tuy nhiên, quy trình yêu cầu người dùng phải tự đọc thông báo rồi tự gõ từng chữ (tên môn, tên bài, giờ nộp) vào app.
  - Sau những buổi học trên trường mệt mỏi, C thường bỏ qua việc nhập liệu trong 3–4 ngày liên tục. Khi app không có dữ liệu đầu vào thì cũng không thể gửi thông báo nhắc nhở được.
- **Thời gian & tổn thất:**
  - Mất trung bình **15 phút/ngày** tự rà soát.
  - Trong học kỳ gần nhất, C đã bị bỏ lỡ **2 bài kiểm tra ngắn** trên LMS do không có ai hay công cụ nào nhắc nhở kịp thời.

---

## 5. Tín hiệu kiểm chứng (Validation Signals)

- **Tín hiệu xác nhận (Confirmation):**
  - Khẳng định giả thuyết rằng: Giải pháp thành công **phải giảm thiểu tối đa thao tác nhập liệu thủ công của người dùng** (Zero-input / Minimal-effort). Nếu bắt sinh viên tự gõ tay lại thông tin thì quy trình chắc chắn sẽ bị bỏ rơi sau vài ngày.
- **Tín hiệu phản bác / Định hướng thiết kế (Disconfirmation / Design Rules):**
  - Sinh viên C nhấn mạnh: Không cần AI phân tích cao siêu hay tự động lập kế hoạch chia nhỏ công việc phức tạp (như Motion). Điều quan trọng nhất là **chính xác về thời gian và có thông báo nhắc hạn trước 24 giờ**.
  - **Quy tắc HITL (Human-in-the-loop):** Sinh viên phải là người bấm nút xác nhận cuối cùng để thêm task vào Google Calendar nhằm đảm bảo tính chủ động và chắc chắn.

