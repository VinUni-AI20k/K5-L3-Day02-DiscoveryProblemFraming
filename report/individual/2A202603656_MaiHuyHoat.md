# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: MAI HUY HOAT 
- MSSV: 2A202603656
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Phượng Hoàng
- Link repo nhóm:

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.


| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi tiếp nhận xe có lỗi cảm biến/điện chập chờn, tôi muốn tra cứu chính xác sơ đồ mạch điện và quy trình đo kiểm ban đầu từ manual của hãng, để không phải tự mò mẫm tháo lắp gây rủi ro hỏng hóc. | Kỹ thuật viên chẩn đoán (Diagnostic Mechanic), Cố vấn dịch vụ | Mất 45–90 phút/ca lỗi chập chờn; diễn ra 3–5 ca/ngày/xưởng; thợ phải lật mở hàng chục file PDF manual dài 500-1500 trang. |
| 2 | Pain từ người khác | Khi chủ xe mang xe đến kiểm tra triệu chứng lạ ("xe bị hẫng khi tăng tốc lúc máy nóng"), tôi muốn Cố vấn dịch vụ ghi nhận đúng bản chất kỹ thuật, để tôi không phải tốn thời gian chạy thử lại xe nhiều lần để nghe lại tiếng kêu/hiện tượng. | Thợ máy/điện xưởng dịch vụ, Khách hàng | 30% lượt xe vào xưởng có mô tả triệu chứng chung chung từ khách; thợ mất 30–45 phút lái thử (test drive) để xác nhận lại lỗi. |
| 3 | Tốn thời gian | Khi lô linh kiện/phụ tùng ô tô mới về kho xưởng, tôi muốn nhanh chóng kiểm tra lỗi ngoại quan và đối chiếu mã SKU, để hoàn tất thủ tục nhập kho và cấp phát cho kỹ thuật viên kịp thời. | Nhân viên kho, Kỹ sư QC đầu vào (Incoming QC), Thợ sửa chữa | Mất 3–5 phút cho từng chi tiết/kiện linh kiện nhỏ; đỉnh điểm 200–300 phụ tùng/ngày; tỷ lệ nhầm mã SKU khoảng 2-4% khi cao điểm. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi Robot hàn/lắp ráp ô tô báo dừng dây chuyền (Downtime), tôi muốn nhanh chóng phân tích log lỗi PLC/Robot và lịch sử cảnh báo, để tìm ra nguyên nhân gốc rễ và khôi phục sản xuất ngay. | Kỹ sư bảo trì tự động hóa (Maintenance Engineer), Trưởng ca | Thời gian dừng dây chuyền (Downtime) trung bình 30–60 phút/sự cố; tần suất 2–4 lần/tuần; chi phí tổn thất hàng ngàn USD/giờ dừng line. |
| 5 | Lặp lại | Khi hoàn tất chẩn đoán tình trạng xe, tôi muốn tự động tổng hợp danh sách phụ tùng thay thế và giờ công tương ứng, để lập báo giá chính xác cho khách hàng mà không phải tra bảng giá manual thủ công. | Cố vấn dịch vụ (Service Advisor), Nhân viên vật tư | Thực hiện 15–20 lần/ngày đối với mỗi Cố vấn dịch vụ; mất 15–20 phút/báo giá phức tạp; dễ xảy ra sai lệch giá phụ tùng giữa kho và báo giá. |
| 6 | Pain từ người khác | Khi đưa xe đi bảo dưỡng định kỳ, tôi muốn biết chính xác thời gian hoàn tất và tiến độ sửa chữa theo thời gian thực, để chủ động công việc cá nhân mà không phải liên tục gọi điện hỏi xưởng. | Chủ xe (Khách hàng cá nhân), Nhân viên chăm sóc khách hàng (CS) | Nhân viên CS nhận 20–30 cuộc gọi/ngày chỉ để trả lời câu hỏi "xe xong chưa"; khách hàng phải chờ đợi thụ động tại phòng chờ xưởng. |
| 7 | Tốn thời gian | Khi chuẩn bị lập kế hoạch bảo trì định kỳ cho các tay máy Robot trên dây chuyền, tôi muốn tổng hợp số giờ vận hành và lịch sử nhiệt độ/độ rung của từng khớp Robot, để thay thế linh kiện trước khi xảy ra sự cố hỏng hóc lớn. | Kỹ sư quản lý thiết bị nhà máy (Asset Manager), Kỹ sư bảo trì | Mất 4–6 giờ/tuần để thu thập và nhập tay dữ liệu từ các tủ điều khiển Robot riêng lẻ vào file Excel theo dõi. |
| 8 | Lặp lại | Khi tiếp nhận danh sách các hạng mục cần thay thế sau chẩn đoán, tôi muốn kiểm tra tình trạng tồn kho thực tế của đúng mã linh kiện đó, để đặt hàng bổ sung từ nhà cung cấp nếu kho xưởng đang hết hàng. | Nhân viên quản lý kho phụ tùng, Bộ phận thu mua (Procurement) | Thực hiện 30–40 lần/ngày; mất 5–10 phút/lần tra cứu chéo giữa hệ thống WMS và kho thực tế; đôi khi phát hiện hết hàng đột xuất khiến xe phải nằm chờ phụ tùng thêm 1–2 ngày. |
**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)


### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tốn thời gian tra cứu tài liệu kỹ thuật & chẩn đoán ban đầu tại xưởng ô tô | Điểm nghẽn rõ ràng, xưởng nào cũng gặp, dễ phỏng vấn thực tế, tác động trực tiếp đến thời gian chờ của khách và năng suất thợ. | Dữ liệu manual của các hãng ô tô có đủ định dạng chuẩn (chữ + sơ đồ điện) để AI truy cập hay không. |
| 2 | Phân loại & kiểm tra lỗi ngoại quan phụ tùng ô tô nhập kho thủ công | Nhu cầu lớn trong quản lý kho vận, tỷ lệ nhầm SKU gây lãng phí nghiêm trọng. | Chi phí triển khai phần cứng/cảm biến kiểm tra ngoại quan có thể cao vượt mức chấp nhận của kho vừa/nhỏ. |
| 3 | Chẩn đoán & phân tích nguyên nhân sự cố dừng dây chuyền (Downtime) Robot hàn | Giá trị kinh tế lớn (giảm chi phí dừng chuyền hàng ngàn USD/giờ). | Khó tiếp cận dữ liệu log nội bộ của nhà máy sản xuất ô tô thực tế để kiểm chứng. |

---

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận xe có lỗi chập chờn/mã lỗi phức tạp, tôi muốn tra cứu nhanh sơ đồ mạch điện và hướng dẫn kiểm tra từ manual của hãng, để chẩn đoán chính xác nguyên nhân mà không mất hàng giờ lật tài liệu PDF. |
| Actor | Kỹ thuật viên chẩn đoán (Primary), Cố vấn dịch vụ (Secondary). |
| Thời điểm / bối cảnh | Tại khu vực tiếp nhận & chẩn đoán của xưởng dịch vụ ô tô khi xe vừa vào xưởng. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận xe & ghi nhận triệu chứng.<br>2. Cắm máy OBD-II quét mã lỗi.<br>3. Mở máy tính tra cứu manual PDF/sơ đồ điện thủ công.<br>4. Đo kiểm thực tế từng chân cảm biến/dây dẫn.<br>5. Lập báo cáo kết luận nguyên nhân & đề xuất thay thế. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (Tra cứu tài liệu PDF manual và tìm sơ đồ điện), mất 45–60 phút/ca lỗi phức tạp. |
| Impact (nếu không giải thì sao) | Năng suất cầu nâng giảm, xe nằm chờ lâu, khách hàng phàn nàn và giảm chỉ số CSI của xưởng. |
| Success metric (baseline → target) | Baseline: 60 phút tra cứu/ca → Target: < 15 phút tra cứu/ca (Giảm 75% thời gian tra cứu). |
| Phương án không dùng AI | Dùng từ khóa Search trong Acrobat Reader hoặc in sẵn các sơ đồ mạch điện phổ biến ra bảng giấy dán tại xưởng. |
| Giả thuyết về AI (nếu có) | Sử dụng RAG (Retrieval-Augmented Generation) để indexing toàn bộ manual kỹ thuật. Thợ chỉ cần nhập triệu chứng hoặc mã lỗi OBD-II, AI trả về đúng vị trí sơ đồ và các bước test khuyến nghị. |
| Cảm nhận nhanh | **Workflow** |

