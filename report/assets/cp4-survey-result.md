# Báo cáo kết quả Micro-Survey & Khảo sát sinh viên (CP4)

> **Mã tài liệu:** `cp4-survey-result`  
> **Phạm vi khảo sát:** 18 sinh viên (gồm 10 sinh viên phỏng vấn định tính ngoài nhóm do Phùng Văn Thanh Cao thực hiện và 8 sinh viên tham gia micro-survey nhanh tại lớp L3B).  
> **Mục tiêu:** Kiểm chứng định lượng về thời gian kiểm tra bài tập mỗi ngày, các kênh tiếp nhận thông tin, tần suất bỏ sót deadline và thái độ đối với giải pháp AI / tự động hóa.

---

## 1. Dữ liệu tổng hợp định lượng

### 1.1. Số lượng kênh thông tin học tập phải theo dõi mỗi ngày

| Số lượng kênh | Số sinh viên (N=18) | Tỷ lệ (%) | Kênh phổ biến nhất |
|:---:|:---:|:---:|---|
| Dưới 2 kênh | 0 | 0.0% | — |
| 2 – 3 kênh | 5 | 27.8% | Canvas LMS + Zalo |
| 4 – 5 kênh | 11 | 61.1% | Canvas LMS + Zalo + Outlook Email + Teams |
| Trên 5 kênh | 2 | 11.1% | Thêm Discord, Google Classroom, Notion |

> **Kết luận:** 100% sinh viên được khảo sát phải theo dõi từ 3 nguồn trở lên. Tình trạng phân mảnh thông tin là phổ quát.

---

### 1.2. Thời gian tiêu tốn cho việc rà soát bài tập mỗi tối

| Khoảng thời gian | Số sinh viên | Tỷ lệ (%) | Nhận định |
|---|:---:|:---:|---|
| Dưới 10 phút | 3 | 16.7% | Chỉ kiểm tra lướt qua LMS hoặc có người nhắc hộ |
| 15 – 25 phút | 12 | 66.7% | Mức trung bình phổ biến: mở từng kênh, lướt tin Zalo, lọc email |
| Trên 30 phút | 3 | 16.7% | Sinh viên làm đồ án nhóm, phải đối chiếu tiến độ của cả nhóm |

> **Baseline thời gian:** Trung bình sinh viên mất **khoảng 18–20 phút/tối**, tương đương với gần **2 giờ/tuần** chỉ cho việc đọc và rà soát thủ công. Trong đó, bước đọc tin nhắn Zalo chiếm thời gian lâu nhất (~6–10 phút).

---

### 1.3. Tần suất bỏ sót hoặc suýt trễ deadline trong 30 ngày gần nhất

| Tình trạng trong tháng qua | Số sinh viên | Tỷ lệ (%) | Nguyên nhân chính được nêu |
|---|:---:|:---:|---|
| Từng bị sót ít nhất 1 deadline (bị trừ điểm) | 9 | 50.0% | Thông báo dời hạn nộp bị trôi trong Zalo hoặc email |
| Từng suýt trễ deadline (phải thức đêm nộp bù) | 5 | 27.8% | Quên bài quiz trên LMS, chỉ nhớ bài lab thực hành |
| Không bị trễ lần nào | 4 | 22.2% | Có thói quen tự chép sổ tay hằng ngày hoặc có bạn nhắc |

> **Tỷ lệ ảnh hưởng:** **77.8% (14/18)** sinh viên gặp rắc rối với việc trễ hoặc suýt trễ deadline trong vòng 1 tháng gần nhất.

---

## 2. Nguồn gốc của các lần bỏ sót thông báo

Khảo sát sâu về nguyên nhân trực tiếp dẫn đến việc bỏ sót hoặc cập nhật trễ hạn nộp:

```text
[83.3%] Tin nhắn dặn dò, đổi lịch trong nhóm Zalo/Teams bị trôi
████████████████████████████████████████ 15/18 người

[61.1%] Email giảng viên bị chìm trong hộp thư rác/thông báo tự động
█████████████████████████████ 11/18 người

[16.7%] Quên không mở Canvas LMS kiểm tra lịch
████████ 3/18 người
```

> **Insight then chốt:** Lịch chính thức trên Canvas LMS rất ít khi bị bỏ sót vì giao diện đã có calendar rõ ràng. **Nguyên nhân cốt lõi gây sót deadline nằm ở các kênh giao tiếp phi cấu trúc (Zalo chat, email)** với những thông báo bất thường phát sinh giữa tuần.

---

## 3. Phản hồi của người dùng đối với các phương án giải pháp

| Phương án giải pháp | Đồng ý / Sẵn sàng dùng | Từ chối / E ngại | Lý do từ chối chính |
|---|:---:|:---:|---|
| **Cấp quyền cho bot tự đọc Zalo cá nhân** | 0 / 18 (0%) | **18 / 18 (100%)** | E ngại rủi ro rò rỉ dữ liệu cá nhân, lộ tin nhắn riêng tư |
| **Tự động đồng bộ LMS qua chuẩn iCal feed** | **18 / 18 (100%)** | 0 / 18 (0%) | Chuẩn mở, an toàn, không cần đăng nhập mật khẩu |
| **Chủ động forward/dán tin nhắn cho bot** | **15 / 18 (83.3%)** | 3 / 18 (16.7%) | 3 người ngại thao tác copy/dán mỗi ngày |
| **Nhận 1 bản tin Daily Digest 22h00 (≤ 5 dòng)** | **16 / 18 (88.9%)** | 2 / 18 (11.1%) | 2 người muốn nhận ngay lập tức thay vì đợi 22h |
| **Bắt buộc người bấm duyệt trước khi lưu vào lịch** | **17 / 18 (94.4%)** | 1 / 18 (5.6%) | Cần sự kiểm soát chắc chắn (Human-in-the-loop) |

---

## 4. Tác động của kết quả khảo sát đến thiết kế quy trình

1. **Hủy bỏ hoàn toàn** phương án can thiệp kiểu Agent tự động đăng nhập tài khoản Zalo cá nhân (loại bỏ rủi ro Viability & Security).
2. **Chuẩn hóa kiến trúc lai (Hybrid Workflow):**
   - LMS: Tự động hóa 100% bằng Rule (chuẩn iCal feed).
   - Zalo / Email: Dùng AI hỗ trợ bóc tách thông tin khi sinh viên chủ động dán hoặc forward nội dung.
   - Trình bày: Gom lại thành bản tin tóm tắt Daily Digest gửi vào 22h00 mỗi tối, khống chế độ dài dưới 5 dòng và luôn yêu cầu sinh viên duyệt trước khi ghi vào lịch Google Calendar.

