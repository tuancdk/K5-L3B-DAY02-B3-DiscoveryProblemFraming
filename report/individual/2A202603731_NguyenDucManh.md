# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:
- MSSV:2A202603731
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: B3
- Link repo nhóm: https://github.com/tuancdk/K5-L3B-DAY02-B3-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi tôi muốn đọc thật nhanh một paper để xác định nội dung paper giải quyết vấn đề gì, phương pháp gì, đóng góp gì và có hạn chế gì để quyết định paper có liên quan đến một đề tài tôi nghiên cứu hay không| Người nghiên cứu | số paper/tuần|
| 2 |Tổng hợp thông tin | Khi tôi cần so sánh các phương pháp tương đương để đánh giá ưu điểm cũng như hạn chế của từng phương pháp để có thể lựa chọn phương pháp phù hợp thay thế cho phương pháp tương đương trong model của tôi để rút ngắn thời gian train mô hình |AI Researcher, AI Engineer |Số paper/lần, thời gian tổng hợp |
| 3 | Lặp lại | Khi chạy nhiều experiment, tôi muốn ghi lại cấu hình của các lần chạy và kết quả của các lần chạy để có thể truy xuất và so sánh các lần chạy | AI Engineer, ML Researcher| Experiment / tuần, phút ghi log |
| 4 | Tốn thời gian | Khi mô hình huấn luyện gặp lỗi, tôi muốn nhận được thông báo mô hình đã dừng huấn luyện ngay lập tức và xác định nguyên nhân từ log, cấu hình để tiếp tục công việc mà không mất quá nhiều thời gian debug|AI Engineer/ ML Engineer | Số lần debug/tuần, thời gian/lỗi |
| 5 | Tổng hợp thông tin | Khi đánh giá một mô hình, tôi muốn tổng hợp các metric của nhiều experiment khác nhau để biết thay đổi nào thật sự giúp mô hình được cải thiện hơn|AI Engineer, ML Researcher |Số experiment, số metric, thời gian tổng hợp |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tìm các paper liên quan(#1) | Khi nghiên cứu hay triển khai một dự án về AI, điều cần quan tâm nhất là biết rõ cách những người trước đã làm được chưa và đã làm như thế nào, họ thành công ở đâu để có thể nhanh chóng tiếp cận, hiểu rõ phương pháp và nhanh chóng có thể năm bắt đưa ra các cải tiến mới | Các paper có thể nhắc ít tới phương pháp chứ chưa thật sự chủ đề là về phương pháp đó có thể gây mất thời gian để đọc.|
| 2 |Tổng hợp, khái quát và so sánh các paper có phương pháp liên quan với phương pháp trong mô hình mà tôi muốn thay thế để thử nghiệm cải tiến(#2) | Khi muốn cải tiến một module trong mô hình học sâu hay mô hình học máy, có một rào cản là không biết phương pháp muốn thay thế có các phương pháp nào khác có cùng ý tưởng hay không, việc tổng hợp và tìm các phương pháp liên quan giúp rút ngắn thời gian nghiên cứu và cải tiến mô hình | Các phương pháp liên quan có thể chưa thật sự phù hợp với mô hình hiện tại|
| 3 | Theo dõi và quản lý cấu hình, kết quả của nhiều experiment| Khi thực hiện nhiều experiment trong quá trình phát triển mô hình, việc ghi lại cấu hình và kết quả giúp tôi truy xuất, đối chiếu và xác định những thay đổi có ảnh hưởng đến hiệu suất mô hình. | Khi thực hiện nhiều experiment trong quá trình phát triển mô hình, việc ghi lại cấu hình và kết quả giúp tôi truy xuất, đối chiếu và xác định những thay đổi có ảnh hưởng đến hiệu suất mô hình.|

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu nghiên cứu một đề tài hoặc phát triển một dự án AI, tôi muốn nhanh chóng tìm và nắm được nội dung, phương pháp, đóng góp và hạn chế của các paper liên quan, để xác định hướng nghiên cứu và tránh mất thời gian tìm hiểu những nghiên cứu không phù hợp. |
| Actor | AI Researcher |
| Thời điểm / bối cảnh | Khi bắt đầu một đề tài nghiên cứu mới hoặc cần tìm hiểu một hướng tiếp cận cho dự án AI. |
| Quy trình hiện tại (3–7 bước) | 

1. Xác định chủ đề và từ khóa nghiên cứu. 
2. Tìm kiếm paper trên Google Scholar, arXiv hoặc các nguồn học thuật. 
3. Đọc tiêu đề và abstract để chọn paper tiềm năng. 
4. Đọc các phần Introduction, Method và Experiments. 
5. Ghi chú vấn đề nghiên cứu, phương pháp, đóng góp và hạn chế. 
6. Đánh giá mức độ liên quan của paper với đề tài đang thực hiện.  |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước đọc và sàng lọc nội dung paper. Một paper có thể chỉ đề cập đến phương pháp cần tìm hiểu mà không tập trung phân tích phương pháp đó. Thời gian thực tế: Chưa đo. |
| Impact (nếu không giải thì sao) | Mất nhiều thời gian tìm hiểu các nghiên cứu không thực sự liên quan, khó nắm bắt nhanh các hướng tiếp cận đã có và có thể bỏ sót những nghiên cứu quan trọng.|
| Success metric (baseline → target) |Thời gian trung bình để sàng lọc một paper: chưa đo → giảm so với baseline. Tỷ lệ paper được xác định đúng mức độ liên quan: chưa đo → tăng so với baseline. |
| Phương án không dùng AI | Xây dựng bộ từ khóa tìm kiếm, sử dụng bộ lọc theo năm, lĩnh vực và mức độ liên quan; tạo checklist đọc paper và bảng ghi chú thống nhất.|
| Giả thuyết về AI (nếu có) |AI có thể hỗ trợ trích xuất và tổng hợp các thông tin chính từ paper như vấn đề nghiên cứu, phương pháp, đóng góp, kết quả và hạn chế, giúp người nghiên cứu sàng lọc nhanh hơn. |
| Cảm nhận nhanh | Workflow / Agent |

Quy trình nháp hiện tại:

```text
    Từ khóa nghiên cứu → Tìm kiếm paper → Đọc tiêu đề và abstract → Chọn paper tiềm năng → Đọc các phần quan trọng → Ghi chú nội dung → Đánh giá mức độ liên quan.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi muốn cải tiến hoặc thay thế một module trong mô hình học sâu/học máy, tôi muốn tổng hợp và so sánh các phương pháp có ý tưởng hoặc chức năng tương đồng, để lựa chọn phương pháp phù hợp và có tiềm năng cải thiện mô hình hiện tại. |
| Actor | AI Researcher / AI Engineer |
| Thời điểm / bối cảnh | 

Khi phân tích một module đang sử dụng trong mô hình và muốn tìm phương pháp thay thế hoặc cải tiến. |
| Quy trình hiện tại (3–7 bước) | 
1. Xác định module hoặc phương pháp đang sử dụng. 
 2. Tìm hiểu nguyên lý hoạt động và vai trò của module. 
 3. Tìm kiếm paper đề xuất các phương pháp có chức năng hoặc ý tưởng tương đồng. 
 4. Đọc và ghi chú cách hoạt động của từng phương pháp. 
 5. So sánh ưu điểm, hạn chế và yêu cầu tính toán. 
 6. Đánh giá khả năng tích hợp vào kiến trúc hiện tại. 
 7. Chọn phương pháp tiềm năng để thử nghiệm.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước tìm kiếm, tổng hợp và so sánh các phương pháp từ nhiều paper. Khó khăn nằm ở việc thông tin được trình bày theo các cách khác nhau và không phải phương pháp nào có ý tưởng tương đồng cũng phù hợp với mô hình hiện tại. Thời gian thực tế: chưa đo.|
| Impact (nếu không giải thì sao) | Mất nhiều thời gian nghiên cứu, khó đánh giá toàn diện các phương pháp thay thế và có thể lựa chọn phương pháp không phù hợp với kiến trúc hoặc mục tiêu của mô hình.|
| Success metric (baseline → target) |Thời gian cần để tổng hợp và so sánh một nhóm phương pháp: chưa đo → giảm so với baseline. Tỷ lệ phương pháp được lựa chọn có thể tích hợp và thử nghiệm thành công: chưa đo → tăng so với baseline. |
| Phương án không dùng AI | Xây dựng bảng so sánh với các tiêu chí thống nhất: nguyên lý, độ phức tạp tính toán, bộ nhớ, ưu điểm, hạn chế, yêu cầu đầu vào và khả năng tích hợp.|
| Giả thuyết về AI (nếu có) | AI có thể hỗ trợ trích xuất thông tin từ nhiều paper, phân nhóm các phương pháp theo ý tưởng hoặc chức năng, sau đó tổng hợp ưu điểm, hạn chế và điểm khác biệt để người nghiên cứu đánh giá.|
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
Xác định module cần cải tiến → Tìm hiểu module hiện tại → Tìm paper về các phương pháp tương đồng → Đọc và ghi chú → Tổng hợp và so sánh → Đánh giá khả năng tích hợp → Chọn phương pháp để thử nghiệm.
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | 

Khi thực hiện nhiều experiment trong quá trình phát triển mô hình AI, tôi muốn lưu lại đầy đủ cấu hình và kết quả của từng lần chạy, để có thể truy xuất, so sánh và xác định những thay đổi ảnh hưởng đến hiệu suất mô hình. |
| Actor |AI Engineer / ML Researcher.|
| Thời điểm / bối cảnh |Khi huấn luyện, tinh chỉnh hoặc thử nghiệm nhiều cấu hình khác nhau của một mô hình. |
| Quy trình hiện tại (3–7 bước) | 
1. Xác định cấu hình experiment cần chạy. 
 2. Thay đổi hyperparameters hoặc module trong mô hình. 
 3. Khởi chạy quá trình training. 
 4. Theo dõi log và quá trình huấn luyện. 
 5. Ghi nhận cấu hình và kết quả sau khi chạy. 
 6. So sánh kết quả với các experiment trước đó.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước ghi nhận, truy xuất và đối chiếu cấu hình với kết quả của nhiều experiment. Thời gian thực tế và tần suất gặp vấn đề: chưa đo.|
| Impact (nếu không giải thì sao) | Khó tái hiện kết quả, dễ nhầm lẫn giữa các cấu hình, khó xác định nguyên nhân khiến hiệu suất thay đổi và có thể phải thực hiện lại experiment.|
| Success metric (baseline → target) | 

Thời gian truy xuất thông tin một experiment: chưa đo → giảm so với baseline. Tỷ lệ experiment có đầy đủ cấu hình và kết quả: chưa đo → tiến tới 100%.|
| Phương án không dùng AI | 

Sử dụng file CSV/Excel hoặc một hệ thống quản lý experiment để lưu cấu hình, log, metric và checkpoint theo mã experiment thống nhất.|
| Giả thuyết về AI (nếu có) | 

AI có thể hỗ trợ phân tích lịch sử experiment, phát hiện xu hướng trong kết quả và gợi ý những yếu tố đáng kiểm tra tiếp theo. Tuy nhiên, việc ghi nhận và quản lý dữ liệu có thể thực hiện bằng workflow thông thường.|
| Cảm nhận nhanh | Workflow|

Quy trình nháp hiện tại:

```text
Xác định cấu hình → Chạy training → Theo dõi log → Ghi nhận kết quả và cấu hình → Lưu trữ → So sánh các experiment.
```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

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
