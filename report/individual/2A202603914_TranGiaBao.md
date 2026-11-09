# Báo cáo cá nhân — 2A202603914_TranGiaBao

> Đổi tên file theo quy tắc `2A202603914_TranGiaBao.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Gia Bảo
- MSSV: 2A202603914
- Email trường: không công khai
- Tên nhóm: HEHEHE
- Link repo nhóm: https://github.com/hoangvu1806/K5-L3B-DAY02-HEHEHE-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

**Chủ đề khảo sát:** Ghi nhận, theo dõi và phân tích lỗi chất lượng trong xưởng sản xuất (Manufacturing Quality Control). Các vấn đề dưới đây là những tình huống cần xác minh với nhân viên QC, tổ trưởng hoặc quản lý xưởng. Chưa có kết quả phỏng vấn nên không coi chúng là những sự việc đã xảy ra tại một doanh nghiệp cụ thể.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi kiểm tra một lô sản phẩm, tôi muốn ghi nhận lỗi theo cùng một quy chuẩn, để người ở ca sau hiểu đúng loại lỗi đã phát hiện. | Nhân viên QC | Cần đối chiếu 10 phiếu QC: số phiếu dùng tên lỗi khác nhau, số phút chỉnh lại thông tin. |
| 2 | Tốn thời gian | Khi cần lập báo cáo chất lượng cuối ca, tôi muốn tổng hợp kết quả kiểm tra nhanh và đúng, để bàn giao kịp thời cho tổ trưởng. | QC, tổ trưởng | Cần bấm giờ từ lúc nhận phiếu đến khi xong báo cáo; số báo cáo/tuần. |
| 3 | Đọc, tổng hợp nhiều thông tin | Khi một mã lỗi xuất hiện liên tiếp, tôi muốn tìm được các lô, máy và ca có cùng lỗi, để khoanh vùng phạm vi cần kiểm tra. | Quản lý chất lượng | Cần ghi nhận thời gian tra cứu, số file/sổ phải mở và số lần truy xuất. |
| 4 | Pain từ người khác | Khi tổ trưởng nhận báo cáo lỗi, tôi muốn biết lỗi nào cần xử lý trước, để không phải hỏi lại QC về mức độ ảnh hưởng. | Tổ trưởng, QC | Cần hỏi tổ trưởng lần gần nhất phải làm rõ báo cáo; ghi số câu hỏi lại. |
| 5 | Lặp lại | Khi chuyển ca, tôi muốn bàn giao rõ các lô đang chờ kiểm tra lại, để ca tiếp theo không xử lý trùng hoặc bỏ sót. | QC hai ca | Cần kiểm tra biên bản bàn giao và số lô bị thiếu trạng thái. |
| 6 | Tốn thời gian | Khi phát hiện sản phẩm không đạt, tôi muốn truy lại được lô nguyên liệu liên quan, để xác định những sản phẩm khác cần kiểm tra. | QC, kho nguyên liệu | Cần đo thời gian tra lô và tỷ lệ hồ sơ thiếu mã truy xuất. |
| 7 | Đọc, tổng hợp nhiều thông tin | Khi họp chất lượng hàng tuần, tôi muốn nhìn thấy tỷ lệ lỗi theo lô, công đoạn và ca sản xuất, để có cơ sở chọn vấn đề cần điều tra. | Quản lý xưởng | Cần đối chiếu cách tổng hợp hiện tại, số bảng dữ liệu và phút làm báo cáo. |
| 8 | Pain từ người khác | Khi một lô hàng bị cách ly do lỗi, tôi muốn được cập nhật kết luận kiểm tra và người phê duyệt, để không xuất nhầm hàng chưa đạt. | Nhân viên kho, QC | Cần kiểm tra số lần hỏi trạng thái và số phiếu thiếu kết luận/phê duyệt. |

**Ý cần kiểm chứng trước:** #2, #3 và #5 vì có quy trình dễ quan sát, bottleneck cụ thể và có thể đo bằng phút hoặc số hồ sơ thiếu thông tin. Các chỉ số trong cột cuối là kế hoạch thu thập bằng chứng, chưa phải số liệu khảo sát.

**Ghi nhận sử dụng AI:** Tôi sử dụng AI để sắp xếp các tình huống thành Job Story và kiểm tra xem có mô tả nhầm giải pháp thành vấn đề không. Chưa có cơ sở để khẳng định các tình huống trên xuất hiện thường xuyên trong một xưởng cụ thể; cần xác minh trực tiếp.

---

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Truy tìm các lô và ca có cùng mã lỗi (#3) | Có thể đo thời gian truy xuất và số hồ sơ cần đọc; phù hợp để thu hẹp bài toán | Doanh nghiệp đã có MES hoặc báo cáo lọc theo mã lỗi chưa? |
| 2 | Tổng hợp báo cáo chất lượng cuối ca (#2) | Công việc có đầu ra rõ, dễ so sánh trước/sau | Bước nhập dữ liệu hay kiểm số liệu mới tốn nhiều thời gian? |
| 3 | Bàn giao lô đang chờ kiểm tra lại (#5) | Liên quan trực tiếp tới phối hợp giữa hai ca, có phương án không cần AI | Thực tế có bị bỏ sót không, hay quy trình hiện tại đã đủ? |

### Problem Card #1 — Truy xuất lịch sử lỗi theo lô, máy và ca sản xuất

| Trường | Nội dung |
|---|---|
| Job Story | Khi một loại lỗi xuất hiện nhiều lần, tôi muốn biết những lô, máy và ca nào có lỗi tương tự, để xác định phạm vi cần kiểm tra. |
| Actor | Nhân viên quản lý chất lượng hoặc kỹ sư QC ở xưởng sản xuất |
| Thời điểm / bối cảnh | Khi QC báo phát hiện mã lỗi lặp lại hoặc trước cuộc họp xử lý lỗi |
| Quy trình hiện tại | 1. Nhận mã lỗi · 2. Mở sổ/file kiểm tra · 3. Lọc các bản ghi liên quan · 4. Đối chiếu lô, máy, ca · 5. Tổng hợp kết quả · 6. Gửi quản lý |
| Bottleneck | Bước 3–4: tìm và đối chiếu bản ghi từ nhiều nguồn; thời gian thực tế: **[cần đo]** |
| Impact | Có thể chậm khoanh vùng lô liên quan hoặc bỏ sót bản ghi cần kiểm tra |
| Success metric | Baseline: [phút/lần truy xuất, tỷ lệ tìm đúng]; target **đề xuất**: giảm 30% thời gian, không giảm độ đầy đủ; đo cùng 10 tình huống truy xuất |
| Phương án không dùng AI | Chuẩn hóa bảng ghi QC, dùng bộ lọc theo mã lỗi/lô/máy/ca và bảng tổng hợp |
| Giả thuyết về AI | Chỉ dùng khi mô tả lỗi bằng ngôn ngữ tự do không thống nhất, hỗ trợ đề xuất mã lỗi tương ứng để QC duyệt |
| Cảm nhận nhanh | Rule trước, Workflow nếu dữ liệu mô tả tự do khiến Rule không đủ |

```text
HIỆN TẠI — thời gian từng bước cần khảo sát
[1 Nhận mã lỗi: ?'] → [2 Mở hồ sơ: ?']
→ [3 Tìm bản ghi: ?'] → [4 Đối chiếu lô/máy/ca: ?']  ← NGHI VẤN BOTTLENECK
→ [5 Tổng hợp: ?'] → [6 Gửi quản lý: ?']
```

### Problem Card #2 — Lập báo cáo chất lượng cuối ca

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc ca sản xuất, tôi muốn tổng hợp số lượng kiểm tra, loại lỗi và số lượng không đạt, để tổ trưởng có báo cáo chính xác trước khi bàn giao. |
| Actor | Nhân viên QC phụ trách báo cáo cuối ca |
| Thời điểm / bối cảnh | Cuối mỗi ca, khi số liệu nằm trong các phiếu kiểm tra hoặc file riêng |
| Quy trình hiện tại | 1. Thu phiếu · 2. Kiểm tra thông tin thiếu · 3. Nhập/tổng hợp số liệu · 4. Đối chiếu tổng · 5. Làm báo cáo · 6. Gửi tổ trưởng |
| Bottleneck | Bước 3: nhập và cộng gộp số liệu; thời gian thực tế: **[cần đo]** |
| Impact | Có thể gửi báo cáo muộn hoặc sai tỷ lệ lỗi nếu nhập liệu không nhất quán |
| Success metric | Baseline: [phút/báo cáo, số lỗi nhập liệu]; target **đề xuất**: giảm 30% thời gian và không tăng sai số; đo trên 10 báo cáo |
| Phương án không dùng AI | Mẫu Excel chuẩn với dropdown mã lỗi, validation và công thức tổng hợp |
| Giả thuyết về AI | Đọc mô tả lỗi tự do hoặc phiếu scan để hỗ trợ nhập dữ liệu, người dùng kiểm lại |
| Cảm nhận nhanh | No AI / Rule có thể đã đủ |

```text
HIỆN TẠI — thời gian từng bước cần khảo sát
[1 Thu phiếu: ?'] → [2 Kiểm tra: ?']
→ [3 Nhập/tổng hợp: ?']  ← NGHI VẤN BOTTLENECK
→ [4 Đối chiếu: ?'] → [5 Tạo báo cáo: ?'] → [6 Gửi: ?']
```

### Problem Card #3 — Bàn giao lô hàng cần kiểm tra lại giữa các ca

| Trường | Nội dung |
|---|---|
| Job Story | Khi giao ca, tôi muốn biết lô nào đang chờ kiểm tra lại, ai phụ trách và hạn xử lý, để ca sau tiếp tục đúng công việc chưa hoàn thành. |
| Actor | Nhân viên QC ca trước, QC ca sau và tổ trưởng |
| Thời điểm / bối cảnh | Cuối ca khi còn lô chưa có kết luận đạt/không đạt |
| Quy trình hiện tại | 1. Rà soát lô đang mở · 2. Tìm phiếu liên quan · 3. Xác định trạng thái · 4. Ghi danh sách bàn giao · 5. Trao đổi với ca sau · 6. Ca sau xác nhận |
| Bottleneck | Bước 2–4: tìm và tổng hợp trạng thái từ hồ sơ; thời gian thực tế: **[cần đo]** |
| Impact | Có nguy cơ kiểm tra trùng, quên lô hoặc bàn giao thiếu người chịu trách nhiệm |
| Success metric | Baseline: [phút/bàn giao; số lô thiếu trạng thái]; target **đề xuất**: giảm 25% thời gian, không còn lô thiếu mã hoặc người phụ trách; đo tối thiểu 10 lần bàn giao |
| Phương án không dùng AI | Sổ bàn giao điện tử với mã lô, trạng thái bắt buộc và chữ ký xác nhận |
| Giả thuyết về AI | Tóm tắt ghi chú bất thường cho ca sau; không tự thay đổi trạng thái duyệt lô |
| Cảm nhận nhanh | Rule; chưa có bằng chứng cần AI |

```text
HIỆN TẠI — thời gian từng bước cần khảo sát
[1 Rà lô: ?'] → [2 Tìm phiếu: ?']
→ [3 Xác định trạng thái: ?'] → [4 Lập danh sách: ?'] ← NGHI VẤN BOTTLENECK
→ [5 Bàn giao: ?'] → [6 Xác nhận: ?']
```

### Card muốn pitch nhất

- **Card số:** 1 — Truy xuất lịch sử lỗi theo lô, máy và ca.
- **Vì sao:** Phạm vi rõ ràng, có khả năng đo bằng thời gian tìm hồ sơ và mức độ đầy đủ của kết quả. Có thể kiểm chứng ngay trên dữ liệu QC đã ẩn danh.
- **Câu hỏi muốn nhóm phản biện:** Nếu xưởng đã lưu dữ liệu vào một file chuẩn và có chức năng lọc theo mã lỗi, còn lý do gì khiến việc truy xuất vẫn chậm?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa có bằng chứng cho thấy xưởng thực sự mất nhiều thời gian truy xuất | Đồng ý | Giữ baseline cần đo, đề nghị khảo sát tình huống truy xuất gần nhất |
| Cùng một lỗi không đồng nghĩa cùng một nguyên nhân | Đồng ý | Chỉ đề xuất khoanh vùng bản ghi, không tự kết luận nguyên nhân gốc |
| Bộ lọc và bảng dữ liệu chuẩn có thể giải quyết phần lớn vấn đề | Đồng ý | Đưa Rule làm phương án thử trước, chưa mặc định dùng AI |

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

- [Đề bài CHECKPOINTS](../../CHECKPOINTS.md)
- [Quy định sử dụng AI](../../RULES.md)
- [Rubric](../../RUBRIC.md)
- [Bổ sung nguồn tài liệu hoặc hồ sơ QC được phép sử dụng sau khi xác minh]
