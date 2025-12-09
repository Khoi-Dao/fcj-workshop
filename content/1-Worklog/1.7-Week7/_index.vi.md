---
title: "Worklog Tuần 7"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---



### Mục tiêu tuần 7:

* Hiểu về Amazon DynamoDB như một dịch vụ cơ sở dữ liệu NoSQL được quản lý hoàn toàn: các mô hình dữ liệu key-value và document, partition keys, sort keys, Global Secondary Indexes (GSI), và các chế độ dung lượng on-demand (theo nhu cầu) so với provisioned (định trước).

* Học cách xây dựng và quản lý Data Lake trên AWS sử dụng các dịch vụ như Amazon S3, AWS Glue, Amazon Athena và Amazon QuickSight cho các khối lượng công việc phân tích.

* Khám phá các dịch vụ Phân tích AWS: Amazon Athena cho các truy vấn SQL serverless trên S3, AWS Glue cho các hoạt động ETL, và Amazon QuickSight cho trí tuệ doanh nghiệp (BI) và trực quan hóa.

* Thực hành các quy trình thu thập (ingestion), chuyển đổi và phân tích dữ liệu trong môi trường đám mây AWS.

* Hiểu các chiến lược tối ưu hóa chi phí và hiệu suất cho các tác vụ phân tích trên AWS.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Thực hành:** Data Lake trên AWS.  <br>&emsp; + Hiểu kiến trúc Data Lake trên AWS sử dụng S3 làm lớp lưu trữ. <br>&emsp; + Tìm hiểu các mô hình nạp dữ liệu (ingestion), lập danh mục (cataloging) và truy vấn. <br>&emsp; +  Khám phá sự tích hợp giữa S3, Glue và Athena cho phân tích.                                                                                                 | 10/20/2025 | 10/20/2025      | [Data Lake trên AWS](https://000035.awsstudygroup.com/) |
| 3   | -   **Thực hành:** Amazon DynamoDB Immersion Day.  <br>&emsp; + Đi sâu vào các khái niệm cốt lõi của DynamoDB: bảng (tables), mục (items), thuộc tính (attributes), khóa chính và chỉ mục. <br>&emsp; + Thực hành tạo bảng, chèn dữ liệu và truy vấn với partition keys và sort keys. <br>&emsp; +  Hiểu các chế độ dung lượng DynamoDB (on-demand so với provisioned) và mô hình tính giá.                                           | 10/21/2025 | 10/21/2025      |  [Amazon DynamoDB Immersion Day](https://000039.awsstudygroup.com/)  |
| 4   | **Thực hành:** Phân tích chi phí và hiệu suất với AWS Glue và Amazon Athena.  <br>&emsp; + Sử dụng AWS Glue để lập danh mục dữ liệu lưu trữ trong S3 và tạo data catalogs. <br>&emsp; + Chạy truy vấn SQL trên dữ liệu S3 sử dụng Amazon Athena. <br>&emsp; +  Phân tích tác động chi phí và tối ưu hóa hiệu suất truy vấn. <br>&emsp; + Hiểu các chiến lược phân vùng (partitioning) để phân tích tiết kiệm chi phí. <br>   **Thực hành:** Làm việc với Amazon DynamoDB. <br>&emsp; + Tạo bảng DynamoDB với lược đồ khóa (key schemas) phù hợp. <br>&emsp; + Thực hiện các thao tác CRUD (Tạo, Đọc, Cập nhật, Xóa) trên các mục DynamoDB. <br>&emsp; + Làm việc với Global Secondary Indexes (GSI) và Local Secondary Indexes (LSI). <br>&emsp; + Thực hành các thao tác truy vấn (query) và quét (scan), hiểu sự khác biệt.   | 10/22/2025 | 10/22/2025      |[Phân tích chi phí và hiệu năng sử dụng với AWS Glue và Amazon Athena ](https://000040.awsstudygroup.com/) <br> [Làm việc với Amazon DynamoDB](https://000060.awsstudygroup.com/) |
| 5   | - **Thực hành:** Xây dựng Data Lake với dữ liệu của bạn.  <br>&emsp; + Xây dựng giải pháp data lake hoàn chỉnh sử dụng các dịch vụ AWS. <br>&emsp; + Triển khai các đường ống nạp dữ liệu (data ingestion pipelines). <br>&emsp; + Thiết lập quy trình chuyển đổi dữ liệu với AWS Glue.  <br>&emsp; +  Tạo các tập dữ liệu sẵn sàng phân tích cho các bước xử lý tiếp theo. <br> - **Thực hành:** Phân tích trên AWS workshop.  <br>&emsp; + Workshop toàn diện bao gồm toàn bộ các công cụ phân tích trên AWS.  <br>&emsp; + Tích hợp nhiều dịch vụ: S3, Glue, Athena và các công cụ trực quan hóa.  <br>&emsp; +  Xây dựng giải pháp phân tích đầu cuối (end-to-end) từ dữ liệu thô đến thông tin chi tiết.                         | 10/23/2025 | 10/23/2025      | [ây dựng Datalake với dữ liệu của bạn ](https://000070.awsstudygroup.com/) <br> [Analytics on AWS workshop](https://000072.awsstudygroup.com/) |
| 6   | - **Thực hành:** Bắt đầu với QuickSight. <br>&emsp; + Tạo trực quan hóa và bảng điều khiển (dashboards) sử dụng Amazon QuickSight. <br>&emsp; + Kết nối QuickSight với nhiều nguồn dữ liệu khác nhau (S3, Athena, RDS, v.v.). <br>&emsp; + Sử dụng AWS Database Migration Service (DMS) để di chuyển dữ liệu.  <br>&emsp; + Xây dựng báo cáo tương tác và chia sẻ thông tin với các bên liên quan.                                                                        | 10/24/2025 | 10/24/2025      | [Bắt đầu với Quick Sight ](https://000073.awsstudygroup.com/) |


### Kết quả đạt được tuần 7:

* Đạt được sự hiểu biết toàn diện về Amazon DynamoDB:

  * DynamoDB là dịch vụ cơ sở dữ liệu NoSQL serverless, được quản lý hoàn toàn với độ trễ thấp (chỉ một chữ số mili-giây).

  * Các khái niệm chính: bảng (tables), mục (items), thuộc tính (attributes), khóa chính (partition key + sort key tùy chọn), và các phương pháp mô hình hóa dữ liệu tốt nhất.

  * Global Secondary Indexes (GSI) và Local Secondary Indexes (LSI) cho các mẫu truy vấn linh hoạt.

  * Các chế độ dung lượng: on-demand (trả tiền theo yêu cầu) so với provisioned (dung lượng dành riêng) và thời điểm nên sử dụng từng loại.

  * DynamoDB Streams để xử lý dữ liệu thời gian thực và ghi nhận thay đổi dữ liệu (CDC).

* Có thêm kinh nghiệm về kiến trúc Data Lake trên AWS:

  * Amazon S3 đóng vai trò nền tảng cho lưu trữ Data Lake với các chính sách vòng đời, đánh phiên bản (versioning) và mã hóa.

* Hiểu sâu hơn về các dịch vụ Phân tích AWS:

  * AWS Glue: Dịch vụ ETL Serverless để khám phá, lập danh mục và chuyển đổi dữ liệu. Glue Data Catalog đóng vai trò là kho lưu trữ metadata tập trung. Glue ETL jobs để chuyển đổi dữ liệu sử dụng Apache Spark. Glue Crawlers để tự động khám phá lược đồ (schema).

  * Amazon Athena: Dịch vụ truy vấn SQL tương tác serverless để phân tích dữ liệu trong S3. Mô hình tính phí theo truy vấn và chiến lược tối ưu chi phí. Tích hợp với Glue Data Catalog cho các truy vấn schema-on-read. Tối ưu hóa hiệu suất truy vấn thông qua phân vùng và định dạng cột (Parquet, ORC).

  * Amazon QuickSight: Dịch vụ trực quan hóa và trí tuệ doanh nghiệp (BI) cloud-native. Tạo bảng điều khiển (dashboards), trực quan hóa và báo cáo. Kết nối với nhiều nguồn dữ liệu (S3, Athena, RDS, Redshift, v.v.). Chia sẻ thông tin chi tiết với các nhóm và nhúng phân tích vào ứng dụng.



