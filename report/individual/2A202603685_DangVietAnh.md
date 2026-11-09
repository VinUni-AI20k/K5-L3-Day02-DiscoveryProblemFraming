# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đặng Việt Anh
- MSSV: 2A202603685
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: C204T1
- Link repo nhóm: https://github.com/nashtran001/K5-L3A-DAY02-C204T1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Bối cảnh: Thanh Tùng là CEO của công ty xuất khẩu máy móc khoảng 5 người. Ở công ty, mọi người dùng google sheet, zalo business để làm việc. Vào mỗi đầu tuần, Tùng cần bảng tổng hợp báo cáo của các thành viên, nhưng dữ liệu nằm rải rác ở trên google sheets và các nhóm chat khác nhau ở Zalo. Hiện Tùng khó để theo dõi được tiến độ của đơn hàng, các báo cáo của thành viên, các khoản tiền vào ra của kế toán và kèm các gợi ý về hàng hoá, đối thủ để lên kế hoạch tuần mới.

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | **Khi** sáng thứ Hai bắt đầu tuần mới, **tôi muốn** có sẵn một báo cáo kinh doanh tuần trước (doanh thu, số đơn, khách mới, đơn đang treo) gom từ các sheet, **để** khỏi copy-paste thủ công và họp đầu tuần đúng giờ. | Tùng và nhân viên | lặp lại 1 lần 1 tuần, tốn 1h mỗi cuối tuần để làm báo cáo |
| 2 | Tốn thời gian | **Khi** lên kế hoạch tuần tới, **tôi muốn** thấy lịch hàng về, các khoản phải thu/phải trả đến hạn **để** chuẩn bị tiền đúng lúc để lấy hàng hoặc xuất hàng ra khỏi kho | Tùng và kế toán | 1 giờ mỗi lần, check lại zalo, CMS, DMS để biết lịch hàng và chuẩn bị khoản chi |
| 3 | Tổng hợp nhiều thông tin | **Khi** đọc lại các nhóm Zalo sau một tuần (khách, NCC, nội bộ), **tôi muốn** có bản tóm tắt các quyết định, cam kết và việc còn treo, **để** không bỏ sót việc quan trọng bị chìm trong hàng trăm tin nhắn. | Tùng và nhân viên phụ trách | Mất 2 giờ 1 ngày để đọc lại hàng trăm tin nhắn trên Zalo, có việc bị quên, miss tin nhắn |
| 4 | Pain từ người khác | **Khi** kế toán và sales phải chuẩn bị số liệu cho buổi họp thứ Hai, **tôi muốn** họ không phải nhập lại cùng một dữ liệu vào nhiều sheet, **để** họ dành thời gian cho khách hàng và giảm sai sót. | Tùng, kế toán; 2–3 nhân viên sales; gián tiếp là Tùng | 30-60 phút mỗi người; cùng một đơn hàng được nhập ở 2–3 nơi; Tùng thường phải hỏi lại khi số giữa các sheet không khớp |
| 5 | Lặp lại | **Khi** nhân viên gửi đề nghị chi (cước tàu, phí hải quan, tạm ứng) qua Zalo, **tôi muốn** thấy tất cả khoản chờ duyệt trong một danh sách kèm chứng từ và số dư tài khoản hiện tại, **để** duyệt một lượt mà không phải lục lại tin nhắn. | Tùng; kế toán; nhân viên xin duyệt chi | Khoảng 10–20 đề nghị/tuần, rải rác trong 3–5 nhóm Zalo; có những khoản bị trễ 1–2 ngày vì tin nhắn bị trôi; kế toán phải nhắc lại nhiều lần |
| 6 | Tốn thời gian | **Khi** đối soát tiền vào – tiền ra cuối tuần, **tôi muốn** sổ thu chi tự khớp với sao kê ngân hàng và công nợ khách/nhà cung cấp, **để** biết chính xác dòng tiền mà không phải dò từng dòng. | Tùng; kế toán | Kế toán mất khoảng 3–4 giờ/tuần để đối soát; Tùng mất thêm khoảng 1 giờ kiểm tra lại; thường lệch vài khoản vì nhập tay hoặc thiếu nội dung chuyển khoản |
| 7 | Pain từ người khác | **Khi** khách hàng hoặc nhà cung cấp hỏi về công nợ, thanh toán hay tiến độ giao hàng, **tôi muốn** nhân viên tự trả lời được từ một nguồn dữ liệu chung, **để** khách không phải chờ và mọi câu hỏi không dồn về CEO. | Khách hàng; NCC; nhân viên; Tùng (điểm nghẽn) | Nhiều câu hỏi/tuần chuyển lên Tùng vì chỉ CEO nắm đủ thông tin; khách phải chờ vài giờ đến 1 ngày; có khách phàn nàn phản hồi chậm qua Zalo |
| 8 | Lặp lại | **Khi** khách hỏi "hàng của tôi đến đâu rồi?", **tôi muốn** tra ngay trạng thái lô hàng (ETD/ETA, thông quan, giao kho), **để** trả lời khách trong vài phút thay vì phải hỏi lại forwarder. | Tùng; sales; khách hàng; forwarder | Khoảng 5–10 câu hỏi/tuần; mỗi câu mất 15–30 phút đi hỏi qua lại; trạng thái do forwarder cập nhật qua Zalo/email chứ không cập nhật vào sheet |
| 9 | Tốn thời gian | **Khi** báo giá cho khách một mẫu máy, **tôi muốn** có sẵn giá vốn mới nhất (giá NCC, tỷ giá, cước, thuế), **để** báo giá nhanh mà vẫn giữ được biên lợi nhuận. | Tùng; sales; khách hàng | Mỗi báo giá mất khoảng 30–60 phút tính lại; khoảng 5–8 báo giá/tuần; tỷ giá và cước thay đổi hàng tuần; đã có trường hợp báo thấp vì dùng giá cũ |
| 10 | Tổng hợp nhiều thông tin | **Khi** cân nhắc nhập mẫu máy mới hoặc tăng số lượng nhập, **tôi muốn** có gợi ý dựa trên lịch sử bán, tồn kho, xu hướng hỏi hàng và giá của đối thủ, **để** ra quyết định nhập hàng có căn cứ thay vì dựa vào cảm tính. | Tùng; sales; dòng tiền của công ty (vốn bị đọng vào hàng tồn) | Quyết định nhập hàng 1–2 lần/tháng, mỗi lô hàng chục đến hàng trăm triệu; thông tin đối thủ thu thập thủ công trên web/Facebook/Zalo; có hàng tồn kho chậm bán |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao. 
Trả lời:
Với AI gợi ý, tôi mong muốn giữ lại những gợi ý trên nhưng trừ gợi ý sau:
gợi ý #10 vì thường báo giá và xu hướng khó có thể biết được khi dung AI gợi ý vì đó là tin nội bộ của khách, thường phải gọi cho khách hàng.
Gợi ý #6 vì luồng tiền vào ra, hoặc ngân hàng là bảo mật, chỉ có kế toán biết, cần người thật kiểm chứng.
Gợi ý #7 vì mỗi nhân viên sale không nên biết về công nợ, mà cái này trực tiếp CEO/kế toán sẽ làm việc với khách hàng, chấp nhận điểm nghẽn.
-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tóm tắt các nhóm Zalo để không sót quyết định, các tin nhắn bị miss và việc còn confirm | Tốn thời gian, phải đọc lại thông tin, dễ bỏ sot thông tin, dữ liệu rời rạc dễ bị trùng lặp, có quá nhiều nhóm | AI có quyền vào Zalo không ? Liệu có bị miss các thông tin quan trọng, AI có hiểu nhầm các ý của thành viên, các tin nhắn sensitive có bị lộ không ? |
| 2 | Xem lịch hàng về và các khoản phải thu/phải trả đến hạn để chuẩn bị tiền | Ảnh hưởng đến thời gian giao hàng cho khách, tiến độ thu chi, hải quan | AI có vào được dữ liệu DMS, CMS của hải quan không ? Hay phải tự nhập bằng tay, hay cần forwarder |
| 3 | Báo cáo kinh doanh tuần tự gom từ các sheet | Lặp lại hàng tuần, hàng ngày, dễ triển khai | Các báo cáo có cần thiết phải sử dụng AI hay không hay là chỉ cần tạo rule để nhân viên cập nhật, liệu báo cáo hàng tuần chỉ mất có 1 giờ thì cần AI hay không ? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | **Khi** đọc lại các nhóm Zalo sau một tuần (khách, NCC, nội bộ), **tôi muốn** có bản tóm tắt các quyết định, cam kết và việc còn treo, **để** không bỏ sót việc quan trọng bị chìm trong hàng trăm tin nhắn. |
| Actor | Thanh Tùng (CEO); nhân viên phụ trách từng nhóm chat |
| Thời điểm / bối cảnh | Hằng ngày (cuối ngày hoặc sáng hôm sau) và đặc biệt đầu tuần; khoảng 10+ nhóm Zalo với khách, nhà cung cấp, forwarder và nội bộ; hàng trăm tin nhắn/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Mở lần lượt từng nhóm Zalo · 2. Kéo ngược lên tin nhắn chưa đọc · 3. Đọc lướt, tìm quyết định, giá, ngày hẹn, yêu cầu · 4. Ghi chú tay hoặc nhớ trong đầu · 5. Nhắn hỏi lại nhân viên nếu chưa rõ · 6. Giao việc / trả lời |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3: đọc lướt và lọc thông tin quan trọng, khoảng 120 phút/ngày |
| Impact (nếu không giải thì sao) | Quên cam kết với khách/NCC (giao hàng, thanh toán, báo giá); phản hồi chậm làm mất uy tín hoặc mất đơn; CEO mất khoảng 10 giờ/tuần chỉ để đọc tin nhắn |
| Success metric (baseline → target) | Thời gian đọc: 120 phút/ngày → ≤ 20 phút/ngày · Số việc bị quên/miss: chưa đo (cần đếm 2 tuần làm baseline) → giảm ≥ 80% |
| Phương án không dùng AI | Quy ước nội bộ: nhân viên phụ trách mỗi nhóm cuối ngày gửi 3–5 dòng tóm tắt theo mẫu (Quyết định / Cam kết / Việc treo); dùng tính năng ghim tin nhắn và nhắc hẹn của Zalo; to-do list chung trên Google Sheets |
| Giả thuyết về AI (nếu có) | LLM đọc tin nhắn của từng nhóm trong ngày/tuần và trích xuất có cấu trúc: quyết định, cam kết (ai, việc gì, hạn), câu hỏi chưa ai trả lời; gửi bản tóm tắt cho Tùng qua Zalo mỗi sáng. Giả thuyết: giảm ≥ 80% thời gian đọc mà không sót việc quan trọng |
| Cảm nhận nhanh | **Workflow** (lấy tin nhắn theo lịch → LLM tóm tắt → gửi bản tóm tắt). Chưa cần Agent |

