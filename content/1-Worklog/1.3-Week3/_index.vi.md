---
title: "Worklog Tuần 3"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---



### Mục tiêu tuần 3:

* Xây dựng nền tảng kiến thức vững chắc về Amazon EC2 và hệ sinh thái của nó (AMI, Backup, Key Pair, EBS, Instance Store, User Data, Metadata).

* Tìm hiểu về EC2 Auto Scaling và vai trò của nó trong việc đảm bảo tính đàn hồi và tối ưu hóa chi phí.

* Tìm hiểu và trải nghiệm các dịch vụ tính toán (compute) liên quan bao gồm EFS, FSx, Lightsail và AWS MGN.

* Củng cố kiến thức về lưu trữ AWS thông qua các bài thực hành (labs) bao gồm S3, AWS Backup và Storage Gateway.

* Củng cố kỹ năng thực tế trong việc cấu hình, quản lý và mở rộng quy mô các EC2 workloads.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Học lý thuyết: <br>&emsp; + Tổng quan về EC2: AMI, Backup, Key Pair   <br>&emsp; +EBS (Elastic Block Store) <br>&emsp; +  Instance Store                                                                                              | 09/22/2025 | 09/22/2025      |1. [Tài liệu AWS EC2](https://docs.aws.amazon.com/ec2/) <br>2. [Tài liệu AWS EBS](https://docs.aws.amazon.com/ebs/) |
| 3   | - Học lý thuyết: <br>&emsp; + EC2 User Data <br>&emsp; + EC2 Metadata                                             | 09/23/2025 | 09/23/2025      | [Hướng dẫn sử dụng AWS EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/) |
| 4   | - Learn theory: <br>&emsp; + EC2 Auto Scaling <br>&emsp; + Các dịch vụ liên quan: EFS, FSx, Lightsail, MGN | 09/24/2025 | 09/24/2025      | [	AWS Auto Scaling](https://docs.aws.amazon.com/autoscaling/) |
| 5   | - **Labs:** <br>&emsp; +  Lab 57: Làm quen với Amazon S3                          | 09/25/2025 | 09/25/2025      | [AWS Study Group - Lab57 : Khởi Đầu Với Amazon S3](https://000057.awsstudygroup.com/vi/) |
| 6   | - **Labs:** <br>&emsp; + Lab 13: Triển khai AWS Backup cho hệ thống <br>&emsp;+ Lab 24: Sử dụng AWS Storage Gateway                                                                                     | 09/26/2025 | 09/26/2025      | [AWS Study Group - Lab13 :Triển khai AWS Backup cho hệ thống](https://000013.awsstudygroup.com/vi/) <br> [AWS Study Group - Lab24:Triển khai File Storage Gateway](https://000024.awsstudygroup.com/vi/) |


### Kết quả đạt được tuần 3:

* Đã xây dựng được nền tảng kiến thức lý thuyết vững chắc về Amazon EC2, bao gồm:

AMI và các chiến lược sao lưu để đảm bảo khả năng phục hồi.

Cách sử dụng Key Pair để xác thực SSH an toàn.

Sự khác biệt giữa EBS (lưu trữ lâu dài) và Instance Store (lưu trữ tạm thời).

Cách User Data và Metadata tự động hóa việc khởi tạo instance và cung cấp cấu hình động.

Vai trò của EC2 Auto Scaling trong việc duy trì hiệu suất và hiệu quả chi phí.

* Đã tìm hiểu các dịch vụ liên quan:

  * Amazon EFS và FSx cho lưu trữ tệp chia sẻ và hiệu suất cao.

  * Amazon Lightsail như một giải pháp thay thế đơn giản hóa cho các quy mô công việc nhỏ.

  * AWS MGN để di chuyển (migrate) workloads lên AWS.

* Đã hoàn thành các bài thực hành (labs):

  * Khởi chạy và quản lý S3 bucket (Lab57).

  * Triển khai AWS Backup để bảo vệ dữ liệu (Lab13).

  * Tích hợp hệ thống on-premises với AWS sử dụng Storage Gateway (Lab24).

* Các kỹ năng chính đạt được:

  * Tự tin phân biệt các loại hình lưu trữ (EBS vs Instance Store vs EFS vs FSx).

  * Tự động hóa vòng đời EC2 với User Data và Auto Scaling.

  * Kết hợp các giải pháp sao lưu và lưu trữ lai (hybrid storage) để tạo ra các kiến trúc có khả năng phục hồi tốt hơn.

