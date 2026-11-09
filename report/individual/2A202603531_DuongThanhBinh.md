# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Dương Thanh Bình
- MSSV: 2A202603531
- Email trường (không bắt buộc, repo có thể để public): 26ai.binhdt2@vinuni.edu.vn
- Tên nhóm: TenNhom
- Link repo nhóm: https://github.com/trinhcongduc112/K5-L3A-DAY02-TenNhom-DiscoveryProblemFraming.git

---

**Bối cảnh:** Binh, Junior AI Engineer trong một nhóm AI khoảng 8 người, phục vụ các ứng dụng của hệ sinh thái VinGroup (giả định: chatbot/trợ lý ảo hỗ trợ chủ xe VinFast và tài xế Xanh SM trong app). Công cụ: Python, GitHub, Jira, Slack, Google Sheets, công cụ gán nhãn, hệ thống log hội thoại. Binh làm việc cùng PM, đội CSKH/vận hành, data engineer, security và các đơn vị yêu cầu AI.

## 2. Scan problem (CP1)

Scan 11 problem, vượt mức tối thiểu 5. Chưa lọc, bước sau mới chọn.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi vừa sửa system prompt hoặc đổi model của chatbot, tôi muốn biết câu trả lời nào xấu đi so với bản cũ, để không phát hành bản làm hỏng câu đã đúng | AI engineer, PM, người dùng app | Bộ test ~120 câu, đọc tay ~100 phút/lần, ~4 lần/tuần (cần bấm giờ) |
| 2 | Lặp lại | Khi nhận batch log hội thoại thật để làm dữ liệu đánh giá, tôi muốn loại thông tin cá nhân (SĐT, địa chỉ, biển số, số khung xe), để dùng dữ liệu mà không vi phạm quyền riêng tư | AI engineer, security, người dùng | ~5.000 hội thoại/batch, ~200 phút/batch, ~2 batch/tháng; regex bỏ sót tên và địa chỉ viết tự do |
| 3 | Tốn thời gian | Khi gán nhãn ý định và lỗi bot cho hội thoại tiếng Việt, tôi muốn nhãn nhất quán giữa các người gán, để bộ đánh giá không dạy model sai | AI engineer, người gán nhãn | ~6 giờ/1.000 mẫu; 2 người gán bất đồng ~20% (cần đo độ đồng thuận) |
| 4 | Tốn thời gian | Khi so sánh 2–3 LLM (API và tự host) cho một tính năng, tôi muốn có chất lượng tiếng Việt, độ trễ và chi phí trên cùng bộ test, để chọn model có căn cứ | AI engineer, PM, finance | ~2 ngày/lần so sánh, ~2 lần/quý |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị bộ test cho tính năng mới, tôi muốn gom câu hỏi thật từ ticket, review app và log, để bộ test phản ánh người dùng thật chứ không phải câu tự nghĩ | AI engineer, QA | 3 nguồn rời rạc; ~4 giờ/bộ 100 câu |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi chính sách bảo hành hoặc cước phí thay đổi, tôi muốn biết tài liệu nào đổi và câu trả lời nào của bot bị ảnh hưởng, để bot không trả lời theo chính sách cũ | AI engineer, CSKH, người dùng | ~30 tài liệu cập nhật/quý; từng có ~3 ca bot trả lời chính sách cũ trong 2 tuần (cần log thật) |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi một đơn vị trong hệ sinh thái gửi yêu cầu "làm AI cho X", tôi muốn biết dữ liệu nào có, ai sở hữu và được phép dùng không, để biết khả thi trước khi cam kết | AI engineer, đơn vị yêu cầu, data owner | ~3 yêu cầu/tháng, mỗi yêu cầu ~3–5 ngày làm rõ dữ liệu |
| 8 | Pain từ người khác | Khi PM hoặc vận hành hỏi "bot hôm qua sao trả lời sai?", họ muốn biết nguyên nhân và có lặp lại không, để quyết định rollback hay chờ sửa | PM, vận hành, AI engineer | ~10 câu hỏi/tuần ở Slack, mỗi ca ~45 phút điều tra |
| 9 | Pain từ người khác | Khi tài xế Xanh SM hỏi bot về thu nhập hay chính sách thưởng phạt mà bot trả lời chung chung hoặc sai, tài xế muốn có câu trả lời đúng ngay, để không phải gọi tổng đài chờ lâu | Tài xế, tổng đài | ~12% hội thoại chuyển người trực sau ≥3 lượt (cần số thật hoặc ước từ mẫu) |
| 10 | Pain từ người khác | Khi data engineer thấy log hội thoại đổi định dạng sau mỗi lần app cập nhật, họ muốn AI engineer báo trước, để pipeline không gãy | Data engineer, AI engineer | ~2 lần/quý pipeline gãy, mỗi lần mất ~1 ngày sửa |
| 11 | Lặp lại | Khi bot đang chạy, tôi muốn biết khi nào chất lượng giảm (sau chiến dịch khuyến mãi, ra dòng xe mới), để xử lý trước khi người dùng phàn nàn | AI engineer, PM | Phát hiện qua phàn nàn thường trễ ~3–5 ngày; đọc mẫu 50 hội thoại/tuần ~2 giờ |

