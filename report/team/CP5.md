## 4. Quy trình trước/sau (CP5)

```text
HIỆN TẠI — 5 bước, khoảng 10 phút, 5/5 bước thủ công

[1 Mở ghi chú: 1'] → [2 Xác định paper: 1']
→ [3 Dò bằng chứng trong PDF: 6'] ← BOTTLENECK
→ [4 Kiểm tra ngữ cảnh: 1'] → [5 Ghi lại vị trí nguồn: 1']

TƯƠNG LAI — 4 bước, khoảng 3 phút, 2/4 bước thủ công

[1 Mở ghi chú có liên kết paper + từ khóa: 0.5']  ← CON NGƯỜI
→ [2 Mở đúng trang/annotation trong Zotero: 0.5'] ← RULE (annotation + page link)
→ [3 Kiểm tra bằng chứng và ngữ cảnh: 1.5']       ← CON NGƯỜI
→ [4 Ghi lại vị trí nguồn vào bảng so sánh: 0.5'] ← CON NGƯỜI

BOUNDARY: Không tự động kết luận paper chứng minh điều gì. Người đọc phải kiểm tra
đoạn trích, ngữ cảnh và đối chiếu với PDF gốc trước khi sử dụng bằng chứng.

PHƯƠNG ÁN QUAY VỀ: Nếu annotation hoặc liên kết sai/mất,
mở PDF gốc và tìm thủ công bằng Ctrl+F hoặc dò theo số trang.
```

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 4 | Gộp thao tác xác định paper và truy cập vị trí nguồn |
| Tổng thời gian | 10' | 3' | Target chính: tối đa 3 phút/lần |
| Bước thủ công | 5/5 | 2/4 | Hai bước chính được hỗ trợ bởi annotation và liên kết nguồn |
| Bottleneck | Dò bằng chứng trong PDF (6') | Kiểm tra bằng chứng và ngữ cảnh (1.5') | Bottleneck mới được giữ lại có chủ đích để đảm bảo độ chính xác |
| Rủi ro mới | Ghi chú thiếu vị trí nguồn | Annotation sai, liên kết hỏng hoặc ghi nhầm trang | Xử lý bằng kiểm tra PDF gốc |
| Chất lượng | Phụ thuộc vào trí nhớ và khả năng tìm kiếm | Phải tìm đúng đoạn và giữ nguyên ngữ cảnh | Không đánh đổi độ chính xác lấy tốc độ |

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Lam, sinh viên mới tham gia nhóm nghiên cứu, thường xuyên đọc và so sánh các paper |
| **Quy trình** | Khi cần sử dụng lại một nhận định từ paper đã đọc: mở ghi chú, xác định paper, dò bằng chứng trong PDF, kiểm tra ngữ cảnh và ghi lại vị trí nguồn |
| **Bottleneck** | Dò bằng chứng trong PDF mất khoảng 6 phút/lần vì ghi chú thiếu số trang, hình hoặc bảng tham chiếu |
| **Impact** | Khoảng 30–40 phút/tuần cho 3–4 lần tìm kiếm; khó bảo vệ nhận định khi không tìm lại được bằng chứng gốc |
| **Success Metric** | Giảm thời gian tìm bằng chứng từ khoảng 10 phút xuống tối đa 3 phút/lần. Đo bằng cách bấm giờ trong các tác vụ tìm kiếm thực tế. Đồng thời yêu cầu tìm đúng đoạn, đúng trang và giữ được ngữ cảnh |
| **Boundary** | Ưu tiên Zotero annotation, liên kết PDF và ghi chú có cấu trúc. AI (nếu thử nghiệm sau này) chỉ gợi ý vị trí bằng chứng, không tự kết luận hoặc tạo trích dẫn chưa được kiểm chứng. Người dùng phải đối chiếu PDF gốc |

**Phản biện nhận được:** AI chỉ ra rằng metric hiện tại chủ yếu đo tốc độ tìm kiếm, chưa chứng minh người dùng tìm được bằng chứng chính xác. Tìm nhanh nhưng sai đoạn hoặc mất ngữ cảnh có thể dẫn đến trích dẫn sai trong nghiên cứu.

**Nhóm đồng ý và bổ sung:** ngoài thời gian tìm kiếm, cần đo tỷ lệ tìm đúng bằng chứng (đúng đoạn, trang/hình/bảng) và khả năng giữ nguyên ngữ cảnh. Chỉ tính một lần tìm kiếm là thành công khi người dùng xác định được nguồn và xác minh được nội dung trong PDF gốc.