Quy trình nháp hiện tại:

```text
[Khách mang xe vào] 
      │
      ▼
[Cố vấn ghi nhận triệu chứng thô] 
      │
      ▼
[Thợ cắm máy đọc lỗi OBD-II] ──► (Có mã lỗi OBD / Triệu chứng chập chờn)
      │
      ▼
[BOTTLENECK: Thợ mở máy tính tra cứu PDF Manual & Sơ đồ điện thủ công] (45 - 60 phút)
      │
      ▼
[Thợ tiến hành đo kiểm thực tế trên xe]
      │
      ▼
[Lập danh sách phụ tùng cần thay & báo giá]
```

---

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi lô linh kiện/phụ tùng ô tô mới về kho xưởng, tôi muốn nhanh chóng kiểm tra lỗi ngoại quan và đối chiếu mã SKU, để nhập kho và cấp phát kịp thời cho kỹ thuật viên. |
| Actor | Nhân viên kho, Kỹ sư QC đầu vào (Incoming QC). |
| Thời điểm / bối cảnh | Khu vực nhận hàng của kho linh kiện phụ tùng ô tô khi nhận hàng từ nhà cung cấp. |
| Quy trình hiện tại (3–7 bước) | 1. Tháo dỡ kiện hàng linh kiện.<br>2. Soi ngoại quan từng chi tiết bằng mắt thường.<br>3. Khảo sát mã SKU trên nhãn và đối chiếu bản vẽ/ERP.<br>4. Nhập tay số lượng và tình trạng vào phần mềm WMS.<br>5. Đưa linh kiện vào vị trí kệ kho. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 & 3 (Soi lỗi ngoại quan và kiểm đối chiếu mã SKU thủ công), mất 3–5 phút/linh kiện. |
| Impact (nếu không giải thì sao) | Dễ bỏ sót lỗi nhỏ (nứt/rách ron), nhầm lẫn mã SKU dẫn đến giao nhầm phụ tùng cho thợ sửa chữa. |
| Success metric (baseline → target) | Baseline: Tỷ lệ nhầm SKU 3% → Target: < 0.5%; Thời gian kiểm tra: 4 phút/món → 1 phút/món. |
| Phương án không dùng AI | Dùng máy quét mã vạch Barcode/QR code chuẩn hóa trên từng bao bì linh kiện. |
| Giả thuyết về AI (nếu có) | Dùng Computer Vision (Visual Inspection) quét nhanh hình ảnh bề mặt linh kiện để phát hiện vết nứt/xước và tự nhận diện mã phụ tùng. |
| Cảm nhận nhanh | **Workflow** |

Quy trình nháp hiện tại:

```text
[Nhận kiện hàng phụ tùng] 
      │
      ▼
[Tháo dỡ bao bì] 
      │
      ▼
[BOTTLENECK: Soi lỗi ngoại quan & đối chiếu SKU thủ công bằng mắt] (3-5 phút/món)
      │
      ▼
[Nhập số lượng thủ công vào WMS] 
      │
      ▼
[Xếp phụ tùng lên kệ kho]
```