Quy trình nháp hiện tại:

```text
[Tin nhắn mới ở 10+ nhóm Zalo]
        │
        ▼
Tùng mở từng nhóm ──► Kéo lên tin chưa đọc ──► Đọc lướt, lọc ý chính  ◄── BOTTLENECK (~120 phút/ngày)
                                                     │
                                                     ▼
                                        Ghi chú tay / nhớ trong đầu
                                                     │
                                  ┌──────────────────┴──────────────────┐
                                  ▼                                     ▼
                       Hỏi lại nhân viên nếu chưa rõ           Giao việc / trả lời
                                                                        │
                                                                        ▼
                                                        (Việc không ghi lại → dễ bị quên)
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | **Khi** lên kế hoạch tuần tới, **tôi muốn** thấy lịch hàng về và các khoản phải thu/phải trả đến hạn, **để** chuẩn bị tiền đúng lúc để lấy hàng hoặc xuất hàng ra khỏi kho. |
| Actor | Thanh Tùng (CEO); kế toán |
| Thời điểm / bối cảnh | Mỗi tuần, thường cuối tuần hoặc sáng thứ Hai khi lên kế hoạch; thông tin nằm ở Zalo (forwarder, NCC), CMS và DMS |
| Quy trình hiện tại (3–7 bước) | 1. Mở Zalo xem forwarder/NCC báo lịch tàu, ETA · 2. Mở CMS/DMS xem đơn hàng, tồn kho, lệnh xuất · 3. Mở sheet công nợ xem các khoản phải thu/phải trả · 4. Ghép thủ công thành lịch tuần (hàng nào về, cần bao nhiêu tiền, khi nào) · 5. Trao đổi với kế toán để chuẩn bị tiền / nhắc khách thanh toán |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 1–4: tra và ghép dữ liệu từ 3 nguồn, khoảng 60 phút/lần |
| Impact (nếu không giải thì sao) | Thiếu tiền đúng lúc phải nộp thuế, cước, phí lấy hàng → hàng nằm cảng phát sinh phí lưu kho/lưu container; trễ xuất kho cho khách; bị động về dòng tiền |
| Success metric (baseline → target) | Thời gian lên kế hoạch: 60 phút/tuần → ≤ 15 phút/tuần · Số lần thiếu tiền hoặc trễ lấy hàng: cần đo baseline → 0 lần/tháng |
| Phương án không dùng AI | Một Google Sheet "Lịch dòng tiền tuần" chung: mỗi lô hàng một dòng (ETA, ngày cần tiền, số tiền, trạng thái); kế toán và người phụ trách hàng cập nhật; dùng công thức/conditional formatting để tô màu các khoản đến hạn trong 7 ngày |
| Giả thuyết về AI (nếu có) | AI chỉ cần ở bước đọc tin nhắn forwarder/NCC trên Zalo để trích ETA và chi phí vào sheet; phần ghép lịch và cảnh báo đến hạn làm bằng rule là đủ |
| Cảm nhận nhanh | **Rule** (sheet + công thức + nhắc hạn); thêm **Workflow** có LLM nếu cần đọc ETA từ tin nhắn Zalo |

Quy trình nháp hiện tại:

```text
   Zalo (forwarder, NCC)        CMS / DMS               Sheet công nợ
   → lịch tàu, ETA        → đơn hàng, tồn, lệnh xuất   → phải thu / phải trả
            │                       │                          │
            └───────────────┬───────┴──────────────────────────┘
                            ▼
              Tùng ghép thủ công thành lịch tuần   ◄── BOTTLENECK (~60 phút/tuần)
                            │
                            ▼
              Trao đổi với kế toán: chuẩn bị tiền, nhắc khách thanh toán
                            │
                            ▼
              Lấy hàng ở cảng / xuất hàng ra khỏi kho
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | **Khi** sáng thứ Hai bắt đầu tuần mới, **tôi muốn** có sẵn một báo cáo kinh doanh tuần trước (doanh thu, số đơn, khách mới, đơn đang treo) gom từ các sheet, **để** khỏi copy-paste thủ công và họp đầu tuần đúng giờ. |
| Actor | Tùng; nhân viên |
| Thời điểm / bối cảnh | 1 lần/tuần, cuối tuần hoặc sáng thứ Hai trước buổi họp; dữ liệu nằm ở nhiều Google Sheets |
| Quy trình hiện tại (3–7 bước) | 1. Nhắc nhân viên cập nhật sheet · 2. Mở từng sheet (bán hàng, kế toán, đơn hàng) · 3. Lọc dữ liệu tuần trước · 4. Copy-paste sang file báo cáo · 5. Tính tổng, so sánh với tuần trước · 6. Gửi báo cáo / trình bày trong buổi họp |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–5: lọc, copy-paste và tính toán, khoảng 60 phút/tuần |
| Impact (nếu không giải thì sao) | Mất khoảng 1 giờ/tuần (~52 giờ/năm); số liệu có thể sai do copy tay; họp trễ hoặc họp với số liệu chưa cập nhật |
| Success metric (baseline → target) | Thời gian làm báo cáo: 60 phút/tuần → ≤ 5 phút/tuần · Sai lệch số liệu: cần đo baseline → 0 |
| Phương án không dùng AI | Gom dữ liệu bằng `IMPORTRANGE` + `QUERY` vào một sheet "Dashboard tuần"; dùng Looker Studio (miễn phí) để có báo cáo tự cập nhật; Apps Script gửi link báo cáo qua email/Zalo mỗi sáng thứ Hai |
| Giả thuyết về AI (nếu có) | Không cần AI cho phần tính số. AI chỉ có thể thêm 3–5 dòng nhận xét (tăng/giảm, đơn treo lâu) bên trên dashboard; giá trị tăng thêm thấp |
| Cảm nhận nhanh | **No AI / Rule** (công thức Sheets + Looker Studio) |

