---
title: "Worklog Tuần 10"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10:
Tự động hóa triển khai hạ tầng với phương pháp Infrastructure as Code (IaC).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tiếp cận phương pháp Infrastructure as Code (IaC). <br> - Tìm hiểu tổng quan về AWS CloudFormation và AWS SAM (Serverless Application Model).                                                  | 23/06/2026   | 23/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Nghiên cứu cấu trúc cơ bản của template AWS SAM. <br> - Tìm hiểu cú pháp viết mã cấu hình hạ tầng bằng định dạng YAML/JSON.                                                                | 24/06/2026   | 24/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | **Thực hành:** <br>&emsp; + Viết mã cấu hình (YAML) để định nghĩa tự động các tài nguyên: AWS Lambda và Amazon DynamoDB.                                                                   | 25/06/2026   | 25/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | **Thực hành:** <br>&emsp; + Bổ sung định nghĩa cấu hình cho Amazon API Gateway vào template. <br>&emsp; + Thiết lập liên kết (Events, Permissions) giữa API Gateway, Lambda và DynamoDB trong file mã. | 26/06/2026   | 26/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | **Thực hành:** <br>&emsp; + Sử dụng AWS SAM CLI để tự động khởi tạo, đóng gói (build/package) và triển khai (deploy) toàn bộ cụm tài nguyên Serverless. <br>&emsp; + So sánh ưu điểm và kiểm tra kết quả so với thao tác thủ công trên Console. | 27/06/2026   | 27/06/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 10:
* Hiểu được khái niệm và lợi ích của Infrastructure as Code (IaC) trong quản lý hạ tầng.
* Thành thạo cú pháp viết cấu trúc AWS SAM template ở định dạng YAML.
* Viết được file template đầy đủ định nghĩa Lambda, DynamoDB và API Gateway.
* Thiết lập liên kết Events và IAM Permissions giữa các dịch vụ trong template.
* Sử dụng được AWS SAM CLI để build, package và deploy toàn bộ serverless stack một cách tự động.
* Nhận thấy được lợi ích về tốc độ, tính nhất quán và dễ quản lý so với cách làm thủ công.


