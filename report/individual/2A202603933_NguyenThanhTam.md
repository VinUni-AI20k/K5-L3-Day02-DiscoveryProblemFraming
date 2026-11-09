# Báo cáo cá nhân — 2A202603933_NguyenThanhTam

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Thành Tâm
- MSSV: 2A202603933
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhom5W
- Link repo nhóm: https://github.com/VinUni-AI20k/K5-L3-Day02-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

> ⚠️ Dữ liệu trong cột "Dấu hiệu thật" ở giai đoạn này là **ước lượng suy luận từ quan sát gián tiếp** (mô tả công việc, trao đổi không chính thức, bối cảnh chung). Chưa có phỏng vấn trực tiếp. Các con số được đánh dấu `[GT]` = Giả thuyết cần verify trước CP2.

**Actor tham chiếu:** Kỹ sư hiện trường / Chỉ huy công trường / Quản lý dự án xây dựng

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (nguồn & mức tin cậy) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi cuối mỗi ngày làm việc tại công trường, tôi muốn tổng hợp nhanh nhật ký thi công (khối lượng hoàn thành, nhân công, thiết bị, vật tư tiêu hao, sự cố) thành 1 báo cáo gửi về văn phòng, để chỉ huy trưởng và chủ đầu tư nắm tiến độ mà tôi không phải gõ lại dữ liệu từ sổ tay vào Excel mỗi tối. | Chỉ huy công trường, Kỹ sư hiện trường, Chỉ huy trưởng, Chủ đầu tư | **Quan sát thật:** Nhật ký công trường là yêu cầu pháp lý bắt buộc theo Nghị định 06/2021/NĐ-CP. **[GT]** ~45–60 phút/ngày gõ thủ công; mỗi dự án có 1–3 kỹ sư hiện trường chịu pain này đồng thời. **Rủi ro verify:** Hiện tại gõ thủ công hay đã có app? |
| 2 | Tốn thời gian | Khi cần quyết toán khối lượng với nhà thầu phụ vào cuối tháng, tôi muốn đối chiếu nhanh khối lượng nghiệm thu thực tế so với dự toán ban đầu và biên bản xác nhận hiện trường, để phê duyệt thanh toán đúng hạn mà không phải lật 3–4 file Excel và bản vẽ riêng lẻ. | Kỹ sư QS (định giá), Chỉ huy trưởng, Nhà thầu phụ, Kế toán dự án | **Quan sát thật:** Quyết toán theo tháng là chu kỳ cố định trong mọi dự án xây dựng. **[GT]** 2–3 ngày/tháng để đối chiếu thủ công; sai lệch khối lượng thường gây tranh chấp thanh toán. **Rủi ro verify:** Dữ liệu nghiệm thu có được lưu số không, hay vẫn là biên bản giấy ký tay? |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận được bộ hồ sơ thiết kế mới (bản vẽ thi công + thuyết minh kỹ thuật + danh mục vật liệu) từ tư vấn thiết kế, tôi muốn nhanh chóng xác định các điểm thay đổi so với phiên bản trước và những yêu cầu kỹ thuật đặc biệt cần lưu ý, để bàn giao đúng thông tin cho tổ trưởng thi công trước khi đổ bê tông. | Kỹ sư hiện trường, Tổ trưởng thi công, Giám sát tư vấn | **Quan sát thật:** Revision bản vẽ trong thi công là sự kiện thường xuyên, đặc biệt với dự án dân dụng phức tạp. **[GT]** Mỗi lần revision: 2–4 tiếng đọc và so sánh thủ công; nếu bỏ sót thay đổi → thi công sai → phá dỡ làm lại tốn kém. |
| 4 | Lặp lại | Khi cần đặt mua vật tư cho tuần thi công tiếp theo, tôi muốn tra nhanh tồn kho hiện tại tại công trường và đối chiếu với kế hoạch thi công, để lập phiếu yêu cầu mua hàng chính xác mà không thiếu hoặc thừa vật tư gây ứ đọng vốn. | Kỹ sư vật tư, Chỉ huy công trường, Phòng Mua hàng | **Quan sát thật:** Lập phiếu yêu cầu vật tư là công việc tuần/2 tuần. **[GT]** Tồn kho thường ghi sổ tay hoặc Excel riêng của từng thủ kho — không có hệ thống tập trung. **[GT]** Thiếu vật tư đột xuất khiến dừng thi công 0.5–1 ngày/sự cố. |
| 5 | Pain từ người khác | Khi giám sát của chủ đầu tư yêu cầu cung cấp hồ sơ nghiệm thu một hạng mục (biên bản kiểm tra vật liệu, biên bản nghiệm thu nội bộ, kết quả thí nghiệm, bản vẽ hoàn công), tôi muốn tập hợp và gửi đủ bộ hồ sơ trong ngày, để không làm chậm tiến độ nghiệm thu và thanh toán đợt. | Kỹ sư hiện trường, Kỹ sư hồ sơ, Chủ đầu tư / Giám sát | **Quan sát thật:** Hồ sơ nghiệm thu phân tán ở nhiều người, nhiều thời điểm — phổ biến trong ngành. **[GT]** Trung bình mất 0.5–1 ngày/hạng mục để gom hồ sơ; thiếu 1 biên bản → chủ đầu tư từ chối nghiệm thu → trễ thanh toán 15–30 ngày. |
| 6 | Tốn thời gian | Khi kỳ họp tiến độ định kỳ 2 tuần/lần với chủ đầu tư sắp diễn ra, tôi muốn so sánh nhanh tiến độ thực tế với đường cong S (kế hoạch) và xác định nguyên nhân lệch tiến độ, để trình bày được phương án xử lý thay vì chỉ báo cáo số liệu thiếu. | PM dự án, Chỉ huy trưởng, Chủ đầu tư | **Quan sát thật:** Họp tiến độ định kỳ là thông lệ tất cả dự án xây dựng. **[GT]** ~3–4 tiếng chuẩn bị slide + cập nhật đường cong S thủ công trên Excel. |
| 7 | Pain từ người khác | Khi xảy ra sự cố kỹ thuật tại công trường (nứt kết cấu, sập cốp pha, tai nạn lao động), tôi muốn lập nhanh báo cáo sự cố đúng mẫu quy định gửi chủ đầu tư và cơ quan quản lý nhà nước, để đáp ứng nghĩa vụ thông báo trong 24h theo quy định pháp luật mà không bỏ sót nội dung bắt buộc. | Chỉ huy trưởng, Ban ATLĐ, Chủ đầu tư, Sở Xây dựng | **Quan sát thật:** Nghị định 06/2021 yêu cầu báo cáo sự cố trong 24h — xác minh được từ văn bản pháp luật. **[GT]** Tần suất sự cố thực tế/dự án — cần số liệu từ người trong ngành. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Giữ lại ý #1 (Nhật ký thi công hằng ngày) và #5 (Gom hồ sơ nghiệm thu) vì impact rõ, actor cụ thể, có cơ sở pháp lý xác minh được. Giữ #3 (Đọc bản vẽ revision) vì hậu quả nặng nếu bỏ sót thay đổi kỹ thuật.
- **Ý loại bỏ:** AI từng gợi ý "Tự động hóa toàn bộ quy trình đấu thầu và lựa chọn nhà thầu". Loại bỏ vì phạm vi quá rộng, liên quan đến pháp lý đấu thầu phức tạp, không phù hợp với mục tiêu làm rõ quy trình trong một buổi lab 4 tiếng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | #1 — Nhật ký thi công hằng ngày | Lặp lại mỗi ngày → ROI cao nhất; actor cụ thể (kỹ sư hiện trường); bottleneck rõ (gõ lại sổ tay → Excel); yêu cầu pháp lý bắt buộc nên adoption không thể bỏ qua; dễ pilot trong 2 tuần | Kỹ sư hiện trường hiện ghi tay hay đã có app? Voice-to-text tiếng Việt kỹ thuật xây dựng có đủ chính xác không? |
| 2 | #5 — Gom hồ sơ nghiệm thu | Downstream impact rõ: thiếu 1 biên bản → trễ thanh toán 15–30 ngày; bottleneck là chờ hồ sơ từ nhiều người; checklist + folder Drive có thể giải một phần nhưng vẫn còn gap | Hồ sơ hiện đang lưu ở đâu (Drive, email, giấy)? Ai là người tổng hợp chính? |
| 3 | #3 — Đọc bản vẽ revision | Hậu quả nặng nếu bỏ sót (phá dỡ làm lại, chi phí cao); bài toán "so sánh 2 tài liệu" phù hợp với AI; không phụ thuộc vào hệ thống bên ngoài | Bản vẽ có ở dạng PDF có thể xử lý được không, hay là DWG/CAD? Revision cloud có được đánh dấu rõ trên bản vẽ không? |

