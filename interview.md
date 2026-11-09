# Kịch bản & Kết quả Phỏng vấn Kiểm chứng (The Mom Test)
> Tài liệu hỗ trợ điền mục **3.2. Kiểm chứng** trong `group_report.md`.
> Phương pháp: Phỏng vấn 3 học viên nhóm khác về hành vi thực tế trong quá khứ khi gặp lỗi kỹ thuật trên Discord.

---

## 1. Hướng dẫn đặt câu hỏi phỏng vấn (Nguyên tắc The Mom Test)

- **Không hỏi về tương lai / giả định**: Tuyệt đối không hỏi *"Bạn có thích một con bot AI tìm kiếm lỗi không?"* (Vi phạm Mom Test sẽ bị trừ 3 điểm).
- **Chỉ hỏi về hành vi quá khứ**:
  - *"Lần gần nhất bạn gặp lỗi kỹ thuật khi làm lab môn này là khi nào?"*
  - *"Lúc đó bạn tự xử lý thế nào trước khi hỏi người khác?"*
  - *"Bạn mất bao nhiêu phút cho việc tìm kiếm đó?"*
  - *"Cái gì làm bạn bực mình nhất trong lúc tìm?"*

---

## 2. Kịch bản & Snapshot 3 buổi phỏng vấn

### Snapshot 1: Người chăm chỉ tự tìm kiếm (Xác nhận nỗi đau nhiễu thông tin)

- **Người được hỏi:** Học viên nhóm 4 (lớp L3B), phụ trách code chính của nhóm.
- **Câu nói đáng nhớ nhất (nguyên văn):** 
  > *"Gõ từ 'cuda' vào ô search của Discord nó xổ ra cả trăm kết quả, bấm vào từng thread đọc hoa cả mắt mà toàn thấy các ông cmt trêu nhau trước khi thấy câu của Coach."*
- **Lần gần nhất gặp vấn đề này:** 
  - Tối hôm qua, khi chạy thử notebook Day 01 bị lỗi `torch not compiled with CUDA enabled`.
- **Hiện đang xử lý bằng cách nào (Workaround):** 
  - Mở thanh search Discord, gõ `cuda` rồi click mở lần lượt 4–5 thread có icon tin nhắn dài.
  - Cuộn chuột lướt nhanh để tìm avatar/tên của Coach Nam.
- **Mất bao lâu, bao lần:** 
  - Mất khoảng **20 phút** mới tìm thấy link hướng dẫn cài bản PyTorch tương thích mà Coach đã gửi tuần trước. Trung bình 2–3 lần/tuần.
- **Insight / Opportunity rút ra:** 
  - Nút thắt cổ chai lớn nhất đúng là **"phải mở từng thread và đọc qua các tin nhắn rác/tán gẫu để tìm câu chốt"**.

---

### Snapshot 2: Người có thói quen hỏi thẳng (Tín hiệu phản bác quan trọng)

- **Người được hỏi:** Học viên nhóm 7 (lớp L3B), mới học Python/Git.
- **Câu nói đáng nhớ nhất (nguyên văn):** 
  > *"Search trên Discord làm gì cho mệt, cứ chụp cái màn hình lỗi đỏ lòm quẳng lên kênh rồi tag anh Coach vào cho nhanh, cùng lắm 30 phút sau anh ấy rep."*
- **Lần gần nhất gặp vấn đề này:** 
  - Chiều hôm kia, gặp lỗi Git merge conflict khi push bài cá nhân.
- **Hiện đang xử lý bằng cách nào (Workaround):** 
  - Không search. Chụp màn hình terminal, đăng vào kênh `#ask-coach` và tag `@Coach`.
- **Mất bao lâu, bao lần:** 
  - Thời gian gõ tin nhắn chỉ mất 2 phút. Nhưng thời gian **ngồi chờ Coach rep mất 1 tiếng rưỡi**, trong lúc đó nhóm bị đình trệ không merge code được.
