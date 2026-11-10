# Báo cáo cá nhân — MSSV_NguyenGiaBao

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: NGUYỄN GIA BẢO
- MSSV: 2A202603647
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:
- Link repo nhóm:

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị đi học mỗi sáng, tôi muốn biết ngay hôm nay học giờ nào, phòng nào, để không đến muộn hay đi sai phòng. | Sinh viên | 2–3 phút/lần, hằng ngày. |
| 2 | Tốn thời gian | Khi ứng tuyển một vị trí mới, tôi muốn biết CV cần sửa chỗ nào cho khớp JD, để tăng cơ hội qua vòng lọc CV. | Người tìm việc | 2 lần/tuần, khoảng 30–45 phút mỗi lần xem và sửa. |
| 3 | Lặp lại | Khi người bán hoặc người mua phế liệu hỏi về giá, cách đăng tin hay thu gom, nhân viên GRAC muốn trả lời đúng và nhanh, để không mất giao dịch ngoài giờ. | Nhân viên GRAC | Hằng ngày, 3–5 phút mỗi lần research vấn đề và trả lời. |
| 4 | Tốn thời gian | Khi ôn luyện thi chứng chỉ tiếng Anh, tôi muốn biết đề nào mình chưa làm, để không làm trùng đề và tập trung vào dạng bài còn yếu. | Người học | 8 phút/ngày cho mỗi lần tìm đề mới phù hợp. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi sắp bán rau củ quả, tôi muốn có tổng hợp, báo cáo giá từ nhiều nguồn, để buôn bán đúng giá thị trường. | Nông dân | 2 tháng/lần, mỗi lần 10–15 phút để tổng hợp và xác thực thông tin. |
| 6 | Pain từ người khác | Khi nhóm chia việc qua chat, tôi muốn biết task của mình là gì, hạn khi nào, đầu ra cần gì, để không làm trùng hoặc làm sai việc. | Cả team | 10–12 câu hỏi về phân công/deadline/link mỗi tuần, đếm trong chat nhóm. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Giữ #6 (phân công trong nhóm):** bù cho lăng kính "Pain từ người khác" mà bản tự scan còn thiếu, và có bằng chứng đếm được ngay trong chat nhóm.
- **Bỏ "dev mới hỏi lại cách setup Lavatu":** dự án ít người mới vào nên tần suất thấp.
- **Bỏ "kiểm duyệt tin đăng sai danh mục trên Lavatu":** chưa có số liệu, trùng actor với #3.
- **Bỏ "viết update 2 tuần/lần cho mentor":** tần suất thấp, impact nhỏ.
- **Không giữ thành dòng riêng "đọc JD để quyết định có nộp không":** chuyển thành một giả định cần kiểm chứng cho card Sửa CV (bottleneck thật có thể nằm ở bước này).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Sửa CV theo JD (#2) | Tốn nhiều thời gian nhất (≈ 60–90 phút/tuần), quy trình rõ ràng, nghẽn ở bước sửa bullet. | Bước nghẽn thật là sửa CV hay quyết định có nộp không? |
| 2 | Phân công trong nhóm (#6) | Bằng chứng đếm được, pain thật, nhiều người gặp. | Số liệu mới đếm trong 1 nhóm, 1 tuần. |
| 3 | CSKH GRAC (#3) | Actor là doanh nghiệp thật, xảy ra hằng ngày. | Dữ liệu khó truy cập và phạm vi dễ bị quá rộng. |

---

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi ứng tuyển một vị trí mới, tôi muốn biết CV cần sửa chỗ nào cho khớp JD, để tăng cơ hội qua vòng lọc CV. |
| Actor | Sinh viên năm 3, năm 4 và những người đang tìm việc. |
| Thời điểm / bối cảnh | Khi thấy JD mới trên các nền tảng tuyển dụng (ITviec, LinkedIn…), thường vào buổi tối, trước hạn nộp. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc JD.<br>2. Đối chiếu yêu cầu với kỹ năng/project của mình.<br>3. Chọn project, viết lại bullet, thêm keyword.<br>4. Chỉnh layout, xuất PDF.<br>5. Nộp. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (viết lại bullet), khoảng 15–20 phút, phải viết lại từ đầu cho mỗi JD. |
| Impact (nếu không giải thì sao) | 2 lần/tuần × 30–45 phút ≈ 60–90 phút/tuần; khoảng 10 vị trí đã đánh giá hoặc nộp trong 3 tháng. Nếu không sửa CV theo JD thì CV chung chung, dễ trượt vòng lọc. |
| Success metric (baseline → target) | Baseline: 30–45 phút/JD → Target: < 15 phút/JD, tỷ lệ được gọi phỏng vấn không giảm. |
| Phương án không dùng AI | CV gốc + kho bullet viết sẵn theo nhóm (RAG, Agent, Web) + checklist keyword: rút ngắn bước 3, nhưng vẫn phải tự đối chiếu JD. |
| Giả thuyết về AI (nếu có) | AI đối chiếu JD với kho bullet, đề xuất bullet và keyword còn thiếu; tôi tự chọn và sửa trước khi nộp. |
| Cảm nhận nhanh | **Workflow** |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 30–45 phút/JD

[1 Đọc JD: 10']
      │
      ▼
[2 Đối chiếu kỹ năng/project: 10']
      │
      ▼
[BOTTLENECK: 3 Viết lại bullet + thêm keyword] (15–20')
      │
      ▼
[4 Chỉnh layout + xuất PDF: 5']
      │
      ▼
[5 Nộp: 1']
```

---

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhóm chia việc qua chat, tôi muốn biết task của mình là gì, hạn khi nào, đầu ra cần gì, để không làm trùng hoặc làm sai việc. |
| Actor | Thành viên nhóm project (người hỏi lại) và trưởng nhóm/người được hỏi (người phải trả lời lại). |
| Thời điểm / bối cảnh | Trong chat nhóm (Zalo/Discord) khi làm project; tin chia việc bị trôi giữa các tin thảo luận khác. |
| Quy trình hiện tại (3–7 bước) | 1. Trưởng nhóm chia việc trong chat.<br>2. Tin nhắn chia việc trôi đi giữa các tin thảo luận.<br>3. Thành viên hỏi lại "ai làm phần này?", "deadline bao giờ?".<br>4. Chờ người khác tìm lại tin cũ hoặc giải thích lại.<br>5. Thành viên bắt đầu làm task. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 (chờ và tìm lại thông tin), khoảng 5–15 phút mỗi lần hỏi. |
| Impact (nếu không giải thì sao) | 10–12 câu hỏi lại/tuần, làm gián đoạn cả người hỏi lẫn người trả lời; dễ làm trùng hoặc làm sai task. |
| Success metric (baseline → target) | Baseline: 10–12 câu hỏi lại/tuần → Target: < 3 câu/tuần. |
| Phương án không dùng AI | Bảng phân công ghim trong nhóm (Notion/Google Sheet) với 4 cột cố định: người làm, việc, hạn, đầu ra; mỗi lần chia việc dùng chung một mẫu tin nhắn. |
| Giả thuyết về AI (nếu có) | Chưa cần AI. Thử phương án không dùng AI trước; chỉ khi bảng không được cập nhật đều mới cân nhắc AI trích task từ tin nhắn chat. |
| Cảm nhận nhanh | **No AI / Rule** |

Quy trình nháp hiện tại:

```text
[Trưởng nhóm chia việc trong chat]
      │
      ▼
[Tin chia việc trôi giữa các tin thảo luận]
      │
      ▼
[Thành viên hỏi lại phân công/deadline/link] (1')
      │
      ▼
[BOTTLENECK: Chờ người khác tìm lại tin cũ / giải thích lại] (5–15')
      │
      ▼
[Thành viên bắt đầu làm task]
```

---

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi người bán hoặc người mua phế liệu hỏi về giá, cách đăng tin hay thu gom, nhân viên GRAC muốn trả lời đúng và nhanh, để không mất giao dịch ngoài giờ. |
| Actor | Nhân viên vận hành GRAC (primary), người dùng sàn Lavatu (secondary). |
| Thời điểm / bối cảnh | Khi khách nhắn qua kênh hỗ trợ của sàn Lavatu, kể cả ngoài giờ làm việc. |
| Quy trình hiện tại (3–7 bước) | 1. Nhận tin nhắn của khách.<br>2. Phân loại câu hỏi (giá / đăng tin / thu gom).<br>3. Tra giá hoặc chính sách.<br>4. Soạn câu trả lời và gửi. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (tra giá/chính sách), 3–5 phút mỗi lần; ngoài giờ không có ai trả lời. |
| Impact (nếu không giải thì sao) | Khách phải chờ, có thể bỏ giao dịch hoặc chuyển sang kênh khác; số tin nhắn/ngày: ___. |
| Success metric (baseline → target) | Baseline: thời gian phản hồi 7 phút → Target: < 5 phút. |
| Phương án không dùng AI | Bộ FAQ + mẫu trả lời nhanh (quick reply) + bảng giá tham khảo công khai trên web. |
| Giả thuyết về AI (nếu có) | AI soạn câu trả lời dựa trên FAQ và bảng giá; nhân viên duyệt trước khi gửi. Ngoài giờ AI chỉ trả lời các câu có trong FAQ, câu hỏi chốt giá thì chuyển cho nhân viên. |
| Cảm nhận nhanh | **Workflow** |

Quy trình nháp hiện tại:

```text
[Khách nhắn hỏi giá / đăng tin / thu gom]
      │
      ▼
[Nhân viên phân loại câu hỏi] (1')
      │
      ▼
[BOTTLENECK: Tra giá / chính sách] (3–5') — ngoài giờ: không ai trả lời
      │
      ▼
[Soạn câu trả lời + gửi] (1–2')
```

---

### Card muốn pitch nhất

- **Card số:** Card #1 (Sửa CV theo JD)
- **Vì sao:** Tốn nhiều thời gian nhất trong 3 card (≈ 60–90 phút/tuần), quy trình rõ ràng, và rất nhiều bạn cùng khóa đang săn thực tập nên dễ phỏng vấn kiểm chứng.
- **Câu hỏi muốn nhóm phản biện:**
  1. Bottleneck thật là bước sửa bullet, hay là bước quyết định có nên nộp vị trí đó không?
  2. Các công cụ có sẵn (ChatGPT, Jobscan, Teal…) đã giải phần lớn bài toán chưa? Nếu rồi thì còn bỏ trống bước nào?

---

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 30–45 phút chỉ dựa trên trí nhớ. | Đồng ý | Bấm giờ thật ở lần sửa CV tiếp theo: 25 phút. |
| Bottleneck thật có thể là bước quyết định có nộp hay không, chứ chưa chắc là bước sửa CV. | Đồng ý một phần | Đưa vào danh sách giả định cần kiểm chứng ở CP4. |
| Gợi ý để AI tự viết toàn bộ CV rồi tự nộp. | Không đồng ý | Giữ boundary: tôi duyệt trước khi nộp, AI không được thêm kỹ năng mà tôi không có. |

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
| CP1 Scan | Góp ý Job Story tự viết; gợi ý thêm vấn đề theo 4 lăng kính. | Chỉ ra Job Story bị cụt/thiếu vế "để…", cột dấu hiệu thiếu tần suất, thiếu lăng kính "Pain từ người khác". | Một số gợi ý chưa có số liệu, tần suất thấp hoặc trùng actor. | Chỉ giữ 1/5 gợi ý (#6) và tự đếm số câu hỏi trong chat nhóm làm bằng chứng. |
| CP2 Problem Card | Chọn top 3, soạn card theo format, đóng vai PM hoài nghi phản biện. | Phát hiện bottleneck có thể nằm ở bước quyết định nộp; nhắc phương án không dùng AI cho card #2. | Số phút từng bước do AI chia ra từ tổng thời gian, chưa phải số đo thật. | Giữ boundary "tôi duyệt trước khi nộp"; không chấp nhận gợi ý để AI tự nộp CV. |
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
