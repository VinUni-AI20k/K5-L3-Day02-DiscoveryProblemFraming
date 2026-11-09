# Báo cáo cá nhân — 2A202603446_NguyenThanhTung

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Thanh Tùng
- MSSV: 2A202603446
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Ban3
- Link repo nhóm: https://github.com/LysLama/K5-L3A-DAY02-Ban3-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi kiểm tra chất lượng tư vấn của 10 saler mỗi ngày trên Pancake, tôi muốn nhanh chóng phát hiện các lỗi sai về tư vấn liều lượng, chống chỉ định và thiếu ưu đãi, để kịp thời chấn chỉnh trước khi đơn hàng xuất kho. | Quản lý chất lượng (QA), Khách hàng, 10 saler | Mất 90–120 phút/ngày rà soát 20–25 đoạn chat (chỉ đạt ~8% trong 300 cuộc chat/ngày trên Pancake). Bằng chứng: Bảng chấm điểm audit QA hàng ngày. |
| 2 | Tốn thời gian | Khi lead mới đổ về từ quảng cáo vào đầu ca sáng, tôi muốn lọc trùng số điện thoại và phân bổ ngay cho đúng telesale đang trực, để khách được gọi trong vòng 15 phút đầu. | Quản lý vận hành, 8 Telesaler, Khách để lại SĐT | Mất 45 phút mỗi sáng tải file Excel từ Ads/Fanpage, rà trùng 150 số điện thoại với dữ liệu 30 ngày qua trên CRM. Bằng chứng: Lịch sử tải lead lúc 8h30 và giờ gọi đầu tiên 9h15. |
| 3 | Cần đọc, tổng hợp | Khi kiểm tra chất lượng telesale hàng tuần, tôi muốn tổng hợp toàn bộ lý do khách từ chối mua thuốc và phản hồi về giá, để báo cáo lại cho bộ phận marketing điều chỉnh nội dung quảng cáo. | Đội ngũ Marketing, Quản lý vận hành, 8 Telesaler | Mất 3 tiếng mỗi chiều thứ Sáu nghe lại 40 cuộc gọi thất bại và đọc ghi chú rải rác. Bằng chứng: Báo cáo tổng kết tuần trễ hạn gửi ban giám đốc 2 lần trong tháng qua. |
| 4 | Lặp lại | Khi đến giờ check-in và check-out mỗi ngày, tôi muốn đối soát nhanh giữa dữ liệu máy chấm công và tin nhắn xin phép nghỉ/đi muộn, để báo cáo chấm công chính xác mà không phải tra cứu thủ công từng người. | Quản lý nhân sự/vận hành, 25 nhân viên | Mất 30 phút/ngày (15 phút sáng, 15 phút chiều) đối chiếu 25 nhân sự giữa vân tay và nhóm Zalo báo phép. Bằng chứng: Bảng công Excel có 12 trường hợp phải sửa tay mỗi tháng. |
| 5 | Pain từ người khác | Khi khách hàng nhận thuốc và phản ánh qua hotline/tin nhắn về việc nhân viên tư vấn sai công dụng hoặc thiếu quà tặng kèm, tôi muốn truy vết ngay lịch sử tư vấn và mã đơn trên Pancake, để xử lý khiếu nại dưới 10 phút. | Nhân viên CSKH, Khách hàng khiếu nại, Quản lý | Mỗi tuần có 3–5 ca khiếu nại, mỗi ca mất 25–40 phút lội lại lịch sử chat Pancake vì saler quên gắn tag phân loại bệnh. Bằng chứng: Ticket khiếu nại trên Zalo CSKH. |
| 6 | Cần đọc, tổng hợp | Khi soạn thảo bài viết chuyên môn và kịch bản 1 video ngắn mỗi tuần, tôi muốn tổng hợp nhanh các nghiên cứu dược lý và quy định quảng cáo thuốc của Bộ Y Tế, để nội dung vừa chuẩn y khoa vừa thu hút người xem. | Nhân viên nội dung/Marketing, Dược sĩ chuyên môn | Mất 4–5 tiếng/bài viết để tra cứu tài liệu dược thư và rà soát từ ngữ nhạy cảm tránh vi phạm chính sách. Bằng chứng: Bài viết từng bị kiểm duyệt nội bộ trả lại 3 lần vì dùng sai thuật ngữ chỉ định. |
| 7 | Lặp lại | Khi có đơn hàng xuất bán mỗi buổi chiều, tôi muốn đối soát số lượng thực xuất từ kho với phiếu xuất kho trên phần mềm, để phát hiện ngay chênh lệch tồn kho thực tế và số lô thuốc. | Thủ kho, Kế toán kho | Mất 45 phút mỗi cuối ngày kiểm đếm 60–80 kiện hàng và gõ lại số lô thuốc vào phần mềm bán hàng. Bằng chứng: Biên bản lệch kho 2 lần/tháng do nhân viên xuất nhầm lô thuốc cận date. |
| 8 | Pain từ người khác | Khi telesale gọi điện cho danh sách khách hàng mới, tôi muốn lọc trước các số điện thoại rác hoặc thuê bao không có thực trước khi bấm gọi, để telesale không lãng phí thời gian chờ máy vô ích. | 8 Telesaler, Quản lý vận hành | Mỗi telesale bấm 60–80 cuộc/ngày thì có 20–25 cuộc là số ảo hoặc thuê bao, tốn 40 phút/người/ngày. Bằng chứng: Thống kê tỷ lệ cước cuộc gọi dưới 5 giây trên tổng đài đạt 32%. |
| 9 | Tốn thời gian | Khi kiểm kê kho hàng định kỳ ngày 25 hàng tháng, tôi muốn lọc ra toàn bộ sản phẩm còn hạn dùng dưới 6 tháng trên kệ kho, để lên kế hoạch xả hàng hoặc đổi trả nhà cung cấp kịp thời. | Quản lý kho, Bộ phận kinh doanh | Mất 6 tiếng đối chiếu danh mục 85 mã thuốc giữa thực tế trên kệ và file Excel date; tháng trước phát hiện trễ 1 lô trị giá 18 triệu đồng hết hạn phải hủy. Bằng chứng: Biên bản hủy dược phẩm quá hạn ngày 15 tháng trước. |
| 10 | Lặp lại | Khi saler kết thúc một phiên tư vấn thành công trên Pancake, tôi muốn kiểm tra xem nhân viên đã gắn đủ thẻ (tags) hành trình khách hàng hay chưa, để dữ liệu remarketing không bị sót. | Trưởng nhóm Sales, Bộ phận Marketing | Mỗi ngày có 15–20% cuộc hội thoại bị bỏ quên không gắn tag, khiến marketing chạy lại quảng cáo vào chính khách đã mua. Bằng chứng: 12 phản hồi từ khách hàng cũ phàn nàn vì liên tục bị gọi lại tư vấn lại từ đầu. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý AI gợi ý mà tôi giữ lại:** Gợi ý về việc *"Lọc số điện thoại ảo và phát hiện tỷ lệ cước dưới 5 giây"* (Problem #8) vì đây là pain point thực tế của đội telesale mà tôi chưa định lượng thành phút cụ thể trước đó.
- **Ý AI gợi ý mà tôi bỏ và vì sao:** AI gợi ý *"Tự động hóa hoàn toàn việc kê đơn thuốc cho bệnh nhân"*. Tôi loại bỏ ngay vì trong ngành dược, việc kê đơn thuốc bắt buộc phải có Dược sĩ/Bác sĩ chịu trách nhiệm pháp lý, rủi ro Viability & Feasibility quá cao và không khả thi cho một bài lab định lượng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Kiểm tra chất lượng tư vấn (QA) của nhân viên sales dược (Problem #1) | Tác động trực tiếp đến an toàn dùng thuốc của khách và doanh thu; quy trình audit hiện tại rất rõ ràng nhưng nghẽn nặng ở khâu đọc/nghe thủ công; impact đo lường được ngay. | Chưa chắc về khả năng nhận diện ngữ cảnh tiếng Việt chuyên ngành y dược khi có tiếng lóng hoặc lỗi chính tả của khách. |
| 2 | Rà soát trùng lặp và phân bổ lead khách hàng cho Telesale (Problem #2) | Bottleneck đo được chính xác theo phút (chậm trễ thời gian vàng liên hệ lead); quy trình có dữ liệu input/output chuẩn hóa rõ ràng. | Chưa chắc liệu giải pháp Rule đơn giản trên Google Sheets/AppSheet đã đủ xử lý chưa, hay cần đến quy trình nâng cao. |
| 3 | Cảnh báo và kiểm soát thuốc cận hạn dùng (date) trong kho (Problem #9) | Rủi ro tài chính trực tiếp (hủy thuốc mất tiền); quy trình nhập/xuất kho hiện tại có sẵn số lô và date trên hóa đơn. | Phụ thuộc nhiều vào tính kỷ luật của thủ kho khi nhập liệu ban đầu (nếu nhập sai thì hệ thống kiểm soát cũng sai). |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi kiểm tra chất lượng tư vấn của 10 saler mỗi ngày, tôi muốn nhanh chóng phát hiện các lỗi sai về tư vấn liều lượng và chống chỉ định thuốc, để kịp thời chấn chỉnh trước khi đơn hàng xuất kho. |
| Actor | Trưởng nhóm QA / Quản trị vận hành bán hàng |
| Thời điểm / bối cảnh | Diễn ra trực tiếp trong ca làm việc của 10 saler (chia thành các khung giờ cao điểm sáng và chiều). Saler liên tục tiếp nhận và chat tư vấn cho khách từ nhiều Fanpage Facebook thông qua phần mềm chat đa kênh bên thứ ba (như Pancake / POS). |
| Quy trình hiện tại (3–7 bước) | 1. Mở giao diện Pancake, chọn từng Fanpage và lọc danh sách hội thoại đang phát sinh của 10 saler trong ca (10 phút).<br>2. Chọn ngẫu nhiên các hội thoại có phát sinh báo giá hoặc chuẩn bị chốt đơn (5 phút).<br>3. Đọc từng luồng tin nhắn (thread) trên Pancake, đối chiếu checklist dược (hỏi bệnh nền, liều lượng, chống chỉ định, dặn dò tương tác thuốc) (90 phút - chia làm 3 lần/ca - Bottleneck).<br>4. Khi phát hiện saler tư vấn sai hoặc thiếu thông tin y khoa, QA nhắn tin riêng qua Zalo nội bộ yêu cầu saler nhắn tin đính chính lại với khách trước khi bấm tạo đơn (15 phút).<br>5. Ghi mã hội thoại Pancake và lỗi vi phạm vào file Excel theo dõi KPI chất lượng của saler (10 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Đọc lướt và đối chiếu checklist thủ công trên giao diện Pancake, mất **90 phút/ngày** trong ca trực. Do tin nhắn từ khách đổ về liên tục trên nhiều Fanpage, QA bị ngợp và chỉ rà soát được khoảng 20–25 hội thoại/ngày (chỉ chiếm ~8% trong tổng số gần 300 hội thoại/ngày của 10 saler). |
| Impact (nếu không giải thì sao) | Trong lúc QA đang đọc 1 hội thoại thì hàng chục hội thoại khác đã chốt đơn xong và được đẩy tự động sang bộ phận kho/in bill vận chuyển. Saler tư vấn sai liều hoặc bỏ qua chống chỉ định (ví dụ: bán thuốc dạ dày/khớp cho người có tiền sử suy thận, phụ nữ có thai) không được phát hiện kịp thời; đơn hàng bị gửi đi dẫn đến nguy cơ khách dùng sai thuốc gây biến chứng, khiếu nại, trả hàng và phạt vi phạm pháp lý ngành dược. |
| Success metric (baseline → target) | • **Baseline:** Kiểm tra ngẫu nhiên được ~20 hội thoại/ngày (~8%), mất 90 phút/ca của QA; độ trễ phát hiện lỗi từ 30–60 phút (nhiều ca in đơn xong mới phát hiện).<br>• **Target:** 100% hội thoại có chốt đơn được quét kiểm tra ngay trong ca; thời gian cảnh báo lỗi dưới 3 phút (trước khi saler bấm tạo đơn trên Pancake); QA chỉ mất 20 phút/ca để xử lý các ca bị gắn cờ đỏ.<br>• **Cách đo:** Tỷ lệ % hội thoại chốt đơn được quét rà soát trước khi tạo mã vận đơn; thời gian trung bình từ khi saler nhắn sai đến khi nhận cảnh báo sửa đổi. |
| Phương án không dùng AI | 1. Tận dụng tính năng Rule/Phím tắt của Pancake: Bắt buộc saler sử dụng bộ tin nhắn mẫu (Quick Reply) đã được dược sĩ soạn sẵn, nghiêm cấm gõ tay tự do.<br>2. Cài đặt Rule tự động: Nếu saler chưa gắn tag "Đã hỏi bệnh nền" mà đã gắn tag "Đã chốt đơn" thì phần mềm chặn không cho tạo đơn hàng sang bên vận chuyển. |
| Giả thuyết về AI (nếu có) | Sử dụng Webhook kết nối từ Pancake/Facebook Graph API đẩy tin nhắn về mô hình LLM. Mô hình đóng vai trò trợ lý QA rà soát theo thời gian thực (real-time): đọc hội thoại, so khớp với bảng chỉ định/chống chỉ định của từng loại thuốc. Nếu phát hiện saler bỏ sót câu hỏi bệnh nền hoặc tư vấn sai liều, hệ thống tự động bắn cảnh báo vào nhóm Zalo/Telegram nội bộ của ca trực để QA can thiệp ngay lập tức. |
| Cảm nhận nhanh | **Workflow** (Hệ thống chạy luồng định sẵn: Bắt tin nhắn Pancake → AI đối soát checklist dược → Cảnh báo ca rủi ro → Con người kiểm tra và xử lý). |

Quy trình nháp hiện tại:

```text
[Mở giao diện Pancake / POS của các Fanpage] (10')
  ──> [Lọc lấy ngẫu nhiên 20-25 hội thoại đang chat trong ca] (5')
  ──> [*NGHẼN* Đọc từng đoạn chat trên Pancake + Soi checklist y dược + Kiểm tra gắn tag] (90' rải rác trong ca)
  ──> [Nhắn tin Zalo nội bộ giục Saler sửa tin nhắn trước khi tạo đơn] (15')
  ──> [Ghi nhận mã hội thoại và lỗi vi phạm vào file Excel KPI] (10')

Tổng thời gian QA: 130 phút/ca làm việc
Tỷ lệ bao phủ kiểm tra: Chỉ đạt ~8% tổng số hội thoại trong ngày
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi lead khách hàng mới đổ về từ quảng cáo, tôi muốn lọc trùng số điện thoại và phân bổ ngay cho đúng telesale chuyên trách bệnh lý đó, để khách được liên hệ trong vòng 15 phút đầu. |
| Actor | Điều phối viên Telesales |
| Thời điểm / bối cảnh | Đầu mỗi ca sáng (8h30) và đầu ca chiều (13h30), khi các chiến dịch quảng cáo Facebook/Google đổ data về form đăng ký và tin nhắn. |
| Quy trình hiện tại (3–7 bước) | 1. Tải danh sách lead từ Ads Manager về file Excel (10 phút).<br>2. **Tra cứu đối soát SĐT với danh mục khách hàng cũ trên CRM để lọc trùng (30 phút - Bottleneck)**.<br>3. Chia danh sách theo khu vực và bệnh lý (15 phút).<br>4. Gửi SĐT vào nhóm Zalo riêng của từng telesale (10 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2: Rà soát thủ công số điện thoại cũ và lịch sử mua thuốc trong vòng 30 ngày trên CRM/Excel, mất **30 phút/lần** (60 phút/ngày). |
| Impact (nếu không giải thì sao) | Tốc độ liên hệ khách hàng bị chậm trễ hơn 45–60 phút; tỷ lệ bắt máy giảm từ 75% xuống 52% vì khách đã rời khỏi điện thoại hoặc mua từ nhà thuốc khác. |
| Success metric (baseline → target) | • **Baseline:** Thời gian từ lúc khách để lại SĐT đến khi telesale nhận được là 55 phút.<br>• **Target:** Giảm xuống dưới 5 phút.<br>• **Cách đo:** So sánh timestamp khách điền form và timestamp telesale bấm cuộc gọi đầu tiên trên tổng đài. |
| Phương án không dùng AI | Dùng Google Apps Script hoặc Webhook (Zapier/Make) kết nối Form về Google Sheet, dùng hàm `VLOOKUP`/`COUNTIF` để lọc trùng tự động và chia đều theo vòng tròn (Round Robin). |
| Giả thuyết về AI (nếu có) | Chưa cần thiết phải dùng AI; phương án Rule và Tự động hóa luồng dữ liệu (Workflow tự động không AI) đã giải quyết triệt để 90% bài toán. |
| Cảm nhận nhanh | **Rule** (Không cần dùng AI). |

Quy trình nháp hiện tại:

```text
[Tải file lead từ Ads] (10') 
  ──> [*NGHẼN* Tra cứu đối soát SĐT cũ trên CRM/Excel] (30') 
  ──> [Phân loại bệnh lý + chia ca trực] (15') 
  ──> [Gửi danh sách vào nhóm Zalo từng telesale] (10')

Tổng thời gian: 65 phút/ca
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi kiểm kê kho hàng định kỳ, tôi muốn nhanh chóng lọc ra toàn bộ các mặt hàng thuốc còn hạn dùng dưới 6 tháng trên toàn bộ kệ hàng, để lên kế hoạch kích cầu xả hàng hoặc đổi trả kịp thời. |
| Actor | Quản lý kho dược |
| Thời điểm / bối cảnh | Ngày 25 hàng tháng hoặc khi chuẩn bị nhập đợt hàng lớn từ nhà máy sản xuất. |
| Quy trình hiện tại (3–7 bước) | 1. In bảng danh mục 85 mã thuốc từ phần mềm (10 phút).<br>2. Cầm bảng giấy đi kiểm tra từng kệ, đọc số lô và date (120 phút).<br>3. **Gõ số liệu thực tế vào Excel và đối chiếu chênh lệch số lượng/date (90 phút - Bottleneck)**.<br>4. Lọc danh sách hàng date < 6 tháng (15 phút).<br>5. Lập biên bản đề xuất xử lý gửi Giám đốc (20 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Nhập liệu thủ công từ giấy vào máy và dò tìm xem lô thuốc nào bị lệch date giữa thực tế và phần mềm, mất **90 phút**. |
| Impact (nếu không giải thì sao) | Hàng cận date bị tồn đọng không phát hiện kịp; mỗi quý trung bình công ty phải tiêu hủy 15–20 triệu đồng tiền thuốc hết hạn sử dụng. |
| Success metric (baseline → target) | • **Baseline:** Tốn 255 phút/lần kiểm kê, độ trễ cảnh báo 30 ngày (chỉ phát hiện vào ngày 25 hàng tháng).<br>• **Target:** Thời gian đối chiếu giảm còn 30 phút; cảnh báo cận date tự động theo thời gian thực (real-time).<br>• **Cách đo:** Giá trị thuốc hủy do hết date giảm về 0 đồng/quý. |
| Phương án không dùng AI | Áp dụng chuẩn hóa quản lý kho FEFO (First Expired, First Out), dán mã QR/BarCode cho từng lô thuốc khi nhập hàng, cài đặt công thức điều kiện trên phần mềm tự tô đỏ các mã thuốc có date < 180 ngày. |
| Giả thuyết về AI (nếu có) | Chụp ảnh phiếu nhập kho/hóa đơn viết tay bằng mô hình OCR trích xuất tự động số lô, hạn dùng vào hệ thống. |
| Cảm nhận nhanh | **Rule** kết hợp mã vạch (Barcode/QR code). |

Quy trình nháp hiện tại:

```text
[In bảng tồn kho giấy] (10') 
  ──> [Đi rà từng kệ thuốc đọc số lô & date] (120') 
  ──> [*NGHẼN* Gõ tay vào Excel + Dò lệch hạn dùng với phần mềm] (90') 
  ──> [Lọc hàng date < 6 tháng] (15') 
  ──> [Làm báo cáo trình sếp] (20')

Tổng thời gian: 255 phút/kỳ kiểm kê
```

### Card muốn pitch nhất

- Card số: **Card #1** (Rà soát chất lượng tư vấn y dược của 10 saler trên phần mềm chat Pancake ngay trong ca làm việc)
- Vì sao:
  1. Đây là bài toán có **rủi ro lớn nhất** trong vận hành công ty dược: Sai sót về liều lượng hay bỏ qua chống chỉ định (bệnh nền tim mạch, huyết áp, phụ nữ mang thai) sẽ gây nguy hiểm trực tiếp đến sức khỏe khách hàng và vi phạm pháp lý y tế.
  2. **Bottleneck cực kỳ nặng và có thật**: QA bị ngợp vì tin nhắn đổ về liên tục trên Pancake từ nhiều Fanpage, mất tới 90 phút/ngày mà chỉ soi ngẫu nhiên được ~8% hội thoại, trong khi đơn hàng vẫn được chốt và in bill đẩy đi kho đều đặn mà không được kiểm soát hết.
  3. **Phù hợp nhất với đề bài Lab**: Ranh giới rất rõ để so sánh giữa Rule (từ khóa cấm/tin nhắn mẫu) và Workflow AI (hiểu ngữ cảnh tư vấn và sàng lọc bệnh nền), giúp nhóm dễ dàng đào sâu ở các checkpoint sau.
- Câu hỏi muốn nhóm phản biện:
  *"Khách hàng mua thuốc trên Facebook thường nhắn tin ngắt quãng, gõ tắt và dùng từ ngữ dân gian/tiếng lóng vùng miền (ví dụ: 'đau bao tử', 'nóng trong', 'dạo này người cấn cấn'). Liệu AI có thể hiểu đúng ngữ cảnh để bắt lỗi saler hay sẽ liên tục 'báo nhầm' (false alarm) làm loạn nhóm chat nội bộ của ca trực? Và giải pháp kỹ thuật kết nối vào Pancake/Facebook sẽ là gì để đảm bảo độ trễ dưới 3 phút?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI chỉ ra rằng việc rà soát theo thời gian thực (real-time) cho toàn bộ câu chat sẽ rất dễ làm phiền saler và gây quá tải hệ thống nếu AI liên tục cảnh báo sai. | Đồng ý | Tôi đã thu hẹp phạm vi can thiệp: Không bắt lỗi mọi câu chat vụn vặt, mà chỉ kích hoạt rà soát tại thời điểm mấu chốt: khi khách báo triệu chứng/tiền sử bệnh và khi saler gửi thông tin báo giá/chốt đơn. |
| AI chất vấn: "Tại sao không dùng tính năng tin nhắn mẫu (Quick Reply) và Rule bắt buộc có sẵn trên Pancake để giải quyết, cần gì AI?" | Đồng ý một phần | Tôi đã bổ sung phân tích vào phần phương án không dùng AI: Rule từ khóa trên Pancake không thể hiểu được ngữ cảnh khi khách hỏi kết hợp nhiều triệu chứng phức tạp hoặc gõ sai chính tả, nhưng tôi vẫn giữ Rule làm tầng lọc thô số 1 trước khi cần AI can thiệp. |
| AI cảnh báo: Success metric ban đầu ghi "giúp saler tư vấn tốt hơn" là định tính, không chấm điểm được theo rubric của lab. | Đồng ý | Tôi đã sửa lại Success Metric thành định lượng cụ thể: **Baseline: Soát 20 cuộc/ngày (8%), tốn 90 phút → Target: Quét 100% cuộc chốt đơn, độ trễ cảnh báo dưới 3 phút, QA chỉ mất 20 phút/ngày** kèm cách đo rõ ràng. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
