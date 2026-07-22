---
title: "Worklog Tuần 12"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12 </b> "
---


### Mục tiêu tuần 12:

* Triển khai toàn bộ hạ tầng và mã nguồn lên AWS, hoàn thiện báo cáo và workshop.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| Thứ 6   | - Tiếp tục cập nhật file entrypoint.js trong dockefile, test lại logic lưu trữ trên s3 trước ở local sau đó build và deloy lên lại ecr.                     | 03/07/2026   | 03/07/2026      |
| Thứ 7  | - Tiếp tục giai đoạn tạo cluster và Task definitions, kiểm trra logic chạy task.   | 04/07/2026   | 04/07/2026      |
| Chủ nhật   | - Test chức năng kiểm thử thủ công, phát hiện ra lỗi logic khiến lambda không đọc đúng file test-scripts đã lưu trong s3, nghiên cứu và tiếp tục sửa lỗi trong file cấu hình docker. | 05/07/2026   | 05/07/2026      |  |
| Thứ 2   | - Tiếp tục kiểm thử và sửa lỗi thiếu biến môi trường, chạy thử thủ công trả về lỗi 401, lịch sử test bị treo ở trạng thái running.     | 06/07/2026   | 06/07/2026       |
| Thứ 3   | - Tiếp tục sửa lỗi logic về vấn đề AI không thể đọc log từ log stream để tóm tắt lỗi được, xóa pricing plan chuyển API key demo dự án về lại free tier để truy cập được log stream trong cloudwatch.           | 07/07/2026   | 07/07/2027  |
| Thứ 4   | - Kiểm tra và sửa lỗi gửi tóm tắt lỗi sau khi test về email nhưng không có nội dung tóm tắt, sửa nốt các lỗi lặt vặt còn sót và trạng thái frontend, edit dần vào workshop.      | 08/07/2026   | 08/07/2026      | <https://www.youtube.com/watch?v=AQlsd0nWdZk&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| Thứ 5   | - Kiểm thử lần cuối và hoàn thành các luồng workshop, tiếp tục hoàn chỉnh báo cáo.       | 09/07/2026   | 09/07/2026      | <https://www.youtube.com/watch?v=AQlsd0nWdZk&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Kết quả đạt được tuần 12:

*Cập nhật và tối ưu hóa thành công file entrypoint.js trong Dockerfile, thực hiện kiểm thử toàn bộ logic lưu trữ dữ liệu trên Amazon S3 tại môi trường local trước khi build lại image mới và push phiên bản chuẩn lên Amazon ECR.

* Khởi tạo và cấu hình hoàn chỉnh ECS Cluster cùng các thông số chi tiết trong Task Definitions.Khắc phục lỗi tích hợp s3.

* Sửa lỗi biến môi trường và xác thực.Xử lý luồng log AI & CloudWatch.

* Xử lý luồng log AI & CloudWatch, giải quyết sự cố AI không đọc được dữ liệu từ Log Stream trên Amazon CloudWatch để tổng hợp báo cáo lỗi.

* Tối ưu hóa hệ thống thông báo và Frontend, sửa lỗi định dạng nội dung email thông báo, đảm bảo các bản tóm tắt lỗi từ AI được gửi đầy đủ, trực quan về cho người dùng


