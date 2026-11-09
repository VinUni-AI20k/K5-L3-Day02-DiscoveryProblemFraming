# Báo cáo cá nhân — 202603664_NguyenVietManhKhai

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp. Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md). Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Viết Mạnh Khải
- MSSV: 2A202603664
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: ABC
- Link repo nhóm: https://github.com/manhkhai205/K5-L3A-Day02-ABC-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| \#  | Lăng kính                         | Job Story: Khi… tôi muốn… để…                                                                                                                                                                                                                                                           | Ai chịu ảnh hưởng?                                              | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)                                                                                    |
| --- | --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Lặp lại                           | Khi nhiều khách nhắn tin hỏi cùng thông số sản phẩm (size, chất liệu, tồn kho) hoặc chính sách đổi trả trong giờ cao điểm, tôi muốn có ngay thông tin chuẩn xác theo đúng mã hàng khách đang hỏi, để phản hồi dưới 1 phút mà không phải mở file tra cứu và gõ lại nhiều lần             | Nhân viên sales trực page / CSKH, Khách mua hàng                | Mất 2–3 phút/tin nhắn để tra cứu và gõ lại; lặp lại 30–50 lần/ca trực (đếm từ lịch sử chat Fanpage/Shopee)                                   |
| 2   | Tốn thời gian                     | Khi khách đã chốt mẫu, số lượng, SĐT và địa chỉ nằm rải rác trong đoạn chat dài, tôi muốn gom đủ thông tin đặt hàng vào đúng các trường tạo đơn, để không phải cuộn ngược đoạn chat copy-paste từng dòng và tránh nhập sai mã hàng/địa chỉ                                              | Nhân viên sales tạo đơn, Nhân viên kho, Khách hàng              | Mất 3–5 phút/đơn để lọc chat và nhập sang POS; 25–40 đơn/ca; trung bình 2–3 đơn/tuần bị nhập nhầm phân loại hoặc sai SĐT/địa chỉ             |
| 3   | Lặp lại                           | Khi khách hỏi một mẫu còn màu/size cụ thể hay không trong lúc đang chạy sale, tôi muốn biết ngay số tồn thực tế có thể bán (đã trừ hàng đang giữ ở đơn nháp khác), để chốt đơn ngay mà không báo nhầm "còn hàng" cho mã đã hết                                                          | Nhân viên sales trực page, Nhân viên kho, Khách hàng            | 15–20 lần/ngày phải chuyển tab sang file kho hoặc nhắn hỏi kho (1–2 phút/lần); 3–4 đơn/tuần phải nhắn xin lỗi khách vì báo còn nhưng kho hết |
| 4   | Lặp lại                           | Khi danh sách vận chuyển mỗi sáng báo có các đơn "Giao không thành công / Chờ xác nhận giao lại", tôi muốn nắm ngay danh sách khách cần liên hệ kèm lý do bưu tá ghi chú, để nhắn/gọi khách xác nhận giao lại trước giờ bưu cục chuyển hoàn                                             | Nhân viên CSKH / Quản lý đơn, Khách hàng                        | Mất 35–45 phút mỗi sáng để lọc danh sách đơn delay từ đơn vị vận chuyển; trung bình 10–15 đơn/ngày                                           |
| 5   | Tốn thời gian                     | Khi kiểm kê kho và chốt số liệu cuối tuần, tôi muốn biết ngay những mã hàng nào đang bị lệch giữa sổ kho thực tế, phần mềm bán hàng và tồn trên sàn TMĐT, để tìm ra nguyên nhân lệch mà không phải dò tay từng dòng Excel                                                               | Nhân viên quản lý kho, Quản lý đơn hàng, Chủ shop               | Mất khoảng 90–120 phút mỗi cuối tuần để xuất 3 file Excel và đối chiếu thủ công; trung bình 5–8 SKU bị lệch mỗi tuần                         |
| 6   | Cần đọc, tổng hợp nhiều thông tin | Khi khách nhắn tin báo nhận sai hàng hoặc hàng lỗi kèm ảnh/video unbox, tôi muốn kiểm tra nhanh lịch sử tư vấn, mã vận đơn gốc, người đóng gói và tồn kho mã thay thế ở một chỗ, để đưa ra phương án đổi trả cho khách ngay trong một lần trao đổi                                      | Nhân viên CSKH, Nhân viên kho đóng gói, Khách hàng              | Mất 10–15 phút/ca khiếu nại để tra chéo 3 nơi (khung chat, phần mềm POS, nhóm Zalo kho); 6–10 ca/tuần                                        |
| 7   | Cần đọc, tổng hợp nhiều thông tin | Khi bắt đầu ca trực mới và nhận bàn giao các hội thoại khách đang tư vấn dở hoặc đang khiếu nại, tôi muốn nắm nhanh khách đã hỏi gì và đã được ca trước hứa hẹn gì, để tư vấn tiếp mạch lạc mà không hỏi lại thông tin khách đã cung cấp                                                | Nhân viên sales/CSKH giữa các ca (ca sáng ↔ ca tối), Khách hàng | Mất 3–4 phút/hội thoại để cuộn đọc lại tin nhắn cũ; 10–15 hội thoại bàn giao/ngày; tuần nào cũng có 2–3 khách phàn nàn vì phải nhắc lại      |
| 8   | Pain từ người khác                | Khi nhân viên kho nhận danh sách đơn cần nhặt hàng và đóng gói trong ngày, họ muốn các yêu cầu đặc biệt của khách (gói quà, che tên sản phẩm, giao giờ hành chính, đổi màu quà tặng) được ghi theo chuẩn cố định trên phiếu in, để không đóng sai hoặc phải chụp đơn nhắn hỏi lại sales | Nhân viên kho/đóng gói, Nhân viên sales tạo đơn, Khách hàng     | Nhân viên kho phải nhắn vào group Zalo nội bộ hỏi lại sales 5–8 lần/ngày; mỗi lần chờ phản hồi 5–10 phút làm ngắt quãng việc đóng gói        |
| 9   | Cần đọc, tổng hợp nhiều thông tin | Khi làm báo cáo cuối tuần cho quản lý, tôi muốn tổng hợp được các lý do chính khiến khách hủy đơn, đổi trả hoặc đánh giá 1–3 sao từ tin nhắn và mục review sàn, để biết mã hàng nào đang bị lỗi chất lượng hoặc mô tả lệch thực tế                                                      | Nhân viên CSKH, Quản lý bán hàng, Bộ phận nhập hàng             | Mất 60–90 phút mỗi chiều thứ Bảy để đọc lại log lý do hoàn đơn và đánh giá xấu của ~40–50 đơn hoàn/tuần                                      |
| 10  | Pain từ người khác                | Khi khách hàng đã gửi trả lại hàng lỗi về kho được 2–3 ngày, họ muốn biết kho đã nhận hàng kiểm tra chưa và khi nào được gửi đơn mới/hoàn tiền, để yên tâm mà không phải chủ động nhắn tin giục shop nhiều lần                                                                          | Khách hàng đổi trả, Nhân viên CSKH, Bộ phận kho/kế toán         | Khoảng 70–80% khách đổi trả (8–12 người/tuần) phải nhắn tin hỏi lại _"Shop nhận được hàng hoàn chưa?"_ ít nhất 1–2 lần (đếm từ lịch sử chat) |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Tự nghĩ ban đầu: ý **#1** (trả lời lặp lại thông tin sản phẩm, chính sách đổi trả) và **#2** (tạo đơn từ thông tin khách hàng trong chat).
- Ý AI gợi ý mà tôi **giữ lại** (sau khi chỉnh lại số liệu theo công việc thật): **#3, #4, #5, #6, #7, #8, #9, #10** (đủ 10 problems trải đều 4 lăng kính) vì phản ánh đúng các điểm nghẽn thật hàng ngày giữa trực page – lên đơn – đối soát kho trong thương mại điện tử.
- Ý tôi **bỏ**:
    - Ý _"Xây dựng trợ lý AI toàn năng tự động tư vấn, chốt đơn và quản lý kho từ A–Z"_: bỏ vì quá rộng, mang tính giải pháp (solution-first) và không chỉ ra một bước bottleneck cụ thể nào.
    - Ý _"Tổng hợp báo cáo phân tích xu hướng thị trường và đánh giá đối thủ hằng tuần"_: bỏ vì không nằm trong công việc vận hành trực page, tạo đơn và kho hàng hằng tuần của nhân viên sales/CSKH.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                                                  | Vì sao chọn                                                                                                                      | Điều còn chưa chắc                                                                                                 |
