---
title: "Worklog Tuần 6"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Nắm vững lý thuyết module06 và hoàn thành các bài lab đồng thời ôn lại lý thuyết các module cũ để nắm vững kiến thức

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| Thứ 6   | - **Thực hành lab48 của module05**tạo môi trường cho workshop bao gồm việc tạo EC2 instance và tạo S3 bucket.Cách cấu hình và sử dụng access key.  | 22/05/2026   | 22/05/2026      | <https://000048.awsstudygroup.com/> |
| Thứ 7  | - Học lý thuyết module06 về Database Concepts review, mô hình chia sẻ trách nhiệm trong dịch vụ cơ sở dữ liệu quản lý, Amaazon RDS và Aurora,  Redshift - Elasticache.     | 23/05/2026   | 23/05/2026      | <https://www.youtube.com/watch?v=OOD2RwWuLRw> <br> <https://www.youtube.com/watch?v=qbrobQZrokY> <br> <https://www.youtube.com/watch?v=UvdiRW34aNI> |
| Chủ nhật   | - **Thực hành lab05:** triển khai và quản lý cơ sở dữ liệu quan hệ trên AWS.Sử dụng Amazon RDS để thiết kế cho xử lý giao dịch trực tuyến (OLTP) và phù hợp nhất với các yêu cầu lưu trữ dữ liệu có cấu trúc và quan hệ. | 24/05/2026   | 24/05/2026      | <https://000005.awsstudygroup.com/> |
| Thứ 2   | - **Thực hành lab43:** Chuyển đổi lược đồ  của cơ sở dữ liệu, theo dõi DMS Migrations và xử lý sự cố với AWS DMS. | 25/05/2026   | 25/05/2026      | <https://000043.awsstudygroup.com/> |
| Thứ 3   | - Ôn lại bài lý thuyết module06, xem trước lab35 của modlue07.       | 26/05/2026   | 26/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ 4   | - Xem lại các video lý thuyết module02, module03.       | 27/05/2026   | 27/05/2026      | <https://www.youtube.com/watch?v=AQlsd0nWdZk&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| Thứ 5   | - Xem lại các video thực hành bài lab module06, module05.      | 28/05/2026   | 28/05/2026      | <https://www.youtube.com/watch?v=B5rOeWQWg1c&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=220> |

### Kết quả đạt được tuần 6:

* Hiểu về mô hình chia sẻ trách nhiệm (Shared Responsibility Model) áp dụng riêng cho các dịch vụ cơ sở dữ liệu được quản lý (Managed Databases), biết phân biệt phần việc hệ thống tự động xử lý (như vá lỗi, sao lưu hạ tầng) và phần việc người dùng cần tối ưu (như thiết kế schema, tối ưu câu lệnh truy vấn).

* Nắm vững nguyên lý hoạt động, kịch bản ứng dụng cụ thể và ưu/nhược điểm của các giải pháp lưu trữ dữ liệu cốt lõi trên AWS:
  * **Amazon RDS & Amazon Aurora:** Giải pháp cơ sở dữ liệu quan hệ tối ưu cho các tác vụ xử lý giao dịch trực tuyến (OLTP), hỗ trợ tính năng High Availability (Multi-AZ) và Read Replicas.
  * **Amazon Redshift:** Hệ thống kho dữ liệu (Data Warehouse) mạnh mẽ phục vụ cho việc phân tích dữ liệu quy mô lớn (OLAP).
  * **Amazon ElastiCache:** Giải pháp bộ nhớ đệm (In-memory caching) sử dụng Redis/Memcached giúp tăng tốc độ phản hồi và giảm tải tối đa cho database cốt lõi.

* Khởi tạo thành công môi trường hạ tầng tiêu chuẩn cho workshop bao gồm máy chủ ảo EC2 Instance và hệ thống lưu trữ Amazon S3.

* Thực hiện thành công việc chuyển đổi lược đồ (Schema Conversion), thiết lập và theo dõi sát sao tiến trình di trú dữ liệu (DMS Migrations).

* Ôn lại và nắm vững hơn các kiến thức module cũ.