---

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi Robot hàn báo dừng dây chuyền, tôi muốn nhanh chóng phân tích log lỗi PLC/Robot, để tìm ra nguyên nhân gốc rễ và khôi phục dây chuyền ngay lập tức. |
| Actor | Kỹ sư bảo trì tự động hóa (Maintenance Engineer), Trưởng ca sản xuất. |
| Thời điểm / bối cảnh | Dây chuyền sản xuất/hàn thân vỏ ô tô tự động khi gặp sự cố dừng line ngoài kế hoạch. |
| Quy trình hiện tại (3–7 bước) | 1. Dây chuyền báo chuông/đèn đỏ dừng khẩn cấp.<br>2. Kỹ sư di chuyển đến tủ điều khiển cell Robot.<br>3. Kết nối máy tính, trích xuất log lỗi PLC/Robot.<br>4. Đọc log thô và đối chiếu mã lỗi hệ thống.<br>5. Xử lý phần cứng/chương trình và khởi động lại line. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 (Đọc và phân tích hàng trăm dòng log thô để khoanh vùng nguyên nhân gốc), mất 30–45 phút. |
| Impact (nếu không giải thì sao) | Dừng dây chuyền (Downtime) gây lãng phí năng suất, chi phí thiệt hại hàng ngàn USD mỗi giờ dừng line. |
| Success metric (baseline → target) | Baseline: MTTR (thời gian xử lý) 45 phút → Target: < 15 phút/sự cố. |
| Phương án không dùng AI | Viết sẵn các mã lỗi phổ biến kèm bảng tra cứu nguyên nhân-cách xử lý (Lookup table) dán trên tủ PLC. |
| Giả thuyết về AI (nếu có) | AI Agent đọc stream log thời gian thực của Robot/PLC, tự động gắn tag nguyên nhân root-cause và gợi ý các bước khắc phục cho kỹ sư. |
| Cảm nhận nhanh | **Agent** |

Quy trình nháp hiện tại:

```text
[Robot báo lỗi dừng cell hàn] 
      │
      ▼
[Kỹ sư di chuyển đến tủ điều khiển] 
      │
      ▼
[Export log thô từ PLC/Robot Controller] 
      │
      ▼
[BOTTLENECK: Đọc & phân tích chuỗi log thô để tìm root-cause] (30-45 phút)
      │
      ▼
[Thực hiện sửa chữa/reset dây chuyền]
```

---

### Card muốn pitch nhất

- **Card số:** Card #1 (Tốn thời gian tra cứu tài liệu kỹ thuật & chẩn đoán ban đầu tại xưởng ô tô)
- **Vì sao:** Đây là điểm nghẽn có tần suất diễn ra hàng ngày tại mọi xưởng dịch vụ ô tô, tính khả thi cao khi ứng dụng RAG AI để giải quyết đúng nỗi đau tra cứu document phức tạp, và dễ dàng phỏng vấn/kiểm chứng với các kỹ thuật viên.
- **Câu hỏi muốn nhóm phản biện:** 
  1. Bài toán này có bị trùng lặp với việc tra cứu mã lỗi OBD-II thông thường không?
  2. Mức độ can thiệp Workflow AI (AI làm trợ lý tra cứu RAG, thợ duyệt và chẩn đoán) đã tối ưu chưa hay cần nâng lên Agent?

---

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI có thể chẩn đoán sai lỗi kỹ thuật gây nguy hiểm khi vận hành xe nếu để AI tự quyết định (Agent). | Đồng ý | Đã chỉnh định vị AI từ Agent xuống **Workflow (AI RAG Trợ lý tra cứu)**. AI chỉ tổng hợp thông tin trích dẫn từ Manual hãng, thợ kỹ thuật là người quyết định chẩn đoán cuối cùng. |
| Mô tả điểm nghẽn ban đầu còn chung chung, chưa phân biệt rõ giữa lỗi phần cứng và lỗi tra cứu thông tin. | Đồng ý | Đã làm rõ điểm nghẽn nằm ở **thời gian tra cứu tài liệu PDF Manual/Sơ đồ điện (45-60 phút)** chứ không phải ở thao tác đo kiểm trên xe. |
| Dữ liệu Manual của các hãng ô tô có thể ở định dạng hình ảnh/PDF không chuẩn khiến RAG khó đọc. | Đồng ý | Thêm phần "Điều còn chưa chắc" vào bảng Top 3 để nhóm thảo luận giải pháp xử lý OCR/Data Prep cho file manual. |

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
