# Lab 21 — Phân tích rủi ro AI qua case study thực tế

- Họ và tên: [Điền họ tên]
- MSSV / mã học viên: [Điền mã]
- Lớp: [Điền lớp]
- Ngành đã chọn: HR / tuyển dụng

### 1. Industry Risk Snapshot

| Nội dung | Đánh giá của tôi và lý do |
| --- | --- |
| Những tác hại chính có thể xảy ra | Ứng viên đủ năng lực có thể bị xếp hạng thấp hoặc loại vì giới, tuổi, chủng tộc, khuyết tật hoặc dấu hiệu thay thế như trường học và khoảng trống nghề nghiệp. Họ có thể mất cơ hội phỏng vấn, việc làm và thu nhập; nhà tuyển dụng cũng có thể bỏ lỡ ứng viên phù hợp. Đây là các rủi ro có thể xảy ra, không khẳng định mọi hệ thống đều gây ra các hậu quả này. |
| Mức độ high-stakes | Cao (đánh giá định tính): tuyển dụng ảnh hưởng trực tiếp đến cơ hội nghề nghiệp, thu nhập và khả năng tiếp cận sinh kế; một quyết định loại sớm có thể chặn cơ hội trước khi ứng viên được gặp người tuyển dụng. Đây không phải kết luận phân loại pháp lý. |
| Dữ liệu nhạy cảm có thể được sử dụng | CV và lịch sử việc làm, học vấn, ngày tốt nghiệp, thông tin liên hệ, câu trả lời/phỏng vấn, giọng nói hoặc hình ảnh; một số hệ thống có thể suy ra tuổi, giới, chủng tộc hoặc tình trạng khuyết tật từ dữ liệu/proxy. Chỉ nêu loại dữ liệu, không đưa dữ liệu cá nhân thật. |
| Nhu cầu human review | Cao (đánh giá định tính): người tuyển dụng được đào tạo nên kiểm tra hồ sơ trước khi loại ứng viên, nhất là khi điểm thấp hoặc hệ thống đưa ra quyết định tự động; cần có cách yêu cầu xem xét lại và kiểm tra kết quả theo nhóm để phát hiện chênh lệch. Người kiểm tra cần có quyền đảo quyết định và đủ thông tin để làm vậy. |

### 2. Case study 1 — Amazon: công cụ AI xếp hạng hồ sơ ứng viên

#### Brief Case

