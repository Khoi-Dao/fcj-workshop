---
title: "Blog 2"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---



# Chuyển đổi tài liệu kỹ thuật SAP bằng GenAI: Tăng tốc tạo tri thức cho SAP Notes với Amazon Bedrock

**Bài viết này được đồng tác giả bởi AWS và SAP**

---

### SAP Notes là gì?


SAP Notes và Knowledge Base Articles (KBA) là những thành phần cốt lõi trong hệ sinh thái hỗ trợ của SAP.
 Các tài liệu này cung cấp hướng dẫn chi tiết và giải pháp cho các vấn đề đã biết trong sản phẩm phần mềm SAP.
SAP Notes tập trung chủ yếu vào chỉnh sửa mã và giải pháp kỹ thuật.


KBAs bổ trợ bằng cách mô tả vấn đề theo ngôn ngữ nghiệp vụ, thường có hình ảnh minh họa.


Kết hợp lại, chúng tạo nên một kho tri thức toàn diện, giúp người dùng và tư vấn viên xử lý và khắc phục sự cố SAP một cách hiệu quả.


---

### Thách thức mà khách hàng gặp phải khi điều hướng hệ thống và tài liệu SAP phức tạp


Khi các chuyên gia SAP ngày càng làm việc trên thiết bị di động để xử lý sự cố nhanh chóng, việc truy cập tài liệu quan trọng như SAP Notes trở thành thách thức lớn.
Mặc dù người dùng mong muốn tra cứu và truy xuất SAP Notes ngay lập tức trên điện thoại hoặc máy tính bảng, nội dung lại chỉ được tối ưu cho trình duyệt máy tính, khiến họ phải phóng to, cuộn nhiều và đọc các đoạn văn dài.
Các bước triển khai quan trọng hoặc sửa lỗi khẩn cấp thường ẩn sâu trong ngôn ngữ kỹ thuật rối rắm và bố cục nhiều trang, không phù hợp với màn hình nhỏ.
Điều này dẫn đến chậm trễ trong việc khắc phục sự cố, tăng nguy cơ sai sót và mệt mỏi nhận thức trong quá trình xử lý nhiệm vụ quan trọng.


---
### Tính năng tóm tắt mà nhóm SAP for Me giới thiệu là gì?

Để khắc phục những thách thức này, nhóm SAP for Me đã hợp tác với AWS.
 Bằng cách sử dụng Amazon Bedrock, họ đã phát triển phiên bản mới của ứng dụng di động có tích hợp tính năng tóm tắt nội dung bằng AI cho SAP Notes và KBAs.
Công nghệ này cho phép người dùng nắm bắt và hiểu nội dung tài liệu kỹ thuật nhanh chóng thông qua các bản tóm tắt ngắn gọn, được tạo tự động.


---

### Tính năng tóm tắt mang lại lợi ích gì cho người dùng SAP for Me Mobile?

* Nhờ tính năng tóm tắt này, người dùng có thể:
  * Nhanh chóng đánh giá mức độ liên quan của SAP Note đối với tình huống nghiệp vụ cụ thể.


  * Tiếp cận ngay yêu cầu và điều kiện triển khai mà không cần đọc toàn bộ tài liệu.


  * Chuyển đổi tài liệu kỹ thuật dài dòng thành nội dung thân thiện với thiết bị di động, làm nổi bật các bước quan trọng mà không cần cuộn trang nhiều.


Điều này giúp rút ngắn đáng kể thời gian xử lý trong các tình huống khẩn cấp.
Các nhóm hỗ trợ Basis, Functional và tư vấn viên có thể làm việc hiệu quả hơn khi di chuyển, trong khi tri thức chuyên sâu trở nên dễ tiếp cận hơn — hỗ trợ ra quyết định nhanh và chính xác.


---

### Xây nền tảng: từ tầm nhìn đến triển khai đầu tiên

##### Nghĩ lớn – Bắt đầu nhỏ

Sau khi tích hợp Amazon Bedrock vào SAP Generative AI Hub (bao gồm Claude 3.5 Sonnet và Amazon Titan) được công bố tại SAP Sapphire 2024, AWS đã phối hợp cùng SAP China Labs tổ chức các hội thảo Generative AI.
Trong quá trình hợp tác, hai bên xác định SAP Notes và KBAs – với hàng triệu tài liệu kỹ thuật – là ứng viên lý tưởng để ứng dụng Generative AI.
 Các nhóm đã duy trì họp hàng tuần, thiết lập hỗ trợ theo yêu cầu, triển khai SAP Generative AI Hub và gọi mô hình Claude thông qua Amazon Bedrock API.
Mặc dù gặp thách thức kỹ thuật ban đầu, nhưng với sự hỗ trợ từ AWS, nhóm SAP đã đáp ứng được thời hạn triển khai trước Giáng Sinh 2024.

##### Những trở ngại ban đầu

Nhóm dự án chịu áp lực thời gian khi cần tóm tắt 6 triệu SAP Notes trong khung thời gian ngắn.
Việc đảm bảo tính chính xác kỹ thuật của các bản tóm tắt AI và xây dựng hệ thống cập nhật hiệu quả cho cả ghi chú mới và cũ là những thách thức quan trọng.


---

### Kiến trúc chuyên sâu: Kho tri thức làm nền tảng

