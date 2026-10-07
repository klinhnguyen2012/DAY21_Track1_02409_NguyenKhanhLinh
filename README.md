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
| High-risk moment | Lúc hệ thống sàng lọc xếp hạng hoặc loại hồ sơ trước khi ứng viên được phỏng vấn, nhất là khi từ chối được gửi tự động mà không có người xem xét thực chất. |
| Stakeholder bị ảnh hưởng | Nguyên đơn Mobley và các ứng viên khác nộp qua nền tảng Workday; trong hồ sơ, họ cáo buộc tác động bất lợi với người da đen, người trên 40 tuổi và người khuyết tật. Nhà tuyển dụng dùng nền tảng cũng liên quan. |
| Failure mode | **Bias / fairness (cáo buộc)** — kết quả sàng lọc có thể gây tác động khác nhau giữa các nhóm được bảo vệ. Hồ sơ nêu giả thuyết về dấu hiệu thay thế như năm tốt nghiệp hoặc khoảng trống việc làm, nhưng cơ chế chưa được xác minh. |
| Layer bắt đầu lỗi | **Chưa đủ bằng chứng.** Hồ sơ cáo buộc công cụ thuật toán/AI gây tác động bất lợi nhưng không xác định đủ nguyên nhân kỹ thuật. **Giả thuyết của tôi:** có thể liên quan đến Model hoặc tiêu chí sàng lọc; cần dữ liệu/kiểm toán để xác định. |
| Harm xảy ra là gì? | **Theo lời Mobley:** ông bị từ chối sau hơn 100 đơn ứng tuyển. **Nguy cơ:** ứng viên đủ năng lực mất cơ hội phỏng vấn, việc làm và thu nhập khi hồ sơ bị loại tự động. Chưa có phán quyết xác nhận AI gây ra các lần từ chối hoặc có phân biệt đối xử. |
| Harm lens | **Opportunity loss** — nguy cơ mất cơ hội phỏng vấn hoặc việc làm; **dignity loss** có thể phát sinh nếu ứng viên bị loại lặp lại mà không được giải thích, nhưng đây là nhận định chứ không phải kết luận của tòa. |
| Severity | **High** — đánh giá của tôi: nếu cáo buộc đúng và sàng lọc bất lợi lặp lại, hậu quả có thể ảnh hưởng đáng kể đến cơ hội nghề nghiệp và thu nhập. Tòa chưa xác nhận hậu quả do AI gây ra. |
| Scale | **Chưa đủ dữ liệu để đánh giá quy mô toàn hệ thống.** Mobley nói ông nộp hơn 100 đơn; con số đó không cho biết có bao nhiêu ứng viên khác bị ảnh hưởng. |
| Probability | **Chưa đủ dữ liệu để đánh giá xác suất tác hại.** Các cáo buộc được phép tiếp tục ở một số phần của vụ kiện không chứng minh xác suất hoặc xác nhận vi phạm. |
| Frequency | **Chưa đủ dữ liệu để đánh giá tần suất lỗi hệ thống.** Hơn 100 đơn là trải nghiệm được nguyên đơn nêu, không phải tỷ lệ lỗi trên toàn bộ hồ sơ. |
| Vì sao? | Hồ sơ tòa là nguồn cho nội dung cáo buộc và số đơn; không phải kết luận cuối cùng về tính đúng sai. Severity là đánh giá của tôi về hậu quả có thể có. Cần dữ liệu kiểm toán theo nhóm, tiêu chí sàng lọc và bằng chứng về mức người thật rà soát để đánh giá scale, probability, frequency và layer kỹ thuật. |