---

### Problem Card #1 — Nhật ký thi công hằng ngày

| Trường | Nội dung |
|---|---|
| Job Story | Khi cuối mỗi ngày làm việc tại công trường, tôi muốn tổng hợp nhanh nhật ký thi công (khối lượng hoàn thành, nhân công, thiết bị, vật tư tiêu hao, sự cố) thành 1 báo cáo gửi về văn phòng, để chỉ huy trưởng và chủ đầu tư nắm tiến độ mà không phải gõ lại dữ liệu từ sổ tay vào Excel mỗi tối. |
| Actor | Kỹ sư hiện trường / Chỉ huy công trường (1–3 người/dự án) |
| Thời điểm / bối cảnh | Cuối mỗi ngày làm việc tại công trường (17:00–19:00), 5–6 ngày/tuần; thực hiện tại lán trại hoặc văn phòng công trường sau giờ thi công |
| Quy trình hiện tại (3–7 bước) | 1. Ghi chép sổ tay thực địa suốt ngày (nhân công từng tổ, thiết bị vận hành, khối lượng từng hạng mục, vật tư xuất kho, sự cố phát sinh) · 2. Về lán/văn phòng công trường, mở file Excel mẫu nhật ký · 3. Gõ lại từng mục từ sổ tay vào Excel (mất 30–40 phút) · 4. Chụp ảnh hiện trường để đính kèm · 5. Gửi file qua email hoặc Zalo về văn phòng chính |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 — gõ lại dữ liệu từ sổ tay vào Excel: **[GT]** ~30–40 phút/ngày; đây là công việc thuần nhập liệu, không tạo thêm giá trị, dễ xảy ra lỗi sót dòng hoặc sai số |
| Impact (nếu không giải thì sao) | **[GT]** ~45–60 phút/ngày/kỹ sư bị lãng phí; với 2 kỹ sư = 90–120 phút lãng phí/ngày/dự án; báo cáo hay bị trễ, thiếu chi tiết, hoặc bỏ sót sự cố nhỏ làm mất bằng chứng khi tranh chấp sau này; vi phạm Nghị định 06/2021 nếu nhật ký không đầy đủ |
| Success metric (baseline → target) | Baseline: **[GT]** 45–60 phút/ngày/kỹ sư (cần bấm giờ thực tế 1 tuần để xác nhận) → Target: < 15 phút/ngày · Đo bằng: kỹ sư tự bấm giờ trong 2 tuần pilot |
| Phương án không dùng AI | Template Excel chuẩn hóa + Google Form trên điện thoại nhập liệu tại chỗ → giảm bước gõ lại nhưng vẫn phải nhập từng trường thủ công |
| Giả thuyết về AI (nếu có) | Kỹ sư nói vào điện thoại (voice memo) tóm tắt ngày làm việc → AI transcribe + parse theo cấu trúc nhật ký (nhân công, thiết bị, khối lượng, sự cố) → điền vào template → kỹ sư review và xác nhận trước khi gửi |
| Cảm nhận nhanh | **Workflow** — các bước định sẵn rõ ràng; AI làm bước parse/điền; con người review trước khi gửi |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~50 phút/ngày

