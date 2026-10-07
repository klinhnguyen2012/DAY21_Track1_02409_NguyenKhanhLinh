## Case study 3 — HireVue: AI phỏng vấn video và việc bỏ phân tích hình ảnh

### Brief Case

- **Tổ chức / sản phẩm:** HireVue, nền tảng phỏng vấn video và đánh giá ứng viên có AI.
- **Thời gian, địa điểm / bối cảnh:** HireVue thông báo tháng 01/2021 rằng hãng đã chủ động bỏ phân tích hình ảnh khỏi các đánh giá mới từ đầu năm 2020. Công cụ được dùng trong quy trình tuyển dụng của khách hàng tại Hoa Kỳ và các thị trường khác.
- **AI được dùng để làm gì:** Trước khi loại bỏ, thành phần phân tích hình ảnh dùng thuật toán để suy ra đặc điểm ứng viên từ nét mặt trong video phỏng vấn. HireVue nói quyết định bỏ tính năng dựa trên nghiên cứu nội bộ cho thấy phân tích hình ảnh không đóng góp đáng kể vào đánh giá so với phân tích ngôn ngữ. Không suy ra rằng tất cả khách hàng hay mọi ứng viên đều bị chấm bằng tính năng này.
- **Vấn đề hoặc sự kiện đáng chú ý:** Các chuyên gia và nhóm quyền dân sự đặt câu hỏi về tính hợp lệ, độ minh bạch và việc dùng khuôn mặt để suy đoán phẩm chất phù hợp công việc. HireVue sau đó bỏ tính năng phân tích hình ảnh khỏi mô hình đánh giá mới. Đây là tranh luận/rủi ro được nêu và thay đổi sản phẩm; nguồn không xác nhận một ứng viên cụ thể bị loại hoặc chịu thiệt hại do phân tích hình ảnh.
- **Số liệu có nguồn:** Tuyên bố giải thích AI năm 2024 của HireVue cho biết hãng lấy mẫu hơn **900.000 hồ sơ ứng viên** để kiểm tra chênh lệch theo giới, tuổi và chủng tộc/sắc tộc; nghiên cứu AI chấm phỏng vấn của hãng nêu tương quan trung bình **r = 0,69** với đánh giá của chuyên gia trên **99.411 câu trả lời phỏng vấn**. Đây là số liệu hãng tự công bố về quy trình/hiệu lực đánh giá, không phải số người bị hại hay số liệu độc lập về tính năng phân tích hình ảnh đã bỏ.
- **Nguồn:** HireVue, “Industry Leadership: New Audit Results, Decision on Visual Analysis,” 12/01/2021 — [thông báo của HireVue](https://www.hirevue.com/blog/hiring/industry-leadership-new-audit-results-and-decision-on-visual-analysis); HireVue, “2024 AI Explainability Statement,” mục mô tả kiểm tra adverse impact và hiệu lực mô hình — [PDF](https://www.hirevue.com/wp-content/uploads/2024/09/HV_2024_AI-Explainability-Statement.pdf).
- **Phân biệt bằng chứng và nhận định:** HireVue xác nhận hãng bỏ phân tích hình ảnh khỏi các đánh giá mới; tuyên bố năm 2024 cung cấp các cỡ mẫu và số tương quan nêu trên. Nhận định của tôi: suy luận đặc điểm nghề nghiệp từ nét mặt có thể gây bất lợi cho ứng viên có biểu hiện, khuyết tật hoặc nền tảng khác với dữ liệu đánh giá. Nguồn không công bố tỷ lệ ứng viên bị ảnh hưởng hoặc kiểm toán độc lập cho tính năng phân tích hình ảnh trước khi bỏ.

### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | Khi ứng viên ghi hình câu trả lời phỏng vấn và hệ thống dùng phân tích hình ảnh để tạo đánh giá ảnh hưởng đến việc được mời phỏng vấn tiếp hoặc tuyển dụng. |
| Stakeholder bị ảnh hưởng | Ứng viên được yêu cầu phỏng vấn video; đặc biệt có thể gặp rủi ro nếu nét mặt, biểu hiện thần kinh/khuyết tật hoặc cách giao tiếp khác chuẩn bị diễn giải sai thành dấu hiệu năng lực. |
| Failure mode | **Bias / fairness; privacy loss (nguy cơ):** suy đoán đặc điểm từ khuôn mặt có thể không công bằng giữa nhóm người và xử lý hình ảnh ứng viên theo cách họ khó kiểm tra. Nguồn xác nhận mối quan ngại và việc bỏ tính năng, không xác nhận thiệt hại cụ thể. |
| Layer bắt đầu lỗi | **Chưa đủ bằng chứng.** Sự kiện liên quan đến chức năng phân tích hình ảnh trong đánh giá mô hình; nguồn công khai không nêu chi tiết kỹ thuật hoặc kiểm soát UX/Safety. Có thể là vấn đề ở Model/tiêu chí đánh giá, nhưng đây là giả thuyết. |
| Harm xảy ra là gì? | **Sự kiện xác nhận:** HireVue đã bỏ phân tích hình ảnh khỏi mô hình đánh giá mới. **Nguy cơ chưa xác nhận:** ứng viên có thể bị đánh giá sai, mất cơ hội hoặc bị phân tích dữ liệu hình ảnh ngoài kỳ vọng. Không có nguồn xác nhận ứng viên cụ thể bị từ chối vì tính năng này. |
| Harm lens | **Opportunity loss** (nguy cơ mất cơ hội); **privacy loss** (nguy cơ mất quyền kiểm soát hình ảnh/dữ liệu phỏng vấn). |
| Severity | **Medium** — đánh giá của tôi: nếu được dùng trong sàng lọc, đánh giá sai có thể ảnh hưởng cơ hội nghề nghiệp và xử lý dữ liệu khuôn mặt có thể xâm phạm riêng tư; mức độ tác hại thực tế chưa được nguồn định lượng. |
| Scale | **Chưa đủ dữ liệu để đánh giá số ứng viên chịu tác động của phân tích hình ảnh.** Mẫu hơn 900.000 hồ sơ và 99.411 câu trả lời là số liệu hãng nêu cho các kiểm tra/đánh giá mô hình, không phải quy mô người bị tính năng hình ảnh gây hại. |
| Probability | **Chưa đủ dữ liệu để đánh giá.** Tuyên bố hãng nói phân tích hình ảnh ít đóng góp vào dự đoán hiệu suất; không công bố xác suất chấm sai hoặc chênh lệch tác động giữa nhóm từ tính năng đã bỏ. |
| Frequency | **Chưa đủ dữ liệu để đánh giá.** Không có số lần tính năng phân tích hình ảnh được dùng, thời gian triển khai theo khách hàng hay tần suất lỗi được công bố trong các nguồn trên. |
| Vì sao? | Thông báo HireVue là căn cứ cho việc bỏ phân tích hình ảnh; tuyên bố giải thích AI cung cấp số liệu cỡ mẫu nhưng do hãng tự công bố và không đo thiệt hại từ tính năng đã bỏ. Vì vậy, harm trong bản đồ chủ yếu là nguy cơ, còn scale, probability và frequency cần dữ liệu triển khai/kiểm toán độc lập. |
