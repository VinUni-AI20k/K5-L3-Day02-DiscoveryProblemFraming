# Bộ Dữ Liệu Kiểm Thử Mẫu (Eval Dataset) — 10 Cặp Input / Output

> **Mục đích:** Đánh giá độ chính xác, tính toàn vẹn bằng chứng và khả năng xử lý biên (edge cases) của bước **AI Workflow** trong việc phân loại nguyên nhân hủy chuyến / ngâm cuốc trên ứng dụng Xanh SM.
> **Tiêu chí chấm đạt:**
> 1. *Classification Accuracy:* Phân loại đúng nhãn nguyên nhân.
> 2. *Evidence Fidelity:* Trích xuất đúng nguyên văn câu nói làm bằng chứng (không hallucination).
> 3. *PII Masking:* 100% thông tin số điện thoại/tên riêng được che mờ.
> 4. *Latency:* Thời gian xử lý $\le 3.0$s.

---

### Case 1: Tài xế cố tình ngâm cuốc và nhắn tin ép khách tự hủy
- **Input:**
  - `telemetry`: Xe đứng im 4 phút tại tọa độ [20.9921, 105.9412], vận tốc: 0 km/h.
  - `traffic_context`: Tốc độ trung bình dòng xe xung quanh: 28 km/h (đường thông thoáng).
  - `chat_log`: `Khách: "Bác tài ơi xe có đến đón không ạ?"` -> `Tài xế: "Anh đang bận chút việc, em hủy hộ anh nhé."`
- **Output mong đợi (AI):**
  - `predicted_label`: "Tài xế cố tình ngâm cuốc ép khách hủy"
  - `confidence`: 0.96
  - `evidence_quote`: "Anh đang bận chút việc, em hủy hộ anh nhé."
  - `recommendation`: "Duyệt vi phạm tài xế; Tự động bảo lưu voucher 100% cho khách hàng."
- **Đánh giá:** ĐẠT.

---

### Case 2: Kẹt xe nghiêm trọng tại nút giao thông (Bất khả kháng)
- **Input:**
  - `telemetry`: Xe di chuyển 80m trong 4 phút, vận tốc: 2.1 km/h.
  - `traffic_context`: Cảnh báo ùn tắc đỏ tại nút giao Cổ Linh - Vĩnh Tuy, vận tốc dòng xe: 3.0 km/h.
  - `chat_log`: `Tài xế: "Em ơi đường Cổ Linh kẹt cứng nhích từng mét, ráng đợi anh 5-7 phút nhé."` -> `Khách: "Em vội đi làm quá không đợi được ạ."`
- **Output mong đợi (AI):**
  - `predicted_label`: "Ùn tắc giao thông bất khả kháng"
  - `confidence`: 0.94
  - `evidence_quote`: "Em ơi đường Cổ Linh kẹt cứng nhích từng mét" kết hợp tốc độ dòng xe 3.0 km/h.
  - `recommendation`: "Miễn trừ trách nhiệm cho tài xế; Hỗ trợ khách đổi xe mới không tính phí."
- **Đánh giá:** ĐẠT.

---

### Case 3: Nhiễu sóng GPS (Urban Canyon) tại chân tòa nhà cao tầng
- **Input:**
  - `telemetry`: Tọa độ xe nhảy giật liên tục giữa hai vị trí cách nhau 250m trong 2 phút (vận tốc tức thời nhảy 70 km/h rồi về 0).
  - `traffic_context`: Bình thường.
  - `chat_log`: `Tài xế: "Anh đang đỗ trước sảnh S1.01 bật đèn khẩn cấp rồi em ơi."` -> `Khách: "Ủa sao trên bản đồ xe anh ở hồ nước?"`
- **Output mong đợi (AI):**
  - `predicted_label`: "Nhiễu định vị viễn thông / Lỗi GPS Urban Canyon"
  - `confidence`: 0.62 (Dưới ngưỡng tự tin 0.90)
  - `evidence_quote`: Tọa độ nhảy giật bất thường + tin nhắn "Anh đang đỗ trước sảnh S1.01".
  - `recommendation`: "Trạng thái nghi vấn kỹ thuật; Chuyển chuyên viên CSKH kiểm tra thủ công, KHÔNG phạt tài xế."
- **Đánh giá:** ĐẠT (Xử lý an toàn khi độ tự tin thấp).

---

### Case 4: Sự cố kỹ thuật phương tiện đột xuất (Thủng lốp xe)
- **Input:**
  - `telemetry`: Xe dừng hẳn sát lề đường cách điểm đón 500m.
  - `traffic_context`: Bình thường.
  - `chat_log`: `Tài xế: "Xe anh vừa dính đinh cán phải sắt xịt lốp rồi, em bấm đổi tài xế khác trên app đi cho kịp giờ nhé."`
- **Output mong đợi (AI):**
  - `predicted_label`: "Sự cố kỹ thuật phương tiện đột xuất"
  - `confidence`: 0.95
  - `evidence_quote`: "Xe anh vừa dính đinh cán phải sắt xịt lốp rồi"
  - `recommendation`: "Ghi nhận sự cố kỹ thuật; Miễn trừ chế tài cho tài xế; Kích hoạt tìm xe thay thế ngay lập tức."
- **Đánh giá:** ĐẠT.

---

### Case 5: Tài xế di chuyển ngược hướng để đón khách ngoài (Gian lận)
- **Input:**
  - `telemetry`: Khoảng cách tới khách tăng từ 700m lên 2.4km trong 5 phút; vận tốc di chuyển 35 km/h theo hướng ngược lại.
  - `traffic_context`: Bình thường.
  - `chat_log`: Khách nhắn 3 tin hỏi không có phản hồi từ tài xế.
