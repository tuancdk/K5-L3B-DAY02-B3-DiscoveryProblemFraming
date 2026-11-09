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
Ban đầu, tôi chủ yếu quan tâm đến những khó khăn trong quá trình nghiên cứu AI của bản thân, chẳng hạn như tìm kiếm paper liên quan, so sánh các phương pháp và theo dõi kết quả thí nghiệm. Tuy nhiên, khi nghe các thành viên khác trình bày, tôi nhận ra mỗi người có những vấn đề khác nhau trong quá trình học tập và làm việc.

Ví dụ, nhóm đề cập đến vấn đề Git Merge Conflict, đặc biệt là khó khăn khi thiếu ngữ cảnh nghiệp vụ để hiểu mục đích của những thay đổi trong code. Trong khi đó, Anh Tuấn đề cập đến việc kiểm tra rubric, tổng hợp chi phí và xử lý lỗi môi trường lập trình.

Qua đó, tôi học được rằng một vấn đề đáng quan tâm không nhất thiết phải là một vấn đề kỹ thuật phức tạp. Điều quan trọng là xác định được vấn đề có ảnh hưởng như thế nào đến quy trình làm việc, mức độ thường xuyên xảy ra và thời gian mà người dùng phải bỏ ra để xử lý. 
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Trong quá trình thảo luận, nhóm có thể dễ dàng đi đến ý tưởng xây dựng một công cụ tự động giải quyết Git Merge Conflict. Tuy nhiên, nếu chỉ tập trung vào việc tự động gộp code thì chưa chắc đã giải quyết được khó khăn thực sự của developer.

Vấn đề không chỉ nằm ở việc Git không thể tự động merge một số thay đổi, mà còn nằm ở việc developer có thể thiếu thông tin về mục đích nghiệp vụ của những thay đổi đó. Vì vậy, nhóm cần phân biệt giữa conflict ở cấp độ code và conflict liên quan đến ý nghĩa hoặc logic của chương trình.

Để tránh solution-first, nhóm cần quay lại phân tích quy trình hiện tại, xác định điểm gây tốn thời gian và làm rõ nguyên nhân của vấn đề. Từ đó, hướng giải pháp được điều chỉnh theo hướng sử dụng AI để phân tích, giải thích và đề xuất cách xử lý, thay vì tự động quyết định merge.


**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có sự thay đổi trong cách tôi lựa chọn vấn đề cần giải quyết. Ban đầu, tôi tập trung vào vấn đề cá nhân là tìm kiếm các paper phù hợp phục vụ nghiên cứu AI. Đây là công việc tôi thường thực hiện và gặp khó khăn khi phải tìm kiếm, sàng lọc, đọc và so sánh nhiều tài liệu khác nhau.

Tuy nhiên, sau khi các thành viên trình bày top 3 problems, tôi nhận ra mỗi người đều có những khó khăn riêng và nhóm cần lựa chọn một vấn đề chung để cùng phân tích. Vì vậy, tôi chuyển sự tập trung từ vấn đề tìm kiếm paper của cá nhân sang problem mà nhóm lựa chọn.

Sự thay đổi này giúp tôi nhìn nhận vấn đề ở góc độ rộng hơn. Thay vì chỉ đánh giá một vấn đề dựa trên trải nghiệm cá nhân, tôi cần xem xét quy trình, mức độ ảnh hưởng và khả năng giải quyết vấn đề trong bối cảnh làm việc của nhóm.


**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Trong CP4 và CP5, vai trò của tôi là research và phân tích các giải pháp hiện có. Nhóm chủ yếu tìm hiểu các công cụ và giải pháp đã được phát triển, chưa thực hiện phỏng vấn người dùng hoặc khảo sát bằng survey.

Qua quá trình research, tôi nhận ra rằng các công cụ hỗ trợ so sánh code có thể giúp developer nhìn thấy sự khác biệt giữa các phiên bản, nhưng việc hiểu mục đích nghiệp vụ đằng sau những thay đổi đó là một vấn đề khác. Điều này giúp tôi phân biệt giữa khả năng xử lý conflict ở cấp độ code và khả năng hỗ trợ developer hiểu ngữ cảnh của thay đổi.

