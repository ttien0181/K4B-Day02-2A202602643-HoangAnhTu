# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Hoàng Anh Tú
- Mã học viên: 2A202602643
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): sinh viên mới ra trường, đang thất nghiệp
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): 
-nghiên cứu, thực nghiệm.
-Đi học.
-Tìm việc làm phù hợp.
-Build dự án cá nhân
-Đọc tin tức công nghệ


---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | AI có thể tốt hơn | Tải, đọc từng bài báo, code thực nghiệm, tinh chỉnh thông số, canh thời gian train | Bản thân | Mỗi lần survey mất 1 tuần, mỗi lần thực nghiệm có thể mất cả tháng|
| 2 | Tốn thời gian | Tốn thời gian di chuyển, quãng đường di chuyển dài | Bản thân | mỗi lượt di chuyển mất 1 giờ đồng hồ, đoạn đường 18KM |
| 3 | Lặp lại| Liên tục check các trang tin tuyển dụng, nộp CV, nhắn HR | Bản thân | Mỗi lượt apply từ tìm hiểu tới nộp CV mất ít nhất 10 phút |
| 4 | Tốn thời gian | Thường xuyên lặp lại các module cũ | Bản thân | Mỗi project dù đơn giản tốn 5 tiếng|
| 5 | Tốn thời gian | Tốn thời gian mở các trang tin và cào các bài viết mới, phù hợp | Bản thân | Mất 10 phút đầu ngày để đọc bài viết mới |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |
| 9 | | | | |
| 10 | | | | |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Liên tục check các trang tin tuyển dụng, nộp CV, nhắn HR| - Workflow rõ ràng, mang tính lặp lại cao (Lọc JD -> Sửa CV -> Viết cover letter -> Nộp).<br>- Bottleneck ở khâu so khớp JD và chỉnh sửa CV tốn nhiều thời gian.<br>- Impact trực tiếp và đo đạc được ngay đến tiến độ tìm việc.| Khả năng tự động hóa trên các nền tảng tuyển dụng (chống cào data/anti-bot) và độ tự nhiên của tin nhắn AI gửi HR.|
| 2 | Thường xuyên lặp lại các module cũ khi build dự án cá nhân | - Tốn 5 tiếng setup lại boilerplate và các module quen thuộc cho mỗi dự án mới.<br>- Các module cũ đã có cấu trúc chuẩn, AI hỗ trợ tái sử dụng và sinh code mẫu rất hiệu quả.<br>- Rút ngắn đáng kể thời gian bắt đầu dự án để tập trung vào core logic. | AI có tạo ra code tương thích hoàn toàn với các phiên bản thư viện/framework mới nhất mà không bị conflict dependencies hay không. |
| 3 | Tải, đọc từng bài báo, code thực nghiệm, tinh chỉnh thông số, canh thời gian train | - Tốn nhiều thời gian nhất (survey mất 1 tuần), khâu đọc/bóc tách insight từ PDF là thế mạnh của AI.<br>- Giải quyết bottleneck ở bước tổng hợp phương pháp và trích xuất siêu tham số (hyperparameters).<br>- Giúp đẩy nhanh tốc độ nghiên cứu và thực nghiệm. | AI có nguy cơ bịa số liệu (hallucination) từ file PDF phức tạp, đòi hỏi phải kiểm tra lại thủ công. |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards) 

---

#### Problem Card #1 — Liên tục check các trang tin tuyển dụng, nộp CV, nhắn HR

