# CP4 — Review tài liệu và thử Rule

Nguồn: chính repo đề Day 02 (bản fork của nhóm, commit `08682e9`). Mọi con số dưới đây chạy lại được bằng các lệnh ghi kèm, chạy ở thư mục gốc repo.

## 1. Đề dài bao nhiêu

Đếm bằng `wc -w` (đếm theo khoảng trắng).

| File | Số từ | Có trong quy trình đọc đề hiện tại (bước 1–4)? |
|---|---:|---|
| README.md | 1.343 | Có |
| RULES.md | 898 | Có |
| CHECKPOINTS.md | 2.174 | Có |
| docs/01-worksheet.md | 3.418 | Có |
| RUBRIC.md | 1.337 | Có |
| SUBMISSION.md | 842 | Có |
| TEAM.md | 349 | Không |
| docs/02-deliverable-example.md | 4.442 | Không (đọc ở CP0) |
| docs/03-international-frameworks.md | 1.032 | Không (đọc thêm) |
| docs/README.md | 84 | Không |
| **Tổng 10 file hướng dẫn** | **15.919** | |
| **6 file đọc ở bước 1–4** | **10.012** | |

## 2. Yêu cầu nằm ở đâu

- Ô tự kiểm `- [ ]`: **32 ô**, gồm 22 ô trong CHECKPOINTS.md (mục "Tự kiểm tra" của CP1–CP7) và 10 ô trong SUBMISSION.md ("Checklist trước khi nộp").
- Quy tắc đặt tên file báo cáo cá nhân được nêu ở **5 nơi**: README.md (dòng 53), RUBRIC.md (dòng 9 và 50), SUBMISSION.md (dòng 48–50 và 96), report/individual/README.md (dòng 3–6), đầu file template. Cả 5 nơi nói giống nhau, **không mâu thuẫn**.
- Danh sách file phải nộp và vị trí đặt file đã được gom ở **1 chỗ**: SUBMISSION.md, mục "Cấu trúc và file phải nộp".

## 3. Điều kiện được / mất điểm trong RUBRIC so với 32 ô tự kiểm

Nhóm tự liệt kê 25 điều kiện làm mất điểm hoặc giới hạn điểm trong RUBRIC.md, rồi tìm ô tự kiểm tương ứng.

| # | Điều kiện (RUBRIC) | Dòng | Ô tự kiểm tương ứng | Lệnh Rule bắt được? |
|---:|---|---:|---|---|
| 1 | C1: thiếu dấu hiệu thật ở quá nửa số dòng → tối đa 4 | 13 | CP1 "Mỗi dòng có ít nhất 1 dấu hiệu thật" | Có |
| 2 | C1: problem là solution trá hình → trừ 1/dòng | 13 | CP1 "Không dòng nào có chữ AI…" | Có |
| 3 | C1: dưới 5 problem → tối đa 3 | 13 | CP1 + SUBMISSION | Có |
| 4 | C2: phải ghi phản biện của AI và đã sửa gì mới đạt 10 | 14 | CP2 "Đã đưa card cho AI…" | Có |
| 5 | C2: bottleneck mơ hồ → trừ 1/card | 14 | CP2, một phần ("đánh dấu bước nghẽn") | Có |
| 6 | C3: chỉ ghi chung chung "đã góp ý" → tối đa 2 | 15 | CP3, một phần ("mỗi thành viên có 1 câu hỏi") | Có |
| 7 | C4: mục 6.1–6.6 dưới 200 từ → tối đa 4 | 16 | **Không có** (chỉ nằm trong lời "Cần làm" của CP7) | Có |
| 8 | C4: reflection do AI viết → C4 = 0 | 16 | CP7 "Reflection không do AI viết" | Có |
| 9 | C5: giải thích sai hoặc thiếu mắt xích → 0–3 | 17 | **Không có** (chỉ nằm trong "Cần hiểu" của CP7) | Có |
| 10 | C6: chỉ bỏ phiếu không lý do → tối đa 3 | 26 | CP3 "Có ghi lý do loại ít nhất 2 candidate" | Có |
| 11 | C7: câu hỏi dạng "Bạn có muốn…" → trừ 3 | 27 | CP4 | Có |
| 12 | C7: link chết hoặc số liệu không nguồn → trừ 2 | 27 | CP4 + SUBMISSION, một phần (chỉ phần link) | Có |
| 13 | C8: thiếu phương án quay về → trừ 3 | 28 | CP5 | Có |
| 14 | C8: thiếu thời gian từng bước → trừ 2 | 28 | **Không có** (chỉ nằm trong lời "Cần làm" bước 1 của CP5) | Có |
| 15 | C9: metric không đo được → trừ 5 | 29 | CP5 "Success Metric có baseline, target và cách đo" | Có |
| 16 | C9: không có tiêu chí đánh giá → trừ 3 | 29 | **Không có** (chỉ nằm trong lời "Cần làm" bước 5 của CP6) | Có |
| 17 | C10: chọn Agent mà không giải thích → tối đa 3 | 30 | CP6 "vì sao không chọn mức đơn giản hơn" | Có |
| 18 | C11: không có ngưỡng dừng → trừ 2 | 31 | CP6 | Có |
| 19 | Sai tên repo hoặc tên file → trừ 5 | 50 | SUBMISSION ô 1 và 2 | Có |
| 20 | Thiếu group_report.md hoặc TEAM.md → phần nhóm 0 | 51 | SUBMISSION ô 5 | Có |
| 21 | Không nộp link repo trên LMS → không có bài để chấm | 52 | SUBMISSION ô 10 | Có (qua ô SUBMISSION; dòng 52 không khớp mẫu tìm) |
| 22 | Không có đóng góp trong TEAM.md → phần nhóm của người đó 0 | 53 | SUBMISSION ô 6 | Có |
| 23 | Bịa kết quả phỏng vấn/survey → C7 = 0 cả nhóm | 54 | **Không có** | Có |
| 24 | Báo cáo cá nhân trùng lặp hoặc phần lớn do AI viết → phần cá nhân 0 | 55 | **Không có** (CP7 chỉ nói về reflection) | Có |
| 25 | Commit API key hoặc thông tin người được phỏng vấn → trừ 5 | 56 | SUBMISSION ô 9 | Có |