[Ghi chép sổ tay thực địa (cả ngày)]
→ [Mở Excel mẫu nhật ký: 5']
→ [Gõ lại từng mục từ sổ tay: 30–40'] ← BOTTLENECK
→ [Chụp ảnh đính kèm: 5']
→ [Gửi email/Zalo về văn phòng: 5']

TƯƠNG LAI — ~15 phút/ngày

[Ghi chép sổ tay thực địa (cả ngày)]
→ [Nói voice memo tóm tắt cuối ngày: 3–5'] ← Thay thế bước gõ lại
→ [AI transcribe + parse → điền vào template: 1–2'] ← AI
→ [Kỹ sư review, bổ sung nếu thiếu: 5–7']  ← CON NGƯỜI (boundary: AI không tự gửi)
→ [Xác nhận và gửi: 2']

Phương án quay về: AI parse sai → kỹ sư tự điền theo template Excel cũ
```

---

### Problem Card #2 — Gom hồ sơ nghiệm thu theo yêu cầu

| Trường | Nội dung |
|---|---|
| Job Story | Khi giám sát của chủ đầu tư yêu cầu cung cấp hồ sơ nghiệm thu một hạng mục (biên bản kiểm tra vật liệu, biên bản nghiệm thu nội bộ, kết quả thí nghiệm, bản vẽ hoàn công), tôi muốn tập hợp và gửi đủ bộ hồ sơ trong ngày, để không làm chậm tiến độ nghiệm thu và thanh toán đợt. |
| Actor | Kỹ sư hiện trường / Kỹ sư hồ sơ (người tổng hợp); liên quan đến kỹ sư thí nghiệm, kỹ sư vật liệu, cán bộ kỹ thuật từng hạng mục |
| Thời điểm / bối cảnh | Khi có yêu cầu nghiệm thu hạng mục (không định kỳ, đột xuất); thường có áp lực thời gian vì liên quan trực tiếp đến thanh toán đợt |
| Quy trình hiện tại (3–7 bước) | 1. Nhận yêu cầu từ giám sát (danh sách hồ sơ cần nộp) · 2. Xác định từng loại biên bản cần có theo checklist nghiệm thu · 3. Liên hệ từng người giữ từng loại hồ sơ qua Zalo/điện thoại · 4. Chờ nhận file scan hoặc bản cứng từ từng người (thường mất nửa ngày vì người bận thi công) · 5. Kiểm tra đủ bộ, đúng nội dung, đúng mốc thời gian · 6. Đóng gói và gửi (email + hard copy) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3+4 — chờ hồ sơ từ nhiều người: **[GT]** ~4–6 tiếng; người giữ hồ sơ không ưu tiên vì đang bận việc thi công; hồ sơ phân tán nhiều nơi (email cũ, folder máy tính cá nhân, bản cứng trong tủ) |
| Impact (nếu không giải thì sao) | Thiếu 1 biên bản → chủ đầu tư từ chối nghiệm thu → trễ thanh toán đợt 15–30 ngày → ảnh hưởng dòng tiền dự án; kỹ sư mất thời gian chạy theo đốc thúc từng người |
| Success metric (baseline → target) | Baseline: **[GT]** 0.5–1 ngày làm việc/hạng mục để gom đủ hồ sơ → Target: < 2 tiếng · Tỷ lệ nghiệm thu passed lần đầu (không bị yêu cầu bổ sung): đo theo số lần nghiệm thu/quý |
| Phương án không dùng AI | Checklist chuẩn hóa theo loại hạng mục + folder Drive chia sẻ theo hạng mục → giảm quên sót nhưng vẫn phải gom thủ công |
| Giả thuyết về AI (nếu có) | AI scan yêu cầu từ giám sát → đối chiếu với kho hồ sơ Drive → báo thiếu tài liệu nào, cần lấy từ ai → tự động gửi nhắc nhở đến người phụ trách → kỹ sư review bộ hồ sơ hoàn chỉnh trước khi gửi |
| Cảm nhận nhanh | **Workflow** — các bước định sẵn; AI làm bước đối chiếu và nhắc nhở; con người kiểm tra và gửi |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~0.5–1 ngày/hạng mục

[Nhận yêu cầu từ giám sát: 15']
→ [Xác định checklist cần nộp: 15']
→ [Liên hệ từng người qua Zalo/điện thoại: 30']
→ [Chờ nhận file từ từng người: 3–5h] ← BOTTLENECK
→ [Kiểm tra đủ bộ, đúng nội dung: 30']
→ [Đóng gói + gửi: 30']

TƯƠNG LAI — ~2 tiếng/hạng mục

[Nhận yêu cầu từ giám sát: 15']
→ [AI đối chiếu với kho Drive → báo thiếu gì: 5'] ← AI
→ [AI tự gửi nhắc nhở đến người phụ trách: 5'] ← AI
→ [Người phụ trách upload hồ sơ: 60'] ← CON NGƯỜI (vẫn cần người upload)
→ [Kỹ sư review đủ bộ: 20']             ← CON NGƯỜI (boundary: AI không tự gửi cho CĐT)
→ [Gửi cho giám sát: 15']

Phương án quay về: AI miss hồ sơ → kỹ sư dùng checklist Excel thủ công
```

---

### Problem Card #3 — Đọc bản vẽ revision, xác định thay đổi kỹ thuật

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận được bộ hồ sơ thiết kế mới (bản vẽ thi công + thuyết minh kỹ thuật + danh mục vật liệu) từ tư vấn thiết kế, tôi muốn nhanh chóng xác định các điểm thay đổi so với phiên bản trước và những yêu cầu kỹ thuật đặc biệt cần lưu ý, để bàn giao đúng thông tin cho tổ trưởng thi công trước khi đổ bê tông. |
| Actor | Kỹ sư hiện trường (người nhận và đọc bản vẽ); Tổ trưởng thi công (người nhận thông tin); Giám sát tư vấn (người phát hành revision) |
| Thời điểm / bối cảnh | Mỗi khi tư vấn phát hành revision bản vẽ (không định kỳ, có thể 1–3 lần/tháng/dự án); thường có áp lực thời gian vì tổ thi công đang chờ để triển khai |
| Quy trình hiện tại (3–7 bước) | 1. Nhận bộ bản vẽ mới qua email (PDF hoặc DWG) · 2. Tìm phiên bản cũ tương ứng trong máy hoặc server · 3. So sánh thủ công từng trang, từng sheet (đọc revision cloud nếu có, hoặc so sánh mắt) · 4. Ghi chép danh sách thay đổi vào sổ hoặc email nội bộ · 5. Họp brief với tổ trưởng thi công · 6. Lưu trữ version mới, đánh dấu version cũ obsolete |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 — so sánh thủ công từng trang: **[GT]** 2–4 tiếng/lần revision; bản vẽ dân dụng thường 30–80+ sheet; không phải sheet nào cũng có revision cloud rõ ràng |
| Impact (nếu không giải thì sao) | Bỏ sót thay đổi kỹ thuật → thi công sai spec → phá dỡ làm lại (chi phí có thể lên đến hàng chục triệu đồng/sự cố) + trễ tiến độ + tranh chấp trách nhiệm với tư vấn |
| Success metric (baseline → target) | Baseline: **[GT]** 2–4 tiếng/lần revision → Target: < 30 phút/lần · Tỷ lệ sự cố thi công sai do missed revision: từ X → 0 (đo theo số sự cố/quý) |
| Phương án không dùng AI | Hệ thống document control (Procore, Autodesk Construction Cloud) có tính năng revision tracking tự động → highlight delta giữa 2 version; nhưng cần đầu tư phần mềm và onboarding |
| Giả thuyết về AI (nếu có) | AI so sánh 2 file PDF bản vẽ → liệt kê danh sách thay đổi theo sheet (kích thước, cao độ, vật liệu, ghi chú) → kỹ sư review danh sách và xác nhận trước khi brief tổ thi công |
| Cảm nhận nhanh | **Workflow** — bước AI là bước so sánh document; con người review và xác nhận (vì AI có thể miss thay đổi tinh vi về ký hiệu kỹ thuật) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~3 tiếng/lần revision

[Nhận bản vẽ mới qua email: 5']
→ [Tìm phiên bản cũ tương ứng: 10–15']
→ [So sánh thủ công từng sheet: 90–180'] ← BOTTLENECK
→ [Ghi chép danh sách thay đổi: 20']
→ [Brief tổ trưởng thi công: 20']
→ [Lưu trữ + đánh dấu obsolete: 10']

TƯƠNG LAI — ~30 phút/lần revision

[Nhận bản vẽ mới qua email: 5']
→ [Upload 2 version vào tool: 2']
→ [AI so sánh → xuất danh sách thay đổi theo sheet: 3–5'] ← AI
→ [Kỹ sư review danh sách, check thay đổi tinh vi: 15'] ← CON NGƯỜI
   (boundary: AI không tự thông báo cho tổ thi công)
→ [Brief tổ trưởng thi công dựa trên danh sách: 10']
→ [Lưu trữ + đánh dấu obsolete: 5']

Phương án quay về: AI so sánh sai/miss → kỹ sư đọc thủ công theo quy trình cũ
```

---

### Card muốn pitch nhất

- **Card số:** #1 — Nhật ký thi công hằng ngày
- **Vì sao:** Lặp lại mỗi ngày làm việc (5–6 ngày/tuần) → ROI cao nhất nếu giải được; bottleneck gõ lại dữ liệu rõ ràng, dễ đo; bắt buộc pháp lý (Nghị định 06/2021) nên người dùng không thể bỏ bước này; giải pháp voice-to-text + AI parse có thể pilot nhanh chỉ cần điện thoại, không cần đầu tư hệ thống.
- **Câu hỏi muốn nhóm phản biện:** (1) Voice-to-text tiếng Việt kỹ thuật xây dựng có đủ chính xác không (tên hạng mục, số liệu)? (2) Kỹ sư hiện trường có chịu thay đổi thói quen ghi sổ tay không? (3) Nếu AI parse sai số liệu khối lượng và kỹ sư không phát hiện → ai chịu trách nhiệm?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 50 phút chỉ là ước lượng, chưa có bấm giờ thực tế | Đồng ý | Đánh dấu `[GT]`, thêm cách đo vào Success metric (bấm giờ 1 tuần trước pilot) |
| Voice-to-text dễ sai tên hạng mục kỹ thuật tiếng Việt | Đồng ý một phần | Thêm bước "kỹ sư review" bắt buộc trước khi gửi; AI không tự động gửi |
| Chưa rõ ai sở hữu template nhật ký — kỹ sư tự làm hay do CĐT áp mẫu | Đồng ý | Thêm vào "Điều còn chưa chắc" ở bảng chọn top 3 |
| Gợi ý làm Agent tự gửi báo cáo về văn phòng mỗi tối | Không đồng ý | Giữ boundary rõ: AI không tự gửi; kỹ sư phải xác nhận trước |

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
