# Interview Snapshot #1 — Trải nghiệm rà soát thông báo & deadline

> **Mã tài liệu:** `cp4-interview-snapshot-1`  
> **Phương pháp:** Phỏng vấn sâu 1-1 theo chuẩn **The Mom Test** (tập trung vào hành vi và sự việc có thật trong quá khứ, không hỏi ý kiến lý thuyết).  
> **Người thực hiện phỏng vấn:** Nguyễn Văn Minh (phụ trách CP4 Kiểm chứng).  
> **Tuân thủ quy định bảo mật:** Tên thật, thông tin liên lạc và dữ liệu định danh của người được phỏng vấn đã được mã hóa/ẩn danh theo quy định trong `RULES.md` và `report/assets/README.md`.

---

## 1. Thông tin đối tượng phỏng vấn

| Trường | Nội dung |
|---|---|
| **Mã định danh** | Sinh viên A |
| **Vai trò** | Sinh viên năm 2 ngành AI / Kỹ thuật máy tính, đang học 5 môn (gồm 3 môn lab thực hành và 1 đồ án nhóm) |
| **Bối cảnh học tập** | Mỗi môn sử dụng một kênh trao đổi riêng (Canvas LMS, 3 nhóm chat Zalo môn, 1 server Discord nhóm làm đồ án, hộp thư sinh viên) |
| **Thời gian phỏng vấn** | 15 phút, trực tiếp tại khu tự học sinh viên |

---

## 2. Trích dẫn đắt giá nhất (Verbatim Quote)

> *"Sợ nhất là hạn nộp bài trên LMS ghi là Chủ nhật, nhưng tối thứ Sáu trợ giảng ghim tin nhắn trong nhóm Zalo bảo nộp sớm vào sáng thứ Bảy để chấm bù; mình mà không lướt Zalo lúc 23h đêm là coi như sáng hôm sau mất trắng 20% điểm."*

---

## 3. Diễn biến sự việc cụ thể gần nhất (Critical Incident)

- **Thời điểm xảy ra:** Thứ Sáu tuần trước (khoảng 21h30).
- **Chuyện gì đã diễn ra:**
  - Trong môn Lập trình Thực hành, trợ giảng thay đổi yêu cầu nộp bài lab: yêu cầu nộp thêm file video demo 2 phút và đẩy hạn nộp lên sớm hơn 1 ngày (thay vì 23h59 Chủ nhật trên LMS thì đổi thành 12h00 trưa thứ Bảy trên Zalo).
  - Tin nhắn dặn dò này được gửi dưới dạng văn bản tự do trong nhóm Zalo có hơn 70 sinh viên.
  - Ngay sau đó, các bạn trong lớp liên tục nhắn tin hỏi bài, cảm ơn, thả sticker khiến thông báo bị trôi khỏi màn hình chính chỉ sau 30 phút.
  - Sinh viên A lúc 23h00 vào rà soát lại tin nhắn trước khi đi ngủ mới vô tình đọc được thông báo ghim, phải thức đến 2h30 sáng để quay video demo cho kịp nộp.

---

## 4. Hành vi thực tế và giải pháp thay thế hiện tại (Workarounds)

- **Cách đang làm:**
  1. Mỗi tối mở lần lượt: Canvas LMS $\rightarrow$ Hộp thư Outlook sinh viên $\rightarrow$ 4 nhóm chat Zalo $\rightarrow$ Kênh Discord đồ án.
  2. Khi thấy tin nhắn có từ khóa *"hạn nộp"*, *"deadline"*, *"dời lịch"*, sinh viên chụp ảnh màn hình rồi gửi vào mục **"Cloud của tôi"** trên Zalo hoặc copy text dán vào ứng dụng Google Keep.
- **Thời gian tiêu tốn:** Mất từ **20–25 phút mỗi tối** (khoảng 22h00–22h30). Lặp lại 4–5 tối trong tuần.
- **Tổn thất/Hậu quả:** 
  - Tháng trước từng bị trễ 1 bài nộp bài tập về nhà môn Toán kỹ thuật do không đọc email thông báo dời deadline của giảng viên.
  - Thường xuyên rơi vào trạng thái căng thẳng sợ bỏ sót thông báo quan trọng.

---

## 5. Tín hiệu kiểm chứng (Validation Signals)

- **Tín hiệu xác nhận (Confirmation):**
  - Giả định rằng sinh viên mất 20–30 phút rà soát mỗi tối là **chính xác**.
  - Giả định rằng các lần sót deadline chủ yếu bắt nguồn từ thông báo phi cấu trúc trên Zalo/Email là **hoàn toàn có thật**.
- **Tín hiệu phản bác / Ranh giới quan trọng (Disconfirmation / Boundary):**
  - **Phản bác giải pháp tự động đọc Zalo:** Sinh viên A kiên quyết phản đối việc cài bot đọc toàn bộ tin nhắn Zalo cá nhân vì lý do an toàn quyền riêng tư: *"Zalo mình còn nhắn tin cho người yêu và gia đình, không bao giờ cấp token hay mật khẩu cho app lạ"*.
  - **Hướng giải quyết:** Chuyển sang cơ chế sinh viên chủ động chọn lọc và forward/dán tin nhắn cho bot xử lý, kết hợp đồng bộ lịch LMS qua chuẩn iCal feed có sẵn.

