# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Thị Thùy Dung
- MSSV: 2A202603552
- Email trường (không bắt buộc, repo có thể để public): 26ai.dungntt@vinuni.edu.vn
- Tên nhóm: VuQuangThai
- Link repo nhóm: https://github.com/vuThai05/K5-L3A-DAY02-VuQuangThai-2A202603545-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại, tốn thời gian |Khi nghiên cứu một bài toán nghiệp vụ y tế mới, tôi muốn tìm được các nguồn thông tin đầy đủ và đáng tin cậy, để không phải tìm kiếm lặp đi lặp lại trên nhiều nền tảng. | BA, Researcher | Số lần tìm kiếm/chủ đề; thời gian tìm tài liệu; số nguồn phải kiểm tra. |
| 2 |Tốn thời gian, tổng hợp nhiều thông tin |Khi phân tích các hệ thống HIS/EHR/AI Agent trên thị trường, tôi muốn xác định và so sánh điểm mạnh, điểm yếu của từng hệ thống theo các tiêu chí thống nhất, để có căn cứ đánh giá sản phẩm và xác định khoảng trống thị trường. | BA, PO,PM |Thời gian phân tích/hệ thống; số hệ thống cần so sánh; số nhận định chưa có bằng chứng. |
| 3 |Lặp lại |Khi tham gia chương trình AI thực chiến, tôi muốn nộp daily standup đúng  thời hạn để tích lũy EXP trong quá trình học tập | Sinh viên tham gia học tập | Mỗi ngày trong quá trình tham gia học tập |
| 4 | Pain từ người khác | Khi cả team nhận được báo cáo phân tích nghiệp vụ từ tôi, họ muốn hiểu nghiệp vụ để tiến hành build MVP | Backend, Frontend và AI Engineer | Một buổi thảo luận trước mỗi lần nhận được thông tin từ tôi |
| 5 | Lặp lại | Khi quá quá nhiều lịch họp thay đổi linh hoạt mỗi tuần, tôi muốn sắp xếp lịch được thông báo từ các kênh rời rạc vào 1 kênh thông báo duy nhất để không bị bỏ quên bất kỳ lịch họp nào | Team | Mỗi tuần 1 lần vào chủ nhật |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.
- Giữ lại ý "Khi phân tích các hệ thống HIS/EHR/AI Agent trên thị trường, tôi muốn xác định và so sánh điểm mạnh, điểm yếu của từng hệ thống theo các tiêu chí thống nhất, để có căn cứ đánh giá sản phẩm và xác định khoảng trống thị trường." vì đây là vấn đề do tôi tự nghĩ, AI chỉ format lại vấn đề cho rõ ràng hơn.
- Bỏ các ý liên quan trực tiếp đến hoạt động survey cho project vì hiện tại nhóm chưa kết luận được pain point.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tìm kiếm và xác minh nguồn thông tin nghiên cứu y tế (#1)| Actor rõ (BA), tần suất cao, quy trình lặp lại, có thể đo thời gian tìm kiếm và kiểm chứng nguồn.| Thời gian thực tế mất bao lâu? Bao nhiêu phần trăm nguồn không phù hợp? |
| 2 | Phân tích điểm mạnh, điểm yếu của các hệ thống HIS/EHR/AI Agent (#2)| Phù hợp trực tiếp với công việc nghiên cứu thị trường của BA, nhiều bước đọc và tổng hợp tài liệu, có đầu ra cụ thể.| Có đủ dữ liệu công khai để đánh giá khách quan từng hệ thống không?|
| 3 | Tổng hợp và theo dõi lịch họp thay đổi (#5)| Actor rõ (thành viên team), quy trình dễ quan sát, bottleneck có thể đo, phù hợp triển khai thử nghiệm nhỏ. |Team có thường xuyên bỏ sót hoặc nhầm lịch họp không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nghiên cứu một bài toán nghiệp vụ y tế mới, tôi muốn tìm được các nguồn thông tin đầy đủ và đáng tin cậy, để không phải tìm kiếm lặp đi lặp lại trên nhiều nền tảng. |
| Actor | Business Analyst phụ trách nghiên cứu nghiệp vụ trong team phát triển AI Agent lĩnh vực y tế.|
| Thời điểm / bối cảnh | Khi bắt đầu nghiên cứu một chủ đề y tế mới, chuẩn bị phân tích nghiệp vụ hoặc tìm hiểu các hệ thống hiện có trên thị trường.|
| Quy trình hiện tại (3–7 bước) | 1. Xác định chủ đề và từ khóa tìm kiếm. 2. Tìm kiếm trên Google, Google Scholar, website bệnh viện, tài liệu sản phẩm. 3. Mở và đọc từng nguồn. 4. Xác minh độ tin cậy, thời điểm công bố và tính liên quan. 5. Đối chiếu các nguồn. 6. Ghi chép và tổng hợp.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: Đọc, chọn lọc và xác minh nguồn thông tin, ước lượng 45 phút/lần nghiên cứu.|
| Impact (nếu không giải thì sao) | 	Ước lượng 120 phút/chủ đề. Nếu nghiên cứu 3 chủ đề/tuần, tổng cộng khoảng 360 phút/tuần cho một BA.|
| Success metric (baseline → target) | Giảm thời gian nghiên cứu từ 120 xuống dưới 60 phút/chủ đề, đồng thời không giảm tỷ lệ thông tin quan trọng có nguồn kiểm chứng.|
| Phương án không dùng AI | Danh mục nguồn uy tín, bộ từ khóa chuẩn theo chủ đề, checklist đánh giá nguồn và thư viện tài liệu nghiên cứu dùng chung.|
| Giả thuyết về AI (nếu có) | AI có thể hỗ trợ tìm kiếm, sàng lọc, đối chiếu thông tin và xác định nguồn liên quan; BA vẫn kiểm chứng bằng tài liệu gốc.|
| Cảm nhận nhanh | Workflow / Agent — cần kiểm chứng xem mức độ tự chủ có thực sự cần thiết. |

Quy trình nháp hiện tại:

```text
flowchart TD
    A["1. Xác định chủ đề và từ khóa<br/>10 phút"]
    B["2. Tìm kiếm trên nhiều nền tảng<br/>20 phút"]
    C["3. Đọc và chọn lọc nguồn<br/>25 phút"]
    D["4. Xác minh độ tin cậy<br/>20 phút"]
    E["5. Đối chiếu thông tin giữa các nguồn<br/>20 phút"]
    F["6. Ghi chép và tổng hợp kết quả<br/>25 phút"]

    A --> B --> C --> D --> E --> F

    classDef normal fill:#E8F1FF,stroke:#3675C5,color:#173A66
    classDef bottleneck fill:#FFE6E6,stroke:#D64545,color:#922020,stroke-width:2px

    class A,B,E,F normal
    class C,D bottleneck
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi phân tích các hệ thống HIS/EHR/AI Agent trên thị trường, tôi muốn xác định và so sánh điểm mạnh, điểm yếu của từng hệ thống theo các tiêu chí thống nhất, để có căn cứ đánh giá sản phẩm và xác định khoảng trống thị trường. |
| Actor | BA phụ trách nghiên cứu thị trường và phân tích sản phẩm; PO/PM sử dụng kết quả để định hướng sản phẩm.|
| Thời điểm / bối cảnh | Khi team nghiên cứu giải pháp y tế hiện có, đánh giá đối thủ hoặc xác định phạm vi chức năng cho MVP.|
| Quy trình hiện tại (3–7 bước) | 1. Xác định các hệ thống cần nghiên cứu. 2. Xây dựng tiêu chí đánh giá. 3. Tìm tài liệu và thông tin sản phẩm. 4. Đọc và trích xuất thông tin về chức năng. 5. So sánh điểm mạnh, điểm yếu. 6. Xác minh và tổng hợp báo cáo.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: Đọc tài liệu và trích xuất bằng chứng về chức năng của từng hệ thống, ước lượng 60 phút/hệ thống.|
| Impact (nếu không giải thì sao) | Ước lượng 150 phút/hệ thống; khi nghiên cứu 4 hệ thống mất khoảng 600 phút (10 giờ), chưa tính thời gian họp review.|
| Success metric (baseline → target) | Giảm thời gian phân tích từ 150 xuống dưới 90 phút/hệ thống; ít nhất 90% nhận định về chức năng có nguồn bằng chứng hoặc được đánh dấu chưa xác minh.|
| Phương án không dùng AI | Bộ tiêu chí benchmarking chuẩn, bảng so sánh cố định, danh mục tài liệu sản phẩm và quy tắc phân loại mức độ xác thực của thông tin.|
| Giả thuyết về AI (nếu có) | AI hỗ trợ trích xuất thông tin từ tài liệu sản phẩm, đối chiếu các tiêu chí và xác định điểm khác biệt; BA chịu trách nhiệm kiểm chứng các kết luận.|
| Cảm nhận nhanh | Workflow / Agent — cần xem có phải truy cập và đối chiếu nhiều nguồn động hay không. |


Quy trình nháp hiện tại:

```text
flowchart TD
    A["1. Xác định hệ thống nghiên cứu<br/>10 phút"]
    B["2. Xây dựng tiêu chí đánh giá<br/>15 phút"]
    C["3. Tìm kiếm tài liệu sản phẩm<br/>25 phút"]
    D["4. Đọc và trích xuất thông tin<br/>60 phút - BOTTLENECK"]
    E["5. So sánh điểm mạnh, điểm yếu<br/>25 phút"]
    F["6. Xác minh và tổng hợp báo cáo<br/>15 phút"]

    A --> B --> C --> D --> E --> F

    classDef normal fill:#E8F1FF,stroke:#3675C5,color:#173A66
    classDef bottleneck fill:#FFE6E6,stroke:#D64545,color:#922020,stroke-width:2px

    class A,B,C,E,F normal
    class D bottleneck
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi có quá nhiều lịch họp thay đổi linh hoạt mỗi tuần, tôi muốn tập hợp thông báo từ các kênh rời rạc vào một nơi dễ theo dõi, để không bỏ quên bất kỳ lịch họp nào. |
| Actor | Thành viên team dự án AI, bao gồm BA, Backend, Frontend, AI Engineer và PM.|
| Thời điểm / bối cảnh | Trong tuần làm việc, đặc biệt khi chuẩn bị lịch cho tuần tiếp theo vào Chủ nhật hoặc khi có thay đổi đột xuất.|
| Quy trình hiện tại (3–7 bước) | 1. Kiểm tra các kênh thông báo. 2. Đọc và xác định lịch họp mới. 3. Đối chiếu các thông báo thay đổi. 4. Tổng hợp lịch họp trong tuần. 5. Kiểm tra trùng lịch. 6. Theo dõi và cập nhật thông báo phát sinh.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Đối chiếu các thông báo thay đổi để xác định thời gian họp cuối cùng, ước lượng 15 phút/tuần.|
| Impact (nếu không giải thì sao) | Ước lượng 50 phút/người/tuần cho việc kiểm tra và tổng hợp lịch. Nếu 5 thành viên cùng thực hiện, tổng cộng khoảng 250 phút/tuần.|
| Success metric (baseline → target) | Giảm thời gian tổng hợp lịch từ 50 xuống dưới 15 phút/người/tuần; không bỏ sót lịch họp hoặc thông báo đổi lịch đã được xác nhận.|
| Phương án không dùng AI | Sử dụng một lịch nhóm thống nhất; quy định người tạo cuộc họp cập nhật trực tiếp lịch chung; mẫu thông báo thay đổi có cấu trúc.|
| Giả thuyết về AI (nếu có) | AI hỗ trợ nhận diện các thông báo lịch họp từ nhiều kênh, xác định thay đổi và hỗ trợ tổng hợp thông tin.|
| Cảm nhận nhanh | Rule / Workflow — chưa có đủ bằng chứng cho thấy cần Agent. |

Quy trình nháp hiện tại:

```text
flowchart TD
    A["1. Kiểm tra các kênh thông báo<br/>10 phút"]
    B["2. Đọc và xác định lịch mới<br/>10 phút"]
    C["3. Đối chiếu thông báo thay đổi<br/>15 phút - BOTTLENECK"]
    D["4. Tổng hợp lịch họp trong tuần<br/>5 phút"]
    E["5. Kiểm tra trùng lịch<br/>5 phút"]
    F["6. Theo dõi và cập nhật phát sinh<br/>5 phút"]

    A --> B --> C --> D --> E --> F

    classDef normal fill:#E8F1FF,stroke:#3675C5,color:#173A66
    classDef bottleneck fill:#FFE6E6,stroke:#D64545,color:#922020,stroke-width:2px

    class A,B,D,E,F normal
    class C bottleneck
```

### Card muốn pitch nhất

- Card số: #2 – Phân tích điểm mạnh, điểm yếu của các hệ thống HIS/EHR/AI Agent trên thị trường.
- Vì sao: Đây là công việc thực tế của BA trong team phát triển AI Agent y tế, đòi hỏi nghiên cứu nhiều hệ thống, đọc tài liệu và đối chiếu thông tin từ nhiều nguồn. Bottleneck rõ ràng ở bước đọc và trích xuất thông tin sản phẩm (ước lượng 60 phút/hệ thống). Kết quả có thể đo lường thông qua thời gian phân tích và tỷ lệ nhận định có bằng chứng.
- Câu hỏi muốn nhóm phản biện: Liệu bottleneck chính có thực sự nằm ở bước đọc và trích xuất thông tin, hay nằm ở việc xác minh tính chính xác và đánh giá điểm mạnh, điểm yếu? Có cần AI Agent hay chỉ cần workflow với bộ tiêu chí benchmarking chuẩn?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Actor chưa đủ cụ thể, BA và PO/PM có vai trò khác nhau trong quy trình.| Có | Xác định BA nghiên cứu thị trường là actor chính; PO/PM là người sử dụng kết quả.| 
| Điểm yếu của sản phẩm có thể bị đánh giá chủ quan do thiếu thông tin công khai.| Có | Phân biệt rõ: chức năng không có, chưa được công bố và chưa xác minh được. Yêu cầu các nhận định phải có bằng chứng.| 

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