Quy trình nháp hiện tại:

```text
Nhắc nhân viên cập nhật sheet
        │
        ▼
Mở sheet bán hàng ─┐
Mở sheet kế toán ──┼──► Lọc dữ liệu tuần trước ──► Copy-paste vào file báo cáo ──► Tính tổng, so sánh
Mở sheet đơn hàng ─┘                 └──────────── BOTTLENECK (~60 phút/tuần) ────────────┘
                                                                                        │
                                                                                        ▼
                                                                       Trình bày trong họp sáng thứ Hai
```

### Card muốn pitch nhất

- **Card số:** #1 – Tóm tắt các nhóm Zalo
- **Vì sao:** Đây là vấn đề tốn thời gian nhất (khoảng 2 giờ/ngày, gấp nhiều lần hai card còn lại), có hậu quả rõ (quên cam kết, bỏ sót tin nhắn), và dữ liệu là văn bản tự do nên rule hay công thức không giải được. Card #2 và #3 phần lớn giải được bằng Google Sheets + rule mà không cần AI.
- **Câu hỏi muốn nhóm phản biện:**
  1. Có lấy được tin nhắn nhóm Zalo một cách hợp lệ không, hay phải đổi kênh làm việc? NCC có đồng ý trên kênh đó không ?
  2. Phương án không dùng AI (nhân viên tự tóm tắt cuối ngày theo mẫu) có đủ tốt không? Nếu đủ thì AI còn đáng làm không?
  3. Làm sao biết được sử dụng AI đáng tin ? AI có miss thông tin nào không ? AI có hiểu nhầm không ? có lọc được thông tin không ?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| #1 Zalo có thể không đọc được tin nhắn | Có | Chuyển sang nền tảng khác hoặc dựa vào API |
