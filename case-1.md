## Case study 1 — Amazon: công cụ AI xếp hạng hồ sơ ứng viên

## Brief Case

- Tổ chức / sản phẩm AI: Amazon; công cụ thử nghiệm dùng machine learning để đánh giá hồ sơ ứng viên.
- Thời gian, địa điểm / bối cảnh: Amazon bắt đầu xây dựng công cụ từ năm 2014; nhóm phát hiện vấn đề về giới vào năm 2015 và dự án bị giải thể vào đầu năm 2017. Công cụ được phát triển tại nhóm kỹ thuật ở Edinburgh, để hỗ trợ tuyển dụng, gồm các vị trí kỹ thuật.
- AI được dùng để làm gì: Đọc hồ sơ và chấm ứng viên từ một đến năm sao nhằm xếp hạng hồ sơ cho nhà tuyển dụng.
- Vấn đề hoặc sự kiện đáng chú ý: Theo Reuters, mô hình học từ hồ sơ nộp cho Amazon trong 10 năm, phần lớn là hồ sơ của nam giới. Công cụ phạt một số hồ sơ có từ “women’s” và hạ điểm ứng viên tốt nghiệp từ hai trường nữ sinh. Amazon đã thử chỉnh các từ cụ thể nhưng lo ngại mô hình vẫn có thể tìm cách phân loại gây bất lợi khác; cuối cùng dừng dự án.
- Số liệu có nguồn: Dữ liệu huấn luyện bao phủ hồ sơ của 10 năm; nhóm xây dựng khoảng 500 mô hình, mỗi mô hình nhận diện khoảng 50.000 thuật ngữ. Đây là quy mô dữ liệu/mô hình được bài báo nêu, không phải số ứng viên bị ảnh hưởng. Reuters không công bố số ứng viên nữ bị loại hoặc mức chênh lệch điểm.
- Nguồn: Jeffrey Dastin, “Amazon scraps secret AI recruiting tool that showed bias against women” — Reuters, 10/10/2018 — [đọc bài trên Investing.com](https://www.investing.com/news/stock-market-news/amazon-scraps-secret-ai-recruiting-tool-that-showed-bias-against-women-1637988), các mục mô tả công cụ và dữ liệu huấn luyện.
- Phân biệt bằng chứng và nhận định: Reuters đưa tin về dấu hiệu thiên lệch, chi tiết của mô hình và việc dự án bị dừng dựa trên các nguồn ẩn danh am hiểu dự án. Nhận định của tôi: cách học từ lịch sử tuyển dụng có thể lặp lại thiên lệch giới nếu lịch sử phản ánh sự thiếu đại diện. Bài báo không cho biết bao nhiêu ứng viên thực tế bị từ chối vì công cụ; Amazon cũng nói nhà tuyển dụng xem gợi ý nhưng không chỉ dựa vào xếp hạng để tuyển.

## Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | Lúc công cụ xếp hạng hồ sơ cho vị trí kỹ thuật và nhà tuyển dụng dùng thứ hạng để chọn ai được xem xét hoặc mời phỏng vấn. |
| Stakeholder bị ảnh hưởng | Ứng viên nữ bị chấm thấp hơn vì dấu hiệu liên quan đến phụ nữ; nhà tuyển dụng có thể bỏ lỡ ứng viên phù hợp. |
| Failure mode | **Bias / fairness** — mô hình học từ hồ sơ lịch sử thiên về nam giới và gắn một số từ/ngữ cảnh với điểm thấp. |
| Layer bắt đầu lỗi | **Model** — Reuters mô tả mô hình học từ dữ liệu lịch sử. Bài báo không công bố kiến trúc hoặc đủ chi tiết kỹ thuật để xác định nguyên nhân chính xác hơn. |
| Harm xảy ra là gì? | Reuters ghi nhận một số hồ sơ bị chấm bất lợi. **Nguy cơ:** ứng viên nữ bị mất cơ hội được xem xét/phỏng vấn khi xếp hạng được dùng trong tuyển dụng. Nguồn không xác nhận ứng viên cụ thể đã mất việc làm vì công cụ. |
| Harm lens | **Opportunity loss** — nguy cơ mất cơ hội tiếp cận phỏng vấn hoặc việc làm. |
| Severity | **High** — đánh giá của tôi: việc bị loại ở bước sàng lọc có thể ảnh hưởng đáng kể đến cơ hội nghề nghiệp. Thiệt hại việc làm cụ thể không được nguồn xác nhận. |
| Scale | **Chưa đủ dữ liệu để đánh giá.** Công cụ còn ở giai đoạn thử nghiệm; Reuters không nêu số ứng viên bị chấm thấp hoặc số quyết định tuyển dụng bị ảnh hưởng. |
| Probability | **Chưa đủ dữ liệu để đánh giá xác suất mất cơ hội.** Reuters xác nhận thiên lệch xuất hiện trong thử nghiệm, nhưng không đo xác suất một ứng viên bị loại vì thiên lệch. |
| Frequency | **Chưa đủ dữ liệu để đánh giá.** Nguồn nêu các loại dấu hiệu bị phạt, không công bố số lần hoặc tỷ lệ lỗi. |
| Vì sao? | Reuters là căn cứ cho việc thiên lệch xuất hiện trong thử nghiệm và dự án đã bị dừng. Severity là nhận định về hậu quả tiềm tàng trong sàng lọc; scale, probability và frequency được để chưa đủ dữ liệu vì nguồn không đưa ra số ứng viên hoặc tỷ lệ tác động. Nhà tuyển dụng được cho biết đã xem gợi ý nhưng không chỉ dựa vào xếp hạng. |
