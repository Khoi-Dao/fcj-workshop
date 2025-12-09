---
title: "Worklog Tuần 5"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---



### Mục tiêu tuần 5:

* Hiểu về Mô hình Trách nhiệm Chia sẻ (Shared Responsibility Model) của AWS.

* Tìm hiểu các dịch vụ bảo mật chính của AWS bao gồm: IAM, Cognito, Security Hub, KMS, Identity Center.

* Củng cố khả năng quản lý tài nguyên và bảo mật thông qua IAM Permissions Boundaries, Resource Tags và các kỹ thuật mã hóa.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Học lý thuyết về Mô hình Trách nhiệm Chia sẻ (Shared Responsibility Model) và các nguyên tắc bảo mật AWS. <br> - Xem tài liệu về các dịch vụ bảo mật AWS: <br>&emsp; + Amazon IAM <br>&emsp; + Amazon Cognito <br>&emsp; + AWS Identity Center <br>&emsp; + AWS KMS <br>&emsp; + AWS Security Hub                                       | 10/06/2025 | 10/06/2025      | [AWS Study group: Triển khai AWS Backup cho hệ thống](https://000013.awsstudygroup.com/vi/)  |
| 3   | - **Thực hành:** <br>&emsp; + Cấu hình và sử dụng AWS Security Hub để giám sát và phát hiện các vấn đề bảo mật.  <br>&emsp; + Tạo và quản lý IAM Users, Roles, và Policies cho các tài khoản AWS.  <br>&emsp; +  Tạo IAM Groups và quản lý quyền truy cập cho nhóm người dùng.                                           | 10/07/2025 | 10/07/2025      | [AWS Study group: Tối ưu chi phí EC2 với Lambda](https://000022.awsstudygroup.com/vi/) |
| 4   | - **Thực hành:** <br>&emsp; + Tối ưu hóa chi phí EC2 sử dụng Lambda để tự động bật/tắt các EC2 instance.  <br>&emsp; + Quản lý truy cập EC2 thông qua Resource Tags sử dụng IAM. | 10/08/2025 | 10/08/2025      | [	AWS Study Group :Quản lý tài nguyên bằng Tag và Resource Groups](https://000027.awsstudygroup.com/vi/) |
| 5   | - **Thực hành:** <br>&emsp; + Cấu hình IAM Permission Boundaries để giới hạn đặc quyền người dùng.  <br>&emsp; + Mã hóa dữ liệu sử dụng AWS KMS.                        | 10/09/2025 | 10/09/2025      |  [AWS Study Group : Quản lý tài nguyên bằng Tag và Resource Groups](https://000027.awsstudygroup.com/vi/)  |
| 6   | - **Nghiên cứu thêm** <br>&emsp;+ Tìm hiểu và áp dụng các phương pháp bảo mật trong AWS Organizations để quản lý đa tài khoản.  <br>&emsp;+ Nâng cao kỹ năng về AWS Identity Center để quản lý và đồng bộ người dùng và nhóm trên các dịch vụ AWS.                                                                                   | 10/10/2025 | 10/10/2025      | [AWS Study Group - : GIỚI HẠN QUYỀN CỦA USER VỚI IAM PERMISSION BOUNDARY](https://000030.awsstudygroup.com/vi/)  |


### Kết quả đạt được tuần 5:

* Hiểu và Áp dụng Mô hình Trách nhiệm Chia sẻ của AWS:

  * Đã hiểu rõ AWS chịu trách nhiệm bảo mật hạ tầng đám mây, trong khi người dùng chịu trách nhiệm bảo mật dữ liệu và ứng dụng của mình.

  * Làm rõ vai trò trong việc đảm bảo tính tuân thủ và bảo vệ khi triển khai các dịch vụ trên AWS.

* Kiến thức lý thuyết về các Dịch vụ Bảo mật Cốt lõi của AWS:

  * Amazon IAM: Đã học cách tạo và quản lý Users, Roles và Policies để kiểm soát quyền truy cập của người dùng và nhóm.

  * Amazon Cognito: Nghiên cứu về quản lý người dùng và xác thực cho các ứng dụng AWS.

  * AWS Identity Center: Hiểu cách liên kết và quản lý quyền truy cập của người dùng trên nhiều dịch vụ AWS.

  * AWS Security Hub: Đã cấu hình và sử dụng để giám sát và phát hiện các mối đe dọa bảo mật.

  * AWS KMS: Thực hành mã hóa dữ liệu lưu trữ (data at rest) và bảo vệ dữ liệu nhạy cảm bằng các khóa mã hóa.

* Triển khai Thực tế các Dịch vụ Bảo mật AWS:

  * Đã cài đặt và cấu hình thành công AWS Security Hub để giám sát liên tục và phát hiện lỗ hổng.

  * Cấu hình IAM Permissions Boundaries để hạn chế đặc quyền người dùng và ngăn chặn truy cập trái phép.

  * Tối ưu hóa chi phí EC2 với Lambda: Tự động hóa việc tắt các EC2 instance không sử dụng để giảm thiểu chi phí vận hành.

  * Kiểm soát truy cập EC2 qua IAM & Resource Tags: Áp dụng các IAM Policy sử dụng thẻ (Tags) để xác định phạm vi truy cập một cách chính xác.

* Nâng cao Kỹ năng Quản lý Tài nguyên AWS:

  * Đã tạo và quản lý IAM Groups và Policies, cải thiện việc kiểm soát truy cập dựa trên nhóm.

  * Học cách quản lý nhiều tài khoản AWS sử dụng AWS Organizations, đảm bảo các chính sách bảo mật nhất quán trên toàn tổ chức.