| #2 Không thể vào DMS, CMS hoặc các nền tảng khác | Có | Chuyển sang dùng forwarder, hoặc yêu cầu cung cấp API |
| #3 Báo cáo tuần, sử dụng các công cụ của gg sheet hoặc excel | Không | AI hoàn toàn có thể đọc được và tổng hợp báo cáo theo format |
---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Đưa ra cho nhóm card problem #1 | Nhóm đã phản biện, và cũng đồng ý 1 phần |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Tại sao phải dùng AI trong khi đã có phần mềm tương tự | Đồng ý |
| Nhận phản biện | Câu hỏi tôi nhận được: Input từ nhiều nguồn và Output thì rất nhiều, làm sao để cho đúng ? Khi nào thì tổng hợp báo cáo ? | Tôi đã sửa gì: Tôi mong muốn báo cáo đầu tuần, tự tạo task nếu tôi thấy miss, hoặc bảo AI note lại |
| Gom cluster / cây OST | | |
| Chọn candidate problem | Chọn cái của tôi và của Nhật | Nhóm đồng ý |
| Kiểm chứng / research | Tìm kiếm trên mạng để kiểm chứng | |
| Quy trình nhóm | Đề xuất quy trình nhóm, 1 người tổng hợp, 1 người research, 1 người báo cáo | nhóm đồng ý |
| Problem Statement | Đề xuất problem statement | Được nhóm chọn ra |
| Mức can thiệp AI | Đề xuất AI đọc toàn bộ tin nhắn | Nhóm không đồng ý |
| Quyết định | Đưa ra quyết định | Not go |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tôi dùng AI để tạo ra câu trả lời | AI hữu ích khi có nhiều câu trả lời khác nhau | AI sai ở chỗ là tạo đề nghị đọc trong zalo, nhưng chưa biết được zalo có thể đọc được hay không ? | Tôi sửa lại là giới hạn của các nền tảng |
| CP2 Problem Card | Tôi dùng AI để đưa ra câu trả lời cho 3 cái problem mà tôi chọn | AI trả lời rất hay và chi tiết | Giống như ở trên AI đã không biết rõ được là cần phải ai duyệt và thông tin có lấy được hay không ? | Sửa nội dung để fit với trường hợp của mình |
| CP4 Research | Để tìm ra xem những công cụ nào đã có và tương tự | AI crawl website để tìm | Chưa tìm hiểu rõ | Tôi chưa sửa gì |
| CP5 Quy trình | Tôi dùng AI để tìm hiểu quy trình | AI tóm tắt được quy trình rất nhanh | AI đưa ra quy trình rất đẹp nhưng có nhiều bước không cần thiết | Tôi cập nhật lại các bước thực tế gặp phải |
| CP5–6 Problem Statement | Dùng AI để biết được có trường hợp nào tương tự không ? | AI tìm rất nhanh | Có thể thông tin không đúng | Tôi dựa trên kinh nghiệm của mình để sửa lại |
| CP6 Mức can thiệp / quyết định | chưa dùng AI để quyết định | None | None | Quyết định not go |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi học được là có những bạn chưa có kinh nghiệm triển khai thực tế nên dẫn tới có những problem không đúng. Có bạn đưa ra vấn đề như là đưa ra hệ thống AI để theo dõi bugs, nhưng thực tế đã có công cụ lớn trên thế giới họ đang làm như là google firebase analytics hoặc sentry. Những công cụ đó thường rẻ, miễn phí với số lượng ít chưa cần AI can thiệp tới.
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Nhóm có bạn đã đưa ra solution-first vì bạn đưa luôn công cụ để check log lẫn là check bugs. Nhưng thực tế bạn ý chưa tìm hiểu rõ xem là trên thế giới hoặc các sản phẩm trên thị trường đã sử dụng công cụ đó chưa. Có ai đang cần dùng AI để làm vấn đề đó hay không.
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi không đổi ý, vì đây đều là những pain point cụ thể của tôi. Đó là khi tôi phải họp quá nhiều và tin nhắn đến quá nhiều khiến cho tôi bị miss, rất mất thời gian để đọc lại vấn đề.
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Tôi chưa thấy bất ngờ vì đều là những problem thật. Có những bạn đã gặp phải giống tôi, đặc biệt những người làm về PM, quản lý rất nhiều nhóm, quản lý ticket, phải tổng hợp lại thông tin từ các nguồn khác nhau để đưa ra quyết định.
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó nhất là xác định được problem có chuẩn xác không. Thường tôi dễ nhầm giữa triệu chứng và vấn đề gốc. Ví dụ như vấn đề của tôi đề ra là triệu chứng thôi, và tôi chỉ giải quyết triệu chứng chứ chưa đưa ra, hoặc tìm được vấn đề gốc của tôi.
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại tôi vẫn chọn vấn đề này, nhưng đưa ra cụ thể hơn vấn đề gốc, và những ví dụ cụ thể hơn để phản biện.
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
