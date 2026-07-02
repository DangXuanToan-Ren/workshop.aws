---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---


### Mục tiêu tuần 9:
Tích hợp xác thực người dùng và tối ưu hóa phân phối ứng dụng Frontend.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Nghiên cứu dịch vụ Amazon Cognito <br> - Tìm hiểu cơ chế xác thực người dùng (User Pool) và luồng Đăng nhập/Đăng ký.                                                                      | 16/06/2026   | 16/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | **Thực hành:** <br>&emsp; + Tích hợp Amazon Cognito với Amazon API Gateway. <br>&emsp; + Cấu hình cấp quyền truy cập an toàn cho các API đã tạo từ Tuần 8.                                     | 17/06/2026   | 17/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu giải pháp lưu trữ giao diện web tĩnh (Frontend) trên Amazon S3. <br> - Nghiên cứu kiến trúc mạng phân phối nội dung Amazon CloudFront (CDN).                                      | 18/06/2026   | 18/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | **Thực hành:** <br>&emsp; + Tải mã nguồn giao diện web tĩnh (HTML/CSS/JS hoặc ReactJS) lên Amazon S3. <br>&emsp; + Thiết lập tính năng Static Website Hosting cho S3 bucket.                 | 19/06/2026   | 19/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | **Thực hành:** <br>&emsp; + Thiết lập và cấu hình Amazon CloudFront phân phối nội dung từ nguồn S3. <br>&emsp; + Kiểm tra và tối ưu hóa tốc độ tải trang (Caching) qua CDN.                  | 20/06/2026   | 20/06/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 9:
* Nắm được kiến trúc và cách hoạt động của Amazon Cognito User Pool cho xác thực người dùng.
* Đã tích hợp thành công Cognito với API Gateway để bảo vệ các endpoint REST API.
* Thiết lập và chạy được trang web tĩnh trên Amazon S3 bằng tính năng Static Website Hosting.
* Cấu hình thành công CloudFront làm CDN phân phối nội dung từ S3, cải thiện tốc độ tải trang nhờ caching.
* Hiểu được cách kết hợp Cognito + API Gateway + S3 + CloudFront để tạo một hệ thống web full-stack an toàn và hiệu quả.


