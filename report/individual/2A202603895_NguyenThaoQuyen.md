# Báo cáo cá nhân — 2A202603895_NguyenThaoQuyen


## 1. Thông tin học viên

- Họ tên: Nguyễn Thảo Quyên
- MSSV:2A202603895
- Tên nhóm: NhomCold
- Link repo nhóm: https://github.com/Ama2352/K5-L3B-DAY02-NhomCold-DiscoveryProblemFraming/tree/main

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Tốn thời gian |Khi khách hàng yêu cầu báo giá phụ tùng ô tô nhưng chỉ cung cấp hình ảnh hoặc tên gọi thông thường, nhân viên muốn xác định đúng phụ tùng theo dòng xe và mã sản phẩm, để tránh báo giá nhầm và mất thời gian tra cứu. | Nhân viên tư vấn phụ tùng, garage, khách hàng| Phát sinh theo từng yêu cầu báo giá; có thể phải tra cứu nhiều danh mục và đối chiếu thủ công; cần đo thời gian tìm kiếm và tỷ lệ xác định sai.|
| 2 |Pain từ người khác |Khi làm việc tại một nhà máy có nhiều SOP và quy trình vận hành, nhân viên mới muốn nhanh chóng tìm được đúng tài liệu và hiểu quy trình cần tuân thủ cho từng công việc, để tránh làm sai quy trình, mất thời gian tra cứu hoặc áp dụng nhầm hướng dẫn. |Nhân viên mới, công nhân vận hành, nhân viên QC, kỹ sư sản xuất, quản lý nhà máy |Nhân viên mới phải đọc và tra cứu nhiều SOP từ các nguồn khác nhau; có thể gặp khó khăn khi xác định tài liệu nào áp dụng cho công việc hoặc phiên bản nào còn hiệu lực |
| 3 |Pain từ người khác | Khi sinh viên liên tục gặp khó khăn với cùng một nội dung, giảng viên muốn xác định những phần kiến thức mà nhiều người chưa hiểu, để điều chỉnh cách giảng dạy.|Giảng viên, sinh viên | Số câu hỏi lặp lại, số sinh viên gặp khó khăn, kết quả kiểm tra.|
| 4 |Lặp lại | 	Khi giảng viên nhận nhiều bài tập, tôi muốn kiểm tra và phân loại bài theo cùng một tiêu chí, để giảm công việc đánh giá lặp lại.|Giảng viên, trợ giảng |Số bài mỗi lớp, thời gian chấm, số lớp phụ trách. |
| 5 | Lặp lại | Khi đến kỳ thu tiền nhà trọ hằng tháng, tôi muốn tổng hợp chỉ số điện, nước, tiền thuê và các khoản phí phát sinh của từng phòng, đối chiếu số đã thanh toán và số còn nợ, để tính đúng số tiền phải thu, thông báo rõ từng khoản cho người thuê và theo dõi thu chi đầy đủ. | Chủ nhà trọ, người quản lý và người thuê | Mỗi tháng phải tổng hợp số liệu theo từng phòng, tính tiền điện nước và đối chiếu các khoản thu. Các chỉ số cần ghi nhận: số phòng quản lý, thời gian chốt sổ mỗi tháng, số khoản phải kiểm tra lại và số phòng còn nợ; không dùng các chỉ số này như số liệu đã đo. |
| 6 | Tốn thời gian | Khi xe xảy ra tai nạn, tôi muốn nhanh chóng xác định các phụ tùng bị hư hỏng và ước lượng chi phí sửa chữa, thay thế, để xác định mức bồi thường dự kiến và chuyển hồ sơ đến cấp phê duyệt phù hợp. | Giám định viên, nhân viên bồi thường, trưởng phòng, giám đốc | Thời gian kiểm tra hư hỏng, tra cứu giá phụ tùng, lập bảng báo giá và chờ phê duyệt hồ sơ 5 đến 7 ngày. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Các ý AI gợi ý mà tôi giữ lại là ý số 3,4. Vì các Job story đọc khá hợp lí, painpoint rõ ràng. Và có các ý tôi trải qua tương tự. 


