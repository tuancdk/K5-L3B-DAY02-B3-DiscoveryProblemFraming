# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: B3
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi merge code bị conflict, lập trình viên trong nhóm muốn hiểu vì sao đoạn code đó được viết và hệ quả của việc giữ/xóa, để resolve đúng mà không làm hỏng tính năng của người khác (candidate #4, Đỗ Lý Hoàng Nam đề xuất)
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Lê Anh Tuấn | Khi sắp tới deadline nộp bài lab, tôi muốn biết bài còn thiếu mục nào so với yêu cầu, để không bị trừ điểm vì sai cấu trúc | Học viên tự nộp bài lab qua repo GitHub | Đối chiếu từng mục với checklist và rubric, khoảng 10 phút/lần; đã bị trừ điểm 2–3 lần | "Đã có giải pháp nào tương tự chưa? Sản phẩm này có gì tốt hơn so với các sản phẩm đó?" (Đỗ Lý Hoàng Nam) |
| 2 | Lê Anh Tuấn | Khi tới cuối tháng, tôi muốn biết mình đã tiêu bao nhiêu vào từng nhóm việc từ nhiều app ngân hàng/ví, để điều chỉnh chi tiêu tháng sau | Người dùng 2–4 app ngân hàng/ví | Phân loại giao dịch (nhất là chuyển khoản ghi nội dung mơ hồ), khoảng 15 phút/tháng; dễ bỏ dở | |
| 3 | Lê Anh Tuấn | Khi cài hoặc chạy tool/thư viện cho bài lab mà gặp lỗi, tôi muốn biết nhanh nguyên nhân và cách sửa, để không mất cả buổi sửa môi trường | Học viên tự cài môi trường trên máy cá nhân | Tìm cách sửa trên mạng và thử từng cách, khoảng 25 phút/lần; 1–2 lần/tuần | |
| 4 | Đỗ Lý Hoàng Nam | Khi merge code bị conflict, tôi muốn hiểu vì sao đoạn code đó được viết và hệ quả của việc giữ/xóa, để resolve đúng mà không làm hỏng tính năng của người khác | Lập trình viên tích hợp code trong nhóm đồ án 3–4 người | Chờ đồng đội trả lời để hiểu ngữ cảnh, 15–30 phút/lần; 1–2 lần/tuần | "Làm thế nào AI có thể biết chính xác mục đích của một đoạn code nếu không có tài liệu hoặc commit message giải thích?" (Lê Anh Tuấn); "Tại sao nên sử dụng giải pháp AI của nhóm thay vì các công cụ sẵn có như GitHub Copilot hoặc Git Merge Tools?" (Nguyễn Đức Mạnh) |
| 5 | Đỗ Lý Hoàng Nam | Khi bắt đầu bài lab có quy chế chấm dài, tôi muốn nắm ngay tiêu chí chấm và các ranh giới bị trừ điểm, để không làm lệch yêu cầu | Sinh viên đọc đề và rà soát tiêu chí cho nhóm | Đọc 15–20 trang đề (~45 phút) và đối chiếu bài với rubric trước khi nộp (~30 phút); từng bị trừ 2 điểm vì sót mục | |
| 6 | Đỗ Lý Hoàng Nam | Khi đến hạn báo cáo tiến độ đồ án hằng tuần, tôi muốn tổng hợp nhanh việc đã xong kèm minh chứng, để nộp đúng hạn mà không mất cả buổi tối | Nhóm trưởng / người viết báo cáo tiến độ | Chụp, ghép ảnh minh chứng (~20 phút) và viết lại changelog thành văn báo cáo (~25 phút); 15 tuần/kỳ | |
| 7 | Nguyễn Đức Mạnh | Khi bắt đầu một đề tài AI, tôi muốn nhanh chóng nắm nội dung, phương pháp, đóng góp, hạn chế của các paper liên quan, để không mất thời gian vào nghiên cứu không phù hợp | AI Researcher | Đọc và sàng lọc nội dung paper; thời gian chưa đo | "Nếu so sánh với việc gửi link bài báo cho Claude/ChatGPT thì sao?" (Lê Anh Tuấn) |
| 8 | Nguyễn Đức Mạnh | Khi muốn thay thế một module trong mô hình, tôi muốn tổng hợp và so sánh các phương pháp tương đồng, để chọn phương pháp phù hợp để thử nghiệm | AI Researcher / AI Engineer | Tìm, tổng hợp và so sánh phương pháp từ nhiều paper; thời gian chưa đo | |
| 9 | Nguyễn Đức Mạnh | Khi chạy nhiều experiment, tôi muốn lưu đầy đủ cấu hình và kết quả từng lần chạy, để truy xuất và so sánh được | AI Engineer / ML Researcher | Ghi nhận, truy xuất, đối chiếu cấu hình với kết quả; thời gian chưa đo | |

*Cột "Câu hỏi phản biện" điền trong buổi pitch, ghi rõ ai hỏi. Mỗi thành viên cần ít nhất 1 câu hỏi.*

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Rà soát yêu cầu bài | #1, #5 | Yêu cầu nằm rải ở nhiều file (đề, rubric, checklist); phải tự đối chiếu bài làm với yêu cầu và dễ sót mục |
| B — Hiểu "vì sao" trước khi sửa code | #3, #4 | Code hỏng (lỗi môi trường, conflict), người sửa phải tìm ra nguyên nhân hoặc ngữ cảnh trước khi dám sửa; thông tin cần nằm ở người khác hoặc rải trên mạng |
| C — Ghi nhận và tổng hợp lịch sử | #2, #6, #9 | Dữ liệu sinh ra rải rác theo thời gian (giao dịch, commit, experiment); đến lúc cần thì phải gom, phân loại, tổng hợp thủ công |
| D — Đọc và tổng hợp tài liệu nghiên cứu | #7, #8 | Đọc nhiều paper dài để lọc ra phần liên quan và so sánh các phương pháp |

*Nháp cluster do AI đề xuất từ bảng pitch; nhóm kiểm và sửa nếu cách gom khác với nhóm đã thống nhất.*

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian resolve conflict khi tích hợp code nhóm mà không làm hỏng tính năng của người khác
├── Opportunity A: Người merge không biết vì sao đồng đội sửa đoạn code đó (thiếu ngữ cảnh)
├── Opportunity B: Phải chờ đồng đội trả lời 15–30 phút mới dám quyết định giữ/xóa
└── Opportunity C: Quyết định giữ/xóa sai gây mất tính năng, chỉ phát hiện khi chạy lại
     ✗ "AI tự resolve conflict"           ← solution, gạch khỏi tầng này
     ✗ "Tool merge 3-way thông minh hơn"  ← solution, gạch khỏi tầng này
```

*Nháp dựng từ Problem Card của Nam; nhóm kiểm lại outcome và các opportunity.*

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "AI tự resolve conflict": mô tả cách giải, không phải pain.
- "Tool merge 3-way thông minh hơn": trùng với tính năng VS Code / KDiff3 đã có; Nam đã tự loại hướng này khi bị phản biện ở CP2.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #4 Hiểu ngữ cảnh khi resolve merge conflict | 5 | 4 | 4 | 4 | 3 | 5 | 5 | **30** |
| Cluster A: Rà soát yêu cầu bài, gộp #1 "Rà soát bài trước khi nộp" (Tuấn) và #5 "Nắm tiêu chí chấm và ranh giới trừ điểm của đề lab" (Nam) | 5 | 5 | 3 | 4 | 5 | 3 | 4 | 29 |
| #7 Đọc và sàng lọc paper | 4 | 4 | 2 | 2 | 3 | 3 | 3 | 21 |

*Nháp do AI đề xuất dựa trên các Problem Card; nhóm thảo luận và sửa điểm trước khi chốt.* Lý do chính của từng mức điểm:

- **#4:** cả 3 thành viên đều code nhóm nên hiểu domain (5); có sự cố cụ thể là bị ghi đè mất 1 hàm, cả nhóm mất thêm 1 giờ debug (pain 4); so sánh được rõ 4 mức: No AI = quy ước commit message/PR description, Rule = CI chạy test sau merge, Workflow = AI tóm tắt ngữ cảnh hai nhánh rồi người quyết định, Agent = AI tự resolve (5); domain kỹ thuật sâu, dễ trượt phạm vi trong một buổi lab (vừa sức 3); con số "15% regression bug" chưa rõ nguồn đo (impact 4).
- **Cluster A:** hai candidate cùng pattern nên chấm chung. #1 (Tuấn): rà soát 15–20 phút mỗi lần nộp, đã bị trừ điểm 2–3 lần. #5 (Nam): đọc 15–20 trang đề khoảng 45 phút và đối chiếu bài với rubric khoảng 30 phút, từng bị trừ 2 điểm vì sót mục. Quy trình rất rõ và làm được ngay trong lab (5); số liệu của #1 mới là ước lượng, chưa bấm giờ (pain 3); checklist hoặc script kiểm cấu trúc (Rule) gần như đủ, ít không gian để so sánh các mức (3).
- **#7:** thời gian và tần suất chưa đo, metric chỉ ghi "giảm so với baseline" (pain 2, impact 2); công cụ có sẵn đã làm được phần lớn (xem câu hỏi phản biện ở dòng 7).

**Candidate được chọn:** #4: Khi merge code bị conflict, tôi muốn hiểu vì sao đoạn code đó được viết và hệ quả của việc giữ/xóa, để resolve đúng mà không làm hỏng tính năng của người khác.

**Vì sao chọn:** Điểm cao nhất shortlist; cả nhóm đều gặp khi làm đồ án nên dễ kiểm chứng; có sự cố thật với hậu quả rõ (mất tính năng, 1 giờ debug); so sánh được đủ 4 mức No AI / Rule / Workflow / Agent. Hai câu phản biện nhận được (AI lấy ngữ cảnh từ đâu khi thiếu commit message; vì sao không dùng Copilot/merge tool có sẵn) là hai giả định quan trọng nhất, sẽ kiểm chứng ở CP4.

**Vì sao loại các candidate còn lại:**

- **Cluster A, gồm #1 "Rà soát bài trước khi nộp" (Tuấn) và #5 "Nắm tiêu chí chấm và ranh giới trừ điểm của đề lab" (Nam):** checklist một trang hoặc script kiểm cấu trúc (Rule) nhiều khả năng đã giải phần lớn, ít không gian để phân tích các mức can thiệp AI; số liệu mới là ước lượng. Ghi vào hướng tiếp theo.
- **#7 (Đọc và sàng lọc paper):** chưa có số liệu đo về thời gian và tần suất; như câu phản biện "so với gửi link cho Claude/ChatGPT thì sao?", công cụ có sẵn đã làm được phần lớn việc tóm tắt paper.
- Các candidate khác (#2, #3, #6, #8, #9) không vào shortlist sau khi gom cluster: hoặc trùng pattern với candidate đã chọn (#3 cùng cluster B), hoặc thiếu số liệu đo (#8, #9), hoặc là việc cá nhân, ít người trong nhóm cùng gặp (#2).

**Xử lý bất đồng (nếu có):** ⚠️ CẦN ĐIỀN: ghi "Không có" nếu cả nhóm đồng thuận, hoặc ghi ai muốn chọn candidate khác và nhóm xử lý thế nào.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
