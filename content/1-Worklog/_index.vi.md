---
title: "Nhật ký công việc"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

Trong trang này sẽ giới thiệu worklog của tôi, hoàn thành chương trình trong vòng 10 tuần (với Tuần 11 và 12 để dành cho hoàn thiện dự án). Nội dung các tuần như sau:

**Tuần 1:** [Làm quen với AWS và các dịch vụ cơ bản trong AWS](1.1-week1/)
- Làm quen với các thành viên, quy định đơn vị
- Tìm hiểu AWS, tạo Free Tier account, Console và CLI
- Thực hành EC2 cơ bản

**Tuần 2:** [Học cách làm việc với AWS Management Console và CLI](1.2-week2/)
- Nghiên cứu đồng bộ giữa Console và CLI
- Thực hành quản lý Key Pairs, Security Groups
- Tổng hợp kỹ năng kết nối và quản lý tài nguyên

**Tuần 3:** [Phân tích các nhóm dịch vụ Compute, Storage, Networking và Database](1.3-week3/)
- Nghiên cứu sâu về các nhóm dịch vụ
- Thực hành kiểm tra và vận hành qua Console và CLI
- Viết log tổng hợp và đánh giá

**Tuần 4:** [Nâng cao kỹ năng quản lý EC2 và EBS](1.4-week4/)
- Củng cố kiến thức EC2, AMI, EBS
- Thực hành khởi tạo, gắn Elastic IP
- Quản lý vòng đời EC2 qua CLI
- Cấu hình sao lưu với EBS Snapshot

**Tuần 5:** [Xây dựng hệ thống Serverless với Lambda và Event-Driven](1.5-week5/)
- Lập trình Lambda, tích hợp thông báo Slack
- Thực hành CloudWatch, Grafana
- Quản lý tài nguyên theo Tag, phân quyền IAM

**Tuần 6:** [Xây dựng CI/CD với AWS Developer Tools](1.6-week6/)
- Nghiên cứu CodeCommit, CodeBuild, CodeDeploy, CodePipeline
- Chuẩn bị mã nguồn, thiết lập kết nối Git
- Thực hành thiết lập luồng CI/CD tự động

**Tuần 7:** [Container hóa và triển khai với ECR và ECS](1.7-week7/)
- Học Docker, ECR, ECS
- Viết Dockerfile, build và push image lên ECR
- Cấu hình ECS Cluster, chạy container trên Fargate

**Tuần 8:** [Xây dựng API RESTful với API Gateway và DynamoDB](1.8-week8/)
- Tạo REST API với API Gateway
- Lưu dữ liệu vào DynamoDB
- Thực hành CRUD qua API

**Tuần 9:** [Tích hợp xác thực và tối ưu phân phối Frontend](1.9-week9/)
- Nghiên cứu Amazon Cognito
- Tích hợp xác thực với API Gateway
- Lưu Frontend lên S3, cấu hình CloudFront

**Tuần 10:** [Tự động hóa với Infrastructure as Code (AWS SAM)](1.10-week10/)
- Học Infrastructure as Code (IaC)
- Viết AWS SAM template
- Deploy toàn bộ serverless stack

**Tuần 11:** [Thiết lập luồng CI/CD cho Frontend](1.11-week11/)
- Nghiên cứu luồng CI/CD cho ứng dụng Frontend
- Thiết lập Git repository và build tự động
- Deploy file tĩnh lên S3 và cấu hình CloudFront invalidation
- Kiểm thử toàn bộ luồng CI/CD

**Tuần 12:** [Kiểm thử hệ thống, quản lý chi phí và báo cáo cuối](1.12-week12/)
- Thực hiện kiểm thử end-to-end (E2E) toàn bộ hệ thống AWS
- Học công cụ quản lý chi phí AWS: Cost Explorer và Budgets
- Dọn dẹp các tài nguyên AWS không còn sử dụng
- Hoàn thành và nộp báo cáo thực tập cuối cùng cùng bài thuyết trình