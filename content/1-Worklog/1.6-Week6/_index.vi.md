---
title: "Worklog Tuần 6"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---



### Mục tiêu tuần 6:

* Ôn tập các khái niệm cơ bản về Cơ sở dữ liệu: mô hình quan hệ (relational model), khóa chính/khóa ngoại (primary/foreign keys), ACID, chuẩn hóa (normalization), OLTP so với OLAP.

* Hiểu về Amazon RDS như một dịch vụ cơ sở dữ liệu quan hệ được quản lý trên AWS: các engines, Multi-AZ, read replicas, sao lưu (backup) và mở rộng (scaling).

* Tìm hiểu lợi ích của Amazon Aurora so với các RDS engines tiêu chuẩn: hiệu suất, tính sẵn sàng cao, tự động mở rộng lưu trữ, tương thích MySQL/PostgreSQL.

* Làm quen với Amazon Redshift như một kho dữ liệu (data warehouse) quy mô petabyte cho phân tích, và phân biệt nó với RDS (tải công việc OLTP).

* Tìm hiểu cách Amazon ElastiCache (Redis / Memcached) cung cấp lớp bộ nhớ đệm (cache) trong bộ nhớ để giảm độ trễ và giảm tải cho cơ sở dữ liệu backend.

* Thực hành Chuyển đổi Schema & Di chuyển CSDL sử dụng AWS DMS và AWS Schema Conversion Tool (SCT) để chuyển cơ sở dữ liệu lên AWS.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Ôn tập các khái niệm CSDL: mô hình quan hệ, ACID, giao dịch, đánh chỉ mục (indexing), chuẩn hóa, OLTP so với OLAP. <br> - Đối chiếu các khái niệm cơ sở dữ liệu tại chỗ (on-premises) truyền thống với các dịch vụ đám mây AWS.                                                                                                   | 10/13/2025 | 10/13/2025      | [AWS Study group Youtube Video](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217) |
| 3   | - Học lý thuyết về Amazon RDS & Amazon Aurora. . <br> - Tìm hiểu về các engine được hỗ trợ, Multi-AZ, sao lưu tự động, snapshots, read replicas và khả năng mở rộng. <br> - So sánh RDS và Aurora về hiệu năng, tính sẵn sàng và chi phí.                                             | 10/14/2025 | 10/14/2025      |  [Hướng dẫn sử dụng AWS AmazonRDS ](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) <br> [Tài liệu AWS AmazonRDS Aurora ](https://aws.amazon.com/rds/aurora/) |
| 4   | - Nghiên cứu Amazon Redshift & Amazon ElastiCache. . <br> - Phân biệt OLTP (RDS/Aurora) với OLAP (Redshift) và lớp bộ nhớ đệm in-memory (ElastiCache).. <br> - Khám phá các trường hợp sử dụng phổ biến: kho dữ liệu & BI, caching sessions, bảng xếp hạng (leaderboard), giới hạn tốc độ (rate limiting), v.v. | 10/15/2025 | 10/15/2025      |[Thông tin về AWS Redshift ](https://aws.amazon.com/redshift/) <br> [Thông tin về AWS Elasticache](https://aws.amazon.com/elasticache/) |
| 5   | - **Thực hành:** <br>&emsp; + Module 06-Lab 5 – Amazon Relational Database Service (Amazon RDS). <br>&emsp; + Tạo một RDS instance, cấu hình security group, parameter group, sao lưu. <br>&emsp; + Kết nối từ máy trạm (client), chạy truy vấn và kiểm tra hoạt động.                            | 10/16/2025 | 10/16/2025      | [Amazon Relational Database Service (Amazon RDS) ](https://000005.awsstudygroup.com/vi/) |
| 6   | - **Thực hành:** <br>&emsp; + Module 06-Lab 43 – Chuyển đổi Schema & Di chuyển Cơ sở dữ liệu. <br>&emsp; + Sử dụng AWS Schema Conversion Tool (SCT) để phân tích và chuyển đổi schema từ DB nguồn sang đích RDS/Aurora/Redshift. <br>&emsp; + Sử dụng AWS Database Migration Service (DMS) để di chuyển dữ liệu   <br>  -  Tổng hợp và ôn tập tất cả các Dịch vụ Cơ sở dữ liệu AWS                                                                        | 10/17/2025 | 10/17/2025      | [Chuyển đổi lược đồ và di dời CSDL ](https://000043.awsstudygroup.com/) |


### Kết quả đạt được tuần 6:
* Củng cố hiểu biết về các khái niệm cốt lõi của cơ sở dữ liệu:

  * Bảng quan hệ, khóa chính/khóa ngoại, tính toàn vẹn quan hệ và đánh chỉ mục (indexing) cơ bản.

  * Các tính chất ACID của giao dịch và tầm quan trọng của chúng trong các tải công việc OLTP.

  * Phân biệt rõ ràng giữa OLTP và OLAP cũng như cách chúng tương ứng với các dịch vụ AWS.

* Đã làm quen thực tế với Amazon RDS:

  * Đã tạo và quản lý các RDS instance thông qua AWS Management Console.

  * Đã xem xét các engine được hỗ trợ (MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, Aurora) và các trường hợp sử dụng điển hình của chúng.

  * Đã thực hành cấu hình Multi-AZ, sao lưu tự động, snapshots, giám sát và các tùy chọn mở rộng cơ bản.

* Đã hiểu các thế mạnh của Amazon Aurora:

  * Aurora là cơ sở dữ liệu cloud-native, tương thích MySQL/PostgreSQL với hiệu suất được cải thiện đáng kể so với các engine tiêu chuẩn.

  * Kiến trúc cụm cơ sở dữ liệu Aurora (Aurora DB cluster), với lớp lưu trữ phân tán trên nhiều AZ.

  * Các endpoint đọc (Reader) và ghi (Writer), tự động mở rộng lưu trữ và thiết kế sẵn sàng cao.

* Hiểu cách sử dụng Amazon Redshift & ElastiCache:

  * Redshift là kho dữ liệu dạng cột (columnar), quy mô petabyte được tối ưu hóa cho phân tích và tải công việc BI.

  * Sự khác biệt giữa Redshift và RDS/Aurora: tối ưu hóa cho các truy vấn phức tạp trên tập dữ liệu lớn thay vì các tải công việc giao dịch.

  * ElastiCache (Redis/Memcached) là lớp bộ nhớ đệm (cache) trong bộ nhớ được quản lý hoàn toàn, độ trễ thấp giúp tăng thông lượng và giảm tải cho các cơ sở dữ liệu backend.


