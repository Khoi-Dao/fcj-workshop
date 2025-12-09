---
title: "Worklog Tuần 4"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---



### Mục tiêu tuần 4:

* Tìm hiểu sâu hơn về dịch vụ lưu trữ cốt lõi của AWS là Amazon S3.

* Nắm vững các khái niệm chính: bucket, object, storage class, access point, static website hosting và CORS.

* Nghiên cứu các giải pháp lưu trữ lai (hybrid storage) và di chuyển dữ liệu như AWS Storage Gateway và AWS Snow Family.

* Trải nghiệm với Amazon FSx for Windows File Server và dịch vụ sao lưu tự động AWS Backup.

* Thực hành triển khai, quản lý và tích hợp các dịch vụ lưu trữ AWS trong môi trường thực tế.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Học lý thuyết về Dịch vụ lưu trữ AWS (S3) <br> - Làm quen với các khái niệm Bucket, Object và cơ chế lưu trữ.                                       | 09/29/2025 | 09/29/2025      |1. [Tài liệu AWS S3](https://docs.aws.amazon.com/s3/)  |
| 3   | - Tìm hiểu về Access Point và Storage Class (Lớp lưu trữ) <br> - Phân biệt các lớp lưu trữ: Standard, IA, Glacier, Deep Archive.                                             | 09/30/2025 | 09/30/2025      | [Thông tin về AWS S3 Storage Class](https://docs.aws.amazon.com/AmazonS3/latest/dev/storage-class-intro.html) |
| 4   | - Tìm hiểu S3 Static Website & CORS, Access Control (Kiểm soát truy cập), Object Key, Hiệu suất và Glacier | 10/01/2025 | 10/01/2025      | [	Hướng dẫn sử dụng AWS S3 web hosting](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html) |
| 5   | - **Labs:** <br>&emsp; + Lab14 – VM Import/Export (Nhập/Xuất máy ảo).                         | 10/02/2025 | 10/02/2025      |  [AWS Study Group - Lab14 : VM Import/Export (Nhập/Xuất máy ảo)](https://000014.awsstudygroup.com/vi/)  |
| 6   | - **Labs:** <br>&emsp;+ Lab25 – Amazon FSx for Windows File Server.  <br> - Ôn tập và củng cố kiến thức về tất cả các dịch vụ lưu trữ AWS services.                                                                                   | 10/03/2025 | 10/03/2025      | [AWS Study Group - Lab25 :Triển khai FSx trên Windows](https://000025.awsstudygroup.com/vi/)  |


### Kết quả đạt được tuần 4:

* Đã hiểu kiến trúc và nguyên lý hoạt động của Amazon S3, bao gồm:

  * Cách tạo và quản lý Buckets, Objects và Access Policies (chính sách truy cập).

  * Các loại Storage Classes khác nhau và chiến lược tối ưu hóa chi phí lưu trữ.

  * Cách cấu hình S3 Static Website Hosting và xử lý CORS cho các ứng dụng web.

* Đã trải nghiệm S3 Glacier – dịch vụ lưu trữ lạnh (cold storage) giúp tiết kiệm chi phí cho dữ liệu ít được truy cập.

* Đã hiểu về Lưu trữ lai (Hybrid Storage) & Di chuyển dữ liệu (Data Migration) thông qua:

  * AWS Snow Family (Snowcone, Snowball, Snowmobile).

  * AWS Storage Gateway – giải pháp kết nối các hệ thống tại chỗ (on-premises) với AWS Cloud.



