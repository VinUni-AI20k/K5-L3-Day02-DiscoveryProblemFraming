# Báo cáo cá nhân — 2A202603905_HoNguyenMinhSang

## 1. Thông tin học viên

**Học viên:** Hồ Nguyễn Minh Sang · MSSV: 2A202603905 · Nhóm Cold.

**Repo nhóm:** https://github.com/Ama2352/K5-L3B-DAY02-NhomCold-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi tham gia cuộc họp nhóm có nhiều nội dung, tôi muốn ghi lại đầy đủ các quyết định và công việc đã thống nhất, để sau họp có ghi chú rõ ràng làm căn cứ thực hiện. | Các thành viên nhóm | Sắp xếp ghi chú khoảng 10–15 phút/buổi (ước lượng, chưa đo). |
| 2 | Tốn thời gian | Khi chuẩn bị trình bày tiến độ dự án trong buổi họp, tôi muốn xác định nhanh các file liên quan và phiên bản đang dùng, để trình bày đúng kết quả đã hoàn thành. | Dev phụ trách trình bày tiến độ | Nhiều file và bản nháp; tìm bản báo cáo khoảng 10–15 phút/lần (ước lượng, chưa đo). |
| 3 | Lặp lại | Khi đến kỳ thu tiền nhà trọ, tôi muốn tổng hợp tiền thuê, điện nước, phí phát sinh và công nợ từng phòng, để thu đúng tiền và theo dõi thu chi đầy đủ. | Chủ nhà trọ, người quản lý và người thuê | Chốt sổ hằng tháng; cần đo thời gian/kỳ, số khoản kiểm lại và số phòng còn nợ. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi nghiên cứu một chủ đề mới có nhiều khái niệm khó, tôi muốn được giải thích bằng ngôn ngữ đơn giản và ví dụ cụ thể, để hiểu bản chất và vận dụng vào việc đang làm. | Người học, dev nghiên cứu kiến thức hoặc công nghệ mới | Cần lời giải thích đơn giản và ví dụ khi research; cần đo thời gian hiểu và kiểm tra khả năng áp dụng. |
| 5 | Pain từ người khác | Khi nhận phần code được bàn giao để tích hợp, tôi muốn biết cách chạy, cấu hình cần thiết và lỗi còn tồn tại, để tiếp tục công việc mà không phải chờ người viết hướng dẫn lại. | Thành viên nhận bàn giao, người phụ trách tích hợp | Thiết lập khoảng 30–60 phút, hỏi lại 2–3 lần/lượt (ước lượng, cần kiểm chứng). |

