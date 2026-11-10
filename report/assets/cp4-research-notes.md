# Ghi chú Research Kỹ thuật & Đánh giá giải pháp tương đồng (CP4)

> **Mã tài liệu:** `cp4-research-notes`  
> **Người thực hiện:** Nguyễn Văn Minh (phụ trách CP4 Research).  
> **Mục tiêu:** Rà soát các giải pháp công nghệ và sản phẩm trên thị trường đã giải quyết từng bước trong bài toán tổng hợp bài tập / deadline, từ đó rút ra bài học thiết kế và tránh việc "sáng tạo lại bánh xe" (reinventing the wheel).

---

## 1. Tổng quan 3 giải pháp được đối sánh

```text
Quy trình tổng hợp bài tập:
[LMS Calendar] ──────────► [1. Canvas iCal Feed] ──► Chuẩn Rule tự động 100%
[Tin nhắn Zalo/Email] ───► [3. n8n AI Task Parser] ─► Mô hình Workflow trích xuất JSON
[Tối ưu hóa lịch học] ──► [2. Motion App] ─────────► Bị loại vì đắt ($19/tháng) & thừa tính năng
```

---

## 2. Phân tích chi tiết từng giải pháp

### 2.1. Canvas LMS Calendar Feed (iCal Feed)
- **Tài liệu tham khảo chính thức:** [Canvas Community — Subscribing to Calendar Feed](https://community.canvaslms.com/t5/Student-Guide/How-do-I-subscribe-to-the-Calendar-feed-using-Google-Calendar/ta-p/522)
- **Cơ chế hoạt động:**
  - Canvas LMS cung cấp sẵn một đường dẫn URL dạng iCalendar (`webcal://...` hoặc `.ics`).
  - Người dùng chỉ cần sao chép link này và dán vào Google Calendar / Apple Calendar ở mục *"Subscribe to Calendar"*.
  - Mọi sự kiện, bài kiểm tra, hạn nộp bài tập được giáo viên tạo trên LMS sẽ tự động đồng bộ về ứng dụng lịch cá nhân của sinh viên theo chu kỳ (thường từ 2–4 tiếng một lần).
- **Điểm mạnh:**
  - Hoàn toàn miễn phí, có sẵn trong hệ thống Canvas LMS của trường.
  - Hoạt động ổn định 100% theo quy tắc (Rule-based), không phụ thuộc vào LLM, không bao giờ bị ảo giác (hallucination) hay sai lệch giờ nộp.
  - Không đòi hỏi cấp quyền truy cập tài khoản hay mật khẩu sinh viên.
- **Điểm yếu / Khoảng trống:**
  - Hoàn toàn **không xử lý được** các thông tin phi cấu trúc: dặn dò ngoài giờ của trợ giảng trên Zalo, thông báo thay đổi hạn nộp đột xuất qua email hay yêu cầu nộp bù bài giảng.
- **Bài học cho nhóm:**
  - **Không dùng AI cho phần LMS**: Bước lấy bài từ Canvas chỉ cần dùng chuẩn iCal feed. Đây là lựa chọn chuẩn xác theo nguyên tắc *"đơn giản nhất có thể"* (Occam's razor).

---

### 2.2. Motion (usemotion.com)
- **Trang chủ sản phẩm:** [Motion: AI-powered calendar and project management](https://www.usemotion.com/)
- **Cơ chế hoạt động:**
  - Người dùng nhập các đầu việc kèm deadline và thời lượng ước tính.
  - Thuật toán AI của Motion tự động phân bổ các việc này vào các khoảng thời gian trống (free slots) trong ngày trên Google/Outlook Calendar, tự động dời lịch khi có việc khẩn cấp chèn vào.
- **Điểm mạnh:**
  - Khả năng tự động xếp lịch và tối ưu hóa thời gian rất ấn tượng.
  - Giao diện trực quan, chuyên nghiệp.
- **Điểm yếu / Khoảng trống:**
  - Chi phí quá đắt đối với sinh viên ($19/tháng khi đóng theo năm hoặc $34/tháng khi đóng từng tháng).
  - Người dùng vẫn phải tự tay gõ từng task hoặc kết nối với Jira/Asana (không có cổng kết nối Zalo hay hệ thống giáo dục Việt Nam).
  - Không hỗ trợ đọc hiểu ngôn ngữ tự nhiên tiếng Việt từ các đoạn chat không có cấu trúc.
- **Bài học cho nhóm:**
  - Sinh viên **không cần một cỗ máy xếp lịch tự động phức tạp**. Nỗi đau thực sự là **bước gom thông tin và trích xuất ngày giờ hạn nộp**, chứ không phải bước xếp việc vào giờ nào để làm.

---

### 2.3. Template n8n: AI Message Summarizer & Task Extractor
- **Mã nguồn workflow mẫu:** [n8n Workflow #1888: Summarize messages using OpenAI](https://n8n.io/workflows/1888-summarize-messages-using-openai/)
- **Cơ chế hoạt động:**
  - Nhận nội dung tin nhắn thông qua Webhook hoặc Bot nhận tin nhắn.
  - Gửi đoạn văn bản vào mô hình LLM (như OpenAI GPT hoặc Claude) kèm Structured Prompt để bóc tách các trường: Tên môn học, Tên nhiệm vụ, Thời hạn (Deadline ISO 8601), và Trích dẫn bằng chứng gốc.
  - Trả về dữ liệu dạng JSON chuẩn hóa để đưa tiếp vào hệ thống cơ sở dữ liệu hoặc lịch.
- **Điểm mạnh:**
  - Khung kiến trúc Workflow rõ ràng: từng bước tách bạch, dễ kiểm soát và tùy biến.
  - Bóc tách ngôn ngữ tự nhiên tiếng Việt rất tốt, kể cả các câu nói tự do như *"thứ 6 nộp nhé các bạn"*, *"hạn nộp trước 12h trưa mai"*.
- **Rủi ro kỹ thuật:**
  - AI có thể trích nhầm mốc thời gian nếu tin nhắn dùng các từ ngữ tương đối mà thiếu mốc quy chiếu (ví dụ: *"mai"*, *"ngày kia"*, *"tuần sau"*).
  - Nếu để AI tự động tạo sự kiện vào lịch mà không có con người kiểm tra thì rủi ro sai sót deadline là rất nguy hiểm.
- **Bài học cho nhóm:**
  - Mượn khung kiến trúc Workflow này để xử lý phần bóc tách tin nhắn Zalo/Email.
  - **Bắt buộc tích hợp nút kiểm tra của con người (Human-in-the-loop - HITL)**: AI chỉ tạo bản nháp Daily Digest, sinh viên bấm duyệt thì mới lưu vào lịch.

---

## 3. Kết luận tổng hợp cho kiến trúc hệ thống

| Bước trong bài toán | Công nghệ lựa chọn | Lý do lựa chọn |
|---|---|---|
| 1. Đồng bộ bài tập chính thức từ LMS | **Rule (Canvas iCal Feed)** | Miễn phí, chính xác 100%, không cần AI |
| 2. Tiếp nhận thông báo Zalo / Email | **Con người chủ động chọn lọc** | Bảo vệ quyền riêng tư 100%, tránh spam |
| 3. Trích xuất môn, bài, deadline | **AI (LLM Workflow parser)** | Xử lý ngôn ngữ tự nhiên tiếng Việt linh hoạt |
| 4. Tổng hợp bản tin Daily Digest 22h00 | **Rule** | Tự động gộp trùng, khống chế ≤ 5 dòng |
| 5. Kiểm tra và xác nhận | **Con người (HITL)** | Chốt chặn an toàn, loại trừ ảo giác AI |
| 6. Lưu vào Google Calendar & Nhắc hẹn | **Rule (Google Calendar API / ICS)** | Ổn định, tự động báo trước 24 giờ |

