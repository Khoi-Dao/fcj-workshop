---
title: "Worklog Tuần 8"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---



### Mục tiêu tuần 8:

* Hoàn thiện Lớp Edge (Biên) và Lưu trữ Frontend: Route 53, S3, CloudFront, AWS WAF và ACM Certificate.

* Thiết lập quản lý DNS với Route 53 hosted zone và cấu hình tên miền.

* Cấu hình S3 bucket cho hosting frontend tĩnh với các chính sách truy cập phù hợp.

* Triển khai CloudFront distribution để phân phối nội dung toàn cầu với Origin Access Control.

* Triển khai bảo vệ AWS WAF với các quy tắc bảo mật (SQL injection, XSS, kiểm soát bot).

* Thiết lập ACM Certificate và kích hoạt HTTPS để phân phối nội dung bảo mật.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Phân tích Yêu cầu Hệ thống & Thiết kế Kiến trúc: <br>&emsp; + Phân tích yêu cầu hệ thống và xem xét sơ đồ kiến trúc hoàn chỉnh. <br>&emsp; + Xác định tất cả các thành phần: Route 53, S3, CloudFront, WAF, ACM, VPC, EC2, RDS, API Gateway. <br>&emsp; + Tạo tài liệu Thiết kế Cấp cao (HLD) với tổng quan kiến trúc. <br>&emsp; + Tài liệu hóa luồng dữ liệu: Users → Route 53 → CloudFront → WAF → S3 (Frontend). <br>&emsp; +  Lập kế hoạch quy hoạch địa chỉ IP và quy ước đặt tên tài nguyên.                                                                                                  | 10/26/2025 | 10/26/2025      | Architecture diagram |
| 3   | - Thiết lập Route 53: <br>&emsp; + Tạo Route 53 hosted zone để quản lý tên miền. <br>&emsp; + Tạo A Record trỏ đến CloudFront distribution.  <br>&emsp; +  Tạo các bản ghi CNAME cho subdomain nếu cần. <br>&emsp; + Cấu hình cài đặt DNS và xác minh quyền sở hữu tên miền. <br>&emsp; + Tài liệu hóa cấu hình DNS và các loại bản ghi. <br> - Cấu hình S3 Frontend Bucket <br>&emsp; + Tạo S3 bucket cho các tài sản tĩnh frontend (FE Bucket) với tên phù hợp. <br>&emsp; + Kích hoạt static website hosting trên S3 bucket. <br>&emsp; + Cấu hình chính sách truy cập công khai cho CloudFront (chặn truy cập công khai, cho phép CloudFront qua OAC). <br>&emsp; + Tải lên các file frontend thử nghiệm (HTML, CSS, JS, hình ảnh) lên S3 bucket. <br>&emsp; + Kiểm thử endpoint website tĩnh và xác minh khả năng truy cập file.                                             | 10/27/2025 | 10/27/2025      | Route 53 documentation <br> S3 documentation |
| 4   | - Thiết lập CloudFront Distribution: <br>&emsp; + Tạo CloudFront distribution với S3 bucket làm origin (nguồn). <br>&emsp; + Cấu hình Origin Access Control (OAC) để truy cập S3 an toàn (thay thế OAI).  <br>&emsp; + Thiết lập các chính sách cache (CachingOptimized, CachingDisabled, v.v.). <br>&emsp; + Cấu hình đối tượng gốc mặc định (default root object - index.html). <br>&emsp; + Ánh xạ tên miền Route 53 tới CloudFront distribution. <br>&emsp; + Kiểm thử CloudFront distribution và xác minh việc phân phối nội dung. | 10/28/2025 | 10/28/2025      | CloudFront documentation |
| 5   | - Tích hợp AWS WAF: <br>&emsp; + Tạo AWS WAF WebACL để bảo vệ CloudFront. <br>&emsp; + Thêm các quy tắc được quản lý: AWS Managed Rules bảo vệ chống SQL injection. <br>&emsp; + Thêm các quy tắc được quản lý: AWS Managed Rules bảo vệ chống XSS (Cross-Site Scripting). <br>&emsp; + Cấu hình quy tắc kiểm soát bot để chặn các bot phổ biến và công cụ cào dữ liệu. <br>&emsp; + Liên kết WAF WebACL với CloudFront distribution. <br>&emsp; +  Kiểm thử các quy tắc WAF bằng cách thử các mẫu tấn công phổ biến và xác minh việc chặn.                          | 10/29/2025 | 10/29/2025      | AWS WAF documentation |
| 6   | - Tích hợp ACM & HTTPS: <br>&emsp; +  Yêu cầu ACM Certificate tại region us-east-1 (bắt buộc cho CloudFront). <br>&emsp; + Xác thực chứng chỉ sử dụng phương pháp xác thực DNS (thêm bản ghi CNAME vào Route 53). <br>&emsp; + Chờ xác thực và cấp phát chứng chỉ. <br>&emsp; + Gắn chứng chỉ ACM vào CloudFront distribution. <br>&emsp; +  Cấu hình CloudFront để chỉ sử dụng HTTPS (chuyển hướng HTTP sang HTTPS). <br>&emsp; +  Kiểm thử kết nối HTTPS và xác minh chứng chỉ SSL/TLS hoạt động chính xác.                                                                                   | 10/30/2025 | 10/30/2025      | ACM documentation |


