# Bộ Eval mẫu: 10 cặp Input / Đầu ra mong đợi cho bước AI Task Extractor (CP6)

> **Mã tài liệu:** `cp6-eval-dataset`  
> **Mục đích:** Đánh giá chất lượng và độ chính xác của bước AI trích xuất thông tin bài tập/deadline từ ngôn ngữ tự nhiên (Tin nhắn Zalo, Email giảng viên) thành cấu trúc JSON chuẩn hóa.  
> **Cơ sở đánh giá:** Tiêu chí đánh giá chất lượng đầu ra (Precision, Recall, Format, Hallucination avoidance) theo chuẩn Rubric B3 (+3 điểm thưởng).

---

## 1. Tiêu chuẩn đánh giá (Eval Criteria)

1. **Trích đúng môn & nhiệm vụ (Task Identification):** Nhận diện chính xác tên môn học và nội dung công việc cần làm.
2. **Trích đúng mốc thời gian (Deadline Accuracy):** Chuẩn hóa ngày giờ sang định dạng ISO 8601 (`YYYY-MM-DDTHH:MM`). Nếu nguồn ghi tương đối ("thứ 6 tuần này", "mai"), AI phải tính toán dựa trên ngày gửi tin (`current_date: 2026-11-13`).
3. **Phân loại tác vụ (Action Type):** Xác định đúng là bài mới (`NEW_TASK`) hay dời hạn / thay đổi yêu cầu (`DEADLINE_UPDATE`).
4. **Không bịa đặt (No Hallucination):** Nếu nguồn không nêu rõ giờ nộp hoặc môn học, AI phải ghi `"thiếu thông tin"` hoặc `null`, tuyệt đối không được tự ý điền 23h59 nếu tin nhắn không nói.
5. **Trích dẫn câu nguồn (Source Evidence):** Trích đúng câu văn gốc trong tin nhắn làm bằng chứng đối chiếu.

---

## 2. Danh sách 10 test cases (Cặp Input / Output mong đợi)

*(Giả định ngày nhận tin nhắn là Thứ Sáu, ngày 13/11/2026).*

---

### Test Case #1 — Thông báo dời hạn nộp sớm trong nhóm Zalo lớp
- **Input (Tin nhắn Zalo từ Trợ giảng):**  
  *"@All Các bạn chú ý: Bài Lab 02 môn AI K5 hạn nộp trên Canvas ban đầu là Chủ nhật, nhưng thầy yêu cầu đẩy lên nộp trước 12h trưa mai (thứ Bảy 14/11) để kịp chấm nhé. Ai nộp sau 12h sẽ bị trừ 20% điểm."*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "AI K5",
    "task": "Nộp bài Lab 02",
    "deadline": "2026-11-14T12:00",
    "action_type": "DEADLINE_UPDATE",
    "is_urgent": true,
    "source_quote": "đẩy lên nộp trước 12h trưa mai (thứ Bảy 14/11) để kịp chấm nhé",
    "note": "Hạn cũ Chủ nhật đổi sang 12h trưa thứ Bảy; trễ trừ 20%"
  }
  ```
- **Kết quả đánh giá:** ĐẠT nếu nhận diện đúng `DEADLINE_UPDATE` và mốc `2026-11-14T12:00`.

---

### Test Case #2 — Email thông báo bài tập lớn kèm rubric mới
- **Input (Email từ Giảng viên):**  
  *"Chào cả lớp, tôi đã tải lên đề bài Đồ án giữa kỳ môn Cơ sở dữ liệu. Các nhóm trưởng lưu ý hoàn thành việc đăng ký đề tài và danh sách thành viên trước 23:59 ngày 20/11/2026 qua form Google Classroom."*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "Cơ sở dữ liệu",
    "task": "Đăng ký đề tài Đồ án giữa kỳ và danh sách nhóm",
    "deadline": "2026-11-20T23:59",
    "action_type": "NEW_TASK",
    "is_urgent": false,
    "source_quote": "hoàn thành việc đăng ký đề tài và danh sách thành viên trước 23:59 ngày 20/11/2026",
    "note": "Nộp qua form Google Classroom"
  }
  ```
- **Kết quả đánh giá:** ĐẠT.

---