**Phân bố lăng kính:** Lặp lại (#1, #2, #11), Tốn thời gian (#3, #4), Cần đọc/tổng hợp (#5, #6, #7), Pain từ người khác (#8, #9, #10).

**AI gợi ý thêm:** *(điền sau khi dùng prompt)*
- Ý AI gợi ý và giữ lại: ...
- Ý AI gợi ý nhưng bỏ (quá rộng / không có quy trình thật / chứa giải pháp): ...

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Kiểm tra hồi quy khi đổi prompt/model (#1) | Lặp lại hằng tuần, quy trình rõ, bottleneck là một bước, đo được bằng phút; đúng việc của AI engineer | LLM chấm điểm có khớp với người chấm không |
| 2 | Làm sạch thông tin cá nhân trong log hội thoại (#2) | Doanh nghiệp bắt buộc phải làm, so sánh được cả 4 mức, rủi ro rõ | Dữ liệu thật không đưa ra API ngoài được, cần làm với dữ liệu mẫu/tổng hợp |
| 3 | Điều tra hội thoại bot trả lời sai (#8) | Pain từ người khác có bằng chứng (Slack), phù hợp agent chỉ đọc | Phạm vi dễ phình thành "agent vận hành toàn hệ thống" |

**Vì sao chưa chọn các ý khác:**
- **#3 Gán nhãn:** chất lượng nhãn khó đo trong một buổi lab.
- **#4 So sánh LLM:** việc làm theo dự án, ít lặp lại.
- **#5, #7:** phụ thuộc vào nhiều nguồn dữ liệu nội bộ, khó mô phỏng.
- **#6 Cập nhật chính sách:** hợp với RAG nhưng cần kho tài liệu thật, để dành làm hướng mở rộng.
- **#9:** vấn đề của người dùng cuối, ít quy trình của kỹ sư.
- **#10, #11:** có thể dùng rule và dashboard là đủ, hoặc cần hạ tầng giám sát thật.

### Problem Card #1 — Kiểm tra hồi quy khi đổi prompt/model

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa sửa system prompt hoặc đổi model của chatbot, tôi muốn biết câu trả lời nào xấu đi so với bản cũ, để không phát hành bản làm hỏng câu đã đúng |
| Actor | Junior AI Engineer phụ trách chatbot hỗ trợ chủ xe/tài xế |
| Thời điểm / bối cảnh | Mỗi lần sửa prompt hoặc thử model mới, ~4 lần/tuần, trước khi PM duyệt phát hành |
| Quy trình hiện tại | 1. Sửa prompt hoặc đổi model · 2. Chạy ~120 câu test qua bot bằng script · 3. Đọc từng câu trả lời, so với đáp án kỳ vọng và bản cũ · 4. Ghi các câu xấu đi vào bảng · 5. Báo PM và QA · 6. Quyết định phát hành hoặc sửa tiếp |
| Bottleneck | Bước 3, đọc và so từng câu trả lời: ~60 phút/lần vì phải đọc cả câu dài, phân biệt "diễn đạt khác nhưng đúng" với "sai thật" |
| Impact | ~100 phút/lần × ~4 lần/tuần ≈ 400 phút/tuần cho 1 AI engineer; ~1/5 lần vẫn bỏ sót câu xấu đi và bị phát hiện sau khi phát hành (cần số thật) |
| Success metric | (1) Thời gian từ ~100 xuống dưới 35 phút/lần; (2) phát hiện ≥90% ca xấu đi mà người chấm tay tìm ra; (3) 0 ca nghiêm trọng (sai chính sách, sai an toàn) bị bỏ sót |
| Phương án không dùng AI | Bảng so sánh bản cũ/bản mới + checklist câu "bắt buộc đúng". Giảm bỏ sót nhưng vẫn phải đọc tay |
| Giả thuyết về AI | Rule kiểm sự kiện cứng (số hotline, mức phí, từ khóa bắt buộc); LLM chấm theo rubric rồi gắn cờ câu nghi ngờ; kỹ sư chỉ đọc các câu bị cờ |
| Cảm nhận nhanh | Workflow |

```text
HIỆN TẠI — ~100 phút/lần (ước lượng)

[1 Sửa prompt/model: 5'] → [2 Chạy 120 câu test: 10'] → [3 Đọc & so từng câu: 60'] ← BOTTLENECK
→ [4 Ghi câu xấu đi: 10'] → [5 Báo PM/QA: 10'] → [6 Quyết định: 5']
```

### Problem Card #2 — Làm sạch thông tin cá nhân trong log hội thoại

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận batch log hội thoại thật để làm dữ liệu đánh giá, tôi muốn loại thông tin cá nhân (SĐT, địa chỉ, biển số, số khung xe), để dùng dữ liệu mà không vi phạm quyền riêng tư |
| Actor | Junior AI Engineer cần dữ liệu thật cho bộ đánh giá và huấn luyện |
| Thời điểm / bối cảnh | Mỗi khi xuất batch mới từ hệ thống log, ~2 lần/tháng, trước khi đưa vào kho dữ liệu dùng chung |
| Quy trình hiện tại | 1. Xin quyền và xuất batch log · 2. Quét regex (SĐT, email) · 3. Đọc mẫu để tìm thông tin cá nhân regex bỏ sót (tên, địa chỉ viết tự do, biển số, số khung xe) · 4. Che bằng token (`<TEN>`, `<DIA_CHI>`) · 5. Kiểm mẫu lần hai · 6. Security duyệt · 7. Đưa vào kho dữ liệu |
| Bottleneck | Bước 3, đọc mẫu tìm thông tin regex bỏ sót: ~120 phút/batch vì tên và địa chỉ tiếng Việt viết nhiều kiểu, có cả không dấu và viết tắt |
| Impact | ~200 phút/batch × ~2 batch/tháng ≈ 400 phút/tháng cho 1 AI engineer; mỗi lần sót là rủi ro vi phạm quy định bảo vệ dữ liệu cá nhân |
| Success metric | (1) Thời gian từ ~200 xuống dưới 80 phút/batch; (2) tỉ lệ bắt được thông tin cá nhân ≥98% trên mẫu 300 hội thoại gán tay; (3) 0 thông tin cá nhân sót trong lần kiểm mẫu cuối |
| Phương án không dùng AI | Quy trình + checklist, bỏ các trường nhạy cảm ngay từ lúc xuất log. Giảm khối lượng nhưng không xử lý được thông tin cá nhân nằm trong nội dung chat |
| Giả thuyết về AI | Rule bắt dữ liệu có định dạng (SĐT, email, số khung xe 17 ký tự); mô hình nhận diện thực thể chạy nội bộ bắt tên và địa chỉ; người kiểm mẫu; security duyệt. Không đưa log thô qua API ngoài công ty |
| Cảm nhận nhanh | Rule cho dữ liệu có định dạng, Workflow cho phần còn lại |

```text
HIỆN TẠI — ~200 phút/batch (ước lượng)

[1 Xin quyền + xuất log: 15'] → [2 Quét regex: 10'] → [3 Đọc mẫu tìm thông tin sót: 120'] ← BOTTLENECK
→ [4 Che token: 15'] → [5 Kiểm mẫu lần 2: 25'] → [6 Security duyệt: 10'] → [7 Đưa vào kho: 5']
```

### Problem Card #3 — Điều tra hội thoại bot trả lời sai

| Trường | Nội dung |
|---|---|
| Job Story | Khi PM hoặc vận hành báo "bot trả lời sai", tôi muốn biết lỗi nằm ở đâu (tài liệu tri thức, truy xuất, prompt hay model) và có lặp lại không, để sửa đúng chỗ và quyết định có cần rollback |
| Actor | Junior AI Engineer trực xử lý phản hồi lỗi của chatbot |
| Thời điểm / bối cảnh | Trong ngày làm việc, thường sau khi có phản ánh từ tổng đài hoặc người dùng |
| Quy trình hiện tại | 1. Nhận báo lỗi trên Slack · 2. Tìm hội thoại trong log · 3. Đối chiếu tài liệu bot đã truy xuất, phiên bản prompt và câu trả lời · 4. Tái hiện lỗi · 5. Tìm hội thoại tương tự có lỗi lặp lại không · 6. Kết luận nguyên nhân và trả lời người báo · 7. Mở ticket sửa |
| Bottleneck | Bước 3, đối chiếu truy xuất, prompt và câu trả lời: ~12 phút/ca vì thông tin nằm ở 3 nơi (log, kho tri thức, repo prompt) |
| Impact | ~45 phút/ca × ~10 ca/tuần ≈ 450 phút/tuần cho nhóm; trong lúc chờ, lỗi có thể lặp lại với người dùng khác |
| Success metric | (1) Thời gian từ ~45 xuống dưới 20 phút/ca; (2) xác định đúng nhóm nguyên nhân ≥80% (kỹ sư xác nhận sau); (3) phản hồi người báo trong 30 phút |
| Phương án không dùng AI | Chuẩn hóa log (ghi sẵn tài liệu truy xuất và phiên bản prompt vào mỗi hội thoại) + mẫu báo lỗi. Có thể giải quyết phần lớn bước 3 |
| Giả thuyết về AI | Agent chỉ đọc: nhận ID hội thoại, lấy log, tài liệu truy xuất, phiên bản prompt; đề xuất nhóm nguyên nhân kèm bằng chứng và số hội thoại tương tự; kỹ sư xác nhận |
| Cảm nhận nhanh | Workflow hoặc Agent (chỉ đọc, cân nhắc ở CP6) |

```text
HIỆN TẠI — ~45 phút/ca (ước lượng)

[1 Nhận báo lỗi: 2'] → [2 Tìm hội thoại: 5'] → [3 Đối chiếu truy xuất/prompt: 12'] ← BOTTLENECK
→ [4 Tái hiện: 10'] → [5 Tìm ca tương tự: 8'] → [6 Kết luận + trả lời: 5'] → [7 Mở ticket: 3']
```

### Bản pitch nhanh (trình bày với nhóm)

```text
┌──────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #1                                              │
│ Khi vừa sửa prompt hoặc đổi model, tôi muốn biết câu nào xấu │
│ đi so với bản cũ, để không phát hành bản làm hỏng câu đúng   │
│ Ai chịu ảnh hưởng? AI engineer, PM, người dùng app           │
│ Quy trình: 1.Sửa → 2.Chạy test → 3.Đọc & so → 4.Ghi lỗi →    │
│   5.Báo PM → 6.Quyết định                                    │
│ Bước nghẽn: Đọc và so từng câu trả lời (~60 phút/lần)        │
│ Đo thành công: từ ~100 xuống dưới 35 phút/lần                │
│ Cảm nhận nhanh: □ No AI □ Rule ■ Workflow                    │
│                 □ Agent □ Chưa biết                          │
└──────────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #2                                              │
│ Khi nhận log hội thoại thật,

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
