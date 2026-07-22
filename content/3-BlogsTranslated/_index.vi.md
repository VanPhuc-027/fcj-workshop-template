---
title: "Các bài blogs đã dịch"
date: 2026-06-30
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

Tại đây sẽ là phần liệt kê, giới thiệu các blogs mà các bạn đã dịch. Ví dụ:

###  [Blog 1 - Bảo Mật Thông Tin Mật Toàn Diện Với GitGuardian Và AWS Secrets Manager](3.1-Blog1/)
Blog này giới thiệu giải pháp kết hợp GitGuardian và AWS Secrets Manager để lấp đầy "khoảng trống hiển thị" trong việc quản lý thông tin mật (secrets). Bạn sẽ tìm hiểu vì sao chỉ lưu trữ credentials tập trung là chưa đủ nếu secret đã bị rò rỉ dưới dạng hardcode trong lịch sử Git, cách công cụ `ggscout` mã hóa secret thành fingerprint tại chỗ (giao thức HMSL) để đối chiếu ẩn danh với mã nguồn mà không để lộ dữ liệu gốc ra ngoài hạ tầng AWS. Bài viết cũng hướng dẫn lộ trình triển khai 5 bước (Monitor, Detect, Investigate, Remediate, Guard) để giám sát, cảnh báo thời gian thực và tự động rotate các secret bị lộ.

###  [Blog 2 - AI-Powered Test Automation: Bước Đột Phá Cho Kiểm Thử Tự Động Từ Amazon Bedrock Và Rapise](3.2-Blog2/)
Blog này giới thiệu cách tích hợp Amazon Bedrock vào công cụ kiểm thử tự động Rapise để giải quyết bài toán script test bị gãy khi giao diện (UI) thay đổi. Bạn sẽ tìm hiểu vì sao các framework automation test truyền thống dựa vào ID/XPath cố định dễ gây ra false positives và tốn chi phí bảo trì, cách AI giúp hệ thống "đọc hiểu" giao diện theo ngữ cảnh, tự động chữa lành (self-healing) script khi UI thay đổi, và tự sinh kịch bản test từ mô tả ngôn ngữ tự nhiên. Bài viết cũng hướng dẫn lộ trình triển khai 5 bước tương tự để kết nối hạ tầng, huấn luyện baseline UI và kích hoạt tính năng tự động sửa lỗi trong CI/CD.

###  [Blog 3 - AWS Transform: Khi AI Tự Động Dọn "Nợ Kỹ Thuật" Cho Cả Ngàn Repository](3.3-Blog3/)
Blog này giới thiệu tính năng Continuous Modernization trong AWS Transform, một công cụ dùng AI để tự động quét và sửa nợ kỹ thuật trên toàn bộ codebase của tổ chức, tìm hiểu vì sao các công cụ rời rạc (phát hiện dependency lỗi thời, lỗ hổng bảo mật, chất lượng code) khiến doanh nghiệp khó sửa lỗi ở quy mô lớn, cách hệ thống vận hành qua 2 chế độ Continuous Mode (tự động tạo Pull Request khi phát hiện repo lệch chuẩn) và Campaign Mode (dành cho các chiến dịch migrate/nâng cấp quy mô lớn). Bài viết cũng đề cập đến việc tích hợp sâu với AWS Security Agent và hỗ trợ giao thức MCP để cắm trực tiếp vào các coding agent hiện có.