# Báo cáo cá nhân — Giang Thái Sơn

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: **Giang Thái Sơn**
- MSSV: **2A202603964**
- Email trường (không bắt buộc): *Không công khai*
- Tên nhóm: **VietnamAirline**
- Link repo nhóm: https://github.com/k1b1t0/K5-L3B-DAY02-VietnamAirline-DiscoveryProblemFraming
- Tài khoản GitHub: [son309](https://github.com/son309)
- Vai trò trong nhóm: **Khảo sát và phân tích vấn đề (CP1–CP2), hỗ trợ xây dựng quy trình trước/sau (CP5).**
- Bối cảnh khảo sát cá nhân: **Fresher AI Engineer mới vào công ty, cần onboarding, học công nghệ và tự xử lý task kỹ thuật.**

> **Phạm vi nguồn:** CP1–CP2 kế thừa bản nháp cá nhân trước đó; CP3–CP6 đối chiếu theo `group_report.md` mới của nhóm. Các con số chưa đo thực tế không được xem là baseline xác nhận. Đóng góp nào chưa có bằng chứng cá nhân được đánh dấu `[CẦN XÁC NHẬN]`.

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi mới vào công ty, tôi muốn nắm rõ quy trình onboarding và môi trường làm việc để sớm bắt đầu công việc được giao. | Fresher AI Engineer, mentor | **[CẦN ĐO]** Số phút tìm hướng dẫn onboarding; số lần phải hỏi mentor; link tài liệu/tin nhắn hỏi lại. |
| 2 | Lặp lại | Khi cần thiết lập lại môi trường phát triển, tôi muốn tìm đúng các bước cấu hình đã sử dụng để không phải lặp lại việc dò lỗi từ đầu. | Fresher AI Engineer | **[CẦN ĐO]** Số lần setup trong tuần; số phút dò lại câu lệnh; log lỗi môi trường. |
| 3 | Lặp lại | Khi chuẩn bị cập nhật công việc hằng ngày, tôi muốn nhớ lại các task và blocker đã xử lý để báo cáo ngắn gọn, không bỏ sót thông tin. | Fresher AI Engineer, team lead | **[CẦN ĐO]** Số phút chuẩn bị daily stand-up; số nguồn phải tìm lại (GitHub, chat, task board). |
| 4 | Tốn thời gian | Khi tiếp nhận dự án mới, tôi muốn hiểu kiến trúc hệ thống và các công nghệ đang sử dụng để có thể tự thực hiện task được giao. | Fresher AI Engineer, mentor | **[CẦN ĐO]** Số giờ đọc README/code; số lần hỏi về luồng xử lý; thời gian trước khi hoàn thành task đầu tiên. |
| 5 | Tốn thời gian | Khi gặp vấn đề kỹ thuật chưa biết cách xử lý, tôi muốn tìm được kiến thức và hướng dẫn phù hợp để tự giải quyết trước khi nhờ mentor. | Fresher AI Engineer, mentor | **[CẦN ĐO]** Phút tìm hiểu mỗi lỗi; số hướng đã thử; số ticket hoặc câu hỏi cần mentor hỗ trợ. |
| 6 | Tốn thời gian | Khi một thư viện hoặc phiên bản môi trường gây lỗi, tôi muốn xác định sự khác biệt giữa cấu hình thực tế và hướng dẫn để sửa đúng nguyên nhân. | Fresher AI Engineer, người review | **[CẦN ĐO]** Thời gian tìm lỗi phụ thuộc phiên bản; số lần cài lại/thử lại; log cài đặt. |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi được giao học một công nghệ mới, tôi muốn đối chiếu tài liệu chính thức và ví dụ triển khai để chọn nội dung cần học trước cho task hiện tại. | Fresher AI Engineer | **[CẦN ĐO]** Số trang/link đã đọc; số giờ nghiên cứu; ghi chú so sánh tài liệu. |
| 8 | Cần đọc, tổng hợp nhiều thông tin | Khi yêu cầu của một task được thảo luận ở nhiều nơi, tôi muốn tổng hợp đúng tiêu chí hoàn thành để tránh triển khai sai hoặc phải làm lại. | Fresher AI Engineer, team lead | **[CẦN ĐO]** Số thread/ticket cần đọc; số lần hỏi làm rõ; số PR phải sửa vì hiểu nhầm yêu cầu. |
| 9 | Pain từ người khác | Khi mentor hướng dẫn nhiều nhân viên mới, tôi muốn người học có thể tra cứu lại các giải thích đã được chia sẻ để mentor không phải trả lời lặp lại cùng câu hỏi. | Mentor, các Fresher | **[CẦN XÁC MINH VỚI MENTOR]** Số câu hỏi trùng nội dung/tuần; số phút giải đáp; thread hỏi đáp. |
| 10 | Pain từ người khác | Khi người kiểm thử báo một lỗi khó tái hiện, tôi muốn nhận đủ các bước và điều kiện phát sinh để phối hợp khắc phục nhanh hơn. | QA Engineer, Fresher AI Engineer | **[CẦN XÁC MINH VỚI QA]** Số ticket thiếu bước tái hiện; số lần trao đổi bổ sung; thời gian mở lại bug. |

**Nếu có dùng AI để gợi ý thêm:** ChatGPT hỗ trợ tổng hợp, phân loại và diễn đạt các Job Stories. Ba ý #1, #4 và #5 đã được trình bày trong bảng pitch CP3 của nhóm (theo `group_report.md`). Các ý còn lại là ứng viên trong bản scan cá nhân, chưa có bằng chứng thực tế.

- Ý được mang đi pitch ở CP3: **#1 (onboarding), #4 (kiến trúc dự án), #5 (tự xử lý lỗi)**.
- Các ý chưa đem pitch: **#2, #3, #6, #7, #8, #9, #10**; chưa có căn cứ để kết luận từng ý đã bị loại sau kiểm chứng.
- Bằng chứng/số đo riêng của CP1: **[CẦN BỔ SUNG TỪ TRẢI NGHIỆM HOẶC LOG THỰC TẾ]**.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | **Onboarding và thiết lập môi trường** (#1) | Actor rõ; có quy trình từ nhận tài liệu đến chạy được môi trường; bottleneck có thể đo theo phút tìm thông tin và số lần hỏi mentor. | Tài liệu thật sự thiếu hay Fresher chỉ chưa biết vị trí? Thời gian bao nhiêu? |
| 2 | **Hiểu kiến trúc dự án và kiến thức cần ưu tiên** (#4) | Gắn trực tiếp với thời gian bắt đầu task; có thể vẽ các bước đọc tài liệu, lần theo code, hỏi mentor. | Bước nghẽn là hiểu code, thiếu tài liệu hay chưa đủ nền tảng? |
| 3 | **Tự tìm cách giải quyết lỗi kỹ thuật** (#5) | Lặp lại trong quá trình học việc, có log/ticket để kiểm chứng, và so sánh được nhiều cách giải quyết. | Có bao nhiêu lỗi trùng lặp? Tài liệu đã đủ hay bản chất lỗi khác nhau? |

### Problem Card #1 — Onboarding và thiết lập môi trường

| Trường | Nội dung |
|---|---|
| Job Story | Khi mới vào công ty, tôi muốn nắm rõ quy trình onboarding và môi trường làm việc để sớm bắt đầu công việc được giao. |
| Actor | Fresher AI Engineer mới nhận việc; mentor hỗ trợ onboarding là người liên quan. |
| Thời điểm / bối cảnh | Những ngày đầu được cấp tài khoản, nhận repository, tài liệu và yêu cầu chạy project ở máy cá nhân. |
| Quy trình hiện tại (3–7 bước) | 1. Nhận thông tin và quyền truy cập; 2. Tìm tài liệu setup; 3. Cài dependencies/cấu hình; 4. Hỏi mentor những mục chưa rõ; 5. Kiểm tra chạy project thành công. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2: tìm đúng tài liệu setup trong nhiều nguồn**; **chưa có số liệu thực tế [CẦN ĐO]**. Cần xác minh liệu bottleneck có thật ở bước 2 thay vì bước cấu hình. |
| Impact (nếu không giải thì sao) | Chậm bắt đầu task đầu tiên, phụ thuộc mentor và có thể lặp lại câu hỏi đã được giải đáp. Chưa lượng hóa impact. |
| Success metric (baseline → target) | **Metric:** thời gian từ lúc bắt đầu tìm hướng dẫn đến khi chạy project thành công. **Baseline:** [CẦN BẤM GIỜ, chưa có]; **target đề xuất:** giảm ít nhất 30% so với baseline. Theo dõi thêm số câu hỏi lặp lại/tuần. |
| Phương án không dùng AI | Trang onboarding tập trung, checklist setup theo hệ điều hành, README có mục lỗi thường gặp và người phụ trách. |
| Giả thuyết về AI (nếu có) | Hỗ trợ tìm đoạn tài liệu phù hợp và giải thích lại bước setup từ nguồn nội bộ đã được duyệt, kèm link gốc; không tự chạy lệnh. |
| Cảm nhận nhanh | **Chưa biết** — ưu tiên thử No AI (checklist + cấu trúc tài liệu) trước khi cân nhắc Workflow có AI. |

Quy trình nháp hiện tại (**thời gian từng bước cần đo thực tế**):

```text
HIỆN TẠI — 5 bước (chưa bấm giờ)
[1 Nhận tài khoản, repository]
      → [2 Tìm tài liệu setup]  ← BOTTLENECK GIẢ ĐỊNH
      → [3 Cài đặt, cấu hình]
      → [4 Hỏi mentor khi vướng]
      → [5 Chạy thử và xác nhận]
```

### Problem Card #2 — Hiểu kiến trúc hệ thống và công nghệ dự án

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận dự án mới, tôi muốn hiểu kiến trúc hệ thống và các công nghệ đang sử dụng để có thể tự thực hiện task được giao. |
| Actor | Fresher AI Engineer mới được phân công vào codebase; mentor hoặc tech lead là người hướng dẫn. |
| Thời điểm / bối cảnh | Ngày đầu tiếp cận repository đã có sẵn, cần biết dữ liệu đi qua những module nào để sửa một chức năng. |
| Quy trình hiện tại (3–7 bước) | 1. Clone và mở repository; 2. Đọc README/tài liệu kiến trúc; 3. Lần theo entry point, API, module và luồng dữ liệu; 4. Hỏi mentor các điểm chưa rõ; 5. Xác nhận lại phạm vi của task được giao. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2: tổng hợp thông tin từ tài liệu kiến trúc phân tán**; **chưa có số liệu thực tế [CẦN ĐO]**. |
| Impact (nếu không giải thì sao) | Khó xác định file cần sửa, kéo dài thời gian thực hiện task đầu tiên và tăng số lần hỏi mentor. Chưa có số liệu kiểm chứng. |
| Success metric (baseline → target) | **Metric:** thời gian để Fresher giải thích được luồng xử lý liên quan đến task và xác định module cần sửa. **Baseline:** [CẦN ĐO]; **target đề xuất:** giảm ít nhất 30%; đối chiếu kết quả với review của mentor. |
| Phương án không dùng AI | Sơ đồ kiến trúc, README theo module, danh sách entry point, walkthrough ngắn và checklist học theo từng task. |
| Giả thuyết về AI (nếu có) | Hỗ trợ giải thích mối liên hệ giữa các module từ code/tài liệu được cấp quyền, kèm đường dẫn file và cảnh báo khi không đủ ngữ cảnh. |
| Cảm nhận nhanh | **Chưa biết** — thử No AI với tài liệu kiến trúc chuẩn hóa trước. |

Quy trình nháp hiện tại (**thời gian từng bước cần đo thực tế**):

```text
HIỆN TẠI — 5 bước (chưa bấm giờ)
[1 Mở repository]
      → [2 Đọc tài liệu kiến trúc]  ← BOTTLENECK GIẢ ĐỊNH
      → [3 Lần theo luồng code]
      → [4 Hỏi mentor khi cần]
      → [5 Xác định module cần sửa]
```

### Problem Card #3 — Tự xử lý vấn đề kỹ thuật trước khi hỏi mentor

| Trường | Nội dung |
|---|---|
| Job Story | Khi gặp vấn đề kỹ thuật chưa biết cách xử lý, tôi muốn tìm được kiến thức và hướng dẫn phù hợp để tự giải quyết trước khi nhờ mentor. |
| Actor | Fresher AI Engineer; mentor và người review khi có lỗi kéo dài. |
| Thời điểm / bối cảnh | Khi chạy project hoặc sửa một chức năng và gặp lỗi mới, chưa biết có hướng dẫn nội bộ tương ứng hay không. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc thông báo lỗi và log; 2. Tìm tài liệu, issue, câu trả lời trước đây; 3. Thử một số hướng khắc phục; 4. Hỏi mentor nếu chưa giải quyết; 5. Chạy lại và xác minh lỗi đã hết. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2: tìm đúng hướng dẫn và đối chiếu với lỗi hiện tại**; **chưa có số liệu thực tế [CẦN ĐO]**. |
| Impact (nếu không giải thì sao) | Mất thời gian thử sai, có nguy cơ lặp lại cách sửa đã thất bại, làm gián đoạn công việc hoặc tốn thời gian hỗ trợ của mentor. |
| Success metric (baseline → target) | **Metric:** thời gian từ lúc ghi nhận lỗi đến khi tìm được hướng xử lý hợp lý và xác minh kết quả. **Baseline:** [CẦN ĐO]; **target đề xuất:** giảm ít nhất 25%; theo dõi tỷ lệ lỗi được xử lý đúng mà không phát sinh lỗi mới. |
| Phương án không dùng AI | Chuẩn hóa bug report, FAQ lỗi phổ biến, lưu issue đã giải quyết có từ khóa và phiên bản môi trường. |
| Giả thuyết về AI (nếu có) | Tìm và tóm tắt các hướng giải quyết liên quan từ log và cơ sở tri thức; chỉ đề xuất bước kiểm tra, yêu cầu Fresher xác nhận trước khi áp dụng. |
| Cảm nhận nhanh | **Chưa biết** — ưu tiên tìm kiếm có cấu trúc, cân nhắc Workflow/RAG nếu tìm kiếm thường không đủ. |

Quy trình nháp hiện tại (**thời gian từng bước cần đo thực tế**):

```text
HIỆN TẠI — 5 bước (chưa bấm giờ)
[1 Đọc log, nhận diện triệu chứng]
      → [2 Tìm tài liệu và hướng xử lý]  ← BOTTLENECK GIẢ ĐỊNH
      → [3 Thử cách xử lý]
      → [4 Hỏi mentor nếu chưa giải quyết]
      → [5 Kiểm tra lại hệ thống]
```

### Card muốn pitch nhất

- **Card cá nhân ưu tiên trong bản nháp:** #2 — Hiểu kiến trúc hệ thống và công nghệ dự án. **Tại CP3, tôi đã đưa cả ba candidate #1, #2, #3 vào bảng pitch của nhóm.**
- **Vì sao (lập luận ban đầu):** Việc hiểu luồng code liên quan trực tiếp đến khả năng tự thực hiện task; có thể đo thời gian xác định module và mức độ phải hỏi mentor. **Chưa có bằng chứng phỏng vấn riêng.**
- **Câu hỏi muốn được phản biện (gợi ý, không phải câu hỏi đã nhận):** "Nếu có sơ đồ kiến trúc và walkthrough tốt, còn cần hệ thống hỗ trợ mới không?" 

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Cả 3 card chưa có baseline đo từ sự kiện thực; phút trong sơ đồ chỉ là giả định. | **[TỰ XÁC NHẬN]** | **Định hướng chỉnh:** bấm giờ một lần làm thật/tra log, thay con số minh họa trước khi nộp. |
| Card #1 chưa phân biệt tài liệu thiếu với tài liệu đã có nhưng khó tìm. | **[TỰ XÁC NHẬN]** | **Định hướng chỉnh:** kiểm tra thư mục onboarding hiện tại và hỏi mentor về tài liệu đang có. |
| Card #2 có thể bị lẫn giữa thiếu tài liệu và thiếu kiến thức nền. | **[TỰ XÁC NHẬN]** | **Định hướng chỉnh:** phỏng vấn Fresher về lần nhận task gần nhất, ghi từng bước vướng. |
| Card #3 có nguy cơ rộng vì các lỗi kỹ thuật rất khác nhau. | **[TỰ XÁC NHẬN]** | **Định hướng chỉnh:** thu hẹp vào một nhóm lỗi cụ thể, ví dụ lỗi cấu hình môi trường. |

> **Lưu ý:** Bảng trên là phản biện do AI đề xuất trong lần soạn bản này, **không phải bằng chứng rằng bạn đã nhận phản biện từ các thành viên** và không khẳng định bạn đã thực hiện các bước sửa. Hãy cập nhật cột "Đồng ý?" và "Đã sửa gì" theo hành động thật của mình.

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

**Vai trò tóm tắt:** Khảo sát và phân tích vấn đề (CP1–CP2), đóng góp ba candidate ở CP3 và hỗ trợ soạn thảo, đối chiếu quy trình Before/After (CP5).

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card (CP3) | Đề xuất 3 vấn đề dành cho Fresher AI Engineer: onboarding, hiểu kiến trúc dự án, tự xử lý lỗi kỹ thuật. | Được ghi tại candidate #13, #14, #15 trong bảng pitch nhóm. |
| Phản biện bài của bạn khác | **[CẦN XÁC NHẬN]** Câu hỏi tôi thực sự đã đặt và người nhận phản biện. | Chưa có tên người hỏi hoặc câu hỏi của tôi trong bảng pitch nhóm. |
| Nhận phản biện | AI phản biện ba Problem Cards cá nhân về baseline và phạm vi vấn đề. **[CẦN XÁC NHẬN]** phản biện từ đồng đội và thay đổi tôi đã thực sự làm. | Có danh sách điểm yếu cần xác minh, chưa nhận là đã đo hay sửa xong. |
| Gom cluster / cây OST (CP3) | Ba candidate của tôi thuộc nhóm **B — Tìm kiếm** trong kết quả phân cụm; **[CẦN XÁC NHẬN]** vai trò trực tiếp khi nhóm gom cluster. | Liên hệ vấn đề tìm tài liệu của Fresher với khó khăn tìm lại thread cũ trên Discord. |
| Chọn candidate problem (CP3) | Tham gia quá trình hội tụ theo báo cáo nhóm; **[CẦN XÁC NHẬN]** phiếu bầu hoặc ý kiến cá nhân của tôi. | Nhóm chọn **tìm lại câu trả lời coach trên Discord (29 điểm)**; candidate onboarding của tôi đạt **23 điểm**, không được chọn. |
| Kiểm chứng / research (CP4) | Đối chiếu phần khảo sát và research của nhóm với vấn đề đã chọn; **[CẦN XÁC NHẬN]** tôi có trực tiếp phỏng vấn hoặc nghiên cứu nguồn nào không. | Báo cáo nhóm ghi nhận **2 cuộc phỏng vấn**, có tín hiệu học viên mất thời gian tìm hướng dẫn/chờ coach. |
| Quy trình nhóm (CP5) | Soạn và hiệu chỉnh bản mô tả As-Is/To-Be, bảng bước có actor/input/output, thời gian, handoff, boundary, fallback và bảng Before/After để đối chiếu với nhóm. | Quy trình trước có **4 bước chính, thêm 2 bước nếu cần hỗ trợ**; tương lai **3 bước, khoảng 8 phút mục tiêu**; học viên vẫn tự kiểm tra và áp dụng. |
| Problem Statement (CP5–CP6) | Đối chiếu bottleneck, impact, metric và boundary với quy trình CP5; **[CẦN XÁC NHẬN]** có trực tiếp sửa bản Problem Statement của nhóm không. | Nhóm dùng mốc sơ bộ **~15 phút/lần** và đặt mục tiêu **dưới 3 phút/lần**; v1 bổ sung chỉ số hỏi lại coach và tỷ lệ bản tóm tắt bị bỏ. |
| Mức can thiệp AI (CP6) | Tìm hiểu phân biệt Rule/Search, AI và Human-in-the-Loop trong quy trình; **[CẦN XÁC NHẬN]** mức độ tham gia quyết định. | Nhóm chọn **Workflow**: tìm thread → AI tóm tắt có dẫn nguồn → học viên kiểm và áp dụng. |
| Quyết định (CP6) | Nắm phương án và ngưỡng dừng của báo cáo nhóm; **[CẦN XÁC NHẬN]** ý kiến cá nhân tại buổi chốt. | Quyết định chung: **Go, pilot phạm vi hẹp trong 2 tuần với 5–10 học viên**. |

**Lưu ý:** Kết quả chung của nhóm không đồng nghĩa tôi trực tiếp thực hiện mọi hạng mục. Những đóng góp chưa được ghi lại trong tài liệu/trao đổi cần tự xác nhận trước khi nộp.

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ ChatGPT hỗ trợ xây dựng và diễn đạt 10 candidate theo 4 lăng kính. | Làm rõ Job Story và actor. | Không tự có chứng cứ thời gian/tần suất. | Giữ 3 candidate được đưa lên bảng pitch nhóm; cần bổ sung bằng chứng thực tế cho từng vấn đề. |
| CP2 Problem Card | Nhờ ChatGPT cấu trúc 3 cards, quy trình, bottleneck, metric và phản biện. | Nêu được bước nghẽn và hướng kiểm chứng. | Các mốc thời gian nháp trước đây không phải số đo thật; phạm vi lỗi kỹ thuật còn rộng. | Loại các phút giả định khỏi sơ đồ cá nhân; để `[CẦN ĐO]`, phân biệt giả thuyết với kết luận. |
| CP4 Research | **[CẦN XÁC NHẬN]** Tôi có trực tiếp dùng AI cho research không. | Có thể hỗ trợ so sánh Discord Search, Forum và bot hỏi đáp. | AI không thay thế phỏng vấn hoặc bằng chứng thực địa. | Chỉ giữ số liệu phỏng vấn được báo cáo nhóm ghi nhận; không tự nhận đã phỏng vấn. |
| CP5 Quy trình | Nhờ ChatGPT hỗ trợ soạn ASCII, bảng Before/After và đối chiếu với báo cáo nhóm. | Phân biệt Rule/Search – AI – con người, boundary và fallback. | Dễ nhầm 15 phút tìm/đọc thread với tổng thời gian xử lý; dễ tự đặt mốc chưa đo. | Tách metric tìm hướng dẫn khỏi tổng quy trình; giữ thời gian mục tiêu ~8 phút và ghi rõ chưa đo đầy đủ baseline. |
| CP5–6 Problem Statement | Nhờ AI hỗ trợ kiểm tra tính nhất quán giữa quy trình, bottleneck, metric và boundary. | Gợi ý phản biện về thiếu bước áp dụng và nguồn hướng dẫn lỗi thời. | Chỉ giảm thời gian chưa chứng minh câu trả lời đúng hoặc hữu ích. | Dựa trên v1 của nhóm: bổ sung đo hỏi lại coach, tỷ lệ bản tóm tắt bị bỏ và link thread gốc. |
| CP6 Mức can thiệp / quyết định | **[CẦN XÁC NHẬN]** phần tôi trực tiếp dùng AI. | Hỗ trợ phân biệt No AI, Rule, Workflow, Agent. | AI có thể đề xuất Agent quá rộng so với bài lab. | Theo quyết định nhóm: Workflow có HITL, pilot 2 tuần và ngưỡng dừng an toàn. |

---

## 6. Reflection (CP7)

> **Phần này phải do Giang Thái Sơn tự viết bằng trải nghiệm thật, không nhờ AI viết thay.** Theo mẫu: tối thiểu **200 từ cho tổng nội dung 6.1–6.6** (không tính 6.7). Nội dung dưới đây để trống để tự hoàn thành.

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

[TỰ VIẾT TỪ TRẢI NGHIỆM THẢO LUẬN]

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

[TỰ VIẾT]

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

[TỰ VIẾT — NÊU PHẢN BIỆN THẬT, KHÔNG SUY ĐOÁN]

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

[TỰ VIẾT]

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

[TỰ VIẾT]

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

[TỰ VIẾT]

**6.7. Hiểu bài:** Giải thích bằng **5–8 câu, không nhìn tài liệu**, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

[TỰ VIẾT THEO CÁCH HIỂU CỦA BẠN]

---

## 7. Tài liệu tham khảo

- Báo cáo nhóm: [`report/team/group_report.md`](../team/group_report.md) — các mục CP3–CP6.
- Bằng chứng phỏng vấn của nhóm: [`report/assets/cp4-interview-snapshot-1.md`](../assets/cp4-interview-snapshot-1.md) và [`report/assets/cp4-interview-snapshot-2.md`](../assets/cp4-interview-snapshot-2.md) — liên kết được dẫn trong báo cáo nhóm, cần kiểm tra file có tồn tại trong repo.
- [Discord — How to Use Search](https://support.discord.com/hc/en-us/articles/115000468588-How-to-Use-Search-on-Discord) — nguồn research nêu trong báo cáo nhóm.
- [Discord Developers — Bots](https://docs.discord.com/developers/bots/overview) — nguồn research nêu trong báo cáo nhóm.
- Hướng dẫn lab: [`docs/01-worksheet.md`](../../docs/01-worksheet.md), [`docs/02-deliverable-example.md`](../../docs/02-deliverable-example.md) và [`CHECKPOINTS.md`](../../CHECKPOINTS.md).