- **Output mong đợi (AI):**
  - `predicted_label`: "Tài xế di chuyển ngược hướng / Nghi vấn chở cuốc ngoài"
  - `confidence`: 0.93
  - `evidence_quote`: Khoảng cách tăng liên tục >1.5km với vận tốc 35 km/h không phản hồi khách.
  - `recommendation`: "Khuyến nghị cảnh cáo tài xế; Hủy chuyến miễn phí và hoàn voucher cho khách."
- **Đánh giá:** ĐẠT.

---

### Case 6: Rào chắn công trình / Phân luồng nội khu tạm thời
- **Input:**
  - `telemetry`: Xe dừng trước rào chắn phân luồng nội khu tòa S2.05 suốt 3 phút.
  - `traffic_context`: Cảnh báo rào chắn công trình tạm thời.
  - `chat_log`: `Tài xế: "Đường nội khu sảnh này đang rào thi công chặn xe ô tô, anh phải chạy vòng qua ngã ba mất thêm 5 phút."`
- **Output mong đợi (AI):**
  - `predicted_label`: "Vướng rào chắn phân luồng công trình"
  - `confidence`: 0.91
  - `evidence_quote`: "Đường nội khu sảnh này đang rào thi công chặn xe ô tô"
  - `recommendation`: "Miễn trừ trách nhiệm cho tài xế; Thông báo thời gian đón kéo dài cho khách lựa chọn."
- **Đánh giá:** ĐẠT.

---

### Case 7: Khách hàng tự đổi ý nhưng đổ lỗi cho tài xế
- **Input:**
  - `telemetry`: Xe di chuyển thẳng tắp về điểm đón với vận tốc 25 km/h, khoảng cách giảm từ 1.2km xuống 300m trong 3 phút.
  - `traffic_context`: Bình thường.
  - `chat_log`: `Khách: "Tôi đi nhờ xe bạn tôi rồi, anh đừng đến nữa hủy cuốc đi."`
- **Output mong đợi (AI):**
  - `predicted_label`: "Khách hàng tự ý hủy chuyến (Tài xế không có lỗi)"
  - `confidence`: 0.97
  - `evidence_quote`: "Tôi đi nhờ xe bạn tôi rồi, anh đừng đến nữa hủy cuốc đi."
  - `recommendation`: "Bảo lưu 100% tỷ lệ hoàn thành cuốc cho tài xế; Áp dụng quy tắc phí hủy đối với khách hàng theo quy chế."
- **Đánh giá:** ĐẠT.

---

### Case 8: Tài xế dùng từ ngữ viết tắt / tiếng lóng để né bộ lọc
- **Input:**
  - `telemetry`: Xe đứng im 4 phút tại quán cà phê.
  - `traffic_context`: Bình thường.
  - `chat_log`: `Tài xế: "k di dc dau e oi tu huy giup a vs dang ban"`
- **Output mong đợi (AI):**
  - `predicted_label`: "Tài xế cố tình ngâm cuốc ép khách hủy (Dùng teencode)"
  - `confidence`: 0.92
  - `evidence_quote`: "k di dc dau e oi tu huy giup a vs dang ban" (Dịch nghĩa chuẩn hóa: "không đi được đâu em ơi tự hủy giúp anh với đang bận").
  - `recommendation`: "Duyệt vi phạm tài xế; Giải cứu cuốc xe cho khách."
- **Đánh giá:** ĐẠT (Mô hình hiểu được ngôn ngữ viết tắt tiếng Việt).

---

### Case 9: Thời tiết bất khả kháng (Mưa bão ngập úng)
- **Input:**
  - `telemetry`: Xe dừng sát khu vực đường trũng ngập nước.
  - `traffic_context`: Cảnh báo ngập úng đô thị mức độ nghiêm trọng.
  - `chat_log`: `Tài xế: "Đoạn đường gom ngập sâu nửa bánh xe ô tô điện không qua được nước vào pin em ơi."`
- **Output mong đợi (AI):**
  - `predicted_label`: "Thời tiết bất khả kháng / Ngập nước đường"
  - `confidence`: 0.96
  - `evidence_quote`: "Đoạn đường gom ngập sâu nửa bánh xe ô tô điện không qua được"
  - `recommendation`: "Miễn trừ trách nhiệm cả hai bên; Tự động đề xuất tuyến đường tránh hoặc phương tiện phù hợp."
- **Đánh giá:** ĐẠT.

---

### Case 10: Tài xế báo "Đã đến nơi" ảo (Fake Arrival)
- **Input:**
  - `telemetry`: Tài xế bấm trạng thái "Đã đến điểm đón" nhưng tọa độ GPS thực tế cách điểm đón 650m và xe đang dừng đèn đỏ.
  - `traffic_context`: Bình thường.
  - `chat_log`: `Khách: "Em đứng ngay sảnh có thấy xe đâu mà anh bấm đến nơi rồi?"`
- **Output mong đợi (AI):**
  - `predicted_label`: "Báo đến điểm đón ảo (Khoảng cách thực >500m)"
  - `confidence`: 0.94
  - `evidence_quote`: Trạng thái "Đã đến nơi" kích hoạt khi khoảng cách GPS còn 650m so với điểm ghim.
  - `recommendation`: "Khuyến nghị cảnh cáo tài xế gian lận thời gian chờ; Không tính phí chờ đối với khách hàng."
- **Đánh giá:** ĐẠT.
