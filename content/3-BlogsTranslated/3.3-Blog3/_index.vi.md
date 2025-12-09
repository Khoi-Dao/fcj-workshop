---
title: "Blog 3"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---



# MOSIP trên AWS: Chuyển đổi nhận dạng số cho chính phủ hiện đại

heo sáng kiến Identification for Development (ID4D) của Ngân hàng Thế giới, có khoảng 850 triệu người trên toàn cầu chưa có giấy tờ tùy thân hợp pháp. Điều này khiến họ không thể tiếp cận các dịch vụ thiết yếu như chăm sóc y tế, giáo dục và phúc lợi xã hội.
Để giải quyết vấn đề này, Atos và Amazon Web Services (AWS) đã hợp tác phát triển một hệ thống nhận dạng số dựa trên nền tảng đám mây sử dụng Modular Open-Source Identity Platform (MOSIP) – giúp các hệ thống nhận dạng trở nên dễ tiếp cận, an toàn và có khả năng mở rộng hơn bao giờ hết.

---

## Nhu cầu về hệ thống nhận dạng số

Đại dịch COVID-19 đã làm thay đổi căn bản cách chúng ta tiếp cận các hệ thống nhận dạng, thúc đẩy nhu cầu về các giải pháp không tiếp xúc trong nhiều lĩnh vực.
 Theo dữ liệu ngành, việc tích hợp công nghệ sinh trắc học (biometric) đóng vai trò quan trọng trong quá trình chuyển đổi số này. Thị trường công nghệ sinh trắc học toàn cầu được dự báo sẽ tăng trưởng từ 34,27 tỷ USD năm 2022 lên 150,58 tỷ USD vào năm 2030.
Các cơ quan chính phủ và người dân đều nhận thức được tầm quan trọng của việc ngăn chặn gian lận và tăng cường bảo mật dữ liệu, đồng thời đảm bảo các phương thức nhận dạng đáng tin cậy, thúc đẩy niềm tin và khả năng tiếp cận trong thế giới ngày càng số hóa hiện nay.

---

## Giải pháp MOSIP trên AWS

MOSIP – được thành lập năm 2018 tại Viện Công nghệ Thông tin Quốc tế Bangalore (IIIT-B) – là một sáng kiến phi lợi nhuận giúp chính phủ các nước triển khai hệ thống nhận dạng số.
 Nền tảng này có kiến trúc mạnh mẽ, linh hoạt và có thể mở rộng, hỗ trợ chính phủ xây dựng cơ sở dữ liệu dân cư và các hệ thống cung cấp dịch vụ công, tạo nền tảng cho nền kinh tế số.
 MOSIP đã được triển khai thành công tại nhiều quốc gia châu Phi, chứng minh khả năng hỗ trợ các dịch vụ thiết yếu thông qua hệ thống nhận dạng số an toàn và dễ tiếp cận.


---
## Thách thức của hệ thống nhận dạng số tại chỗ (on-premises)


Khi các chính phủ trên thế giới tìm cách triển khai hệ thống nhận dạng an toàn và đáng tin cậy, họ thường gặp nhiều thách thức khi duy trì mô hình triển khai tại chỗ:
  * Chi phí hạ tầng cao, gây rào cản lớn khi bắt đầu.


  * Khả năng mở rộng hạn chế, khó đáp ứng nhu cầu dân số tăng nhanh.


  * Lỗ hổng bảo mật, quy trình bảo trì phức tạp và khó tích hợp với hệ thống hiện có.


  * Cần đội ngũ IT chuyên biệt, chi phí bảo trì cao, và quy trình sao lưu thủ công dễ sai sót.


  * Triển khai hệ thống mới gặp sự phản đối từ người dùng truyền thống, cần nhiều đào tạo bổ sung.


  * Lo ngại về quyền riêng tư, tuân thủ pháp lý, và rào cản kỹ năng số cản trở việc áp dụng.


  * Việc đảm bảo khả năng bao trùm cho các khu vực xa xôi và nhóm yếu thế vẫn là một thách thức.


---

##  Lợi ích của hệ thống nhận dạng số trên nền tảng đám mây

