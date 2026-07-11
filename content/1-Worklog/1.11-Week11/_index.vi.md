---
title: "Worklog Tuần 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Mục tiêu tuần 11:

* Hoàn thiện sơ đồ kiến trúc, bắt đầu phân chia công việc bắt tay vào dự án và cấu hình được cơ bản các dịch vụ.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Chỉnh sửa sơ đồ kiến trúc, chuyển qua hướng sự kiện, nhóm các dịch vụ vào các khung cho dễ kiểm soát và vẽ luồng đi.          | 29/06/2026   | 29/06/2026      |
| 3   | - Tiếp tục chỉnh sửa, thêm public subnet và private subnet để tăng tính bảo mật.Chỉnh sửa các nhầm lẫn về icon dịch vụ. Nhờ thành viên gửi vào nhóm và nhận phản hồi và đánh giá ổn cho sơ đồ kiến trúc, có thể bắt đầu gia đoạn thực hiện.     | 30/06/2026   | 30/06/2026      |  |
| 4   | - Đọc và đánh giá, góp ý bổ sung cho kế hoạch và phân chia công việc của thành viên trong nhóm.Cùn thống nhất ngôn ngữ và các công nghệ sử dụng.  | 01/07/2026   | 01/07/2026      |  |
| 5   | -        | 02/07/2026   | 15/08/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Họp nhóm và thảo luận về tiến độ công việc.Cài đặt và cấu hình AWS CLI.     | 03/07/2026   | 03/07/2026     |  |
| 7   | - Cấu hình Docker theo phân công công việc, chỉnh sửa và test thử trước ở local về việc chạy kịch bản keiemr thử và lưu trữ lên S3 bucket.              | 04/07/2026   | 04/07/2026      |  |
| Chủ nhật  | - Deloy docker images lên ECR, kiểm tra các tính ổn định và cấu hình lại cho đúng với Task definitions   | 04/07/2026   | 04/07/2026      |  |

### Kết quả đạt được tuần 11:

* Hoàn thiện và chuẩn hóa thành công sơ đồ kiến trúc hệ thống, chuyển đổi mô hình thành công sang kiến trúc hướng sự kiện (Event-driven Architecture). Thực hiện đóng gói và phân nhóm các dịch vụ vào các phân vùng logic giúp luồng dữ liệu (Data flow) trở nên mạch lạc, dễ kiểm soát.

* Tăng cường tối đa tính bảo mật cho hệ thống bằng cách tái cấu trúc phân vùng mạng, phân định rõ ràng các vùng mạng công cộng (Public Subnet) và vùng mạng riêng tư (Private Subnet). Sửa đổi toàn bộ các sai sót về mặt nhận diện icon dịch vụ đám mây.

* Bản thiết kế kiến trúc cuối cùng đã xuất sắc thông qua vòng phản biện, nhận được đánh giá rất tốt từ cộng đồng và toàn đội, chính thức đóng tài liệu thiết kế để chuyển sang giai đoạn triển khai (Implementation).



