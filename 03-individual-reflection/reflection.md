# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Nguyễn Khắc Quang
- Mã học viên: 2A202602885
- Nhóm: Nhóm 6 thành viên — Leader Nguyễn Văn Ước
- Candidate problem nhóm chọn: Soạn thảo dự thảo Báo cáo bài tập lớn Word 40–60 trang từ Codebase và Schema DB

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Chuẩn bị hai candidate: #7 phân loại review VinFast và #8 tra cứu hướng dẫn sử dụng VinFast | Bổ sung cho nhóm góc nhìn về Customer Voice và bài toán RAG trong hệ sinh thái xe điện |
| Pitch Problem Card | Trình bày actor, nguồn dữ liệu công khai, bottleneck phân loại feedback và truy xuất đúng tài liệu/model xe | Hai candidate VinFast được đưa vào danh sách 12 bài toán để nhóm so sánh |
| Challenge bài của bạn khác | Dùng kết quả tìm hiểu Swagger và Mintlify để đặt lại câu hỏi liệu công cụ có sẵn đã giải đủ bài viết báo cáo hay chưa | Giúp nhóm tránh giả định phải xây mới toàn bộ và nhận ra khoảng trống ở file Word theo mẫu trường cùng phần thuyết minh nghiệp vụ |
| Gom trùng / cluster | Cung cấp thông tin để nhóm xếp bài #7 vào cụm phân loại phản hồi và bài #8 vào cụm truy xuất tài liệu chuyên sâu | Làm rõ điểm chung giữa xử lý văn bản phi cấu trúc, phân loại và truy xuất có nguồn |
| Chọn candidate problem | Ban đầu tôi ưu tiên domain xe điện VinFast, sau đó đồng ý chuyển sang bài #11 khi nhóm so sánh khả năng tiếp cận dữ liệu và pilot trong lab | Nhóm hội tụ vào candidate có codebase, schema DB và template Word thật để kiểm chứng |
| Validation / research | Tìm hiểu Swagger/OpenAPI Generator và Mintlify để xem giải pháp hiện có làm được gì | Xác định Swagger chủ yếu trích xuất API thô, còn Mintlify thiên về tài liệu web; chưa giải quyết trực tiếp file Word theo mẫu của trường |
| Workflow nhóm | Dùng kết quả research để làm rõ vị trí của công cụ có sẵn trong pipeline | Phần trích xuất API/DB được đặt ở tầng Rule; AI chỉ draft thuyết minh; sinh viên review và xuất file |
| Problem Statement | Góp ý thu hẹp bài toán về dự thảo báo cáo từ code/schema thay vì “AI làm báo cáo hoàn chỉnh” | Scope và boundary rõ hơn: không tự code, không tự nộp và không bịa kết quả thực nghiệm |
| Rule / Workflow / Agent | Chỉ ra Rule/Swagger tạo được bảng dữ liệu kỹ thuật nhưng không tự tạo đúng báo cáo Word học thuật của trường | Củng cố lựa chọn Workflow kết hợp Rule + AI draft + Human-in-the-loop, không chọn Agent tự động 100% |
| Decision | Đồng ý với quyết định Go cho pilot nhỏ sau khi nhóm ưu tiên dữ liệu sẵn có và khả năng đo thời gian | Pilot tập trung một module có API/schema thật; có metric thời gian, độ chính xác và thời gian review |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Đóng góp rõ nhất của tôi là phần research giải pháp có sẵn. Việc đối chiếu Swagger và Mintlify giúp nhóm xác định không nên xây lại khả năng trích xuất API, đồng thời chỉ ra khoảng trống thực tế là tạo báo cáo Word đúng mẫu trường và phần thuyết minh vẫn cần AI hỗ trợ cùng sinh viên kiểm duyệt.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Nhờ AI gợi ý thêm góc nhìn quanh VinFast và chuẩn hóa bảng 10 problems | Giúp mở rộng actor từ chủ xe sang Product Team, Customer Service và Service Center | AI có xu hướng suy đoán pain/quy trình nội bộ và đề xuất predictive maintenance khi không có sensor data | Tôi loại claim không có nguồn, tách fact/inference/assumption và giữ nhãn “chưa kiểm chứng” |
| Problem Card | Dùng AI sắp xếp actor, workflow, bottleneck, metric, non-AI alternative và boundary | Ba card có cấu trúc đồng nhất, dễ pitch và so sánh | AI đưa target khi chưa có baseline nội bộ và tên card đôi lúc solution-first | Tôi đổi target thành giả thuyết, viết lại problem-first và yêu cầu validation trước kết luận |
| Workflow | Nhờ AI chuyển mô tả thành Mermaid và gợi ý điểm Rule/AI/human handoff | Nhìn rõ AI chỉ nên can thiệp tại một bước, không ôm toàn quy trình | Flow ban đầu đơn giản hóa quyền dữ liệu và bước fallback | Tôi bổ sung source permission, human review, abstain và đường quay về xử lý thủ công |
| Research | Dùng AI hỗ trợ từ khóa/tổng hợp, sau đó tự mở trang Swagger và Mintlify để đối chiếu | Tiết kiệm thời gian xác định công cụ và pattern đã tồn tại | AI dễ nói chung rằng công cụ “tự động hóa tài liệu” mà không phân biệt web docs với Word template của trường | Tôi chỉ giữ kết luận kiểm được: Swagger xuất đặc tả/API thô; các công cụ chưa giải quyết trọn workflow báo cáo Word của nhóm |
| Problem Statement | Dùng AI phản biện field còn rộng và boundary chưa rõ | Giúp tách actor, bottleneck, impact, metric và phạm vi không làm | AI có thể biến số 210 → 55 phút thành kết quả đã đạt dù đây mới là baseline/target của nhóm | Tôi giữ cách diễn đạt trước/sau, cách đo và không gọi target là kết quả pilot |
| Rule / Workflow / Agent | Dùng AI tạo khung so sánh ba mức trên cùng một bài toán | Giúp thấy Agent là dư thừa khi pipeline đã tuyến tính | AI ban đầu thiên về giải pháp nhiều tự động hóa | Tôi dựa vào Swagger/Mintlify và thảo luận nhóm để chọn Workflow: Rule trích xuất, AI draft, người duyệt |
| Decision | Không để AI chốt thay; chỉ dùng AI gợi ý rủi ro, pilot và rollback | Bổ sung tiêu chí dừng nếu AI hallucinate hoặc không tiết kiệm thời gian | AI không biết dữ liệu/code/template nào nhóm thực sự có | Tôi cùng nhóm chọn Go dựa trên dữ liệu sẵn có và giữ Human Boundary trước khi xuất PDF |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Ban đầu tôi thích hai bài toán về xe điện VinFast vì đây là domain có quy mô người dùng lớn và nhiều dữ liệu văn bản để nghiên cứu. Khi nghe 12 candidate của các bạn, tôi nhận ra một bài toán hấp dẫn chưa chắc phù hợp với lab nếu nhóm không thể tiếp cận dữ liệu thật để kiểm chứng. Bài viết báo cáo từ codebase và schema DB thuyết phục tôi hơn vì cả nhóm có sẵn code, cấu trúc dữ liệu và template Word để chạy thử. Đóng góp rõ nhất của tôi là tìm hiểu Swagger và Mintlify nhằm kiểm tra giải pháp hiện có trước khi đề xuất xây mới. Kết quả research cho thấy Swagger hỗ trợ trích xuất đặc tả API nhưng không tự tạo được báo cáo Word theo mẫu trường và cũng không thay sinh viên viết phần thuyết minh nghiệp vụ. Từ đó tôi hiểu vì sao nhóm tách Rule cho dữ liệu kỹ thuật, AI cho bản nháp diễn giải và con người cho bước kiểm duyệt cuối. Câu hỏi của bạn Tâm về vị trí AI trong sáu bước giúp nhóm tránh thiết kế một Agent tự động toàn bộ. Cảnh báo của bạn Chinh về văn phong sáo rỗng cũng làm tôi thấy Human Boundary không chỉ để bắt lỗi kỹ thuật mà còn để bảo đảm bài viết mang giọng của sinh viên. Tôi đã thay đổi lựa chọn ban đầu không phải vì bài VinFast không có giá trị, mà vì bài báo cáo có evidence và khả năng pilot tốt hơn trong thời gian lab. Phần khó nhất với tôi là phân biệt target 210 xuống 55 phút với kết quả đã kiểm chứng; nhóm vẫn phải bấm giờ pilot trước khi khẳng định hiệu quả. Nếu làm lại, tôi sẽ challenge mạnh hơn nguồn của các con số baseline và yêu cầu mỗi metric ghi rõ cách đo ngay từ lúc shortlist. Sau buổi thảo luận, tôi hiểu rõ hơn mạch problem → workflow → bottleneck → metric → boundary và chỉ chọn AI ở bước mà Rule thuần túy chưa giải quyết đủ.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