Việc triển khai MOSIP trên AWS mang lại nhiều lợi ích cho chính phủ, bao gồm:
  * Tối ưu vận hành và tài chính:
 Mô hình trả theo mức sử dụng (pay-as-you-go) loại bỏ chi phí đầu tư ban đầu, và khả năng tự động mở rộng (auto scaling) giúp đáp ứng nhu cầu dân số tăng trưởng.
 Các dịch vụ AWS Managed Services giảm chi phí hạ tầng và loại bỏ bảo trì định kỳ.


  * Bảo mật và khả năng truy cập cao:
 Hệ thống hoạt động ổn định nhờ tích hợp khôi phục sau thảm họa (disaster recovery).
 AWS cung cấp mã hóa, quản lý danh tính, và tính năng bảo mật toàn diện, giúp tuân thủ quy định và giảm chi phí quản lý rủi ro.


  * Tích hợp và tính liên tục trong kinh doanh:
 MOSIP dễ dàng kết nối với hệ thống hiện có và các dịch vụ tương lai của chính phủ.
 Sao lưu tự động đảm bảo tính liên tục mà không cần đầu tư thêm.
 Mô hình đám mây giúp triển khai nhanh hơn, giảm phức tạp vận hành, đồng thời mang lại bảo mật và hiệu năng cấp doanh nghiệp.


---

## Giải pháp triển khai lai (Hybrid Deployment)


VĐể đáp ứng nhu cầu khác nhau của chính phủ, MOSIP trên AWS hỗ trợ bốn mô hình triển khai:
1. Hybrid deployment: Tách biệt môi trường sản xuất và thử nghiệm.


2. Split security model: Giữ khóa bảo mật và sao lưu tại chỗ.


3. Sensitive data protection: Lưu dữ liệu công dân tại chỗ, chỉ dùng đám mây cho các dịch vụ khác.


4. AWS Outposts: Cung cấp đầy đủ năng lực AWS ngay trong trung tâm dữ liệu của chính phủ.


---

## Tối ưu chi phí

Theo phân tích bằng AWS Pricing Calculator, việc triển khai MOSIP trên AWS giúp tiết kiệm đáng kể so với mô hình truyền thống:

| Quy mô | Nhỏ                                                                                                                                                                                                  | Trung bình | Lớn   |
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ---------------------------------------------------------------------------------- |
| Ước tính chi phí/tháng   | USD $4,168                                                                                                    | USD $9,896.10  | USD $14,395.85       |                                                                                    |
| Số lượng đăng ký mỗi ngày  | Hàng trăm  | Hàng chục nghìn | Hàng trăm nghìn      | 
| Chi phí mỗi lượt đăng ký   | USD $1.39  | USD $0.033  | USD $0.0048       | 
| Mức khả dụng   | Một AZ   | Hai AZ | Cấp doanh nghiệp      | 
| Mục đích sử dụng   | Thí điểm / quy mô nhỏ        | Hạ tầng sản xuất	 | Sản xuất toàn diện      | 

Hệ thống hạ tầng nền tảng (~4.000 USD/tháng) bao gồm Amazon VPC, AWS Transit Gateway, VPN, AWS Network Firewall, AWS CodeBuild, Amazon ECR, tạo nền tảng cho mọi quy mô triển khai MOSIP

---

## So sánh với mô hình tại chỗ (on-premises):

  * Đầu tư ban đầu: 2–3 triệu USD


  * Duy trì trung tâm dữ liệu: 500.000–750.000 USD/năm


  * Nhân sự IT chuyên biệt: 250.000–400.000 USD/năm


  * Nâng cấp phần cứng mỗi 3–5 năm: 1–1,5 triệu USD

Mô hình đám mây giúp giảm 60–70% chi phí đầu tư ban đầu, giảm 40–50% chi phí vận hành, và rút ngắn thời gian triển khai từ 12–18 tháng xuống còn 3–6 tháng.


---

## Tác động đối với chính phủ

Giải pháp MOSIP trên AWS mang lại:
  * Cải thiện hiệu quả cung cấp dịch vụ công


  * Tăng khả năng bao trùm số cho mọi công dân


  * Củng cố an ninh dữ liệu


  * Tối ưu sử dụng nguồn lực


  * Khả năng mở rộng linh hoạt cho dân số lớn

Cách tiếp cận dựa trên đám mây giúp biến nhận dạng số từ một gánh nặng tài nguyên thành công cụ thúc đẩy dịch vụ công, cho phép chính phủ tập trung vào phục vụ người dân thay vì quản lý hạ tầng.


---

## Kết luận

Đối với các chính phủ đang tìm cách hiện đại hóa hệ thống nhận dạng công dân, MOSIP trên AWS là giải pháp toàn diện kết hợp hiệu quả chi phí, khả năng mở rộng và bảo mật cao.
 Việc triển khai thành công tại nhiều quốc gia đã chứng minh tính tin cậy và hiệu quả của nền tảng này, khiến nó trở thành lựa chọn lý tưởng cho những chính phủ cam kết chuyển đổi số và nâng cao dịch vụ công.