### Kết quả đạt được tuần 8:

* Hoàn thành phân tích hệ thống và thiết kế kiến trúc:

  * Đã phân tích yêu cầu hệ thống và xem xét sơ đồ kiến trúc tổng thể.

  * Đã tạo tài liệu Thiết kế Cấp cao (HLD) với tổng quan kiến trúc và mối quan hệ giữa các thành phần.

  * Tài liệu hóa luồng dữ liệu (data flow) từ người dùng qua các dịch vụ edge đến lưu trữ frontend.

  * Thiết lập quy ước đặt tên tài nguyên và tài liệu kế hoạch.

* Thiết lập quản lý DNS Route 53:

  * Đã tạo Route 53 hosted zone để quản lý tên miền.

  * Cấu hình các bản ghi A và CNAME để định tuyến tên miền.

  * Xây dựng nền tảng DNS để kết nối tên miền với CloudFront distribution.

* Cấu hình S3 cho hosting frontend tĩnh:

  * Đã tạo S3 bucket cho các tài sản tĩnh (static assets) của frontend với quy ước đặt tên phù hợp.

  * Kích hoạt tính năng static website hosting trên S3 bucket.

  * Cấu hình chính sách truy cập công khai: chặn truy cập công khai trực tiếp, cho phép CloudFront truy cập thông qua Origin Access Control.

  * Đã tải lên các tệp frontend thử nghiệm và xác minh chức năng hosting web tĩnh.

* Triển khai CloudFront distribution:

  * Đã tạo CloudFront distribution với S3 bucket làm origin (nguồn).

  * Cấu hình Origin Access Control (OAC) để truy cập S3 an toàn (giải pháp thay thế hiện đại cho OAI).

  * Thiết lập các chính sách cache (cache policies) để tối ưu hóa phân phối nội dung.

  * Ánh xạ tên miền Route 53 tới CloudFront distribution.

  * Đã xác minh việc phân phối nội dung qua CDN CloudFront trên toàn cầu.

* Triển khai bảo vệ AWS WAF:

  * Đã tạo AWS WAF WebACL với các quy tắc bảo mật toàn diện.

  * Thêm AWS Managed Rules để bảo vệ chống SQL injection.

  * Thêm AWS Managed Rules để bảo vệ chống XSS (Cross-Site Scripting).

  * Cấu hình quy tắc kiểm soát bot để chặn các bot độc hại và công cụ cào dữ liệu (scrapers).

  * Liên kết WAF WebACL với CloudFront distribution.

  * Đã kiểm thử các quy tắc WAF và xác minh khả năng bảo vệ chống lại các mẫu tấn công phổ biến.

* Kích hoạt HTTPS với ACM Certificate:

  * Đã yêu cầu và xác thực ACM Certificate tại region us-east-1 (bắt buộc cho CloudFront).

  * Sử dụng phương pháp xác thực DNS với các bản ghi CNAME trong Route 53.

  * Gắn chứng chỉ ACM vào CloudFront distribution.

  * Cấu hình CloudFront để bắt buộc dùng HTTPS (chuyển hướng HTTP sang HTTPS).

  * Đã xác minh chứng chỉ SSL/TLS hoạt động chính xác và các kết nối bảo mật được thiết lập.


