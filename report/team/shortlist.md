# Shortlist

### Opportunity Solution Tree rút gọn

```text
OUTCOME: Giảm thời gian tìm lại bằng chứng từ paper,
         đồng thời đảm bảo nhận định có căn cứ và truy xuất được nguồn.

├── Opportunity: Ghi chú hiện tại thiếu vị trí cụ thể của bằng chứng
│   (số trang, hình, bảng hoặc đoạn văn).
│
├── Opportunity: Sinh viên phải dò thủ công trong PDF
│   để tìm lại đoạn chứa thông tin cần thiết.
│
├── Opportunity: Cần kiểm tra ngữ cảnh xung quanh bằng chứng
│   để tránh trích dẫn sai hoặc hiểu sai nhận định.
│
└── Opportunity: Việc ghi lại và truy xuất nguồn chưa được
    chuẩn hóa giữa các paper.

     ✗ "AI chatbot đọc paper"       ← solution, không phải opportunity
     ✗ "RAG-based paper assistant" ← solution, không phải opportunity
     ✗ "Tự động tóm tắt PDF"       ← solution, không phải opportunity
```

### Chấm điểm shortlist

Thang điểm 1–5, dựa trên thông tin hiện có trong ba Problem Cards.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được 4 mức | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Tìm lại bằng chứng từ paper | 5 | 5 | 4 | 5 | 5 | 5 | 4 | **33** |
| So sánh biến thể tín hiệu | 5 | 5 | 4 | 4 | 4 | 5 | 3 | **30** |
| Tổng hợp thông tin trước Sprint Planning | 5 | 4 | 2 | 3 | 3 | 4 | 4 | **25** |

**Chọn:** Tìm lại bằng chứng từ paper.

**Vì sao chọn:**

- **Scope rõ:** Tập trung vào một tác vụ cụ thể: tìm đúng đoạn, hình hoặc bảng chứa bằng chứng trong paper đã đọc.
- **Có baseline:** Hiện tại mất khoảng 10 phút/lần, trong đó 6 phút dành cho việc dò PDF.
- **Đo lường được:** Có thể bấm giờ trước và sau thử nghiệm, đồng thời kiểm tra độ chính xác của vị trí bằng chứng và ngữ cảnh.
- **Có baseline không dùng AI:** Zotero annotation, ghi số trang, hình/bảng và liên kết trực tiếp đến PDF. Nhóm có thể kiểm tra liệu AI thực sự tạo thêm giá trị hay không.
- **Vừa sức lab:** Không cần tích hợp Slack, Jira, Drive hay xây dựng hệ thống truy xuất dữ liệu đa nguồn.

**Vì sao loại hai candidate kia:**

- **Tổng hợp thông tin trước Sprint Planning:** Impact tiềm năng lớn nhưng phạm vi dữ liệu quá rộng, phụ thuộc quyền truy cập nhiều nền tảng và chưa có baseline thực nghiệm. Mục tiêu giảm 50% thời gian hiện mới là giả thuyết.
- **So sánh biến thể tín hiệu:** Có quy trình và metric khá rõ, nhưng domain quant research tương đối đặc thù. Ngoài ra, cần phân biệt được việc AI diễn giải bảng kết quả với việc AI thực sự hiểu được ảnh hưởng của từng thay đổi. Không nên để AI suy luận quan hệ nhân quả từ dữ liệu quan sát.

**Bất đồng:** Chưa có thông tin về bất đồng thực tế giữa các thành viên nên không nên tự tạo tên hoặc quan điểm. Có thể ghi nhận candidate so sánh biến thể tín hiệu là hướng tiếp theo nếu nhóm muốn mở rộng sang workflow phân tích dữ liệu.

### Hướng thử nghiệm tiếp theo

| Mức | Phương án | Mục đích |
|---|---|---|
| 1 | Manual PDF search | Baseline hiện tại |
| 2 | Structured notes + Zotero | Đánh giá giải pháp không dùng AI |
| 3 | Keyword / BM25 retrieval | Đánh giá tìm kiếm truyền thống |
| 4 | Semantic retrieval / RAG | Đánh giá giải pháp AI-assisted |

**Metrics cần đo:**

- Retrieval time: Thời gian tìm được bằng chứng.
- Evidence hit rate: Tỷ lệ tìm đúng bằng chứng.
- Context correctness: Mức độ chính xác của ngữ cảnh được truy xuất.
- Citation accuracy: Độ chính xác của vị trí nguồn được trích dẫn.

**Lưu ý:** Không mặc định RAG là giải pháp tốt nhất. Nếu Zotero + structured notes đã giải quyết được vấn đề với chi phí thấp, nhóm nên thừa nhận điều đó. Mục tiêu của lab là tìm ra giải pháp tốt nhất cho problem, không phải tìm cách nhét LLM vào mọi workflow.