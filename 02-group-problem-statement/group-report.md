# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1   | Nguyễn Văn Ước | 2A202602445 | Leader (Facilitator) |
| 2   | Chu Minh Quân | 2A202602709 | Thành viên |
| 3   | Trần Trọng Chinh | 2A202602720 | Thành viên |
| 4   | Đinh Thị Minh Tâm | 2A202602433 | Thành viên |
| 5   | Nguyễn Khắc Quang | 2A202602885 | Thành viên |
| 6   | Nguyễn Việt Thành | 2A202602924 | Thành viên |

**Candidate problem nhóm chọn (1 câu):**

Tự động hóa soạn thảo dự thảo Báo cáo bài tập lớn Word 40–60 trang từ Codebase và Schema DB, giúp sinh viên giảm thời gian viết tài liệu từ 210 phút xuống dưới 60 phút mà vẫn đảm bảo 100% chuẩn format quy định của khoa.

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Nguyễn Việt Thành | Xử lý sự cố trừ tiền ví điện tử / thẻ ngân hàng mà không có chuyến xe Xanh SM (Green SM) | Sinh viên, Khách đi xe Xanh SM & Chuyên viên CSKH | Đối soát thủ công giữa cổng ví điện tử (MoMo/ZaloPay) và hệ thống máy chủ chuyến xe bị ngâm từ 3–7 ngày làm việc | Pain thật, gây ức chế tài chính lớn nhất vì sinh viên bị giam tiền cuối tháng; có nhiều phản ánh thực tế từ cộng đồng sinh viên và khiếu nại chưa được xử lý kịp thời; workflow tuyến tính, đo lường được hiệu quả rõ ràng khi tự động hóa đối soát hoàn tiền. |
| 2 | Nguyễn Việt Thành | Đọc & hiểu kết quả xét nghiệm y khoa sơ bộ trên App MyVinmec cho sinh viên / người trẻ | Sinh viên, Người trẻ khám sức khỏe & Bác sĩ tư vấn Vinmec | Sinh viên không hiểu thuật ngữ y khoa viết tắt, tự tra Google 30–45 phút gây lo âu bệnh tật quá mức (Cyberchondria), vào phòng khám hỏi dồn dập làm mất thời gian bác sĩ | AI/LLM phát huy tối đa thế mạnh tóm tắt thuật ngữ y khoa bình dân; tuy nhiên domain y tế nhạy cảm, rủi ro ảo giác (hallucination) cao, bắt buộc phải có ranh giới con người (Human Boundary) nghiêm ngặt. |
| 3 | Chu Minh Quân | Viết Pull Request description chi tiết (tóm tắt logic code thay đổi, dependencies mới, hướng dẫn test) khi merge code | Thành viên tạo PR & Người review/merge code (cả nhóm) | Đọc diff và gõ tóm tắt tính năng bằng tay mất 20–25 phút/PR (6–8 PR/tuần); viết sơ sài dễ lọt bug hoặc conflict | Tần suất lặp lại cao, dữ liệu git diff có cấu trúc rõ; phù hợp làm Workflow tự động hóa tóm tắt code; kiểm chứng được ngay trên repo GitHub. |
| 4 | Chu Minh Quân | Rà soát, chuẩn hóa định dạng và lọc nhiễu tập dữ liệu câu hỏi - đáp (QA dataset) thu thập thủ công | 4 thành viên thu thập/gán nhãn & người huấn luyện mô hình | Đối chiếu thủ công từng cặp QA với guideline mất 3.5–4 tiếng/đợt (định kỳ 2 tuần/lần); tỷ lệ lỗi format hoặc nhãn ước tính khoảng 15–20% | Phù hợp thế mạnh hiểu ngôn ngữ của LLM; giải quyết trực tiếp chất lượng dữ liệu mô hình; cần tính toán chi phí API và ranh giới con người duyệt ca khó. |
| 5 | Trần Trọng Chinh | Phân loại và copy-paste thủ công bug report / feedback từ kênh Discord, Google Form vào Jira backlog | Product Owner, QA / Support & Dev team | Đọc tin nhắn lộn xộn, chuẩn hóa format lỗi và gán tag vào Jira mất 60 phút/ngày | Quy trình lặp lại hàng ngày rất rõ; đo lường thời gian chính xác (60'/ngày); nhưng chất lượng input Discord đa dạng (tiếng lóng, viết tắt, ảnh mờ) làm tăng rủi ro trích xuất sai. |
| 6 | Trần Trọng Chinh | Trích xuất User Story và Acceptance Criteria (AC) từ biên bản họp thô (raw meeting transcript) với khách hàng/mentor | Business Analyst / Nhóm trưởng & Khách hàng, Mentor | Lọc yêu cầu từ transcript dài mất 45 phút/buổi họp, dễ sót yêu cầu ngầm và mất thời gian format | Giải quyết đúng nỗi đau sót yêu cầu sau họp; đầu ra User Story + AC có format chuẩn mực; thách thức ở tiếng Việt khẩu ngữ ngắt quãng và nói chen ngang. |
| 7 | Nguyễn Khắc Quang | Tổng hợp và phân loại phản hồi người dùng xe điện VinFast từ App Store, Google Play và cộng đồng thành nhóm vấn đề & insight có cấu trúc | Product Team, Customer Service, Service Center & Khách hàng | Review nằm rải rác đa kênh, không được gom cụm theo mức độ nghiêm trọng và chủ đề (pin, trạm sạc, app) dẫn đến xử lý chậm | Domain thực tế quy mô lớn với lượng xe và người dùng lưu hành tăng trưởng nhanh; dữ liệu review App Store/Google Play công khai dễ thu thập; LLM phân loại sentiment và gom cụm rất tốt. |
| 8 | Nguyễn Khắc Quang | Trợ lý tra cứu thông tin hướng dẫn sử dụng xe điện, vị trí trạm sạc và chính sách bảo hành VinFast từ nhiều tài liệu rời rạc | Chủ xe VinFast mới, Khách hàng tiềm năng & Tổng đài CSKH | Người dùng mới mất nhiều thời gian tra cứu sách hướng dẫn dày hàng trăm trang và website; hay phải gọi lên tổng đài hỏi các câu hỏi lặp lại | Bài toán RAG/Search tài liệu rất trực quan, có tài liệu PDF HDSD chính thức; nhưng dễ trượt sang hướng "làm chatbot chung chung" nếu không có kịch bản và ranh giới rõ ràng. |
| 9 | Đinh Thị Minh Tâm | Làm rõ yêu cầu phân tích dữ liệu mơ hồ từ bộ phận kinh doanh (Ambiguous Analytics Request) thành đặc tả kỹ thuật rõ ràng | Data Analyst & Business Stakeholders | Yêu cầu kinh doanh mơ hồ, thiếu bối cảnh khiến DA phải hỏi lại nhiều vòng (clarification rounds), tỷ lệ làm lại (rework) cao | Bài toán kết hợp Data + Business rất hay; LLM có thế mạnh hiểu ngữ cảnh kinh doanh và gợi ý metric/schema phân tích; điểm can thiệp AI rất rõ. |
| 10 | Đinh Thị Minh Tâm | Tìm và tổng hợp hạn chót nộp bài từ nhiều nguồn rải rác (Student Deadline Overload) cho sinh viên | Sinh viên & Ban cán sự lớp | Thông báo deadline phân tán trên LMS, Zalo, Teams, email khiến sinh viên tốn thời gian tra cứu và dễ bỏ quên deadline quan trọng | Rất gần gũi với sinh viên, dễ làm phỏng vấn (interview) và kiểm chứng ngay trong lớp; giải pháp phù hợp với Workflow trích xuất thông tin. |
| 11 | Nguyễn Văn Ước | Soạn thảo dự thảo Báo cáo bài tập lớn Word 40–60 trang từ Codebase và Schema DB | Sinh viên phụ trách viết báo cáo & Trưởng nhóm bài tập lớn | Đọc lại code của cả nhóm để viết mô tả chức năng, kẻ bảng API và dàn trang Word mất 3–4 tiếng trước mỗi đợt nộp | Xuất hiện ở mọi môn học cuối kỳ, tốn nhiều công sức nhất; quy trình rõ ràng (từ code $\rightarrow$ mô tả $\rightarrow$ dàn trang); đo lường được ngay bằng thời gian. |
| 12 | Nguyễn Văn Ước | Bóc tách đề bài & Rubric 10–15 trang tiếng Anh thành Checklist Task và tiêu chí nộp bài | Nhóm trưởng môn học & Thành viên nhóm | Đọc hiểu tài liệu dài tiếng Anh mất 1.5–2 tiếng; hay bị bỏ sót các yêu cầu phụ/tiêu chí ẩn của rubric khiến bị trừ điểm oan | Giải quyết ngay khâu đầu vào của dự án, tránh rủi ro làm lệch yêu cầu; dữ liệu đầu vào là file PDF spec/rubric rõ ràng. |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| **A. Hỗ trợ quy trình Kỹ thuật & Báo cáo Đồ án** | • #3: Viết PR description<br>• #11: Viết báo cáo bài tập lớn từ Codebase<br>• #12: Bóc tách Rubric thành Checklist Task | Dữ liệu đầu vào kỹ thuật (code diff, schema database, file PDF đề bài); chuyển hóa từ dữ liệu kỹ thuật sang tài liệu báo cáo/task có cấu trúc theo quy chuẩn. | Gần gũi và thực tế nhất với sinh viên CNTT; dữ liệu nội bộ có sẵn trong lab; workflow rõ ràng; con người kiểm duyệt dễ dàng trước khi nộp. |
| **B. Phân loại & Xử lý Ticket / Phản hồi người dùng** | • #1: Sự cố trừ tiền ví điện tử Xanh SM<br>• #5: Phân loại bug Discord vào Jira<br>• #7: Phân loại review xe điện VinFast | Tiếp nhận dữ liệu người dùng đa kênh (tin nhắn lỗi, đánh giá app, khiếu nại giao dịch); phân loại theo chủ đề/mức độ nghiêm trọng; tự động hóa đối soát hoặc điều hướng backlog. | Tác động kinh doanh (ROI) và độ bức xúc của user rất lớn; tuy nhiên dữ liệu thật thường thuộc diện bảo mật của doanh nghiệp (Xanh SM, VinFast). |
| **C. Chuyển hóa Yêu cầu mơ hồ & Trích xuất Tài liệu chuyên sâu** | • #6: Trích xuất User Story + AC từ meeting transcript<br>• #8: Tra cứu HDSD và chính sách xe điện VinFast<br>• #9: Làm rõ yêu cầu phân tích dữ liệu DA | Xử lý văn bản phi cấu trúc, dài hoặc mơ hồ (biên bản họp khẩu ngữ, sách HDSD hàng trăm trang, yêu cầu nghiệp vụ sơ sài); bóc tách thành format chuẩn phục vụ ra quyết định. | Tận dụng tối đa thế mạnh đọc hiểu ngữ cảnh của LLM; thách thức nằm ở việc lọc nhiễu tiếng Việt khẩu ngữ và kiểm soát nguy cơ hallucination. |
| **D. Chuẩn hóa Dữ liệu & Trợ lý Đời sống - Sức khỏe** | • #2: Giải thích xét nghiệm y khoa App Vinmec<br>• #4: Rà soát & lọc nhiễu QA dataset<br>• #10: Tổng hợp deadline sinh viên từ nhiều nguồn | Thu thập, lọc thông tin phân tán hoặc thuật ngữ chuyên ngành phức tạp (chỉ số y tế, lịch nộp bài, cặp câu hỏi - đáp) để cung cấp thông tin tinh gọn, dễ hiểu cho người dùng. | Ý tưởng hữu ích cho đời sống cá nhân; tuy nhiên bài y tế có rủi ro trách nhiệm pháp lý cao, bài deadline gặp rào cản phân mảnh quyền truy cập tài khoản. |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

> **7 câu hỏi thẩm định:**
> 1. Có ai trong nhóm hiểu workflow thật đủ sâu không?
> 2. Actor có cụ thể không?
> 3. Bottleneck có phải một bước cụ thể không?
> 4. Impact có thể đo không?
> 5. Có thể vẽ before/after workflow không?
> 6. Có thể so sánh Rule / Workflow / Agent không?
> 7. Có quá rộng cho lab hôm nay không?

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| **#11: Soạn thảo dự thảo Báo cáo bài tập lớn Word 40–60 trang từ Codebase & Schema DB** (Nguyễn Văn Ước) | • Cả 6 thành viên đều là sinh viên năm 4, trực tiếp trải qua workflow hàng kỳ nên hiểu sâu từng bước.<br>• Bottleneck cực kỳ cụ thể (bước kẻ bảng API & viết diễn giải luồng tính năng chiếm khoảng 95').<br>• Metric đo lường định lượng rõ ràng (giảm từ khoảng 3.5 tiếng $\rightarrow$ dưới 1 tiếng, bám sát format khoa); dữ liệu code/DB có sẵn trong lab để thử nghiệm ngay; scope vừa vặn hoàn hảo. | • Nguy cơ AI bị quá tải context hoặc "ảo giác" (hallucination) tham số nếu codebase quá lớn.<br>• Định dạng xuất ra Word dễ bị lệch bảng biểu nếu không có script Rule định hình khung trước. |
| **#1: Xử lý sự cố trừ tiền ví điện tử / thẻ ngân hàng không có chuyến xe Xanh SM** (Nguyễn Việt Thành) | • Pain point thực tế gây bức xúc tài chính, thành viên nhóm từng gặp và ghi nhận nhiều phản ánh khiếu nại thực tế từ người dùng.<br>• Workflow đối soát 2 chiều (ví điện tử $\leftrightarrow$ máy chủ chuyến xe) mang tính logic, tuyến tính và rõ ràng.<br>• Đo lường hiệu quả rõ rệt (rút ngắn thời gian hoàn tiền từ nhiều ngày làm việc xuống dưới 15 phút); phân định rõ Rule (đối soát tự động) vs Human (duyệt ca tranh chấp). | • Không có quyền truy cập trực tiếp vào hệ thống cơ sở dữ liệu và API nội bộ của GSM, nhóm chỉ có thể xây dựng luồng giả lập (mock data).<br>• Rào cản bảo mật dữ liệu giao dịch tài chính người dùng. |
| **#3: Viết Pull Request (PR) description chi tiết từ Git diff khi merge code** (Chu Minh Quân) | • Quy trình kỹ thuật diễn ra hàng tuần (6–8 PR/tuần), actor lập trình viên rất quen thuộc.<br>• Dữ liệu đầu vào chuẩn mực và có cấu trúc cao (`git diff`, commit log, file changes).<br>• Có thể thử nghiệm trực tiếp ngay trên GitHub repo của nhóm trong buổi lab; so sánh Rule/Workflow/Agent rất tường minh. | • AI có thể chỉ tóm tắt lại thay đổi cú pháp code bề mặt mà không nắm bắt được dụng ý nghiệp vụ (business logic) nếu commit của thành viên viết cẩu thả.<br>• Impact phạm vi hẹp hơn so với việc viết cả báo cáo bài tập lớn. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **#11: Soạn thảo dự thảo Báo cáo bài tập lớn Word 40–60 trang từ Codebase & Schema DB** | 5 | 4 | 4 | 4 | 5 | 4 | 4 | **30** |
| **#3: Viết Pull Request (PR) description chi tiết từ Git diff khi merge code** | 4 | 4 | 4 | 3 | 4 | 4 | 4 | **27** |
| **#1: Xử lý sự cố trừ tiền ví điện tử / thẻ ngân hàng không có chuyến xe Xanh SM** | 4 | 3 | 5 | 4 | 2 | 3 | 4 | **25** |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
#11: Soạn thảo dự thảo Báo cáo bài tập lớn Word 40–60 trang từ Codebase và Schema DB (Nguyễn Văn Ước)
```

**Vì sao chọn (4-5 câu):**

```text
1. Cả 6 thành viên trong nhóm đều là sinh viên năm 4 CNTT, đang trực tiếp đối mặt với đồ án tốt nghiệp và các bài tập lớn cuối kỳ nên nắm bắt trọn vẹn từng bước trong quy trình thực tế mà không cần giả định.
2. Dữ liệu đầu vào (mã nguồn, cấu trúc database, file template Word chuẩn của khoa) có sẵn ngay trên máy tính của các thành viên, giúp nhóm có thể kiểm chứng, chạy thử nghiệm và đo lường ngay trong 4 tiếng của buổi lab.
3. Điểm nghẽn (bottleneck) tại khâu đọc code để kẻ bảng API và viết diễn giải luồng tính năng cực kỳ rõ ràng, chiếm khoảng 45,2% tổng thời gian làm báo cáo (95/210 phút), thống nhất với phân tích quy trình.
4. Tác động đo lường được định lượng rất sắc nét: cắt giảm từ khoảng 3.5 tiếng (210 phút) xuống còn khoảng 1 tiếng (~55 phút) và hạn chế tối đa các lỗi lệch định dạng theo mẫu quy định của trường.
5. Ranh giới con người kiểm duyệt (Human Boundary) cực kỳ tự nhiên: AI hỗ trợ soạn thảo dự thảo thô và trích xuất tham số, sinh viên bắt buộc chịu trách nhiệm rà soát logic chuyên môn trước khi xuất file nộp điểm thật.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
• Đối với bài #1 (Xử lý sự cố trừ tiền ví điện tử Xanh SM): Dù có nỗi đau tài chính rất thực tế và nhiều phản ánh từ người dùng, nhóm không thể truy cập vào hệ thống cơ sở dữ liệu và API đối soát nội bộ của bên dịch vụ. Nếu làm trong lab, nhóm buộc phải dùng dữ liệu giả lập (mock data), làm giảm tính xác thực của việc kiểm chứng và khó triển khai pilot thực tế.
• Đối với bài #3 (Viết Pull Request description chi tiết từ Git diff): Bài toán này rất khả thi về mặt kỹ thuật, tuy nhiên phạm vi tác động (impact) chỉ nằm ở mức độ viết tóm tắt commit nội bộ giữa các dev với nhau. So với bài viết toàn bộ báo cáo Word 40–60 trang để chấm điểm môn học, bài toán PR description có quy mô hẹp hơn và khó thể hiện sự phối hợp đa dạng giữa Rule-based và AI Workflow bằng bài báo cáo.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
• Ban đầu bạn Thành và bạn Quang rất ủng hộ bài toán Xanh SM (#1) vì tính thực tiễn cao, chạm đúng nỗi bức xúc lớn của sinh viên khi bị giam tiền cuối tháng và có ROI kinh doanh rất rõ.
• Tuy nhiên, sau khi bạn Ước và bạn Quân phân tích về rào cản "Không thể tiếp cận hệ thống backend thật của bên dịch vụ xe trong buổi lab" và nguy cơ bài toán bị thiên về Rule-based đối soát database thuần túy, nhóm đã thảo luận lại.
• Nhóm đồng thuận chọn bài Báo cáo bài tập lớn (#11) vì vừa giải quyết nỗi đau trực tiếp của hầu hết thành viên, vừa có sẵn dữ liệu thật để validate và xây dựng workflow hoàn chỉnh ngay tại lớp.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| **Phỏng vấn trực tiếp các thành viên trong nhóm** | 3 thành viên nhóm (Chu Minh Quân, Trần Trọng Chinh, Nguyễn Việt Thành) | • **Chu Minh Quân (Backend & API):** *"Kỳ trước làm bài tập lớn Web, mình mất gần 2 tiếng chỉ để mở từng controller dò endpoint kẻ bảng Word 20 API. Lúc code sửa kiểu dữ liệu từ string sang int mà trong Word quên update, lúc thầy vấn đáp soi ra là bị trừ 0.5 điểm ngay."*<br>• **Trần Trọng Chinh (Testing & Docs):** *"Sát deadline nộp 23h59, cả nhóm mới gom code lại. Mình phải thức trắng đêm đến 4h sáng chỉ để căn chỉnh font Times New Roman 13, giãn dòng 1.5 và format lại các bảng biểu bị tràn lề giấy Word."*<br>• **Nguyễn Việt Thành (Frontend):** *"Kỳ trước nhóm mình từng bị trừ 1.0 điểm trình bày vì bảng schema DB và tham số API lệch so với code trên GitHub do bạn viết tự gõ tay lại."* | • Chu Minh Quân: *"Nếu môn nào thầy cho nộp kèm link Postman hoặc Swagger export thì chỉ cần xuất file JSON là xong, không phải gõ tay nhiều."*<br>• Trần Trọng Chinh: *"Sợ nhất dùng AI viết văn báo cáo thì văn phong bị sáo rỗng, kiểu 'Hệ thống này đóng vai trò vô cùng quan trọng...', đọc vào thầy biết ngay là copy ChatGPT."* | Nhóm nhận ra: Không phải môn nào giảng viên cũng nhận link Postman/Swagger mà bắt buộc có văn bản Word đóng tập. Đồng thời ghi nhận phản bác về văn phong: **AI tuyệt đối không viết văn sáo rỗng**, chỉ đóng vai trò tóm tắt luồng kỹ thuật (Input $\rightarrow$ Process $\rightarrow$ Output) và trích xuất tham số; sinh viên trực tiếp viết phần phân tích kết quả thử nghiệm. |
| **Khảo sát mở rộng sinh viên trong lớp** | 10 sinh viên năm 4 cùng khóa | • **9/10 sinh viên được khảo sát** xác nhận từng phải thức khuya, thậm chí thức trắng đêm trước ngày nộp chỉ để format báo cáo Word và chụp ảnh giao diện demo.<br>• **8/10 sinh viên được khảo sát** từng bị trừ từ 0,5 đến 1,5 điểm vì lỗi định dạng bảng biểu, thiếu chú thích hình hoặc lệch format chuẩn của khoa. | 2 bạn cho rằng: *"Nếu phân công một bạn chuyên viết báo cáo từ tuần thứ 8 thì sẽ không bị dồn việc vào tuần cuối."* | Xác nhận điểm nghẽn lớn nhất là việc gom dữ liệu phân tán và gõ tay cơ học sát hạn chót; cần cơ chế tự động hóa trích xuất từ codebase để giảm tải công sức. |
| **Ghi nhận từ nhận xét đồ án kỳ trước** | Các bài tập lớn đã bảo vệ của các thành viên | • 3/3 thành viên được hỏi đều xác nhận từng có bài bị giảng viên ghi chú: *"Báo cáo thiếu mô tả chi tiết các tham số request/response, bảng mục lục bị lỗi font, một số bảng biểu tràn lề in ấn."* | Nhóm có điểm trình bày tối đa là nhóm dùng template chuẩn và kiểm tra chéo kỹ lưỡng trước khi nộp. | Thấy rõ pain point có thật và lặp lại; giải pháp cần tập trung vào việc tự động map dữ liệu chính xác vào đúng mẫu template Word của trường. |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Pain thật không nằm ở việc sinh viên "lười viết", mà nằm ở việc mất quá nhiều thời gian làm việc cơ học (kẻ bảng API, copy schema DB, định dạng thụt lề Word) khiến sát giờ nộp không còn thời gian đầu tư vào phần phân tích logic nghiệp vụ và kết quả thử nghiệm. AI chỉ phát huy giá trị khi kết hợp với Rule trích xuất tham số chính xác, tránh văn phong sáo rỗng.
```

Bằng chứng đính kèm (nếu có): `Ghi nhận trực tiếp từ biên bản phỏng vấn 3 thành viên trong nhóm (Chu Minh Quân, Trần Trọng Chinh, Nguyễn Việt Thành) và kết quả khảo sát 10 sinh viên trong lớp; hiện chưa đính kèm tệp ảnh riêng trong workspace.`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Swagger / OpenAPI Generator** | [https://swagger.io/tools/swagger-codegen/](https://swagger.io/tools/swagger-codegen/) | Trích xuất API từ code annotations thành tài liệu cấu trúc (JSON/YAML/HTML/Markdown). | Cực kỳ chuẩn xác nhờ cơ chế Rule-based, không có ảo giác, tự động cập nhật khi code thay đổi. | Chỉ sinh trang web API thô hoặc Markdown; không tạo được file Word theo template học thuật của trường ĐH Việt Nam; không viết được diễn giải luồng nghiệp vụ tổng quan. | Tận dụng Swagger/OpenAPI làm tầng tiền xử lý (Rule-based) để trích xuất sạch tham số API trước khi đưa vào AI, tránh để AI tự đoán thông số kỹ thuật. |
| **Mintlify / GitBook AI** | [https://mintlify.com/](https://mintlify.com/) | Tự động đọc repository code để sinh trang tài liệu kỹ thuật (developer documentation) cho sản phẩm phần mềm. | UI cực đẹp, AI tóm tắt hàm và luồng dữ liệu tự nhiên, hiểu được cấu trúc nhiều ngôn ngữ (Python, JS, Java). | Phục vụ trang web docs thương mại (SaaS); không xuất file Word (.docx), không hỗ trợ mục lục 3 cấp, bảng biểu, chú thích hình chuẩn thể thức văn bản đại học. | Học hỏi cách Mintlify trích xuất ngữ cảnh code theo module/controller; tuy nhiên nhóm cần tập trung vào output cuối là format Word (.docx) chuẩn của khoa. |
| **GitHub Copilot / Cursor Code-to-Doc Pattern** | [https://github.com/features/copilot](https://github.com/features/copilot) | Dùng LLM đọc ngữ cảnh file mã nguồn để draft tài liệu giải thích kiến trúc và luồng xử lý. | Hiểu sâu logic nghiệp vụ phức tạp, viết câu văn tự nhiên, giải thích được các luồng xử lý liên file. | Dễ phát sinh ảo giác (hallucination) nếu prompt mơ hồ; định dạng Markdown tự do, sinh viên vẫn phải copy paste thủ công sang Word và tự dàn trang. | Cần thiết kế prompt dạng cấu trúc nghiêm ngặt (JSON Schema output); bắt buộc phải có Human Review duyệt nội dung và dùng script chèn tự động vào file mẫu Word. |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
1. NÊN BUILD: Một giải pháp lai (Hybrid Workflow): Tận dụng Rule-based (OpenAPI/Schema script) để trích xuất bảng dữ liệu kỹ thuật chuẩn xác $\rightarrow$ Dùng LLM soạn thảo dự thảo thuyết minh luồng nghiệp vụ theo đúng khung sườn $\rightarrow$ Script tự động đổ dữ liệu vào Template Word (.docx) của khoa $\rightarrow$ Sinh viên rà soát lại (Human in the loop).
2. KHÔNG NÊN BUILD: Tuyệt đối không cố xây dựng một "Agent tự động viết 100% báo cáo từ A đến Z" vì sẽ tạo ra văn phong sáo rỗng, dễ bị ảo giác thông số và vi phạm liêm chính học thuật.
```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
CURRENT STATE — 210 phút (~3.5 tiếng)

[1 Đọc code & commit cả nhóm: 45' - Nhóm trưởng] 
→ [2 Chạy app, chụp ảnh màn hình demo: 30' - Người viết] 
→ [3 Đọc code kẻ bảng API & schema DB: 45' - Người viết]  <-- BOTTLENECK 1
→ [4 Soạn thảo thuyết minh luồng tính năng: 50' - Người viết]  <-- BOTTLENECK 2
→ [5 Dàn trang template Word chuẩn khoa: 30' - Người viết] 
→ [6 Cả nhóm rà soát chéo & xuất PDF: 10' - Cả nhóm]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | Nhóm trưởng / Người viết | Repository GitHub, commit log các nhánh | Danh sách chức năng đã hoàn thành | 45 phút / đợt nộp | Handoff từ các dev push code sang người tổng hợp; mất thời gian đọc code người khác viết. |
| 2 | Người viết báo cáo | Ứng dụng chạy local trên máy cá nhân | 15–20 ảnh chụp màn hình các luồng giao diện | 30 phút / đợt nộp | Thao tác thủ công, phải chạy qua từng kịch bản người dùng để chụp ảnh minh họa. |
| 3 | Người viết báo cáo | Source code Controllers, Routes, Models | Bảng đặc tả 15–25 API và Schema các bảng DB | 45 phút / đợt nộp | **BOTTLENECK 1:** Đọc từng hàm để gõ tay tham số, URL, request/response; dễ sai lệch kiểu dữ liệu (int/string). |
| 4 | Người viết báo cáo | Mã nguồn xử lý logic + Ảnh demo | 20–30 trang văn bản thuyết minh luồng nghiệp vụ | 50 phút / đợt nộp | **BOTTLENECK 2:** Phải diễn giải code kỹ thuật thành câu chữ học thuật; dễ cạn ý tưởng, làm vội sát deadline. |
| 5 | Người viết báo cáo | Bản nháp text + Template Word của khoa | File Word thô 40–60 trang theo đúng mẫu | 30 phút / đợt nộp | Căn chỉnh lề, font Times New Roman 13, giãn dòng 1.5, tạo mục lục tự động; dễ bị vỡ format bảng. |
| 6 | Cả nhóm sinh viên | File Word hoàn chỉnh | File PDF cuối cùng nộp hệ thống LMS | 10 phút / đợt nộp | Handoff kiểm tra chéo lần cuối trước khi nộp điểm thật. |

**Bottleneck chính (2-3 câu):**

```text
Điểm nghẽn nghiêm trọng nhất nằm ở Bước 3 (Kẻ bảng đặc tả API & Schema DB) và Bước 4 (Soạn thảo văn bản thuyết minh luồng nghiệp vụ từ code), chiếm tới 95 phút (~45% tổng thời gian). Sinh viên bị vắt kiệt sức vào việc gõ tay các thông số kỹ thuật lặp đi lặp lại và cố gắng diễn đạt lại code thành lời văn, dẫn đến sai sót thông số so với thực tế và không còn thời gian đầu tư vào phần đánh giá kết quả.
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
FUTURE STATE — 55 phút

[1 Export Swagger spec & Schema DB: 5' - Rule máy]
→ [2 AI phân tích code & draft thuyết minh luồng: 10' - AI Workflow]
→ [3 Chụp ảnh màn hình demo chèn vào dự thảo: 15' - Người làm]
→ [4 Script tự động map dữ liệu vào Template Word: 5' - Rule máy]
→ [5 Sinh viên review, chỉnh sửa thuật ngữ & số liệu: 15' - HUMAN BOUNDARY]
→ [6 Nhóm rà soát lần cuối & xuất file PDF: 5' - Người làm]

Fallback: Nếu AI sinh văn phong sáo rỗng hoặc sai luồng → Sử dụng bảng dữ liệu thô từ Rule (Swagger) và tự gõ 2-3 gạch đầu dòng theo khung mẫu có sẵn.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| **Tổng thời gian hoàn thành** | 210 phút (~3.5 giờ) | 55 phút (~1 giờ) | Bấm giờ thực tế từ lúc bắt đầu tổng hợp code đến khi hoàn tất xuất file PDF sau khi rà soát. |
| **Số bước thực hiện** | 6 bước tuần tự | 6 bước (tối ưu hóa tự động) | Đếm số công đoạn trong pipeline. |
| **Số bước thủ công** | 6 bước đều phải làm tay | 3 bước (Bước 3 chụp ảnh, Bước 5 review, Bước 6 xuất PDF) | Số bước có sự can thiệp trực tiếp của con người. |
| **Thời gian tại điểm nghẽn** | 95 phút gõ bảng & viết văn | 25 phút (AI draft 10' + Người review 15') | Giảm khoảng 73,7% thời gian tại khâu nghẽn nhất (từ 95 phút xuống còn 25 phút). |
| **Rủi ro mới phát sinh** | Mệt mỏi gõ nhầm thông số, trễ deadline | Rủi ro AI bị ảo giác (hallucination) văn phong | Mục tiêu giảm thiểu rủi ro nhờ bước Human Review trực tiếp rà soát và chỉnh sửa tại Bước 5 trước khi xuất file PDF. |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Sinh viên năm 4 ngành Công nghệ thông tin phụ trách viết tài liệu báo cáo kỹ thuật và Trưởng nhóm bài tập lớn/đồ án môn học. |
| **Workflow** | Quy trình tổng hợp báo cáo bài tập lớn Word 40–60 trang cuối kỳ gồm 6 bước: đọc code cả nhóm $\rightarrow$ chụp ảnh giao diện demo $\rightarrow$ kẻ bảng API và DB $\rightarrow$ soạn thảo thuyết minh luồng tính năng $\rightarrow$ dàn trang Word theo mẫu $\rightarrow$ xuất PDF nộp bài. |
| **Bottleneck** | Trong quy trình hiện tại, điểm nghẽn nằm ở Bước 3 (Kẻ bảng đặc tả API/DB: 45') và Bước 4 (Soạn thảo văn bản thuyết minh từ mã nguồn: 50'), tốn 95 phút do sinh viên phải đọc lại code của nhiều người và tự tay gõ lại từng tham số kỹ thuật. |
| **Impact** | Tốn 3–4 tiếng trước mỗi đợt nộp bài; 9/10 sinh viên được khảo sát phải thức khuya sát hạn chót; từng bị trừ từ 0,5 đến 1,5 điểm do lệch chuẩn định dạng hoặc sai lệch thông số giữa báo cáo và code thật. |
| **Success Metric** | Giảm tổng thời gian viết báo cáo từ khoảng 3.5 tiếng (210') xuống còn dưới 1 tiếng (dưới 60', tiết kiệm trên 70% thời gian); văn bản bám sát quy chuẩn format Word của khoa; đặt mục tiêu các bảng đặc tả API và DB khớp chính xác với mã nguồn thật. |
| **Boundary** | Chỉ áp dụng cho các bài tập lớn/project phần mềm có sẵn mã nguồn và cấu trúc DB; hệ thống chỉ đóng vai trò soạn thảo dự thảo bản nháp (draft) và trích xuất dữ liệu, tuyệt đối không tự động nộp bài thay sinh viên và không thay thế phần đánh giá kết quả thử nghiệm thực tế. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: Metric *"chất lượng văn phong thuyết minh của AI"* còn mang tính cảm tính, chưa có tiêu chuẩn định lượng cụ thể.
- Tôi sửa gì: Bổ sung bộ tiêu chí nghiệm thu (Acceptance Criteria) cho dự thảo của AI: Bắt buộc mô tả theo cấu trúc 3 phần (Input $\rightarrow$ Process $\rightarrow$ Output), không chứa các từ ngữ cảm thán/sáo rỗng.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [ ] Thấp (có đúng/sai rõ) / [x] Cao (nhiều cách trả lời vẫn OK) — Vì sao: Phần viết thuyết minh luồng nghiệp vụ có thể diễn đạt bằng nhiều câu chữ khác nhau miễn là đúng bản chất kỹ thuật; tuy nhiên phần bảng API lại có độ mơ hồ thấp (tham số đúng/sai tuyệt đối).
- Độ phức tạp: [ ] Thấp (1-2 bước) / [x] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao: Cần phối hợp liên hoàn từ 4 nguồn dữ liệu: Mã nguồn (Controllers) $\rightarrow$ Cấu trúc Database $\rightarrow$ Ảnh chụp demo $\rightarrow$ Template mẫu file Word của khoa.

**Bài toán nhóm nằm ở ô nào:**

```text
Ô: Độ mơ hồ Cao x Độ phức tạp Cao
```

**Vì sao (2-3 câu):**

```text
Bài toán đòi hỏi sự kết hợp giữa 2 thái cực: Vừa cần tính chính xác tuyệt đối ở tầng thông số kỹ thuật (URL, method, schema) từ nhiều file mã nguồn, vừa cần năng lực tổng hợp ngôn ngữ tự nhiên để diễn giải logic hoạt động thành câu văn học thuật mạch lạc theo đúng khung sườn quy định.
```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Dùng script OpenAPI Generator bóc tách API annotations thành bảng Markdown + thư viện `python-docx` tự động điền template Word. | Đủ nếu giảng viên chỉ yêu cầu nộp tài liệu API Reference dạng bảng thô, không yêu cầu thuyết minh luồng tính năng. | Hoàn toàn không viết được câu văn nào giải thích nghiệp vụ; sinh viên vẫn phải tự gõ tay toàn bộ 20–30 trang thuyết minh. | **CHỌN MỘT PHẦN:** Dùng làm tầng tiền xử lý trích xuất dữ liệu sạch và tầng hậu xử lý dàn trang Word. |
| **Workflow** | Xây dựng pipeline có điều phối: Rule bóc tách dữ liệu chuẩn $\rightarrow$ Đưa context vào LLM để draft văn bản thuyết minh theo khung Input-Process-Output $\rightarrow$ Điền tự động vào template Word $\rightarrow$ Sinh viên review & ký duyệt. | Đủ cho toàn bộ quy trình viết báo cáo học thuật, vì luồng xử lý đi theo các bước tuần tự cố định và có con người kiểm duyệt ở chặng cuối. | LLM có thể diễn giải chưa sát nếu tên biến trong code đặt cẩu thả; kỳ vọng giảm thiểu rủi ro nhờ ranh giới con người (Human Boundary) trực tiếp rà soát và chỉnh sửa. | **CHỌN LÀM GIẢI PHÁP CHÍNH:** Tối ưu hóa giữa chi phí, độ chính xác và khả năng tự động hóa. |
| **Agent** | Xây dựng Autonomous Agent tự động clone GitHub repo, tự phân tích kiến trúc, tự gọi tool chụp ảnh màn hình, tự chạy test và tự submit bài lên LMS trường. | Khi hệ thống cần xử lý tự động 100% mà không có bất kỳ sự can thiệp nào của sinh viên. | Rủi ro "ảo giác" dây chuyền (cascading errors), chi phí gọi LLM rất cao, hành vi không đoán định được (non-deterministic) dễ làm hỏng cấu trúc báo cáo và vi phạm quy chế thi cử. | **KHÔNG CHỌN:** Quá phức tạp và dư thừa so với yêu cầu bài toán. |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. **Rule có giải được 70-80% case không?** -> Không, Rule chỉ giải quyết được phần kẻ bảng API và dàn trang Word (~40% khối lượng), hoàn toàn bất lực ở khâu viết thuyết minh luồng nghiệp vụ học thuật.
2. **Các bước có đi thẳng một đường không hay phải rẽ nhánh?** -> Các bước đi thẳng một đường tuyến tính: Bóc tách mã nguồn $\rightarrow$ AI sinh bản nháp thuyết minh $\rightarrow$ Chèn ảnh demo $\rightarrow$ Map template Word $\rightarrow$ Người review.
3. **Có thật sự cần Agent tự lập kế hoạch + gọi tool không?** -> Hoàn toàn không cần, vì cấu trúc bài báo cáo đã được quy định cứng bằng template mẫu của khoa (không cần Agent tự suy nghĩ bước tiếp theo).
4. **Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?** -> Sinh viên phụ trách viết báo cáo phát hiện ngay tại Bước 5 khi rà soát bản nháp Word và có thể chỉnh sửa trực tiếp câu chữ trong 5–10 phút.
5. **Có hạ được từ Agent → Workflow → Rule không?** -> Có thể hạ tầng linh hoạt: Tầng trích xuất API và format Word là Rule thuần túy; nếu tầng AI gặp sự cố, hệ thống vẫn xuất được khung báo cáo chuẩn kèm bảng dữ liệu để sinh viên tự viết tiếp.

**Mức chọn:**

```text
Workflow (Kết hợp Rule tiền/hậu xử lý + AI draft nội dung có Human-in-the-loop)
```

**Vì sao chọn (3-4 câu):**

```text
Nhóm chọn Workflow vì quy trình gồm nhiều bước nối tiếp từ nhiều nguồn dữ liệu (code, DB, ảnh, Word) cần sự điều phối chặt chẽ. AI (LLM) phát huy tối đa giá trị ở điểm nghẽn lớn nhất là soạn thảo thuyết minh luồng nghiệp vụ từ code thô, trong khi các bước thông số kỹ thuật và căn lề Word đặt mục tiêu đạt độ chuẩn xác cao nhờ cơ chế Rule-based được kiểm thử trước. Đây là giải pháp an toàn, hiệu quả, kiểm soát được chi phí và đặt con người ở vị trí kiểm duyệt cuối cùng.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Nếu chỉ dùng Rule thuần túy (như Swagger/Postman), hệ thống chỉ sinh ra các bảng thông số kỹ thuật khô khan mà không thể viết được các đoạn văn giải thích luồng xử lý nghiệp vụ cho người đọc hiểu. Sinh viên vẫn sẽ phải bỏ ra 50–60 phút ngồi gõ tay từng trang thuyết minh, nghĩa là điểm nghẽn lớn nhất vẫn không được giải quyết.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Sinh viên năm 4 ngành CNTT phụ trách viết tài liệu kỹ thuật và Trưởng nhóm bài tập lớn/đồ án môn học. |
| **Workflow** | Quy trình gồm 6 bước: Trích xuất Swagger & Schema DB $\rightarrow$ AI soạn thảo dự thảo thuyết minh luồng tính năng $\rightarrow$ Chụp ảnh màn hình demo $\rightarrow$ Script điền tự động vào template Word chuẩn $\rightarrow$ Sinh viên rà soát, chỉnh sửa thuật ngữ $\rightarrow$ Xuất file PDF nộp bài. |
| **Bottleneck** | **Trong quy trình hiện tại**, điểm nghẽn nằm ở **Bước 3** (Kẻ bảng API/DB: 45') và **Bước 4** (Soạn thảo văn bản thuyết minh từ mã nguồn: 50'), tốn 95 phút do phải đọc lại code của nhiều người và tự gõ thủ công từng thông số kỹ thuật. Quy trình mới giải quyết bằng cách tự động trích xuất thông số và hỗ trợ soạn thảo. |
| **Impact** | Mất 3–4 tiếng trước mỗi đợt nộp; 9/10 sinh viên được khảo sát phản ánh phải thức khuya sát hạn chót; từng bị trừ từ 0,5 đến 1,5 điểm trình bày do lệch chuẩn format hoặc sai sót thông số so với code thật. |
| **Success Metric** | Giảm tổng thời gian hoàn thành từ 210 phút xuống dưới 60 phút (tiết kiệm trên 70% thời gian); văn bản bám sát mẫu Word chuẩn của khoa; tham số API khớp đúng với mã nguồn thật; hầu hết các hàm nghiệp vụ chính đều có bản nháp thuyết minh rõ ràng theo cấu trúc Input-Process-Output. |
| **Boundary** (làm / không làm) | **LÀM:** Tự động trích xuất bảng API/DB từ code, sinh dự thảo văn bản thuyết minh kỹ thuật và dàn trang theo file mẫu Word của khoa.<br>**KHÔNG LÀM:** Không tự động code thay sinh viên, không tự động nộp bài lên portal trường, không tự bịa số liệu thực nghiệm (phần này sinh viên phải tự điền). |
| **AI intervention point** | AI can thiệp ngay sau bước Rule bóc tách dữ liệu kỹ thuật thô (Bước 1) và trước bước đổ dữ liệu vào Template Word (Bước 4). Nhiệm vụ của AI là đọc hiểu logic hàm để sinh bản nháp thuyết minh nghiệp vụ. |
| **Mức chọn** | **Workflow:** Kết hợp Rule (trích xuất thông số + format Word) và LLM (soạn thảo dự thảo thuyết minh) với Human-in-the-loop duyệt nội dung cuối cùng. |
| **Rủi ro & người thật kiểm tra** | **Rủi ro lớn nhất:** AI sinh câu chữ sáo rỗng hoặc "ảo giác" mô tả sai luồng xử lý của hàm.<br>**Người kiểm tra:** Sinh viên viết báo cáo bắt buộc phải đọc rà soát toàn bộ văn bản tại Bước 5, đối chiếu logic với code thật và chỉnh sửa trước khi xuất file PDF. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | **Yes** | Actor là sinh viên viết báo cáo, workflow 6 bước trước/sau được định lượng thời gian chi tiết đến từng phút. |
| Baseline + metric đo được chưa? | **Yes** | Baseline hiện tại là 210 phút (từng bị trừ 0,5–1,5 điểm format và tham số), mục tiêu cải thiện là dưới 60 phút và bảo toàn điểm format theo quy chuẩn khoa. |
| Data/input đủ dùng chưa? | **Yes** | Toàn bộ mã nguồn, schema database và file mẫu Word của trường đều có sẵn trên máy cá nhân của nhóm. |
| AI sai, hậu quả chấp nhận được không? | **Yes** | Hậu quả chỉ là câu chữ bản nháp bị lệch, sinh viên phát hiện ngay trong bước review và sửa trực tiếp trong Word trước khi nộp. |
| Có người review/owner không? | **Yes** | Sinh viên phụ trách tài liệu và nhóm trưởng là người chịu trách nhiệm trực tiếp đọc duyệt toàn bộ báo cáo. |
| Có cách non-AI đơn giản hơn không? | **Yes (nhưng không đủ)** | Đã phân tích giải pháp Rule-based (Swagger), nhưng Rule chỉ sinh bảng thô chứ không thể viết văn thuyết minh nghiệp vụ. |

**Decision:**

```text
Go
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Quyết định Go được đưa ra dựa trên bằng chứng khảo sát thực tế vững chắc (đại đa số sinh viên được khảo sát đều gặp khó khăn về thời gian và từng bị trừ điểm trình bày) và tính khả thi cao trong môi trường lab. Bài toán có quy trình tuyến tính rõ ràng, dữ liệu đầu vào sẵn có, định lượng ROI sắc nét (tiết kiệm 155 phút/bài) và ranh giới kiểm duyệt của con người được thiết lập rất chặt chẽ. Việc kết hợp Rule-based để đảm bảo độ chính xác tham số và AI Workflow để giải quyết nút thắt viết văn bản là phương án tối ưu, không có rủi ro pháp lý hay phụ thuộc dữ liệu bên thứ ba.
```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
• Dữ liệu thử nghiệm: 1 module Quản lý người dùng & Xác thực (User & Auth Module) gồm 5 API (login, register, profile, refresh token, logout) và 2 bảng database từ bài tập lớn môn Lập trình Web.
• Quy trình chạy tay: Chạy script trích xuất Swagger JSON của module $\rightarrow$ Đưa prompt vào Claude/ChatGPT để sinh dự thảo thuyết minh cho 5 API này $\rightarrow$ Dùng script chèn bảng và text vào template Word mẫu của khoa.
• Đo 3 chỉ số cốt lõi:
  1. Thời gian trích xuất & sinh dự thảo: Mục tiêu < 3 phút.
  2. Độ chuẩn xác của bảng tham số API so với code thật: Khớp đúng kiểu dữ liệu, endpoint và tham số, không để xảy ra sai sót kỹ thuật cơ bản.
  3. Thời gian sinh viên đọc rà soát và chỉnh sửa hoàn thiện: Mục tiêu < 10 phút.
```

**Nếu Not Yet — cần validate gì trước:**

```text
(Không áp dụng vì nhóm đã quyết định Go)
```

**Nếu No-Go — làm gì thay AI:**

```text
(Không áp dụng vì nhóm đã quyết định Go)
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Nhóm sẽ kích hoạt Rollback quay về quy trình cũ trong 2 trường hợp:
1. Chi phí gọi API LLM vượt quá ngân sách cho phép hoặc hệ sinh thái API của AI gặp sự cố gián đoạn kết nối sát giờ nộp bài (< 2 tiếng trước hạn chót).
2. Tỷ lệ lỗi ảo giác (hallucination) trong lời văn vượt quá 30% nội dung (do code đặt tên biến quá tối nghĩa khiến AI hiểu sai toàn bộ luồng).
-> Khi Rollback: Tắt tầng sinh text AI, chỉ sử dụng script Rule để trích xuất bảng thông số API/DB đổ vào Word, sinh viên sẽ quay lại tự tay gõ tóm tắt tính năng theo các gạch đầu dòng ngắn gọn.
```

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [x] Có validation (quote thật) + research (link kiểm được)
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