---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Xác định hư hỏng và ước lượng chi phí sửa chữa (#6) | Quy trình nhiều bước, kết hợp nhận diện hình ảnh, tra cứu phụ tùng và ước lượng chi phí; impact theo thời gian phản hồi và số trường hợp phải đối chiếu lại có thể đo được. | Độ chính xác nhận diện hư hỏng; độ tin cậy của dữ liệu giá và chi phí ước lượng. |
| 2 | Tra cứu và xác định phụ tùng ô tô (#1) | Pain cụ thể, phát sinh thường xuyên; sai mã hoặc sai tương thích dẫn đến phải tra cứu lại và đổi trả. | Khả năng tiếp cận dữ liệu; độ chính xác khi xác định phụ tùng theo dòng xe và mã sản phẩm. |
| 3 | Kiểm tra và phân loại bài tập (#4) | Công việc lặp lại, có thể chuẩn hóa rubric và đánh giá mức độ nhất quán giữa AI với người chấm. | Khó đánh giá chất lượng với bài tự luận, câu trả lời sáng tạo và các trường hợp cần nhận định chuyên môn. |

### Problem Card #1 — Xác định hư hỏng và ước lượng chi phí sửa chữa (#6)

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận yêu cầu bồi thường kèm hình ảnh xe bị tai nạn, tôi muốn xác định các bộ phận bị hư hỏng và ước lượng chi phí sửa chữa, để có cơ sở đánh giá mức bồi thường và tư vấn cho khách hàng. |
| Actor | Nhân viên giám định tổn thất, nhân viên xử lý bồi thường bảo hiểm ô tô. |
| Thời điểm / bối cảnh | Khi khách hàng gửi hình ảnh xe sau tai nạn và yêu cầu đánh giá mức độ hư hỏng, chi phí sửa chữa. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận hình ảnh và thông tin xe. 2. Kiểm tra hình ảnh tổng thể. 3. Xác định các vị trí và bộ phận bị hư hỏng. 4. Tra cứu phụ tùng cần thay thế hoặc sửa chữa. 5. Tìm kiếm giá phụ tùng và công sửa chữa. 6. Tổng hợp chi phí dự kiến. 7. Chuyển kết quả cho bộ phận có thẩm quyền xác nhận. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5, tra giá và công sửa chữa: giả thuyết 8 phút trong kịch bản 30 phút thao tác/vụ; khoảng 20–40 phút ban đầu là ước lượng tổng, không phải số đo bước này. |
| Impact (nếu không giải thì sao) | Thời gian xử lý hồ sơ kéo dài; kết quả ước lượng có thể thiếu nhất quán giữa các nhân viên; ảnh hưởng đến thời gian phản hồi khách hàng và tiến độ giải quyết bồi thường. |
| Success metric (baseline → target) | Thời gian đánh giá ban đầu: 20–40 phút/vụ → target thử nghiệm ≤21 phút/vụ so với kịch bản 30 phút (giảm 30%); đo 10 hồ sơ tương đương, tách thời gian chờ; độ chính xác xác định bộ phận hư hỏng và sai số ước lượng chi phí được đánh giá trên tập hồ sơ đã có kết quả giám định thực tế. |
| Phương án không dùng AI | Xây dựng danh mục hư hỏng, bảng giá phụ tùng chuẩn hóa, checklist đánh giá theo dòng xe và biểu mẫu tính chi phí. |
| Giả thuyết về AI (nếu có) | Kết hợp Computer Vision để nhận diện vị trí và mức độ hư hỏng, hệ thống tra cứu phụ tùng và dữ liệu giá để đề xuất danh sách sửa chữa cùng chi phí dự kiến. |
| Cảm nhận nhanh | No AI trước; Workflow chỉ hỗ trợ các bước cố định khi có dữ liệu kiểm chứng, không có căn cứ cần Agent |

Quy trình nháp hiện tại:

```text
KỊCH BẢN ƯỚC LƯỢNG — 30 phút thao tác/vụ, không tính chờ phê duyệt
[1 Nhận thông tin 2'] → [2 Kiểm ảnh 3'] → [3 Xác định hư hỏng 5']
→ [4 Tra phụ tùng 6'] → [5 Tra giá và công 8' — BOTTLENECK giả thuyết]
→ [6 Tổng hợp 4'] → [7 Chuyển duyệt 2']
```

### Problem Card #2 - Tra cứu và xác định phụ tùng ô tô (#1)
 
| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tìm phụ tùng thay thế cho một dòng xe cụ thể, tôi muốn xác định đúng tên, mã và loại phụ tùng tương thích, để tránh chọn nhầm sản phẩm và đảm bảo quá trình sửa chữa diễn ra chính xác. |
| Actor | Nhân viên kỹ thuật, nhân viên phụ tùng, nhân viên giám định và xử lý bồi thường bảo hiểm. |
| Thời điểm / bối cảnh | Khi tiếp nhận yêu cầu tra cứu phụ tùng từ thông tin xe, hình ảnh bộ phận hoặc mô tả hư hỏng. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận thông tin xe (hãng, dòng xe, năm sản xuất). 2. Tiếp nhận tên hoặc hình ảnh phụ tùng cần tìm. 3. Tìm kiếm trong danh mục phụ tùng hoặc file dữ liệu. 4. Đối chiếu tên gọi, mã sản phẩm và thông số kỹ thuật. 5. Kiểm tra khả năng tương thích với dòng xe. 6. Xác nhận phụ tùng phù hợp và tra cứu giá. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, tìm trong danh mục: giả thuyết 5 phút trong kịch bản tổng 15 phút/lần. Khoảng 10–20 phút ban đầu là ước lượng tổng, cần kiểm bằng nhật ký tra cứu. |
| Impact (nếu không giải thì sao) | Chọn sai phụ tùng, phát sinh chi phí đổi trả hoặc sửa chữa; kéo dài thời gian xử lý hồ sơ và phụ thuộc nhiều vào kinh nghiệm của nhân viên. |
| Success metric (baseline → target) | Thời gian tra cứu: 10–20 phút/lần → target ≤7,5 phút/lần so với kịch bản 15 phút; bấm giờ 10 lượt cùng nhóm xe, ghi số lần phải sửa mã; tỷ lệ xác định đúng phụ tùng và tỷ lệ tương thích được kiểm chứng trên tập dữ liệu có nhãn chuẩn. |
| Phương án không dùng AI | Chuẩn hóa danh mục phụ tùng, xây dựng từ điển tên gọi đồng nghĩa, mã hóa theo hãng và dòng xe, bổ sung bộ lọc theo thông số kỹ thuật. |
| Giả thuyết về AI (nếu có) | Kết hợp tìm kiếm từ khóa, tìm kiếm ngữ nghĩa và bộ lọc metadata để truy xuất phụ tùng từ tên gọi, mô tả hoặc hình ảnh; sau đó đối chiếu thông tin xe để xếp hạng các sản phẩm tương thích. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
KỊCH BẢN ƯỚC LƯỢNG — 15 phút/lần
[1 Thông tin xe 1'] → [2 Tên/ảnh phụ tùng 1'] → [3 Tìm danh mục 5' — BOTTLENECK giả thuyết]
→ [4 Đối chiếu mã 3'] → [5 Kiểm tương thích 3'] → [6 Xác nhận giá 2']
```


### Problem Card #3 — Kiểm tra và phân loại bài tập (#4)

| Trường | Nội dung |
|---|---|
| Job Story | Khi học viên nộp bài tập, tôi muốn kiểm tra kết quả, phân loại lỗi và đánh giá mức độ hoàn thành theo tiêu chí có sẵn, để phản hồi kịp thời và theo dõi tiến độ học tập của từng học viên. |
| Actor | Giáo viên, trợ giảng, người phụ trách quản lý chất lượng học tập. |
| Thời điểm / bối cảnh | Sau mỗi buổi học, bài kiểm tra hoặc khi học viên hoàn thành và nộp bài tập. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận bài tập của học viên. 2. Đọc và kiểm tra câu trả lời. 3. Đối chiếu với đáp án hoặc rubric. 4. Xác định câu trả lời đúng, sai hoặc chưa đầy đủ. 5. Chấm điểm và phân loại lỗi. 6. Viết nhận xét và đề xuất nội dung cần cải thiện. 7. Tổng hợp kết quả học tập. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, đọc và kiểm tra: giả thuyết 2 phút trong kịch bản 8 phút/bài có cấu trúc. Khoảng 5–10 phút ban đầu là ước lượng tổng, không dùng như số đo riêng bước đọc. |
| Impact (nếu không giải thì sao) | Giáo viên và trợ giảng mất nhiều thời gian cho công việc lặp lại; thời gian phản hồi học viên chậm; tiêu chí đánh giá có thể thiếu nhất quán giữa những người chấm. |
| Success metric (baseline → target) | Thời gian kiểm tra: 5–10 phút/bài → target ≤4,8 phút/bài so với kịch bản 8 phút; bấm giờ 10 bài cùng loại và đối chiếu kết quả người chấm; mức độ nhất quán giữa kết quả đánh giá và người chấm đạt ít nhất 90% trên tập bài đã được chấm chuẩn. |
| Phương án không dùng AI | Xây dựng ngân hàng đáp án, rubric chấm điểm, bộ quy tắc kiểm tra tự động cho câu hỏi trắc nghiệm và câu trả lời có cấu trúc. |
| Giả thuyết về AI (nếu có) | Sử dụng mô hình ngôn ngữ để đối chiếu câu trả lời với rubric, phân loại lỗi, đề xuất điểm số và tạo nhận xét. Giáo viên kiểm tra lại các trường hợp không chắc chắn trước khi công bố kết quả. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
KỊCH BẢN ƯỚC LƯỢNG — 8 phút/bài
[1 Nhận bài 0.5'] → [2 Đọc bài 2' — BOTTLENECK giả thuyết]
→ [3 Đối chiếu rubric 1.5'] → [4 Xác định lỗi 1']
→ [5 Chấm 1'] → [6 Nhận xét 1.5'] → [7 Tổng hợp 0.5']
```

### Card muốn pitch nhất

- Card số: Card số 1 
- Vì sao: actor và quy trình rõ, có thể tách thời gian giám định khỏi thời gian chờ phê duyệt.
- Câu hỏi muốn nhóm phản biện: “Bước nghẽn nằm ở tra cứu giá hay chờ phê duyệt; checklist và bảng giá chuẩn đã đủ chưa?”

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Đề xuất Agent vượt nhu cầu của quy trình có bước cố định | Đồng ý ở vòng rà soát tài liệu | Chuyển sang thử No AI trước; chỉ xem Workflow khi dữ liệu và nhu cầu đã kiểm chứng |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Phản biện bài của bạn khác | Không có câu hỏi trực tiếp được ghi lại. | Không có bản ghi trong tài liệu hiện tại |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Chọn candidate problem | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Kiểm chứng / research | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Quy trình nhóm | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Problem Statement | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Mức can thiệp AI | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| Quyết định | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý #3 và #4, theo ghi nhận ở CP1 | Mở rộng góc nhìn giáo dục | Dấu hiệu còn là chỉ số cần đo, không phải số quan sát | Giữ phân biệt giả thuyết và bằng chứng |
| CP2 Problem Card | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| CP4 Research | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| CP5 Quy trình | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| CP5–6 Problem Statement | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |
| CP6 Mức can thiệp / quyết định | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại | Không có bản ghi trong tài liệu hiện tại |

---

## 6. Reflection (CP7)

**Trạng thái bằng chứng:** phần trả lời cá nhân không có nội dung trải nghiệm trong bản nguồn. Giữ câu hỏi để tác giả tự trả lời; không xem mục này là đã đáp ứng C4/C5.

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

- [Báo cáo nhóm và nguồn research](../team/group_report.md#10-tài-liệu-tham-khảo).