```text
Problem 1 câu:
Liên tục phải check các trang tin tuyển dụng, lọc JD, chỉnh sửa CV, viết cover letter và nộp CV cho mỗi ứng tuyển.

Actor:
Sinh viên mới ra trường đang tìm việc.

Thời điểm / bối cảnh:
Hàng ngày khi có JD mới; tần suất cao khi áp lực tìm việc tăng.

Current workflow 3-7 bước:
1. Mở các trang tuyển dụng (LinkedIn, TopCV, ITviec...) và lướt JD mới
2. Lọc JD phù hợp với kỹ năng/vị trí mục tiêu
3. Đọc chi tiết JD để hiểu yêu cầu
4. Chỉnh sửa CV phù hợp với JD (bổ sung keyword, thay đổi thứ tự mục)
5. Viết cover letter cá nhân hóa
6. Nộp CV qua trang tuyển dụng
7. Nhắn tin HR hoặc chatbot xác nhận đã nộp

Bottleneck:
Bước 4-5 (Chỉnh sửa CV và viết cover letter) tốn nhiều thời gian nhất vì mỗi JD có yêu cầu khác nhau, phải thay đổi thủ công nhiều chỗ.

Impact:
Mỗi lượt apply mất ít nhất 10 phút; nếu apply 5 vị trí/ngày thì mất ~50 phút. Giảm xuống còn 2-3 phút/lượt thì tiết kiệm ~35-40 phút/ngày.

Success metric:
Thời gian mỗi lượt apply < 3 phút; số lượng apply/ngày tăng từ 5 lên 15+ vị trí; tỷ lệ phỏng vấn được mời tăng.

Non-AI alternative:
Chuẩn bị sẵn 3-4 template CV, copy-paste và chỉnh sửa nhanh; dùng cover letter chung.

AI hypothesis:
AI đọc JD, trích xuất keyword, đề xuất phần CV cần bổ sung/chỉnh sửa, và viết cover letter cá nhân hóa theo JD; kết nối API tuyển dụng để auto-apply.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[x] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 10 phút

[1 Lướt JD: 2'] → [2 Lọc JD: 1'] → [3 Đọc JD: 1'] → [4 Chỉnh CV: 4'] → [5 Viết cover letter: 2'] → [6 Nộp CV: 0.5']  <-- bottleneck (bước 4-5)

FUTURE STATE — 2 phút

[1 Lướt JD: 1'] → [2 Lọc JD: 0.5'] → [3 Đọc JD: 1'] → [4 AI tạo CV/cover letter: 0.5'] → [5 Human review & gửi: 0.5']  <-- human boundary

Fallback: Nếu AI sai keyword hoặc cover letter không phù hợp, human tự chỉnh bằng template sẵn có.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — Thường xuyên lặp lại các module cũ khi build dự án cá nhân

```text
Problem 1 câu:
Mỗi khi bắt đầu dự án cá nhân mới đều phải setup lại các module boilerplate quen thuộc (auth, database, logging, API client...) từ các dự án trước.

Actor:
Sinh viên mới ra trường đang build dự án cá nhân.

Thời điểm / bối cảnh:
Đầu mỗi dự án mới; tần suất 1-2 dự án/tuần.

Current workflow 3-7 bước:
1. Xác định loại dự án và stack công nghệ
2. Tìm dự án trước có module tương tự
3. Copy thư mục module vào dự án mới
4. Cập nhật package.json / requirements, điều chỉnh dependencies
5. Chạy build để kiểm tra lỗi compatibility
6. Fix lỗi import, config, version conflicts
7. Tùy chỉnh nhỏ cho phù hợp ngữ cảnh mới

Bottleneck:
Bước 4-6 (Cập nhật dependencies và fix lỗi compatibility) tốn thời gian nhất vì phiên bản thư viện thay đổi, cấu trúc project khác nhau.

Impact:
Mỗi dự án tốn 5 tiếng setup; nếu build 4 dự án/tháng thì mất 20 tiếng. Giảm xuống 1 tiếng/dự án thì tiết kiệm 16 tiếng/tháng.

Success metric:
Thời gian setup boilerplate < 1 giờ/dự án; số dự án hoàn thành/tháng tăng gấp đôi.

Non-AI alternative:
Tạo 1 template boilerplate chung cho mỗi stack; mỗi dự án clone template rồi tùy chỉnh.

AI hypothesis:
AI nhận yêu cầu mô tả dự án, tự động sinh module boilerplate phù hợp với stack/phiên bản mới nhất, đi kèm config và hướng dẫn tích hợp.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 5 tiếng