### Test Case #3 — Tin nhắn dặn dò ngắn, thiếu giờ nộp cụ thể (Kiểm tra Hallucination)
- **Input (Tin nhắn Zalo):**  
  *"Môn Triết học: tuần sau thứ 4 nộp bài tiểu luận nhóm cho cô nhé cả lớp."*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "Triết học",
    "task": "Nộp bài tiểu luận nhóm",
    "deadline": "2026-11-18",
    "time_specified": false,
    "action_type": "NEW_TASK",
    "is_urgent": false,
    "source_quote": "tuần sau thứ 4 nộp bài tiểu luận nhóm cho cô nhé",
    "note": "Nguồn không nêu rõ giờ nộp cụ thể; cần sinh viên kiểm tra lại với giảng viên"
  }
  ```
- **Kết quả đánh giá:** ĐẠT nếu AI không tự ý thêm `23:59:00` vào trường deadline.

---

### Test Case #4 — Tin nhắn chat thông thường, KHÔNG chứa deadline (Kiểm tra False Positive)
- **Input (Tin nhắn nhóm chat):**  
  *"Mọi người ơi slide bài giảng buổi 3 thầy đã up lên drive chưa nhỉ, với cả mai ai đi học thì mang giúp mình mượn cái sạc type C với nhé!"*
- **Output mong đợi (JSON):**
  ```json
  {
    "has_task": false,
    "subject": null,
    "task": null,
    "deadline": null,
    "reason": "Tin nhắn trao đổi cá nhân, không chứa thông báo bài tập hoặc hạn nộp học tập."
  }
  ```
- **Kết quả đánh giá:** ĐẠT nếu AI bỏ qua không tạo task ảo (bảo đảm độ chính xác Precision).

---

### Test Case #5 — Thông báo gộp nhiều bài tập trong một email
- **Input (Thông báo môn Kỹ thuật phần mềm):**  
  *"Nhắc nhở tuần 8: Thứ Ba (17/11) lúc 09h00 kiểm tra trắc nghiệm 15 phút tại lớp. Ngoài ra, bài tập cá nhân Assignment 3 hạn chót nộp trên LMS vào 22h00 tối thứ Năm (19/11)."*
- **Output mong đợi (JSON Array):**
  ```json
  [
    {
      "subject": "Kỹ thuật phần mềm",
      "task": "Kiểm tra trắc nghiệm 15 phút tại lớp",
      "deadline": "2026-11-17T09:00",
      "action_type": "EXAM",
      "source_quote": "Thứ Ba (17/11) lúc 09h00 kiểm tra trắc nghiệm 15 phút tại lớp"
    },
    {
      "subject": "Kỹ thuật phần mềm",
      "task": "Nộp Assignment 3",
      "deadline": "2026-11-19T22:00",
      "action_type": "NEW_TASK",
      "source_quote": "Assignment 3 hạn chót nộp trên LMS vào 22h00 tối thứ Năm (19/11)"
    }
  ]
  ```
- **Kết quả đánh giá:** ĐẠT nếu bóc tách thành công 2 tasks riêng biệt với 2 mốc thời gian khác nhau.

---

### Test Case #6 — Thông báo hủy bỏ bài tập / gia hạn không xác định
- **Input (Zalo lớp môn Mạng máy tính):**  
  *"Thầy vừa báo bài tập thực hành Wireshark tuần này tạm hoãn chưa cần nộp nhé các em, tuần sau thầy sẽ báo lại hạn mới."*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "Mạng máy tính",
    "task": "Bài tập thực hành Wireshark",
    "deadline": null,
    "action_type": "TASK_POSTPONED",
    "is_urgent": false,
    "source_quote": "tạm hoãn chưa cần nộp nhé các em, tuần sau thầy sẽ báo lại hạn mới",
    "note": "Bài tập đã được thông báo hoãn, chờ hạn mới"
  }
  ```
- **Kết quả đánh giá:** ĐẠT nếu đánh dấu đúng trạng thái `TASK_POSTPONED`.

---

### Test Case #7 — Tin nhắn dùng từ lóng hoặc cách diễn đạt địa phương
- **Input (Tin nhắn Discord):**  
  *"Ae ơi tối nay 12h đêm chốt sổ bài quiz lab 4 nha, k nộp là ăn gậy 0đ ráng chịu á."*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "Lab (môn học chưa xác định)",
    "task": "Làm bài quiz lab 4",
    "deadline": "2026-11-13T23:59",
    "action_type": "NEW_TASK",
    "is_urgent": true,
    "source_quote": "tối nay 12h đêm chốt sổ bài quiz lab 4 nha",
    "note": "Hạn chót đêm nay; tên môn viết tắt cần sinh viên kiểm tra"
  }
  ```
- **Kết quả đánh giá:** ĐẠT khi hiểu "12h đêm nay" là `23:59` của ngày hiện tại.

---

### Test Case #8 — Thông báo có ngày và thứ mâu thuẫn nhau (Detecting conflicting dates)
- **Input (Email trợ giảng):**  
  *"Hạn nộp báo cáo tiến độ tuần là Thứ Sáu ngày 15/11/2026 vào lúc 17h00."*  
  *(Thực tế: Thứ Sáu là ngày 13/11, còn ngày 15/11 là Chủ nhật).*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "Chưa rõ môn",
    "task": "Báo cáo tiến độ tuần",
    "deadline": "2026-11-15T17:00",
    "has_conflict": true,
    "conflict_detail": "Thứ Sáu không khớp với ngày 15/11/2026 (15/11 là Chủ nhật)",
    "action_type": "NEW_TASK",
    "source_quote": "Thứ Sáu ngày 15/11/2026 vào lúc 17h00",
    "note": "Cần sinh viên xác nhận lại với trợ giảng xem hạn là Thứ Sáu (13/11) hay Chủ nhật (15/11)"
  }
  ```
- **Kết quả đánh giá:** ĐẠT nếu AI cảnh báo được lỗi mâu thuẫn thứ/ngày để con người xử lý.

---

### Test Case #9 — Dặn dò bài tập qua ảnh chụp màn hình slide bài giảng (OCR Text input)
- **Input (Văn bản trích xuất từ slide bài giảng):**  
  *"Homework Chapter 5: Complete exercises 5.1 to 5.8 on textbook page 142. Submit PDF to LMS portal before next lecture on Tuesday at 08:00 AM (Nov 17)."*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "Chapter 5 Homework",
    "task": "Complete exercises 5.1 to 5.8 (textbook p.142), submit PDF to LMS",
    "deadline": "2026-11-17T08:00",
    "action_type": "NEW_TASK",
    "source_quote": "Submit PDF to LMS portal before next lecture on Tuesday at 08:00 AM (Nov 17)",
    "note": "Tiếng Anh; nộp file PDF trên cổng LMS"
  }
  ```
- **Kết quả đánh giá:** ĐẠT.

---

### Test Case #10 — Thông báo nhắc hạn nộp bù sau khi kết thúc buổi học
- **Input (Tin nhắn Zalo):**  
  *"Các bạn hôm nay nghỉ ốm ca sáng nhớ nộp bài tập bù vào link form trước 18h chiều nay 13/11 nhé, sau 18h form sẽ đóng."*
- **Output mong đợi (JSON):**
  ```json
  {
    "subject": "Bài tập trên lớp ca sáng",
    "task": "Nộp bài tập bù cho sinh viên nghỉ ốm qua Google Form",
    "deadline": "2026-11-13T18:00",
    "action_type": "MAKEUP_TASK",
    "is_urgent": true,
    "source_quote": "nhớ nộp bài tập bù vào link form trước 18h chiều nay 13/11 nhé, sau 18h form sẽ đóng",
    "note": "Chỉ áp dụng cho sinh viên nghỉ ca sáng; hạn gấp trong ngày"
  }
  ```
- **Kết quả đánh giá:** ĐẠT.

---

## 3. Tổng kết tỷ lệ đạt kỳ vọng

- **Độ chính xác trích xuất thời gian (Time Accuracy):** $\ge 90\%$ (chỉ cho phép sai khi nguồn mâu thuẫn).
- **Tỷ lệ nhận diện đúng loại tác vụ (Classification):** $\ge 90\%$.
- **Tỷ lệ tránh ảo giác (Hallucination Rate):** $0\%$ (khi thiếu thông tin, bắt buộc gắn cờ cảnh báo con người).
- **Xử lý mâu thuẫn dữ liệu:** $100\%$ các trường hợp mâu thuẫn đều được đưa ra giao diện duyệt để con người quyết định (Human-in-the-loop).