**AI gợi ý thêm:** sau khi tự scan 4 ý (#1–#4), tôi hỏi AI và giữ lại ý #5 về bàn giao code vì có actor và quy trình cụ thể.

---

## 3. Top 3 Problem Cards (CP2)

Thời gian trong ba card là ước lượng, cần kiểm tra bằng bấm giờ thực tế.

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp ghi chú cuộc họp (#1) | Nhiều nội dung cần ghi lại; quy trình rõ; đo được thời gian tổng hợp và mức độ đầy đủ của ghi chú | Bước tốn công nhất là ghi chép hay sắp xếp lại? Có thường bỏ sót quyết định không? |
| 2 | Chốt sổ thu chi nhà trọ hằng tháng (#3) | Lặp lại theo kỳ, có đầu vào và đầu ra rõ; kiểm tra được số tiền từng phòng và tình trạng thanh toán | Các khoản phí được phân bổ ra sao? Bước tốn công là nhập chỉ số, tính tiền hay đối chiếu thanh toán? |
| 3 | Hiểu khái niệm khó khi research (#4) | Nhu cầu được nêu trực tiếp; có thể giới hạn ở một khái niệm và kiểm tra bằng việc tự giải thích, làm ví dụ | Cách giải thích nào phù hợp kiến thức nền? Nhanh hơn có giúp hiểu đúng và áp dụng được không? |

### Problem Card #1 — Tổng hợp ghi chú cuộc họp

| Trường | Nội dung |
|---|---|
| Job Story | Khi tham gia cuộc họp nhóm có nhiều nội dung, tôi muốn ghi lại đầy đủ các quyết định và công việc đã thống nhất, để sau họp có ghi chú rõ ràng làm căn cứ thực hiện. |
| Actor | Thành viên nhóm tổng hợp ghi chú cuộc họp |
| Thời điểm / bối cảnh | Ngay sau cuộc họp dự án, khi cần lưu quyết định và phân công |
| Quy trình hiện tại | 1. Đọc lại ghi chú đã ghi trong họp · 2. Gom nội dung theo chủ đề · 3. Tách quyết định và công việc · 4. Đối chiếu người phụ trách, hạn đã thống nhất · 5. Lưu bản ghi chú hoàn chỉnh |
| Bottleneck | Bước 2, gom ghi chú theo chủ đề: khoảng 5 phút (ước lượng) |
| Impact | Khoảng 15 phút/buổi để sắp xếp ghi chú; có nguy cơ bỏ sót quyết định hoặc đầu việc |
| Success metric | 15 → ≤5 phút/buổi; không bỏ sót hoặc ghi sai quyết định và đầu việc. Bấm giờ 3 buổi họp, đối chiếu ghi chép chung |
| Phương án không dùng AI | Mẫu ghi chú chung: chủ đề, quyết định, đầu việc, người phụ trách và hạn; làm rõ ngay trong họp |
| Giả thuyết về AI (nếu có) | AI gom ghi chú theo chủ đề, trích quyết định và đầu việc kèm nguồn; người tổng hợp kiểm tra trước khi lưu. Không tự bổ sung phân công |
| Cảm nhận nhanh | Workflow |

```text
HIỆN TẠI ƯỚC LƯỢNG — 15 phút/buổi

[1 Đọc lại ghi chú: 3'] → [2 Gom nội dung theo chủ đề: 5'] ← BOTTLENECK
→ [3 Tách quyết định và công việc: 3']
→ [4 Đối chiếu phân công và hạn đã thống nhất: 2'] → [5 Lưu ghi chú: 2']
```

### Problem Card #2 — Chốt sổ thu chi nhà trọ hằng tháng

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến kỳ thu tiền nhà trọ, tôi muốn tổng hợp tiền thuê, điện nước, phí phát sinh và công nợ từng phòng, để thu đúng tiền và theo dõi thu chi đầy đủ. |
| Actor | Chủ nhà trọ hoặc người quản lý thu tiền |
| Thời điểm / bối cảnh | Cuối tháng, trước khi gửi bảng tiền cho từng phòng |
| Quy trình hiện tại | 1. Tập hợp chỉ số điện nước đầu/cuối kỳ · 2. Kiểm tra đơn giá, tiền thuê và cách phân bổ phí · 3. Tính các khoản phải thu theo phòng · 4. Đối chiếu thanh toán, công nợ và chi phí vận hành · 5. Lập thông báo tiền và tổng hợp sổ thu chi |
| Bottleneck | Bước 4, đối chiếu thanh toán và công nợ theo phòng/kỳ: khoảng 10 phút (ước lượng) |
| Impact | Có nguy cơ thu thiếu, tính trùng hoặc bỏ sót nợ; khó giải thích khoản chênh lệch cho người thuê |
| Success metric | 30 → ≤15 phút/kỳ với cùng số phòng; không tính trùng, mọi thanh toán gắn đúng phòng/kỳ. Bấm giờ khi đủ chỉ số và chứng từ, kiểm lại bằng phép tính độc lập |
| Phương án không dùng AI | Bảng tính có chỉ số, đơn giá, tiền thuê, phí theo thỏa thuận, số đã trả và công nợ; tách chi phí vận hành khỏi khoản thu người thuê |
| Giả thuyết về AI (nếu có) | AI trích phòng, kỳ và số tiền từ chứng từ để người quản lý kiểm tra; công thức tính tiền và công nợ. Không tự đặt đơn giá hoặc xác nhận đã nhận tiền |
| Cảm nhận nhanh | Rule |

```text
HIỆN TẠI ƯỚC LƯỢNG — 30 phút/kỳ, cùng số phòng và chứng từ

[1 Tập hợp chỉ số: 5'] → [2 Kiểm đơn giá và phí: 3']
→ [3 Tính khoản phải thu: 7'] → [4 Đối chiếu thanh toán: 10'] ← BOTTLENECK giả thuyết
→ [5 Lập thông báo và sổ thu chi: 5']
```

### Problem Card #3 — Hiểu khái niệm khó khi research

| Trường | Nội dung |
|---|---|
| Job Story | Khi nghiên cứu một chủ đề mới có nhiều khái niệm khó, tôi muốn được giải thích bằng ngôn ngữ đơn giản và ví dụ cụ thể, để hiểu bản chất và vận dụng vào việc đang làm. |
| Actor | Người học hoặc dev nghiên cứu chủ đề mới |
| Thời điểm / bối cảnh | Khi tài liệu có thuật ngữ hoặc công thức vượt kiến thức nền |
| Quy trình hiện tại | 1. Xác định câu hỏi cần hiểu · 2. Đọc đoạn tài liệu liên quan · 3. Tra thuật ngữ và tìm cách diễn giải khác · 4. Tìm ví dụ rồi đối chiếu tài liệu gốc · 5. Tự giải thích và thử áp dụng |
| Bottleneck | Bước 3, tra thuật ngữ và tìm cách giải thích dễ hiểu: khoảng 8 phút/khái niệm (ước lượng) |
| Impact | Khoảng 25 phút/khái niệm theo kịch bản; dễ nhớ định nghĩa nhưng hiểu sai cách dùng |
| Success metric | 25 → ≤15 phút/khái niệm; tự giải thích đúng, nêu điều kiện áp dụng và làm được một ví dụ mới. Đo 3 lượt trước/sau với độ khó tương đương, đối chiếu tài liệu gốc |
| Phương án không dùng AI | Tài liệu nhập môn, bảng thuật ngữ, ví dụ có lời giải và trao đổi với người hướng dẫn |
| Giả thuyết về AI (nếu có) | AI giải thích đoạn tài liệu bằng lời đơn giản, ví dụ từng bước và điều kiện áp dụng theo kiến thức nền. Người học đối chiếu nguồn và tự làm ví dụ mới |
| Cảm nhận nhanh | Workflow |

```text
HIỆN TẠI ƯỚC LƯỢNG — 25 phút/khái niệm

[1 Xác định câu hỏi: 2'] → [2 Đọc đoạn tài liệu: 5']
→ [3 Tra thuật ngữ và cách diễn giải: 8'] ← BOTTLENECK giả thuyết
→ [4 Tìm ví dụ, đối chiếu nguồn: 5'] → [5 Tự giải thích và áp dụng: 5']
```

**AI phản biện card #1:**

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 15 phút và bước gom ghi chú 5 phút chỉ là ước lượng | Đồng ý | Ghi rõ số giả định; thêm cách bấm giờ trong 3 buổi họp |
| Chỉ đo tốc độ, thiếu kiểm tra chất lượng ghi chú | Đồng ý | Thêm điều kiện không bỏ sót hoặc ghi sai quyết định và đầu việc |
| Xác định bottleneck là hỏi lại người chủ trì sau họp | Không đồng ý | Giữ bước gom ghi chú là bottleneck giả thuyết; điểm chưa rõ được hỏi ngay trong họp |

---

## 4. Tôi đã tham gia phần nào

| Hoạt động | Tôi đã làm gì? | Kết quả |
|---|---|---|
| Pitch Problem Card | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Phản biện bài của bạn khác | Không có câu hỏi trực tiếp được ghi lại. | Không có bản ghi trong tài liệu hiện tại |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Kiểm chứng / research | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Quy trình nhóm | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |

---

## 5. Dùng AI

| Checkpoint | Dùng AI để làm gì? | Hữu ích ở đâu? | Sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm sau khi tự scan 4 ý | Bổ sung #5: bàn giao code | Đề xuất số liệu khi chưa đo | Giữ ý #5; ghi số liệu là ước lượng |
| CP2 Problem Card | Soạn nháp 3 card, vẽ quy trình và phản biện bằng vai PM hoài nghi | Chỉ ra metric thiếu chất lượng, baseline chưa đo và cần thử phương án đơn giản hơn | Xác định sai bottleneck là hỏi lại người chủ trì sau họp | Giữ bước gom ghi chú; thêm điều kiện chất lượng và cách đo thời gian |

---

## 6. Reflection


Phần trả lời trải nghiệm cá nhân không có trong bản nguồn; không coi là đã đáp ứng C4/C5.

**6.1. Tôi học được gì khi nghe top 3 của các bạn khác?**

**6.2. Nhóm nhận ra và xử lý solution-first thế nào?**

**6.3. Một lần tôi đổi ý sau phản biện?**

**6.4. Kiểm chứng có làm tôi bất ngờ không?**

**6.5. Điều khó nhất khi viết Problem Statement?**

**6.6. Nếu làm lại, tôi thay đổi điều gì?**

**6.7. Tự giải thích chuỗi problem → quy trình → metric → boundary → mức can thiệp → quyết định bằng 5–8 câu.**

## 7. Tài liệu tham khảo

- [Báo cáo nhóm và nguồn research](../team/group_report.md#10-tài-liệu-tham-khảo).
