---
title: "Worklog Tuần 12"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.12. </b> "
---


### Mục tiêu tuần 12:
- Kiểm thử toàn bộ hệ thống, quản lý chi phí và hoàn thiện báo cáo thực tập tốt nghiệp.


### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Thực hiện rà soát và kiểm thử toàn diện (End-to-End Testing) toàn bộ kiến trúc hệ thống AWS đã triển khai từ các tuần trước.<br>- Đảm bảo luồng hoạt động từ Frontend đến Backend và Database diễn ra trơn tru. | 07/07/2026 | 07/07/2026 | |
| 3 | - Tìm hiểu công cụ quản lý chi phí tại AWS Cost Explorer và AWS Budgets.<br>- Phân tích chi phí hiện tại, thiết lập cảnh báo ngân sách để theo dõi và đưa ra giải pháp tối ưu hóa chi phí. | 08/07/2026 | 08/07/2026 | |
| 4 | - Thực hành: Tiến hành rà soát, dọn dẹp và gỡ bỏ các tài nguyên AWS (như EC2 instance, EBS volume, DynamoDB table, S3 bucket...) không còn được sử dụng.<br>- Đảm bảo về hiệu quả sử dụng các tài nguyên phát sinh chi phí ngoài ý muốn sau khi kết thúc thực tập. | 09/07/2026 | 09/07/2026 | |
| 5 | - Thu thập, tổng hợp số liệu và log từ quá trình thực hành thực tế trong suốt 12 tuần.<br>- Phân tích và đánh giá kết quả đạt được so với mục tiêu ban đầu đề ra. | 10/07/2026 | 10/07/2026 | |
| 6 | - Viết tổng kết, định dạng lại tài liệu và hoàn thiện toàn bộ báo cáo thực tập tốt nghiệp.<br>- Chuẩn bị file báo cáo bản trình chiếu để xin đánh giá, chữ ký xác nhận từ Cán bộ hướng dẫn thực tập (FCA) và Giảng viên hướng dẫn tại trường, sau đó nộp sản phẩm cuối cùng. | 11/07/2026 | 11/07/2026 | |


### Kết quả đạt được tuần 12:
- Hoàn thành thành công kiểm thử end-to-end (E2E) toàn bộ hệ thống ứng dụng đặt vé xem phim, bao gồm tất cả các dịch vụ AWS (VPC, EC2, S3, CloudFront, SQS, SNS, SES, RDS, ElastiCache, Cognito, API Gateway, CodePipeline, CodeBuild, CloudWatch...).
- Xác nhận và đảm bảo tất cả các luồng hoạt động của hệ thống hoạt động đúng: Đăng ký người dùng, đăng nhập, đặt vé, xác nhận đặt chỗ, gửi thông báo, hủy vé,...
- Nắm vững các công cụ quản lý chi phí AWS:
  - Sử dụng Cost Explorer để phân tích và theo dõi chi phí.
  - Thiết lập AWS Budgets để gửi cảnh báo khi chi phí gần đạt ngân sách.
  - Xác định và tối ưu hóa chi phí (ví dụ: dừng EC2 khi không dùng, sử dụng loại instance phù hợp, dọn dẹp tài nguyên không dùng).
- Thực hiện dọn dẹp tài nguyên thành công:
  - Dừng và terminate các EC2 không dùng.
  - Xóa các EBS volume, Elastic IP, CloudFormation Stack không dùng.
  - Dọn dẹp các S3 bucket, DynamoDB table, CloudFront distribution,...
- Thu thập và tổng hợp tất cả dữ liệu, báo cáo, worklog trong suốt 12 tuần thực tập.
- Phân tích và đánh giá kết quả đạt được:
  - Hoàn thành 100% các mục tiêu thực tập.
  - Thành công triển khai một ứng dụng web hoàn chỉnh, đầy đủ chức năng trên AWS.
  - Nắm vững các dịch vụ AWS cốt lõi và các quy tắc DevOps (CI/CD, IaC).
- Viết và hoàn thành báo cáo thực tập tốt nghiệp bằng cả tiếng Anh và tiếng Việt.
- Chuẩn bị file trình chiếu, tập luyện thuyết trình và nộp tất cả các sản phẩm cho FCA và giảng viên trường.