Tuy nhiên, do nhóm chưa phỏng vấn hoặc khảo sát người dùng thực tế nên tôi không thể kết luận rằng vấn đề đã được người dùng xác nhận hoặc giải pháp đề xuất chắc chắn hiệu quả. Đây cũng là một hạn chế trong quá trình kiểm chứng mà tôi nhận thấy.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó nhất đối với tôi là xác định và diễn đạt đúng vấn đề cốt lõi mà không đưa giải pháp vào quá sớm. Khi nhắc đến Git Merge Conflict, suy nghĩ đầu tiên có thể là cần một công cụ tự động merge code. Tuy nhiên, đây mới chỉ là hướng giải pháp chứ chưa thể hiện đầy đủ vấn đề mà developer đang gặp phải.

Tôi cần phân biệt giữa triệu chứng và nguyên nhân. Git báo conflict là một tình huống kỹ thuật, trong khi khó khăn lớn hơn có thể là developer không hiểu được ý định của người viết code trước đó và phải liên hệ đồng đội để bổ sung ngữ cảnh.

Ngoài ra, việc lựa chọn metric cũng là một thách thức. Nhóm cần xác định những chỉ số phù hợp như thời gian xử lý conflict và tỷ lệ lỗi logic sau khi merge. Những chỉ số này cần được đo lường thực tế, không nên nhầm lẫn giữa số liệu ước lượng, mục tiêu kỳ vọng và kết quả đã kiểm chứng.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu được thực hiện lại, tôi sẽ dành nhiều thời gian hơn cho việc thu thập bằng chứng về vấn đề trước khi tập trung nghiên cứu giải pháp. Trong vai trò Research CP4/CP5, tôi đã chủ yếu tìm hiểu các công cụ và giải pháp hiện có. Tuy nhiên, tôi nhận thấy research về công cụ chưa đủ để chứng minh rằng người dùng thực sự gặp vấn đề hoặc giải pháp đó phù hợp với quy trình của họ.

Tôi sẽ đề xuất nhóm phỏng vấn một số developer hoặc thực hiện khảo sát để hiểu rõ hơn cách họ xử lý Git Merge Conflict trong thực tế. Đồng thời, tôi sẽ chú ý phân biệt số liệu đo được, số liệu ước lượng và mục tiêu kỳ vọng để tránh đưa ra những kết luận thiếu cơ sở.

Tôi cũng sẽ phản biện nhóm mạnh hơn ở câu hỏi: "Vấn đề thực sự là Git không thể tự động merge code hay developer đang thiếu thông tin để hiểu ý định của những thay đổi?". Bên cạnh đó, cần đánh giá liệu vấn đề có nhất thiết phải sử dụng AI hay có thể giải quyết một phần bằng rule hoặc workflow thông thường. Điều này giúp nhóm tránh sử dụng AI chỉ vì muốn xây dựng một sản phẩm có AI, thay vì xuất phát từ nhu cầu thực tế.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.


Problem của nhóm là developer thiếu business context khi xử lý Git Merge Conflict, khiến họ gặp khó khăn trong việc hiểu mục đích của những thay đổi trong code. Quy trình hiện tại bắt đầu khi Git phát hiện conflict, developer phải đọc hai phiên bản code, liên hệ đồng đội để hỏi ý định thay đổi, chờ phản hồi rồi mới quyết định cách xử lý. Hai metric có thể sử dụng để đánh giá là thời gian xử lý conflict và tỷ lệ lỗi logic hoặc regression sau khi merge. Boundary của giải pháp là AI được phép phân tích commit history, PR description và Git diff để giải thích thay đổi, nhận diện rủi ro và đề xuất hướng xử lý. AI không tự ý commit hoặc merge code. Mức can thiệp phù hợp là Workflow kết hợp AI và Human-in-the-loop, thay vì Agent tự động hoàn toàn. Cuối cùng, developer vẫn là người kiểm tra đề xuất, đưa ra quyết định merge và chịu trách nhiệm về kết quả.
---

## 7. Tài liệu tham khảo

-