**Kết quả:** 6/25 điều kiện **không có** ô tự kiểm nào (dòng 7, 9, 14, 16, 23, 24), 3/25 chỉ có một phần (dòng 5, 6, 12). Ba trong sáu điều kiện đó có mức trừ cụ thể: trừ 2 (dòng 14), trừ 3 (dòng 16), tối đa 4/10 (dòng 7).

Cách tách điều kiện là của nhóm: tách hoặc gộp khác thì con số 25 có thể đổi nhẹ.

## 4. Thử Rule: 2 lệnh gom

```bash
grep -n -- '- \[ \]' CHECKPOINTS.md SUBMISSION.md
grep -nE 'trừ|tối đa|bị 0|= 0|không được|0–3' RUBRIC.md
```

Trên Windows: chạy trong Git Bash (đi kèm Git for Windows), hoặc dùng ô tìm kiếm của VS Code với chế độ regex.

| Chỉ số | Kết quả |
|---|---:|
| Dòng ô tự kiểm | 32 |
| Dòng điều kiện trong RUBRIC | 24 |
| Tổng số dòng đầu ra | 56 |
| Tổng số từ đầu ra (`wc -w`) | 1.687 |
| Điều kiện bắt được (so với bảng mục 3) | **25/25** |
| Dòng nhiễu (không phải điều kiện) | 5/56 (khoảng 9%): RUBRIC dòng 3, 11, 24, 36, 48 |

**Hạn chế đã thấy:**

- Đầu ra chưa xếp theo CP. Các dòng bảng trong RUBRIC dài, vẫn phải đọc kỹ.
- Lệnh dựa vào cách viết của đề Day 02: ô `- [ ]` và các chữ "trừ", "tối đa", "bị 0". Đề lab khác viết khác thì lệnh có thể bắt thiếu mà không báo.
- Mới thử trên 1 đề.

Đã chạy lại bằng GNU grep 3.12: kết quả giống hệt (32 / 24 / 56 dòng / 1.687 từ).

## 5. Thử lệnh kiểm tên

```bash
# Tên repo: đúng mẫu thì in "đúng"
git remote get-url origin | grep -vF 'TenNhom' \
  | grep -qE '/K5-L3[AB]-DAY02-[A-Za-z0-9]+-DiscoveryProblemFraming(\.git)?$' \
  && echo "Tên repo: đúng" || echo "Tên repo: SAI hoặc khác chữ hoa/thường, đọc lại SUBMISSION"

# Tên file báo cáo cá nhân: in ra file nào sai mẫu MSSV_HoTen.md (không in gì là đúng)
ls report/individual | grep -vE '^(README|[0-9][0-9A-Z]*_[A-Za-z]+)\.md$'
```

| Thử | Kết quả |
|---|---|
| Repo của nhóm (`K5-L3B-DAY02-LuckyTeam-DiscoveryProblemFraming`) | Đúng |
| 8 tên repo thử, nhóm tự đặt theo quy tắc trong SUBMISSION, gồm 2 tên đúng và 6 kiểu sai hay gặp (thay `git remote get-url origin` bằng `echo "https://github.com/x/<tên>"`) | Khớp 8/8, xem bảng dưới |
| Tên file: `2A202603943_NguyenDucHai.md`, `README.md` | Không báo (đúng) |
| Tên file: `MSSV_HoTen.md`, `NguyenVanAn_20241234.md`, `20241234-NguyenVanAn.md` | Báo cả 3 (đúng) |

| Tên repo thử | Lệnh báo | Đúng với quy tắc? |
|---|---|---|
| `K5-L3B-DAY02-LuckyTeam-DiscoveryProblemFraming.git` | đúng | ✅ |
| `K5-L3A-DAY02-NhomA-DiscoveryProblemFraming` | đúng | ✅ |
| `K5-L3-Day02-DiscoveryProblemFraming` (để nguyên tên mặc định khi fork) | SAI | ✅ |
| `K5-L3B-DAY02-TenNhom-DiscoveryProblemFraming` (để nguyên chữ `TenNhom`) | SAI | ✅ |
| `K5-DAY02-LuckyTeam-DiscoveryProblemFraming` (thiếu `L3B`) | SAI | ✅ |
| `K5-L3B-Day02-LuckyTeam-DiscoveryProblemFraming` (`Day02` chữ thường) | SAI | ✅ (đề chưa nói có phân biệt hoa/thường; lệnh báo để người dùng tự xem lại) |
| `K5-L3B-DAY02-NguyenVanAn-20241234-DiscoveryProblemFraming` (mẫu cũ `HoTen-MSSV`) | SAI | ✅ |
| `K5-L3B-DAY02-LuckyTeam-DiscoverProblemFraming` (sai chính tả) | SAI | ✅ |

Chạy được với cả GNU grep và ugrep. Lệnh viết theo thứ tự "lọc `TenNhom` trước, so mẫu sau" vì với `grep -qv` trên đầu vào rỗng, hai bản grep trả kết quả khác nhau.
