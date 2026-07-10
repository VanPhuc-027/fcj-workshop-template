---
title: "Worklog Tuần 3"
date: 2024-05-04
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Mục tiêu tuần 3:

* Hoàn thành module03, nắm rõ lý thuyết về Amazon Elastic Compute Cloud(EC2), Lightsail, EFS/FSX, AWS Migration Service(MGN), thực hành các bài lab về tạo s3, cloudfront, load data,...

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Học lý thuyết module03 tìm hiểu về các thành phần trong EC2**: <br> +Instance type. <br> +AMI / Backup / Key Pair. <br> Elastic block store và Instance store.                                    | 04/05/2026   | 04/05/2026      | <https://www.youtube.com/watch?v=e7XeKdOVq40> |
| 3   | - **Học tiếp lý thuyết module03 tìm hiểu về:** <br> User data, Meta data, EC2 auto scaling. <br> EFS/FSx - Lightsail - MGN.                                            | 05/05/2026   | 05/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   |- **Thực hành lab13:** tạo ra một kế hoạch sao lưu (backup plan) cho các tài nguyên đang hoạt động trên AWS như EBS Volumes, RDS Databases, DynamoDB Tables, hay EFS File Systems.<br> &emsp; + Cách sử dụng AWS CLI | 06/05/2026   | 06/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - **Thực hành lab24:** <br> - Tạo S3 bucket và tạo EC2 Instance sử dụng AMI Storage Gateway mà AWS đã cung cấp sẵn. <br> - Sử dụng AWS Storage Gateway: tạo Storage Gateway, tạo File Share và kết nối ổ đĩa    | 07/05/2026   | 07/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - **Thực hành lab57:**thực hiện tạo S3 bucket và sau đó upload dữ liệu lên để chuẩn bị cho việc host static website.        | 07/05/2026   | 07/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Ôn lại lý thuyết module03, xem lại các video hướng dẫn thực hành lab.      | 08/05/2026   | 08/05/2026      | <https://www.youtube.com/watch?v=AQlsd0nWdZk&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |


### Kết quả đạt được tuần 3:

* Nắm vững kiến thức nền tảng cốt lõi của Module 03, hiểu rõ cơ chế hoạt động, kiến trúc và cách phân loại các thành phần trong hệ sinh thái tính toán và lưu trữ của AWS.

* Phân biệt thành công các loại Instance type (General Purpose, Compute Optimized, Memory Optimized,...) để tối ưu hóa chi phí và hiệu năng cho từng bài toán thực tế.

* Hiểu sâu về cách quản lý vòng đời EC2 thông qua AMI (Amazon Machine Image), cơ chế bảo mật bằng Key Pair, và phân biệt rõ ràng kịch bản sử dụng giữa bộ lưu trữ bền vững EBS (Elastic Block Store) với bộ lưu trữ tạm thời tốc độ cao Instance store.

* Làm chủ các khái niệm nâng cao của EC2 bao gồm: Tự động hóa cấu hình lúc khởi tạo bằng User data, truy xuất thông tin hệ thống qua Meta data, và cơ chế tự động co giãn hệ sinh thái nhờ EC2 Auto Scaling dựa trên nhu cầu tải.

* Có cái nhìn tổng quan và phân biệt được các giải pháp lưu trữ/dịch vụ khác như hệ thống tệp chia sẻ EFS/FSx, dịch vụ máy chủ ảo đơn giản Amazon Lightsail, và quy trình dịch chuyển hệ thống lên đám mây với AWS Migration Service (MGN).



