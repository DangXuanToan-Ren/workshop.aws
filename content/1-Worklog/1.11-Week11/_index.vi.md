---
title: "Worklog Tuần 11"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---



### Mục tiêu tuần 11:

* Thiết lập luồng CI/CD (Tích hợp và Triển khai liên tục) để tự động hóa quy trình phát hành ứng dụng Frontend.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Nghiên cứu về luồng CI/CD cho ứng dụng Frontend. <br> - Đánh giá và lựa chọn công cụ để cấu hình pipeline (sử dụng AWS CodePipeline, CodeBuild hoặc GitHub Actions).                       | 30/06/2026   | 30/06/2026      |
| 3   | - Thực hành: <br>&emsp; + Thiết lập mã nguồn trên Git repository. <br>&emsp; + Cấu hình bước đầu tiên của pipeline để hệ thống tự động build mã nguồn mỗi khi có thay đổi code mới.         | 01/07/2026   | 01/07/2026      |
| 4   | - Thực hành: <br>&emsp; + Tích hợp bước tự động đồng bộ (sync) các file tĩnh (static files) của ứng dụng Frontend sau khi build thành công lên kho lưu trữ Amazon S3.                        | 02/07/2026   | 02/07/2026      |
| 5   | - Thực hành: <br>&emsp; + Viết cấu hình kịch bản tự động thực hiện thao tác Invalidation (xóa bộ nhớ đệm) trên Amazon CloudFront vào quy trình pipeline.                                    | 03/07/2026   | 03/07/2026      |
| 6   | - Kiểm thử toàn diện toàn bộ luồng CI/CD. <br> - Đẩy (push) một thay đổi code nhỏ và theo dõi quá trình hệ thống tự động build, deploy và xóa cache để giúp giao diện được cập nhật ngay lập tức mà không cần thao tác thủ công. | 04/07/2026   | 04/07/2026      |


### Kết quả đạt được tuần 11:

* Nắm được khái niệm và luồng hoạt động cơ bản của CI/CD (Continuous Integration / Continuous Deployment).
* Đã lựa chọn và cấu hình thành công pipeline bằng GitHub Actions (hoặc AWS CodePipeline tùy theo lựa chọn).
* Thiết lập thành công Git repository và kết nối với hệ thống CI/CD.
* Tự động hóa quá trình build mã nguồn Frontend mỗi khi có commit mới được push lên repo.
* Tích hợp thành công bước deploy file tĩnh lên Amazon S3 sau khi build hoàn tất.
* Thực hiện được thao tác CloudFront Invalidation tự động để xóa cache, giúp người dùng thấy được thay đổi mới nhất ngay lập tức.
* Kiểm thử toàn bộ luồng CI/CD thành công: chỉ cần push code, hệ thống sẽ tự động hoàn tất build → deploy → invalidate cache.
* Hiểu rõ lợi ích của CI/CD: giảm thiểu lỗi thủ công, tăng tốc độ phát hành, đảm bảo tính nhất quán giữa các môi trường.