Dự án sử dụng Retrieval-Augmented Generation (RAG) để cung cấp câu trả lời chính xác cho người dùng trực tiếp từ SAP Notes và KBAs, loại bỏ việc tìm kiếm thủ công qua nhiều tài liệu.
Khách hàng được hưởng lợi từ truy cập tức thì tới thông tin chính xác và liên quan, giúp tăng tốc quá trình xử lý sự cố.

##### 1. Giai đoạn xử lý dữ liệu
Hệ thống RAG bắt đầu với pipeline thu thập và xử lý dữ liệu tùy chỉnh cho SAP Notes và KBAs:
  * Thu thập, làm sạch và chuyển đổi tài liệu HTML thành định dạng có thể truy xuất.


  * Trích xuất văn bản, siêu dữ liệu (số note, phiên bản phát hành, tính áp dụng).


  * Giải quyết tham chiếu chéo giữa các tài liệu.


  * Áp dụng phân đoạn ngữ nghĩa và nhận dạng thực thể (entity recognition) để chia nội dung thành các khối ngữ cảnh có ý nghĩa.


  * Mã hóa các khối này thành vector embedding đa chiều bằng Amazon Titan Embedding Model, sau đó lưu trữ trong HANA vector database để truy vấn tương tự nhanh chóng.

##### 2. Giai đoạn truy vấn

Khi người dùng gửi câu hỏi, hệ thống sẽ:
  * Dùng HANA vector database để truy xuất top-k đoạn nội dung có ngữ nghĩa gần nhất.


  * Thực hiện xếp hạng lại (reranking) dựa trên độ liên quan, ngày phát hành và phạm vi áp dụng.


  * Ngữ cảnh được đưa vào mô hình Claude 3.5 Sonnet thông qua SAP Generative AI Hub trên Amazon Bedrock, mô hình sẽ tổng hợp câu trả lời tự nhiên, ngắn gọn và chính xác, có trích dẫn nguồn gốc rõ ràng.

Cách tiếp cận lai này đảm bảo tốc độ và độ chính xác, giúp giảm thiểu hiện tượng “ảo giác” (hallucination) và rút ngắn thời gian xử lý sự cố theo thời gian thực.

---

### Giá trị và lợi ích cho khách hàng


Hai sáng kiến “Summary for SAP Notes/KBA” và “RAG for SAP Notes/KBA” mang lại giá trị kinh doanh to lớn, bao gồm:
  * Truy cập thông tin nhanh và chính xác hơn, giúp rút ngắn thời gian khắc phục sự cố.


  * Tối ưu hóa năng suất và giảm thời gian gián đoạn hệ thống.


  * Tăng khả năng tận dụng sản phẩm SAP, nâng cao trải nghiệm hỗ trợ khách hàng.


  * Tăng cường hiệu quả vận hành thông qua khả năng tra cứu thông minh và truy xuất ngữ cảnh.


---

### Bước tiếp theo: Gợi ý trực tuyến theo ngữ cảnh

Nhóm SAP for Me đang mở rộng từ tóm tắt cơ bản sang RAG có tác nhân (agentic RAG) và đồ thị tri thức (knowledge graph).
 Những bước này sẽ giúp:
  * Cung cấp hướng dẫn kỹ thuật thông minh và có ngữ cảnh.


  * Hình dung mối liên hệ giữa các hệ thống và bản đồ tri thức.


  * Tích hợp hỗ trợ dự đoán và gợi ý cá nhân hóa, nhằm cải thiện trải nghiệm người dùng toàn diện.

Mục tiêu cuối cùng là xây dựng một hệ thống hỗ trợ mạnh mẽ, trực quan và thích ứng cao cho người dùng SAP.

---

### Kết luận

Hành trình Generative AI của SAP for Me thể hiện tác động chuyển đổi sâu sắc của AI khi được ứng dụng hợp lý vào phần mềm doanh nghiệp.
 Thông qua Amazon Bedrock và Claude 3.5 Sonnet, SAP đã giải quyết bài toán tiếp cận tri thức, triển khai khả năng tóm tắt tự động cho kho tài liệu kỹ thuật khổng lồ.
Mặc dù gặp nhiều thách thức ban đầu như đào tạo nhân sự AI và đảm bảo độ chính xác kỹ thuật, sự hợp tác giữa SAP và AWS đã giúp hoàn thành tính năng tóm tắt trước kỳ nghỉ lễ 2024.
Thành tựu này không chỉ là một cột mốc kỹ thuật, mà còn là bước ngoặt trong cách người dùng SAP truy cập và sử dụng tri thức kỹ thuật trên thiết bị di động.
Lộ trình sắp tới – với agentic RAG, knowledge graph và gợi ý chủ động – thể hiện tầm nhìn chiến lược chuyển đổi từ tài liệu tĩnh sang hệ thống tri thức động, kết nối và thông minh.
 Điều này hứa hẹn chuyển đổi mô hình hỗ trợ khách hàng của SAP từ giải quyết sự cố bị động sang hướng dẫn chủ động được cá nhân hóa.

 ---

 Chúng tôi khuyến khích bạn trải nghiệm các tính năng mới của ứng dụng SAP for Me Mobile, và khám phá cách Generative AI có thể thay đổi hoàn toàn việc hỗ trợ kỹ thuật và quản lý tri thức.
 Hãy liên hệ với chúng tôi để tìm hiểu cách bạn có thể tận dụng Amazon Bedrock nhằm nâng cao hiệu quả và khai mở giá trị cho tổ chức của mình.