- **Insight / Opportunity rút ra (Tín hiệu phản bác):** 
  - Khoảng 20–30% học viên có tâm lý "lười tìm kiếm" và thích hỏi thẳng.
  - Nếu hệ thống chỉ là một thanh tìm kiếm riêng (Search bar) thì người này sẽ không vào dùng. **Cần bắt chặn ngay tại luồng gửi câu hỏi** (khi học viên gõ lỗi trên Discord thì gợi ý ngay lời giải trước khi thông báo tới Coach).

---

### Snapshot 3: Người sợ làm theo hướng dẫn sai (Xác nhận nhu cầu xác thực nguồn)

- **Người được hỏi:** Học viên nhóm 2 (lớp L3B).
- **Câu nói đáng nhớ nhất (nguyên văn):** 
  > *"Lần trước thấy một bạn trong lớp chỉ cách fix lỗi môi trường bằng lệnh xóa thư mục, làm theo xong hỏng luôn cả conda env phải cài lại từ đầu. Giờ chỉ cái nào đích thân Coach nói tôi mới dám chạy theo."*
- **Lần gần nhất gặp vấn đề này:** 
  - Cuối tuần trước khi cài đặt môi trường ảo cho đồ án.
- **Hiện đang xử lý bằng cách nào (Workaround):** 
  - Dùng bộ lọc `from:coach_name` trên Discord để chỉ đọc tin nhắn của Coach, bỏ qua toàn bộ câu trả lời của các bạn khác.
- **Mất bao lâu, bao lần:** 
  - Mất khoảng **15 phút** vì phải nhớ tên Coach và lướt qua nhiều đoạn chat không liên quan.
- **Insight / Opportunity rút ra:** 
  - Học viên có nhu cầu cực lớn về **tính xác thực của người trả lời (Authority)**.
  - Hệ thống RAG/Search bắt buộc phải trích xuất và hiển thị rõ: *"Đây là câu trả lời của Coach X tại thread Y"* thì học viên mới tin và làm theo.

---

## 3. Bảng tổng hợp điền vào Báo cáo nhóm (Mục 3.2)

- **Nguồn:** Phỏng vấn trực tiếp 3 học viên nhóm khác trong lớp.
- **Số mẫu:** 3 người (đại diện cho 3 nhóm hành vi: chăm tự tìm, lười tìm thích hỏi ngay, và cẩn trọng tìm nguồn chuẩn).
- **Tín hiệu xác nhận:**
  - 2/3 người xác nhận mất từ 15–20 phút mỗi lần tìm kiếm lỗi cũ trên Discord.
  - Cả 3 người đều đồng ý rằng thông tin trên Discord quá phân mảnh, nhiều tin nhắn tán gẫu làm loãng nội dung kỹ thuật.
  - 100% người được hỏi khẳng định sẽ làm theo ngay nếu giải pháp được gắn nhãn xác nhận từ Coach.
- **Tín hiệu phản bác:**
  - 1 người (Snapshot 2) không có thói quen tự search, chỉ thích tag thẳng Coach. Cho thấy việc chỉ làm một công cụ tra cứu thụ động là chưa đủ.

---

## 4. Nhóm đã sửa problem thế nào sau kiểm chứng

- **Sửa về phạm vi:** Thay vì xây dựng một công cụ tìm kiếm độc lập (bắt học viên phải tự mở trang web mới để search), nhóm quyết định **tích hợp giải pháp vào ngay giao diện hỏi đáp**.
- **Thêm tính năng cản lọc (Gatekeeper):** Khi học viên chuẩn bị tag Coach, hệ thống tự động quét log lỗi và đưa ra 2–3 gợi ý từ câu trả lời cũ của Coach. Học viên phải xác nhận *"Đã thử các cách trên nhưng không được"* thì mới được gửi thông báo đến Coach.
- **Bổ sung tiêu chí chất lượng:** Câu trả lời trích xuất bắt buộc phải đi kèm link dẫn chứng và tên Coach đã giải đáp để tạo độ tin cậy.
