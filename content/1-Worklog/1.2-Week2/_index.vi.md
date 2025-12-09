---
title: "Worklog Tuần 2"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---


### Mục tiêu tuần 2:

* Hiểu khái niệm và cấu trúc của VPC (CIDR, Subnet, Route Table, ENI).

* Học cách cấu hình tường lửa trong VPC (NACL, Security Group).

* Hiểu khái niệm về các dịch vụ mạng: VPN, Direct Connect.

* Trải nghiệm với Load Balancer.

* Thực hành tạo và cấu hình các thành phần cốt lõi: VPC, Subnet, Route Table, IGW, EBS, Elastic IP.

* Hiểu về kết nối từ xa đến EC2 thông qua SSH.

* Trải nghiệm Hybrid DNS sử dụng Route 53 Resolver.

* Trải nghiệm kết nối nhiều VPC sử dụng VPC Peering.

* Thử nghiệm AWS Transit Gateway để quản lý kết nối giữa các VPC.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Học lý thuyết <br> - VPC là gì và cách tối ưu hóa việc sử dụng dịch vụ đám mây  <br> - Tìm hiểu về VPC: <br>&emsp; + Subnet, CIDR <br>&emsp; + Bảng định tuyến (Route table) <br> &emsp; +ENI (Giao diện mạng đàn hồi)                                                                                                 | 09/15/2025 | 09/15/2025      |1. [Tài liệu AWS VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) <br>2. [Video YouTube - AWS VPC](https://www.youtube.com/watch?v=O9Ac_vGHquM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=25) |
| 3   | - Cấu hình tường lửa VPC: NACL, Security Group <br> - VPN, Direct Connect <br> - Cân bằng tải (Load Balancer) <br> - Tài nguyên tài liệu bổ sung                                              | 09/14/2025 | 09/14/2025      | [Video YouTube - AWS Security](https://www.youtube.com/watch?v=O9Ac_vGHquM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=25) |
| 4   | - **Thực hành (Labs):** <br>&emsp; + VPC + Subnet <br>&emsp; + Route Table <br> &emsp; + IGW (Cổng Internet) <br> &emsp; + EBS <br> &emsp; + ... <br> -  điều kiển từ xa vào EC2 sử dụng SSH <br> - Tìm hiểu Elastic IP | 09/15/2025 | 09/15/2025      | [AWS Study Group - 000003 : Bắt đầu với Amazon Virtual Private Cloud (VPC) và AWS Site-to-Site VPN](https://000003.awsstudygroup.com/vi/) |
| 5   | - **Thực hành (Labs):** <br>&emsp; + Thiết lập Hybrid DNS với Route 53 Resolver <br>&emsp;+ Thiết lập VPC Peering                          | 09/16/2025 | 09/16/2025      | [AWS Study Group - 000010 : Thiết lập Hybrid DNS với Route 53 Resolver](https://000010.awsstudygroup.com/vi/) <br> [AWS Study Group - 000019 : Thiết lập VPC Peering](https://000019.awsstudygroup.com/vi/)|
| 6   | - **Thực hành (Labs):** <br>&emsp; + Tiếp tục trải nghiệm VPC Peering <br>&emsp;+ Thiết lập AWS Transit Gateway                                                                                     | 09/17/2025 | 09/17/2025      | [AWS Study Group - 000020 : Tổng quan về AWS Transit Gateway](https://000020.awsstudygroup.com/vi/) |


### Kết quả đạt được tuần 2:

* Đã hiểu nền tảng của Amazon VPC và các thành phần chính: CIDR blocks, subnets, route tables, và ENIs.

* Đã trải nghiệm hoạt động bảo mật VPC sử dụng cả Security Groups và Network ACLs, đồng thời hiểu sự khác biệt về phạm vi và trường hợp sử dụng của chúng.

* Đã tìm hiểu các dịch vụ mạng của AWS: VPN và Direct Connect.

* Đã học về Elastic Load Balancing và vai trò của nó trong việc phân phối lưu lượng để đảm bảo tính sẵn sàng cao (high availability).

* Đã thực hiện các bài lab về các yếu tố thiết yếu của VPC: tạo subnet, cấu hình route table, gắn internet gateway (IGW), làm việc với EBS và quản lý Elastic IP.

* Củng cố kỹ năng truy cập và quản lý EC2 instance một cách an toàn qua SSH.

* Đã thử nghiệm và thực hành kết nối nhiều VPC thông qua VPC Peering.

* Đã triển khai AWS Transit Gateway để thiết kế và quản lý kiến trúc đa VPC có khả năng mở rộng.


