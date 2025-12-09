---
title: "Worklog Tuần 10"
date: 2025-09-10
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---



### Mục tiêu tuần 10:

* Triển khai **Backend Layer**: EC2 instances trong private subnet với application runtime và cấu hình Auto Scaling.
* Thiết lập **Amazon RDS** database trong private subnet với cấu hình và parameter groups phù hợp.
* Deploy backend application và thiết lập kết nối giữa EC2 và RDS sử dụng Secrets Manager.
* Cấu hình **API Gateway** REST API với tích hợp EC2 backend.
* Tích hợp **Amazon Cognito** User Pool với API Gateway cho authentication và authorization.
* Cấu hình **Auto Scaling Group** cho EC2 instances với Launch Template cho scalability.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Làm quen với các thành viên FCJ <br> - Đọc và lưu ý các nội quy, quy định tại đơn vị thực tập                                                                                             | 11/08/2025   | 11/08/2025      |
| 3   | - Tìm hiểu AWS và các loại dịch vụ <br>&emsp; + Compute <br>&emsp; + Storage <br>&emsp; + Networking <br>&emsp; + Database <br>&emsp; + ... <br>                                            | 12/08/2025   | 12/08/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tạo AWS Free Tier account <br> - Tìm hiểu AWS Console & AWS CLI <br> - **Thực hành:** <br>&emsp; + Tạo AWS account <br>&emsp; + Cài AWS CLI & cấu hình <br> &emsp; + Cách sử dụng AWS CLI | 13/08/2025   | 13/08/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu EC2 cơ bản: <br>&emsp; + Instance types <br>&emsp; + AMI <br>&emsp; + EBS <br>&emsp; + ... <br> - Các cách remote SSH vào EC2 <br> - Tìm hiểu Elastic IP   <br>                  | 14/08/2025   | 15/08/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - **Thực hành:** <br>&emsp; + Tạo EC2 instance <br>&emsp; + Kết nối SSH <br>&emsp; + Gắn EBS volume                                                                                         | 15/08/2025   | 15/08/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 10:

* Triển khai thành công **Amazon RDS database**:

  * Tạo RDS subnet group trong private subnet để cô lập database.
  * Launch RDS instance (MySQL/PostgreSQL) với instance class và cấu hình phù hợp.
  * Cấu hình RDS parameter group với database-specific settings.
  * Thiết lập automated backups, encryption at rest, và monitoring.
  * Cấu hình RDS security group để chỉ cho phép kết nối từ EC2 Security Group.
  * Lưu trữ database credentials an toàn trong AWS Secrets Manager.

* Thiết lập **EC2 backend infrastructure**:

  * Launch EC2 instance trong private subnet với instance type phù hợp.
  * Cài đặt và cấu hình application runtime environment (Java/Python/Node.js).
  * Cấu hình EC2 instance với IAM role cho AWS service access.
  * Tạo base AMI từ EC2 instance đã cấu hình cho Auto Scaling Group.
  * Tài liệu hóa cấu hình EC2 và application setup procedures.

* Deploy **backend application**:

  * Deploy backend application code lên EC2 instance.
  * Cấu hình application để kết nối với RDS sử dụng credentials từ Secrets Manager.
  * Kiểm tra database connectivity và xác minh connection functionality.
  * Kiểm tra basic application functionality và database operations (CRUD).
  * Tài liệu hóa deployment process và application configuration.

* Cấu hình **API Gateway REST API**:

  * Tạo REST API với resources, methods, và integration points.
  * Thiết lập API Gateway VPC Link để kết nối với private subnet resources (EC2).
  * Cấu hình API Gateway integration với EC2 backend sử dụng HTTP/HTTPS.
  * Bật CORS cho frontend access với proper headers.
  * Kiểm tra API endpoints và xác minh tích hợp với EC2 backend.

* Tích hợp **Amazon Cognito** cho authentication:

  * Tạo Cognito User Pool với password policies, MFA, và email verification.
  * Tạo Cognito User Pool App Client cho application integration.
  * Cấu hình Cognito Authorizer trong API Gateway cho authenticated API access.
  * Kiểm tra user registration, login, và authenticated API access flows.
  * Thiết lập secure user authentication và authorization.

* Cấu hình **Auto Scaling Group** cho scalability:

  * Tạo Launch Template dựa trên base AMI cho consistent instance configuration.
  * Tạo Auto Scaling Group với Launch Template trong private subnet.
  * Cấu hình Auto Scaling policies (target tracking, step scaling) cho automatic scaling.
  * Thiết lập capacity limits phù hợp (minimum, desired, maximum).
  * Kiểm tra scale-out và scale-in functionality để xác minh automatic scaling.



