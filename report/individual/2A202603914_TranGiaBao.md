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

Tôi chọn quan sát các công việc thường gặp khi nhận dự án website, làm rõ yêu cầu, phát triển và kiểm thử. Các mốc thời gian chưa có dữ liệu đo được sẽ ghi rõ là cần bổ sung thay vì ước lượng thành số liệu thực tế.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi khách gửi phản hồi sau mỗi lần demo website, tôi muốn tổng hợp các yêu cầu theo từng lần chỉnh sửa, để không bỏ sót lúc bàn giao. | Developer, khách hàng | Có công việc nhận feedback và sửa website trong dự án freelance; **cần đối chiếu** số lần/tuần và phút tổng hợp từ dự án cụ thể. |
| 2 | Tốn thời gian | Khi nhận brief website chưa rõ nghiệp vụ, tôi muốn xác định các yêu cầu còn thiếu trước khi báo giá, để tránh hiểu sai phạm vi. | Freelancer, khách hàng | Có công việc trao đổi yêu cầu và báo giá dự án; **cần đối chiếu** số lần phải hỏi lại và thời gian. |
| 3 | Đọc, tổng hợp nhiều thông tin | Khi kiểm thử một web app có nhiều vai trò người dùng, tôi muốn xác định đủ bước tái hiện lỗi và kết quả mong đợi, để người sửa có thể kiểm tra lại. | Tester, developer | Có bối cảnh kiểm thử web app; **cần đối chiếu** ticket/ảnh/video và thời gian lập báo cáo lỗi. |
| 4 | Pain từ người khác | Khi khách hỏi tiến độ dự án, tôi muốn có thông tin cập nhật theo từng hạng mục, để trả lời chính xác mà không phải kiểm lại mọi thay đổi. | Khách hàng, developer | Có công việc báo cáo tiến độ dự án; **cần đếm** số lần khách hỏi cập nhật từ tin nhắn thực tế. |
| 5 | Lặp lại | Khi nhận thông báo một lỗi đã sửa, tôi muốn biết những trường hợp cần kiểm tra lại, để không bỏ sót lỗi cũ sau mỗi lần cập nhật. | Tester, developer | Có công việc retest sau khi fix; **cần đo** số vòng retest và số ticket mở lại. |
| 6 | Tốn thời gian | Khi phải bàn giao website cho khách, tôi muốn có checklist các chức năng và tài khoản cần bàn giao, để tránh phải bổ sung nhiều lần. | Developer, khách hàng | [Kiểm tra các lần bàn giao, số đầu mục thiếu và thời gian bổ sung.] |
| 7 | Đọc, tổng hợp nhiều thông tin | Khi dự án thay đổi phạm vi giữa chừng, tôi muốn đối chiếu yêu cầu mới với phần việc đã thống nhất, để xác định đâu là chỉnh sửa và đâu là phát sinh. | Freelancer, PM, khách hàng | [Tìm phiên bản brief/hợp đồng và số lần thay đổi phạm vi thực tế.] |
| 8 | Pain từ người khác | Khi developer nhận bug report, họ muốn có đủ môi trường, bước thao tác và bằng chứng, để không phải hỏi lại tester. | Developer, tester | [Đếm các ticket từng bị yêu cầu bổ sung thông tin.] |

**Cách chọn:** Tôi ưu tiên những vấn đề có quy trình rõ và có thể đo bằng thời gian xử lý, số lượt hỏi lại hoặc số ticket. Các dòng #6–#8 là hướng mở rộng, chỉ giữ nếu tìm được tình huống thực tế tương ứng.

**Sử dụng công cụ hỗ trợ:** Tôi đã dùng AI để kiểm tra cách diễn đạt Job Story và phản biện danh sách. Chưa xem các gợi ý chưa kiểm chứng là bằng chứng thực tế. Ý tưởng xây một hệ thống tự quản lý toàn bộ dự án không được đưa vào danh sách vì đó là giải pháp quá rộng, không phải một pain cụ thể.