- Tổ chức / sản phẩm AI: Amazon; công cụ thử nghiệm dùng machine learning để đánh giá hồ sơ ứng viên.
- Thời gian, địa điểm / bối cảnh: Amazon bắt đầu xây dựng công cụ từ năm 2014; nhóm phát hiện vấn đề về giới vào năm 2015 và dự án bị giải thể vào đầu năm 2017. Công cụ được phát triển tại nhóm kỹ thuật ở Edinburgh, để hỗ trợ tuyển dụng, gồm các vị trí kỹ thuật.
- AI được dùng để làm gì: Đọc hồ sơ và chấm ứng viên từ một đến năm sao nhằm xếp hạng hồ sơ cho nhà tuyển dụng.
- Vấn đề hoặc sự kiện đáng chú ý: Theo Reuters, mô hình học từ hồ sơ nộp cho Amazon trong 10 năm, phần lớn là hồ sơ của nam giới. Công cụ phạt một số hồ sơ có từ “women’s” và hạ điểm ứng viên tốt nghiệp từ hai trường nữ sinh. Amazon đã thử chỉnh các từ cụ thể nhưng lo ngại mô hình vẫn có thể tìm cách phân loại gây bất lợi khác; cuối cùng dừng dự án.
- Số liệu có nguồn: Dữ liệu huấn luyện bao phủ hồ sơ của 10 năm; nhóm xây dựng khoảng 500 mô hình, mỗi mô hình nhận diện khoảng 50.000 thuật ngữ. Đây là quy mô dữ liệu/mô hình được bài báo nêu, không phải số ứng viên bị ảnh hưởng. Reuters không công bố số ứng viên nữ bị loại hoặc mức chênh lệch điểm.
- Nguồn: Jeffrey Dastin, “Amazon scraps secret AI recruiting tool that showed bias against women” — Reuters, 10/10/2018 — [đọc bài trên Investing.com](https://www.investing.com/news/stock-market-news/amazon-scraps-secret-ai-recruiting-tool-that-showed-bias-against-women-1637988), các mục mô tả công cụ và dữ liệu huấn luyện.
- Phân biệt bằng chứng và nhận định: Reuters đưa tin về dấu hiệu thiên lệch, chi tiết của mô hình và việc dự án bị dừng dựa trên các nguồn ẩn danh am hiểu dự án. Nhận định của tôi: cách học từ lịch sử tuyển dụng có thể lặp lại thiên lệch giới nếu lịch sử phản ánh sự thiếu đại diện. Bài báo không cho biết bao nhiêu ứng viên thực tế bị từ chối vì công cụ; Amazon cũng nói nhà tuyển dụng xem gợi ý nhưng không chỉ dựa vào xếp hạng để tuyển.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | Khi mô hình xếp hạng hồ sơ và nhà tuyển dụng dùng thứ hạng để quyết định ai được xem xét hoặc phỏng vấn. |
| Stakeholder bị ảnh hưởng | Ứng viên nữ, đặc biệt người có kinh nghiệm/hoạt động liên quan đến phụ nữ hoặc học tại trường nữ sinh; nhà tuyển dụng và Amazon cũng chịu rủi ro về chất lượng, công bằng và niềm tin. |
| Failure mode | Thiên lệch trong dữ liệu huấn luyện khiến mô hình học các mẫu gắn với lịch sử tuyển dụng nam giới, rồi dùng dấu hiệu liên quan đến giới làm tín hiệu đánh giá thấp. |
| Layer bắt đầu lỗi | Model — nguồn gợi ý vấn đề nằm ở mô hình học mẫu từ dữ liệu tuyển dụng lịch sử. Reuters không cung cấp chi tiết kỹ thuật đủ để xác định chính xác nguyên nhân bên trong mô hình. |
| Harm xảy ra là gì? | Reuters xác nhận mô hình có dấu hiệu chấm bất lợi cho các hồ sơ có từ “women’s” và người tốt nghiệp từ hai trường nữ sinh; dự án bị dừng. Việc ứng viên cụ thể mất cơ hội việc làm do công cụ là nguy cơ hợp lý, nhưng bài báo không xác nhận số người hay trường hợp tuyển dụng cụ thể. |
| Harm lens | Công bằng / phân biệt đối xử trong cơ hội tiếp cận việc làm; minh bạch và khả năng giải trình. |
| Severity | High — nhận định: nếu thứ hạng ảnh hưởng đến quyền được phỏng vấn, tác động có thể ảnh hưởng đáng kể đến cơ hội nghề nghiệp. Chưa có dữ liệu về hậu quả cụ thể với từng ứng viên. |
| Scale | Chưa xác định số ứng viên bị tác động. Công cụ được thiết kế để hỗ trợ sàng lọc hồ sơ; nguồn chỉ nêu dữ liệu huấn luyện 10 năm và quy mô mô hình, không nêu số người bị loại. |
| Probability | Có bằng chứng thiên lệch đã xuất hiện trong thử nghiệm; xác suất một ứng viên cụ thể bị loại vì thiên lệch không thể ước lượng từ bài báo. |
| Frequency | Không rõ. Reuters không công bố tần suất lỗi hoặc số hồ sơ bị chấm thấp. |
| Vì sao? | Các đánh giá về thiên lệch dựa trên Reuters. Mức severity là nhận định về hệ quả tiềm tàng của sàng lọc tuyển dụng. Không có số liệu đủ để định lượng scale, probability hoặc frequency cho ứng viên; nhà tuyển dụng được cho biết đã xem gợi ý nhưng không chỉ dựa vào xếp hạng. |

### 3. Case study 2 — Mobley v. Workday: cáo buộc thiên lệch trong sàng lọc ứng viên

#### Brief Case

- Tổ chức / sản phẩm AI: Workday, nhà cung cấp nền tảng quản trị nhân sự và công cụ sàng lọc ứng viên có dùng thuật toán/AI và machine learning.
- Thời gian, địa điểm / bối cảnh: Vụ kiện liên bang tại California, khởi kiện năm 2023. Nguyên đơn Derek Mobley nói ông nộp đơn từ năm 2017 qua các doanh nghiệp dùng công cụ Workday. Tòa liên bang ra quyết định về yêu cầu bác đơn ngày 12/07/2024; vụ kiện vẫn đang tiếp diễn theo hồ sơ tòa năm 2026.
- AI được dùng để làm gì: Theo đơn kiện, công cụ đánh giá, xếp hạng, sàng lọc và có thể đề xuất chuyển tiếp hoặc từ chối hồ sơ cho doanh nghiệp sử dụng nền tảng.
- Vấn đề hoặc sự kiện đáng chú ý: Mobley cáo buộc công cụ sàng lọc gây tác động bất lợi cho ứng viên da đen, trên 40 tuổi và/hoặc khuyết tật. Tòa năm 2024 cho phép một số khiếu nại về tác động phân biệt tiếp tục ở giai đoạn tố tụng; đây không phải phán quyết rằng Workday đã phân biệt đối xử. Năm 2026, vụ kiện vẫn có hồ sơ tố tụng tiếp diễn.
- Số liệu có nguồn: Quyết định tòa ngày 12/07/2024 ghi nhận cáo buộc của Mobley rằng ông đã ứng tuyển hơn 100 vị trí tại các doanh nghiệp dùng công cụ Workday kể từ năm 2017. Đây là số đơn do nguyên đơn nêu, không phải số ứng viên bị ảnh hưởng đã được tòa xác minh. Hồ sơ không cho biết tỷ lệ từ chối của toàn bộ người dùng nền tảng.
- Nguồn: *Mobley v. Workday, Inc.*, Order Granting Preliminary Collective Certification, N.D. Cal., 16/05/2025, trang 4 — [bản quyết định trên GovInfo](https://www.govinfo.gov/content/pkg/USCOURTS-cand-3_23-cv-00770/pdf/USCOURTS-cand-3_23-cv-00770-1.pdf). Cập nhật tố tụng: *Mobley v. Workday, Inc.*, Order, N.D. Cal., 01/07/2026 — [bản quyết định](https://law.justia.com/cases/federal/district-courts/california/candce/3%3A2023cv00770/408645/372/).
- Phân biệt bằng chứng và nhận định: Hồ sơ tòa xác nhận có vụ kiện, nội dung khiếu nại và quyết định tố tụng; hơn 100 đơn là cáo buộc của Mobley. Tòa năm 2024 kết luận một số khiếu nại đủ cơ sở để tiếp tục ở giai đoạn tố tụng, không kết luận rằng công cụ gây ra phân biệt đối xử. Nhận định của tôi: nếu lọc tự động chặn hồ sơ trước khi con người xem, ứng viên có thể mất cơ hội phỏng vấn; nguồn chưa xác định mức độ tác động trên toàn hệ thống.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | Khi hệ thống sàng lọc xếp hạng hoặc loại hồ sơ trước khi ứng viên được phỏng vấn; đặc biệt nếu thư từ chối được phát tự động mà không có người xem xét thực chất. |
| Stakeholder bị ảnh hưởng | Ứng viên nộp hồ sơ qua nền tảng Workday; trong vụ kiện, các nguyên đơn cáo buộc tác động bất lợi với người da đen, người trên 40 tuổi và người khuyết tật. Nhà tuyển dụng sử dụng công cụ cũng liên quan. |
| Failure mode | Nguy cơ công cụ tạo kết quả sàng lọc có tác động khác nhau giữa các nhóm được bảo vệ; có thể có proxy như tuổi tốt nghiệp hoặc khoảng trống việc làm. Cơ chế cụ thể trong vụ này chưa được xác lập. |
| Layer bắt đầu lỗi | Model — cáo buộc tập trung vào thuật toán/AI sàng lọc và xếp hạng. Chưa có đủ bằng chứng công khai trong quyết định được dẫn để xác định thành phần kỹ thuật hoặc nguyên nhân gốc cụ thể. |
| Harm xảy ra là gì? | Mobley khai đã bị từ chối sau hơn 100 đơn ứng tuyển. Nguy cơ là người đủ năng lực mất cơ hội phỏng vấn/việc làm và thu nhập. Chưa có phán quyết xác nhận các lần từ chối do AI hoặc do phân biệt đối xử. |
| Harm lens | Công bằng và cơ hội tiếp cận việc làm; tác động kinh tế và khả năng giải trình khi quyết định bị tự động hóa. |
| Severity | High — nhận định: nếu sàng lọc bất lợi lặp lại, nó có thể cản trở cơ hội nghề nghiệp và thu nhập. Chưa có kết luận tư pháp về hậu quả thực tế trong vụ này. |
| Scale | Chưa xác định quy mô toàn hệ thống. Con số hơn 100 là số vị trí Mobley nói ông đã ứng tuyển, không phải số người bị tác động. |
| Probability | Không thể ước lượng từ hồ sơ này. Khiếu nại nêu một nguy cơ cần điều tra; việc tòa cho một số yêu cầu tiếp tục không chứng minh xác suất hoặc xác nhận vi phạm. |
| Frequency | Mobley nói ông nhận từ chối qua hơn 100 đơn; tần suất lỗi hệ thống trên toàn bộ hồ sơ không rõ. |
| Vì sao? | Dữ liệu định lượng gắn với nguyên đơn và lời khai trong hồ sơ. Tòa giải quyết ngưỡng tố tụng, không phải tính đúng sai cuối cùng. Cần dữ liệu kiểm toán theo nhóm, tiêu chí sàng lọc, và bằng chứng về mức con người rà soát để kết luận thêm. |