| ---- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| 1    | Tạo đơn từ hội thoại chat (#2)                           | Xảy ra liên tục mỗi ngày (25–40 lần/ca), quy trình rõ từng bước, đo thời gian và tỷ lệ sai sót dễ dàng, rất vừa sức một buổi lab | Địa chỉ khách viết tắt/thiếu phường xã hoặc đổi ý giữa chừng trong chat thì xử lý bằng Rule hay AI sẽ ổn định hơn? |
| 2    | Trả lời lặp lại về thông số SP & chính sách đổi trả (#1) | Tần suất rất cao (30–50 lần/ca), ảnh hưởng trực tiếp đến tốc độ phản hồi và tỷ lệ chốt đơn                                       | Bao nhiêu % câu hỏi giải quyết được chỉ bằng bộ phím tắt (quick replies) có sẵn mà không cần AI?                   |
| 3    | Tra cứu chéo khi xử lý khiếu nại đổi/trả hàng (#6)       | Mỗi ca tốn 10–15 phút vì thông tin nằm rải rác ở 3 nơi, khách đang bức xúc nên cần phản hồi nhanh                                | Việc nối dữ liệu giữa khung chat, phần mềm POS và kho có khả thi trong phạm vi nhỏ không?                          |

### Problem Card #1

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                                                                                                                               |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi khách đã chốt mẫu, số lượng, SĐT và địa chỉ nằm rải rác trong đoạn chat dài, tôi muốn gom đủ thông tin đặt hàng vào đúng các trường tạo đơn, để không phải cuộn ngược đoạn chat copy-paste từng dòng và tránh nhập sai mã hàng/địa chỉ                                                                                                                                             |
| Actor                                     | Nhân viên sales trực page kiêm lên đơn (bán hàng TMĐT / Fanpage)                                                                                                                                                                                                                                                                                                                       |
| Thời điểm / bối cảnh                      | Ngay sau khi khách nhắn chốt mua trên khung chat (đặc biệt dồn dập vào khung giờ cao điểm 12h–14h và 20h–22h)                                                                                                                                                                                                                                                                          |
| Quy trình hiện tại (3–7 bước)             | 1\. Cuộn ngược đoạn chat (15–30 tin nhắn) để tìm tên SP, màu, size, số lượng, SĐT, địa chỉ, ghi chú · 2. Mở tab phần mềm tạo đơn (POS) · 3. Copy-paste SĐT, tên, địa chỉ và chọn lại Tỉnh/Quận/Phường từ dropdown · 4. Gõ tìm mã SKU sản phẩm, chọn phân loại màu/size và nhập số lượng · 5. Tóm tắt lại thông tin đơn gửi vào chat để khách xác nhận · 6. Bấm lưu và đẩy đơn sang kho |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 1 + Bước 3 & 4 (đọc ngược đoạn chat rời rạc rồi copy-paste/chọn lại từng trường sang POS): mất khoảng 3–4 phút/đơn                                                                                                                                                                                                                                                                |
| Impact (nếu không giải thì sao)           | Với 30 đơn/ca, nhân viên mất \~100–120 phút/ngày chỉ để nhập liệu thủ công; giờ cao điểm bị ùn ứ tin nhắn khách mới; trung bình 2–3 đơn/tuần bị sai phân loại màu/size hoặc sai địa chỉ dẫn đến phí hoàn hàng                                                                                                                                                                          |
| Success metric (baseline → target)        | Thời gian tạo 1 đơn giảm từ trung bình 4 phút xuống dưới 1 phút; số đơn nhập sai thông tin khách/SKU giảm từ 2–3 đơn/tuần xuống 0–1 đơn/tuần                                                                                                                                                                                                                                           |
| Phương án không dùng AI                   | Gửi form mẫu 1 tin nhắn yêu cầu khách điền đủ (Họ tên + SĐT + Địa chỉ + Màu/Size) trước khi chốt; kết hợp phím tắt copy nhanh. Nhược điểm: nhiều khách ngại điền form hoặc vẫn nhắn tách lẻ nhiều câu                                                                                                                                                                                  |
| Giả thuyết về AI (nếu có)                 | AI đọc đoạn hội thoại vừa chat, tự trích xuất thành JSON/bảng chuẩn (Tên, SĐT, Địa chỉ tách sẵn Tỉnh/Huyện/Xã, Mã SKU, Size, Màu, Ghi chú) + soạn sẵn tin nhắn xác nhận đơn; nhân viên sales chỉ kiểm lại 1 lần rồi bấm tạo đơn                                                                                                                                                        |
| Cảm nhận nhanh                            | Workflow                                                                                                                                                                                                                                                                                                                                                                               |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 4 phút/đơn (~120 phút/ca cho 30 đơn)

[1 Cuộn chat tìm SĐT, địa chỉ, mẫu/size: 60s] ← BOTTLENECK 1
→ [2 Mở phần mềm POS tạo đơn mới: 15s]
→ [3 Copy-paste Tên, SĐT, Địa chỉ + chọn Tỉnh/Huyện/Xã: 75s] ← BOTTLENECK 2
→ [4 Tìm mã SKU, chọn màu/size, số lượng, ghi chú: 45s]
→ [5 Gõ lại tóm tắt đơn gửi khách xác nhận: 30s]
→ [6 Lưu đơn & chuyển kho: 15s]
```

### Problem Card #2

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                                                                                       |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi nhiều khách nhắn tin hỏi cùng thông số sản phẩm (size, chất liệu) hoặc chính sách đổi trả trong giờ cao điểm, tôi muốn có ngay thông tin chuẩn xác theo đúng mã hàng khách đang hỏi, để phản hồi dưới 1 phút mà không phải mở file tra cứu và gõ lại nhiều lần                                                                             |
| Actor                                     | Nhân viên trực page / CSKH thương mại điện tử                                                                                                                                                                                                                                                                                                  |
| Thời điểm / bối cảnh                      | Trong ca trực page hằng ngày, nhất là khi chạy quảng cáo nhiều khách hỏi cùng lúc về bảng size và quy trình đổi trả                                                                                                                                                                                                                            |
| Quy trình hiện tại (3–7 bước)             | 1\. Đọc tin nhắn và xác định mẫu sản phẩm khách đang hỏi (qua ảnh hoặc link) · 2. Mở file Google Sheets thông số sản phẩm / bảng quy đổi size theo chiều cao cân nặng · 3. Tìm dòng sản phẩm tương ứng và đối chiếu số đo của khách · 4. Mở file quy định đổi trả (nếu khách hỏi chính sách) · 5. Soạn câu trả lời vào khung chat và gửi khách |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3 (chuyển tab tìm đúng mã sản phẩm trong bảng Sheets nhiều SKU và đối chiếu thông số): mất khoảng 1,5–2 phút/lần                                                                                                                                                                                                                        |
| Impact (nếu không giải thì sao)           | Mất 2,5–3 phút/tin nhắn × 40 lượt hỏi/ca = \~100–120 phút/ca; phản hồi chậm quá 5 phút làm khách thoát chat sang shop khác                                                                                                                                                                                                                     |
| Success metric (baseline → target)        | Thời gian phản hồi câu hỏi thông số/chính sách giảm từ 2,5–3 phút xuống dưới 45 giây/tin nhắn                                                                                                                                                                                                                                                  |
| Phương án không dùng AI                   | Bộ câu trả lời nhanh (Quick Replies / Saved Replies) gắn theo từ khóa + ảnh bảng size chuẩn gắn sẵn vào từng album sản phẩm                                                                                                                                                                                                                    |
| Giả thuyết về AI (nếu có)                 | Dựa trên sản phẩm khách đang hỏi và chiều cao/cân nặng khách nhắn, AI gợi ý sẵn câu trả lời nháp kèm size phù hợp và chính sách đổi trả đúng mã hàng để nhân viên bấm gửi sau khi đọc lướt                                                                                                                                                     |
| Cảm nhận nhanh                            | Rule / Workflow                                                                                                                                                                                                                                                                                                                                |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 2,5–3 phút/lượt hỏi (~100 phút/ca cho 40 lượt)

[1 Xem ảnh/link xác định mẫu khách hỏi: 20s]
→ [2 Chuyển tab mở Sheets thông số & tìm mã SKU: 60s] ← BOTTLENECK
→ [3 Đối chiếu chiều cao/cân nặng khách với bảng size: 30s]
→ [4 Gõ câu tư vấn + chính sách đổi trả vào chat: 45s]
→ [5 Kiểm tra & gửi khách: 15s]
```

### Problem Card #3

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                                                                                                                                                       |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi khách nhắn tin báo nh ận sai hàng hoặc hàng lỗi kèm ảnh/video unbox, tôi muốn kiểm tra nhanh lịch sử tư vấn, mã vận đơn gốc, người đóng gói và tồn kho mã thay thế ở một chỗ, để đưa ra phương án đổi trả cho khách ngay trong một lần trao đổi                                                                                                                                                            |
| Actor                                     | Nhân viên CSKH xử lý sau bán và Nhân viên kho                                                                                                                                                                                                                                                                                                                                                                  |
| Thời điểm / bối cảnh                      | Khi khách hàng nhận đơn và nhắn tin khiếu nại muốn đổi size/màu hoặc báo sản phẩm lỗi/giao nhầm                                                                                                                                                                                                                                                                                                                |
| Quy trình hiện tại (3–7 bước)             | 1\. Nhận tin nhắn + ảnh/video phản ánh của khách và xin SĐT/mã đơn · 2. Tra mã đơn trên POS để xem sản phẩm đã đặt trên đơn là gì · 3. Cuộn lại lịch sử chat cũ lúc mua để xem lỗi do sales lên nhầm đơn hay do kho nhặt nhầm · 4. Nhắn vào group Zalo kho để hỏi ca đóng gói và kiểm tra tồn kho thực tế của mã cần đổi · 5. Chờ kho xác nhận rồi nhắn lại phương án giải quyết & hướng dẫn thu hồi cho khách |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & 4 (đối chiếu lịch sử chat cũ + nhắn hỏi kho chờ xác nhận tồn thực tế): mất 8–10 phút/ca                                                                                                                                                                                                                                                                                                               |
| Impact (nếu không giải thì sao)           | Mỗi ca mất 12–15 phút (6–10 ca/tuần = \~90–120 phút/tuần); khách phải chờ lâu dễ bức xúc và đánh giá 1 sao trên sàn trước khi shop kịp xử lý                                                                                                                                                                                                                                                                   |
| Success metric (baseline → target)        | Thời gian từ lúc khách gửi đủ thông tin đến lúc chốt phương án đổi trả giảm từ 15 phút xuống dưới 5 phút/ca                                                                                                                                                                                                                                                                                                    |
| Phương án không dùng AI                   | Phiếu form tiếp nhận đổi trả chuẩn + quy tắc phân quyền cho CSKH tự quyết định đổi ngay với đơn dưới một mức giá trị nhất định nếu đã có video unbox rõ ràng                                                                                                                                                                                                                                                   |
| Giả thuyết về AI (nếu có)                 | Khi nhập SĐT/mã đơn, hệ thống gom thông tin đơn POS + tóm tắt đoạn chốt đơn cũ + tồn kho mã thay thế và gợi ý phương án xử lý theo đúng quy định đổi trả của shop                                                                                                                                                                                                                                              |
| Cảm nhận nhanh                            | Workflow                                                                                                                                                                                                                                                                                                                                                                                                       |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 14 phút/ca khiếu nại (~100 phút/tuần)

[1 Tiếp nhận tin nhắn + ảnh/video & xin SĐT: 2']
→ [2 Tra đơn trên phần mềm POS: 2']
→ [3 Đọc lại lịch sử chat lúc chốt đơn để xác định nguyên nhân: 4'] ← BOTTLENECK 1
→ [4 Nhắn group Zalo kho hỏi người đóng & tồn mã đổi: 4'] ← BOTTLENECK 2
→ [5 Phản hồi phương án & tạo đơn đổi cho khách: 2']
```

### Card muốn pitch nhất

- Card số: **Card #1 — Tạo đơn từ hội thoại chat**
- Vì sao: Đây là công việc lặp lại nhiều nhất mỗi ngày của nhân viên sales trực page, các bước thủ công rất rõ ràng, dữ liệu đầu vào nằm sẵn ngay trong đoạn hội thoại (không cần quyền truy cập hệ thống phức tạp), dễ đo baseline và dễ so sánh rạch ròi giữa No AI (form mẫu) – Rule (regex bắt SĐT) – Workflow (AI trích xuất thông tin từ chat tự nhiên sang các trường tạo đơn).
- Câu hỏi muốn nhóm phản biện: _"Nếu bắt buộc khách điền theo form mẫu cố định (No AI / Rule) thì đã giải quyết được bao nhiêu % vấn đề rồi? Khi nào mới thật sự cần đến AI đọc hội thoại để trích xuất thông tin đơn hàng?"_

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                                                                                            | Đồng ý?         | Đã sửa gì                                                                                                                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ở Card #1, nếu khách nhắn 1 tin nhắn chuẩn cấu trúc thì chỉ cần Rule/Regex hoặc copy nhanh, chưa chắc cần AI                  | Đồng ý một phần | Làm rõ bối cảnh thực tế: khách thường nhắn rải rác qua 5–10 câu chat (đổi màu, đổi size, gửi SĐT ở câu trên, địa chỉ viết tắt ở câu dưới), và bổ sung phương án "Form mẫu" vào mục _Phương án không dùng AI_ để đối chiếu |
| Metric ban đầu chỉ đo thời gian tạo đơn (từ 4 phút xuống 1 phút), nếu làm nhanh nhưng trích xuất sai size/địa chỉ thì hại hơn | Đồng ý          | Bổ sung metric chất lượng: _"Số đơn nhập sai thông tin khách/SKU giảm từ 2–3 đơn/tuần xuống 0–1 đơn/tuần"_ và giữ bước nhân viên sales kiểm tra trước khi bấm lưu đơn                                                     |
| Baseline 4 phút/đơn và 30 đơn/ca đang là con số ước lượng theo cảm giác                                                       | Đồng ý          | Ghi chú cần bấm giờ thực tế trên 10 đơn liên tiếp ở ca trực gần nhất để lấy baseline chính xác ở bước kiểm chứng (CP4)                                                                                                    |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì?         | Kết quả / ảnh hưởng tới bài nhóm |
| -------------------------- | ---------------------- | -------------------------------- |
| Pitch Problem Card         | Trình bày 3 Problem Cards về vận hành TMĐT (#4 Tạo đơn từ chat, #5 Trả lời thông số SP & đổi trả, #6 Xử lý khiếu nại đổi trả) | Bài #4 (Tạo đơn từ hội thoại chat) đạt 34/35 điểm và được cả nhóm chọn làm bài toán chính |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Hỏi Trọng (#2 Onboarding): *"Dùng script/rule theo chức danh có giải quyết được luôn không?"*; Hỏi Thắng (#9 Bác sĩ cấp cứu): *"Nhóm có tiếp cận được bác sĩ và biên bản thật trong buổi học hôm nay không?"* | Giúp nhóm nhận ra bài #2 chỉ cần Rule và bài #9 có rủi ro Feasibility/Viability quá cao trong phạm vi buổi lab |
| Nhận phản biện             | Câu hỏi tôi nhận được: Trọng hỏi *"Nếu khách hàng muốn thay đổi thông tin hoặc sản phẩm khác giữa chừng thì sao?"*; Thắng hỏi về việc dùng Quick Replies / Form mẫu | Tôi đã sửa gì: Bổ sung trường hợp khách đổi ý màu/size nhiều lần trong chat làm bottleneck cốt lõi và đưa phương án Form mẫu vào kiểm chứng ở CP4 |
| Gom cluster / cây OST      | Cùng nhóm gom 9 candidate thành 3 Cluster (A: Đọc hội thoại trích xuất; B: Tra cứu đa nguồn; C: Quy trình IT lặp lại) và vẽ cây OST cho bài tạo đơn | Tách bạch được 3 Opportunities thật khỏi các giải pháp đội lốt ("chatbot tự động chốt đơn") |
| Chọn candidate problem     | Cung cấp số liệu thực tế và log hội thoại mẫu để chấm điểm 7 tiêu chí | Nhóm đồng thuận chọn bài #4 để đi tiếp CP4–CP6 |
| Kiểm chứng / research      | Cung cấp log 15 đơn hàng thật trên Fanpage, phỏng vấn nhanh 2 nhân viên trực page và đối chiếu tính năng có sẵn của Pancake POS / Sapo Social | Giúp nhóm phát hiện phần bắt SĐT đã có sẵn bằng Rule trên POS, từ đó thu hẹp bài toán vào phần đọc ngữ cảnh chốt SKU rải rác và chuẩn hóa địa chỉ/ghi chú |
| Quy trình nhóm             | Vẽ quy trình hiện tại (6 bước, 240 giây) và quy trình tương lai (5 bước, ~55 giây) phân tách rõ bước Rule, bước AI, bước Con người (HITL) và phương án Fallback | Nhóm dùng làm sơ đồ chính trong mục 4.1–4.3 của `group_report.md` |
| Problem Statement          | Cùng nhóm soạn Problem Statement v0 và cập nhật lên v1 sau phản biện (thu hẹp phạm vi vào đơn hội thoại dài ≥ 6 tin nhắn, bổ sung metric chất lượng ≥ 85% đơn nháp đúng) | Hoàn thiện mục 5 và mục 7 của `group_report.md` kèm 4 tiêu chí đánh giá đầu ra (eval) |
| Mức can thiệp AI           | Phân tích so sánh 4 mức (No AI / Rule / Workflow / Agent), điền AI Canvas và trả lời 2 câu hỏi Google PAIR (chọn Augment; tránh lỗi điền bừa False Positive bằng cách ép trả về `null` khi thiếu thông tin) | Nhóm chốt chọn mức **Workflow** kết hợp Rule có sẵn của POS |
| Quyết định                 | Cùng nhóm đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability), thiết kế Pilot 2 tuần (100 đơn) và đặt ngưỡng dừng cụ thể | Nhóm thống nhất quyết định **Go (phạm vi nhỏ)** |

---

## 5. Dùng AI

| Checkpoint                     | Tôi dùng AI để làm gì?                                                                                  | AI hữu ích ở đâu?                                                                                                                           | AI sai hoặc hời hợt ở đâu?                                                                         | Tôi sửa gì bằng nhận định của mình?                                                                                                                       |
| ------------------------------ | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CP1 Scan                       | Gợi ý thêm các problem theo 4 lăng kính từ vai trò sales/CSKH TMĐT và chuẩn hóa câu sang dạng Job Story | Giúp mở rộng nhanh từ 2 ý ban đầu lên 8 problem bao phủ đủ cả trực page, tạo đơn, khiếu nại và đối soát kho                                 | Các con số ước lượng ban đầu còn chung chung; có gợi ý hơi rộng nếu không giới hạn phạm vi         | Chọn lọc lại 6 ý sát nhất với việc vận hành hàng tuần, loại bỏ các ý quá rộng ("trợ lý AI toàn năng") và điền lại tần suất/thời gian theo ca trực thực tế |
| CP2 Problem Card               | Đóng vai PM hoài nghi để phản biện Top 3 Problem Cards                                                  | Chỉ ra rủi ro nếu chỉ đo tốc độ tạo đơn mà bỏ qua tỷ lệ nhập sai SKU/địa chỉ, và nhắc đối chiếu với phương án dùng Form mẫu / Quick Replies | Chưa tính đến thực tế khách hàng TMĐT thường nhắn tin tách lẻ nhiều dòng và ngại điền form cố định | Bổ sung metric chất lượng (giảm số đơn sai thông tin) và giữ bước nhân viên sales duyệt lại trước khi lưu đơn                                             |
| CP4 Research                   | Tìm kiếm các công cụ POS/Social Commerce đã giải quyết bài toán tạo đơn từ khung chat (Pancake, Sapo, OpenAI Structured Outputs) | Giúp đối chiếu nhanh bước nào phần mềm có sẵn đã làm tốt (quét SĐT, lưu khách cũ) và bước nào còn bỏ trống | AI đôi khi mô tả như thể phần mềm POS đã tự hiểu được toàn bộ nội dung chat tự nhiên | Kiểm tra lại tài liệu thực tế của Pancake/Sapo: chỉ ra rằng POS mới chỉ bắt SĐT/địa chỉ 1 dòng bằng Rule, còn phần khách đổi ý mẫu/màu/size qua nhiều câu chat vẫn phải đọc tay |
| CP5 Quy trình                  | Hỗ trợ chuẩn hóa sơ đồ ASCII quy trình trước/sau và bảng Before/After | Trình bày rõ ràng thời gian từng bước và điểm nghẽn (bottleneck) | Có xu hướng gộp bước "bắt SĐT bằng Rule" và "trích xuất SKU bằng AI" làm một bước chung | Tách riêng bước Rule có sẵn của POS (Bước 1) và bước AI trích xuất JSON (Bước 2), đồng thời ghi rõ Boundary không tự động đẩy đơn sang kho |
| CP5–6 Problem Statement        | Phản biện Problem Statement v0 để tìm lỗ hổng về Actor, Metric và Boundary | Chỉ ra việc gộp chung mọi đơn hàng vào Actor sẽ làm nhiễu baseline vì 40% đơn ngắn không cần AI | Chưa đưa ra ngưỡng con số cụ thể cho tỷ lệ bản nháp đạt yêu cầu | Tự đặt ngưỡng cụ thể ở v1: thu hẹp vào hội thoại ≥ 6 tin nhắn, yêu cầu ≥ 85% đơn nháp chỉ sửa tối đa 1 trường và ép trả về `null` kèm câu trích dẫn gốc `source_quote` |
| CP6 Mức can thiệp / quyết định | Rà soát AI Canvas, bộ tiêu chí đánh giá (Eval) và khung 4 rủi ro trước khi chốt Go/No-Go | Giúp cấu trúc hóa rõ ràng 4 tiêu chí Đạt/Không đạt cho đầu ra JSON của AI | Gợi ý tích hợp thẳng vào POS ngay từ đầu | Đổi sang phương án Pilot gọn nhẹ trong 2 tuần (100 đơn) trước khi xây Extension tích hợp sâu, kèm ngưỡng dừng nếu > 25% đơn nháp phải sửa từ 2 trường trở lên |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi nghe 3 vấn đề về quản trị hệ thống IT của Trọng (reset mật khẩu, onboarding tài khoản, phân quyền) và 3 vấn đề về bệnh viện/quản lý dự án của Thắng (báo cáo tháng, phân việc, bàn giao ca trực bác sĩ cấp cứu), tôi nhận ra rằng một vấn đề nghe có vẻ rất lớn và cấp thiết chưa chắc đã phù hợp để làm ngay nếu không tiếp cận được người dùng thật và dữ liệu thật để kiểm chứng. Ngược lại, những bài toán có quy trình cố định theo phòng ban như onboarding tài khoản thì chỉ cần dùng Rule/Script tự động hóa chứ chưa cần đến AI.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có, ở đầu CP3 khi vẽ cây Opportunity Solution Tree, nhóm từng viết nhánh *"Làm chatbot AI tự động chốt đơn và đẩy thẳng sang kho"*. Khi rà lại quy tắc tầng Opportunity chỉ được chứa nỗi đau (pain) chứ không chứa công cụ, nhóm đã gạch bỏ ý đó khỏi cây OST và quay lại bóc tách 3 nguyên nhân gốc làm nhân viên mất thời gian: thông tin nằm rải rác qua nhiều câu chat, khách đổi ý màu/size giữa chừng và phải chọn lại địa chỉ 3 cấp trên POS.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Lúc mới pitch Card #1, tôi nghĩ cần làm một công cụ AI đọc tin nhắn để tạo đơn từ A–Z cho mọi đơn hàng trên Fanpage và chỉ đo thời gian tạo đơn (từ 4 phút xuống 1 phút). Sau khi Trọng phản biện *"Nếu khách thay đổi thông tin hoặc đổi mẫu giữa chừng thì sao?"* và kiểm tra lại tính năng của Pancake/Sapo, tôi đã đổi ý hoàn toàn: phần bắt SĐT đã có Rule của POS làm rất tốt và 40% đơn nhắn gọn không cần AI; tôi thu hẹp bài toán vào 60% đơn có hội thoại tư vấn dài và bổ sung metric đo tỷ lệ sai đơn.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất khi kiểm tra lại 15 đơn hàng thật và hỏi 2 bạn trực page là: các phần mềm POS hiện nay như Pancake hay Sapo đã tự tô sáng SĐT và đồng bộ khách cũ rất nhanh, nhưng lại hoàn toàn "mù ngữ cảnh" khi khách nhắn kiểu tham chiếu ngược (*"lấy chị cái áo trắng đầu tiên nhưng đổi sang size L"*). Ngoài ra, phương án gửi Form mẫu bắt khách tự điền lại thông tin (No AI) tưởng là đơn giản nhất nhưng thực tế bị tới ~70% khách bỏ qua vì họ quen nhắn tin tự nhiên.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là viết sao cho đủ cụ thể về bước nghẽn (bottleneck) và ranh giới (boundary) mà không lồng sẵn giải pháp công nghệ vào câu mô tả vấn đề, đồng thời thiết lập được bộ Success Metric cân bằng giữa tốc độ (< 1 phút/đơn) và độ chính xác (≥ 85% đơn nháp chỉ sửa tối đa 1 trường, không làm tăng số đơn giao nhầm).

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, ngay từ bước CP2 tôi sẽ bấm giờ thực tế trên 20 đơn liên tiếp phân loại sẵn theo "đơn nhắn gọn 1 dòng" và "đơn tư vấn dài" thay vì ước lượng trung bình chung 4 phút/đơn. Tôi cũng sẽ phản biện nhóm mạnh hơn ở câu hỏi Google PAIR ngay từ sớm: ép rõ quy tắc nếu khách chưa nói rõ màu/size thì hệ thống bắt buộc phải trả về trống (`null`) và báo đỏ chứ tuyệt đối không được đoán mò.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi _problem → quy trình → metric → boundary → mức can thiệp AI → quyết định_ của bài nhóm mình.
Bài toán của nhóm bắt đầu từ việc nhân viên sales trực page phải mất trung bình 4 phút để cuộn đọc lại 15–30 câu chat rải rác (khi khách hỏi nhiều mẫu và đổi ý màu/size giữa chừng) rồi copy-paste từng trường sang phần mềm POS tạo đơn. Trong quy trình 6 bước hiện tại, bước bắt SĐT đã có sẵn bằng Rule trên POS, còn điểm nghẽn thật sự nằm ở bước đọc lọc lựa chọn cuối cùng của khách và chuẩn hóa địa chỉ viết tắt (chiếm 180/240 giây). Nhóm đặt mục tiêu (metric) giảm thời gian tạo đơn hội thoại dài từ 4 phút xuống dưới 1 phút, đạt tối thiểu 85% đơn nháp chỉ cần sửa tối đa 1 trường và giữ số đơn sai thông tin từ 2–3 đơn/tuần xuống không quá 1 đơn/tuần. Để tránh rủi ro giao nhầm hàng gây tốn phí ship hoàn 2 chiều, nhóm đặt boundary cứng là AI không tự động bấm lưu đơn đẩy sang kho và tuyệt đối không tự đoán màu/size khi khách nói mơ hồ (phải để `null` kèm cảnh báo đỏ và câu trích dẫn gốc cho nhân viên kiểm tra). Vì đầu vào là ngôn ngữ chat tự nhiên có độ mơ hồ cao nhưng các bước xử lý cố định, nhóm chọn mức can thiệp là **Workflow** (Rule bắt SĐT → AI trích xuất JSON đơn nháp + câu xác nhận → Nhân viên sales duyệt và bấm Lưu). Do các rủi ro Value, Usability, Feasibility đều ở mức thấp và đã kiểm chứng trên log đơn thật, nhóm quyết định **Go** với một Pilot gọn nhẹ trong 2 tuần (100 đơn hội thoại dài) kèm ngưỡng dừng nếu trên 25% đơn nháp phải sửa từ 2 trường trở lên.

---

## 7. Tài liệu tham khảo

- Tài liệu hướng dẫn Pancake POS & Vpage — Tạo đơn hàng từ hội thoại Fanpage: https://pancake.vn
- Sapo Social (Sapo Omni) — Tính năng tạo đơn trên khung chat Facebook: https://www.sapo.vn/quan-ly-ban-hang-online.html
- OpenAI Documentation — Structured Outputs (JSON Schema extraction): https://platform.openai.com/docs/guides/structured-outputs
- Anthropic — *Building Effective Agents* (Workflow vs. Agent): https://www.anthropic.com/research/building-effective-agents
- Tài liệu bài học: [01-worksheet.md](../../docs/01-worksheet.md), [02-deliverable-example.md](../../docs/02-deliverable-example.md).