---

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp phản hồi chỉnh sửa website (#1) | Có actor, điểm bắt đầu/kết thúc rõ và có thể đối chiếu task thực tế | Mất bao lâu mỗi lần tổng hợp? Bao nhiêu feedback bị bỏ sót? |
| 2 | Làm rõ brief trước báo giá (#2) | Liên quan trực tiếp đến phạm vi công việc và trao đổi với khách | Thời gian chậm do thiếu brief hay do chờ phản hồi? |
| 3 | Viết bug report khi kiểm thử (#3) | Có đầu ra rõ là ticket với bước tái hiện và bằng chứng | Bước tái hiện hay bước viết ticket mới tốn thời gian nhất? |

### Problem Card #1 — Tổng hợp phản hồi chỉnh sửa website

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách gửi nhiều đợt feedback sau demo, tôi muốn theo dõi yêu cầu và trạng thái xử lý ở một nơi, để không bỏ sót hạng mục khi bàn giao. |
| Actor | Freelancer developer trực tiếp nhận yêu cầu và sửa website |
| Thời điểm / bối cảnh | Sau mỗi lần gửi bản demo cho khách xem và góp ý |
| Quy trình hiện tại | 1. Nhận phản hồi · 2. Đọc và tách từng yêu cầu · 3. Đối chiếu với feedback cũ · 4. Ghi đầu việc · 5. Chỉnh sửa website · 6. Kiểm tra và gửi khách xác nhận |
| Bottleneck | Bước 3 — đối chiếu phản hồi mới với các yêu cầu trước đó; **chưa có thời gian đo** |
| Impact | Có nguy cơ bỏ sót hoặc làm trùng yêu cầu, cần trao đổi lại trước bàn giao |
| Success metric | Baseline: [phút tổng hợp/đợt, số feedback sót]; target đề xuất: giảm ít nhất 25% thời gian mà số feedback sót không tăng; đo trên ít nhất 5 đợt chỉnh sửa tương đương |
| Phương án không dùng AI | Dùng một bảng task chung, đánh mã từng yêu cầu và cập nhật trạng thái |
| Giả thuyết về AI | Hỗ trợ tách yêu cầu từ đoạn phản hồi đã nhập và gợi ý các yêu cầu trùng; developer vẫn xác nhận |
| Cảm nhận nhanh | Rule trước; Workflow chỉ khi cách thủ công vẫn mất nhiều thời gian |

```text
HIỆN TẠI — tổng thời gian chưa đo

[1 Nhận feedback: ?'] → [2 Tách yêu cầu: ?']
→ [3 Đối chiếu yêu cầu cũ: ?']  ← BOTTLENECK CẦN KIỂM CHỨNG
→ [4 Ghi task: ?'] → [5 Chỉnh sửa: ?']
→ [6 Kiểm tra và xác nhận: ?']
```

### Problem Card #2 — Làm rõ brief trước báo giá

| Trường | Nội dung |
|---|---|
| Job Story | Khi brief dự án chưa đủ thông tin, tôi muốn làm rõ các luồng nghiệp vụ và phạm vi cần xây dựng, để ước lượng công việc và báo giá phù hợp. |
| Actor | Freelancer developer phụ trách trao đổi yêu cầu và báo giá |
| Thời điểm / bối cảnh | Khi nhận dự án mới, trước khi chốt báo giá và hợp đồng |
| Quy trình hiện tại | 1. Nhận brief · 2. Đọc và phân tích · 3. Ghi lại yêu cầu chưa rõ · 4. Hỏi khách · 5. Xác nhận phạm vi · 6. Ước lượng và báo giá |
| Bottleneck | Bước 3 — xác định thông tin còn thiếu; thời gian chờ khách ở bước 4 phải đo riêng |
| Impact | Báo giá có thể thiếu hạng mục, phải sửa nhiều lần hoặc phát sinh tranh luận khi triển khai |
| Success metric | Baseline: [phút phân tích/brief, lượt hỏi lại]; target đề xuất: giảm 20% thời gian phân tích mà số yêu cầu bị hiểu sai không tăng; đo từ ít nhất 3 brief |
| Phương án không dùng AI | Checklist discovery theo loại dự án, mẫu brief bắt buộc xác nhận |
| Giả thuyết về AI | Đánh dấu các câu mơ hồ, gợi ý câu hỏi làm rõ; không tự quyết định phạm vi |
| Cảm nhận nhanh | No AI / Rule; cân nhắc Workflow nếu brief đa dạng và quá nhiều thông tin |

```text
HIỆN TẠI — tách thời gian làm và thời gian chờ

[1 Nhận brief: ?'] → [2 Phân tích: ?']
→ [3 Tìm yêu cầu thiếu: ?']  ← BOTTLENECK CẦN KIỂM CHỨNG
→ [4 Gửi câu hỏi/chờ phản hồi: ? giờ]
→ [5 Xác nhận phạm vi: ?'] → [6 Lập báo giá: ?']
```

### Problem Card #3 — Viết bug report và tái kiểm thử

| Trường | Nội dung |
|---|---|
| Job Story | Khi phát hiện lỗi trên web app, tôi muốn ghi lại các bước tái hiện và bằng chứng rõ ràng, để developer sửa đúng lỗi và tester kiểm tra lại được. |
| Actor | Manual tester/QA kiểm thử chức năng web app |
| Thời điểm / bối cảnh | Khi kiểm thử trước bàn giao và sau các đợt sửa lỗi |
| Quy trình hiện tại | 1. Chạy test case · 2. Phát hiện lỗi · 3. Tái hiện lỗi · 4. Chụp ảnh/quay video · 5. Viết ticket · 6. Chuyển developer · 7. Retest |
| Bottleneck | Bước 3 — tái hiện lỗi, hoặc bước 5 — mô tả ticket; cần bấm giờ để xác định bước chính |
| Impact | Developer có thể phải hỏi lại, kéo dài vòng sửa và nghiệm thu |
| Success metric | Baseline: [phút/ticket; số ticket phải bổ sung thông tin]; target đề xuất: giảm 20% thời gian lập ticket và không tăng tỷ lệ ticket bị yêu cầu làm rõ; đo trên ít nhất 10 ticket |
| Phương án không dùng AI | Template cố định: môi trường, steps, expected, actual, bằng chứng và mức độ nghiêm trọng |
| Giả thuyết về AI | Tóm tắt ghi chú và log thành bản ticket để tester duyệt trước khi gửi |
| Cảm nhận nhanh | Rule trước; Workflow nếu khối lượng lỗi đủ lớn |

```text
HIỆN TẠI — tổng thời gian chưa đo

[1 Chạy case: ?'] → [2 Phát hiện lỗi: ?']
→ [3 Tái hiện lỗi: ?']  ← BƯỚC CẦN ĐO
→ [4 Lưu bằng chứng: ?'] → [5 Viết ticket: ?'] ← BƯỚC CẦN ĐO
→ [6 Gửi developer: ?'] → [7 Retest: ?']
```

### Card muốn pitch nhất

- **Card số:** 1 — Tổng hợp phản hồi chỉnh sửa website.
- **Vì sao:** Phạm vi tương đối gọn, dễ phân tách từng bước và có thể kiểm chứng qua lịch sử yêu cầu thay đổi.
- **Câu hỏi muốn nhóm phản biện:** Nếu dùng chung một bảng theo dõi feedback có mã yêu cầu và trạng thái, phần nào vẫn gây mất thời gian nhiều nhất?

### AI phản biện Problem Card #1

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa có thời gian baseline, nên chưa chứng minh đây là bottleneck lớn nhất | Đồng ý | Giữ thời gian chưa đo thay vì tự gán số; xác định cần bấm giờ qua các đợt feedback |
| Có thể chỉ cần một bảng task chung, chưa chứng minh cần AI | Đồng ý | Bổ sung phương án không AI và ưu tiên thử trước |
| Chỉ đo thời gian nhanh hơn thì chưa đủ | Đồng ý | Thêm chỉ số số yêu cầu bị bỏ sót vào success metric |

**Điểm cần xác minh sau phản biện:** Với Card #1, nếu dùng bảng task chuẩn đã giảm được phần lớn thời gian và không còn sót yêu cầu, không nên chọn AI chỉ để tăng độ phức tạp.

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
- [Bổ sung nguồn tài liệu thực tế sau khi xác minh]