[1 Xác định stack: 0.5'] → [2 Copy module cũ: 0.5'] → [3 Cập nhật config: 1'] → [4 Fix dependencies: 2'] → [5 Tùy chỉnh: 1']  <-- bottleneck (bước 4)

FUTURE STATE — 1 tiếng

[1 Mô tả dự án cho AI: 0.2'] → [2 AI sinh boilerplate: 0.5'] → [3 Human review & integrate: 0.3']  <-- human boundary

Fallback: Nếu AI sinh module không tương thích với thư viện mới, dùng template boilerplate có sẵn và chỉnh tay.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Tải, đọc từng bài báo, code thực nghiệm, tinh chỉnh thông số, canh thời gian train

```text
Problem 1 câu:
Tải, đọc hàng loạt bài báo khoa học, bóc tách phương pháp và siêu tham số, code thực nghiệm, tinh chỉnh thông số và canh thời gian train mất nhiều thời gian.

Actor:
Sinh viên mới ra trường đang nghiên cứu/thực nghiệm.

Thời điểm / bối cảnh:
Đầu mỗi đợt survey hoặc khi bắt đầu thử nghiệm mô hình mới; tần suất 1-2 lần/tuần khi đang làm dự án.

Current workflow 3-7 bước:
1. Tìm và tải bài báo liên quan từ Google Scholar/arXiv
2. Mở từng PDF, đọc abstract và đọc lướt các section quan trọng
3. Ghi chú phương pháp, kiến trúc, bộ dữ liệu, kết quả chính
4. Trích xuất siêu tham số (hyperparameters) từ paper
5. Code lại phương pháp hoặc tìm repo mẫu
6. Chạy thực nghiệm, canh thời gian train, theo dõi loss/accuracy
7. Ghi log kết quả, so sánh với paper

Bottleneck:
Bước 2-4 (Đọc PDF và trích xuất thông số) tốn nhiều thời gian nhất; đặc biệt khó khi PDF nhiều công thức, bảng số liệu phức tạp.

Impact:
Survey mất 1 tuần, thực nghiệm mất cả tháng. Nếu survey giảm còn 1-2 ngày và thực nghiệm giảm 30-40% thời gian thì rút ngắn đáng kể tốc độ nghiên cứu.

Success metric:
Thời gian survey từ 1 tuần xuống 1-2 ngày; thời gian setup + chạy thử nghiệm giảm 40%; số paper đọc hiểu được/tuần tăng gấp 3 lần.

Non-AI alternative:
Dùng Zotero quản lý paper, ghi chú thủ công bằng Notion, dùng template code có sẵn.

AI hypothesis:
AI đọc PDF, trích xuất phương pháp và hyperparameters, đề xuất cấu hình thử nghiệm, sinh code mẫu theo paper, dự đoán thời gian train và báo cáo kết quả tự động.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[x] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — Survey 5 ngày, thực nghiệm 20 ngày

[1 Tìm paper: 0.5'] → [2 Đọc PDF: 3'] → [3 Ghi chú: 1'] → [4 Trích xuất params: 1'] → [5 Code thử nghiệm: 5'] → [6 Train & monitor: 10'] → [7 Log & so sánh: 1']  <-- bottleneck (bước 2-4)

FUTURE STATE — Survey 1 ngày, thực nghiệm 12 ngày

[1 AI search & tổng hợp paper: 0.5'] → [2 Human chọn paper phù hợp: 0.5'] → [3 AI đọc & trích xuất: 1'] → [4 AI đề xuất config: 0.5'] → [5 Human review & quyết định: 0.5'] → [6 Chạy thử nghiệm: 8'] → [7 AI log & so sánh: 1']  <-- human boundary (bước 5)

Fallback: Nếu AI trích xuất sai số liệu/hyperparameters, đọc lại PDF trực tiếp hoặc so sánh với các paper khác.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Card #3 — Tải, đọc từng bài báo, code thực nghiệm, tinh chỉnh thông số, canh thời gian train
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Workflow rõ ràng: đọc PDF → trích xuất params → code thử nghiệm → train.
Số đo cụ thể: survey từ 1 tuần xuống 1-2 ngày, thời gian thực nghiệm giảm 40%.
Impact trực tiếp: rút ngắn đáng kể tốc độ nghiên cứu, giảm chi phí thời gian và tài nguyên GPU.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
- Làm sao đảm bảo AI không bịa số liệu khi đọc PDF có công thức/bảng phức tạp? Độ chính xác trích xuất hyperparameters thực tế là bao nhiêu?
- Nếu AI đề xuất config thử nghiệm không khả thi (ví dụ: quá lớn so với GPU hiện có), workflow sẽ xử lý như thế nào?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: Nguy cơ hallucination cao với PDF có nhiều công thức toán học, bảng số liệu dày; trích xuất params có thể sai phụ thuộc định dạng file.
- Tôi sửa gì: Thêm bước human review bắt buộc sau bước AI trích xuất; cross-check với ít nhất 1 paper khác; nếu sai thì fallback về đọc PDF trực tiếp hoặc dùng tool chuyên dụng (PDF parser + OCR).

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge
