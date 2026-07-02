---
title: "Event 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---

# BÁO CÁO THU HOẠCH SỰ KIỆN: AWS & GENERATIVE AI (EVENT 2)


## I. Tổng Quan Sự Kiện

Sự kiện tập trung vào việc áp dụng thực tế các dịch vụ AWS và AI tạo sinh (GenAI) vào các bài toán kỹ thuật chuyên sâu. Nội dung trải dài từ kỹ thuật tối ưu hóa AI (Context Engineering, xử lý tính ngẫu nhiên của LLM), kiến trúc hệ thống (CloudFront, Multi-Agent), cho đến trải nghiệm xây dựng sản phẩm thực tế từ các cuộc thi Hackathon.


## II. Danh Sách Diễn Giả & Chủ Đề

- Anh Thịnh: "Context Is Everything - Build Second Brain".
- Anh Hải Anh: "Friendly AI Assistant w/ Amazon Quick".
- Team VIB: "36 hrs with LotusHacks - Building UTMorpho".
- Anh Thịnh: "From Edge To Origin: CloudFront as Your Foundation".
- Anh Đức Đào: "Non-Determinism of Deterministic LLM Settings".
- Chị Vy Lam: "Enterprise-Grade Multi-Agent System".


## III. Ghi Nhận Nội Dung Nổi Bật

### 1. Anh Thịnh — Context Is Everything (Tối ưu hóa ngữ cảnh AI)
- Nhiều kết quả AI gây thất vọng bắt nguồn từ việc cung cấp ngữ cảnh kém, chứ không phải do mô hình AI tệ.
- Một ngữ cảnh tốt cần xác định rõ 4 yếu tố: Mục tiêu, Tình huống, Ràng buộc, và Bằng chứng/Dữ liệu liên quan.
- Sai lầm cần tránh: Không nên nhồi nhét toàn bộ dữ liệu hỗn độn trên mạng vào prompt ("Internet Puller"), không yêu cầu AI làm những việc quá hiển nhiên, và không đưa ra các yêu cầu mơ hồ thiếu ràng buộc.
- Tương lai của việc sử dụng AI đang dịch chuyển từ việc chỉ viết prompt đơn thuần sang việc xây dựng các "Hệ thống Ngữ cảnh" (Prompt → Context → Memory) hay còn gọi là "Bộ não thứ hai" (Second Brain).


### 2. Anh Hải Anh — Friendly AI Assistant (Trợ lý AI với Amazon Q)
- Các mô hình AI tác tử (Agentic AI) được xây dựng dựa trên việc tích hợp dữ liệu công ty và không gian trí thức an toàn.
- Việc sử dụng trợ lý AI giúp đơn giản hóa và tăng tốc quá trình chuyển đổi từ việc phân tích thông tin (insight) sang hành động thực tế (action).
- Trợ lý AI có thể ứng dụng làm "PM Assistant" để tự động hóa các tác vụ lặp lại như: tự động tạo biên bản cuộc họp (MoM), gửi email cho các bên liên quan và lên lịch họp.


### 3. Team VIB — Xây dựng sản phẩm UTMorpho trong 36 giờ
- Quá trình xây dựng sản phẩm dưới áp lực lớn đòi hỏi đội ngũ phải trải qua các bước: Thiết lập, xây dựng phần cốt lõi, đối mặt với khó khăn ở giai đoạn giữa, và tinh chỉnh trước khi thuyết trình.
- Các thách thức thực tế khi làm hackathon bao gồm: AI tạo ra quá nhiều dữ liệu dư thừa (Overgeneration), sự mệt mỏi/kiệt sức khi gần đến giờ thuyết trình, và giới hạn số lượng token (Token Limits).
- Bài học rút ra: Sự thật vọng với các giải pháp hiện tại chính là nguồn tạo ra ý tưởng thực tế, và trong môi trường cường độ cao, sự đồng bộ của nhóm (Team Sync) là yếu tố quan trọng nhất.


### 4. Anh Thịnh — Tối ưu hóa hạ tầng với Amazon CloudFront
- Khách hàng thường gặp khó khăn về rủi ro khi làm động lượng truy cập hoặc bị tấn công mạng, dẫn đến các chi phí đơn CDN không ngoài dự kiến.
- CloudFront cung cấp giải pháp bảo mật với giá cước cố định, kết hợp WAF, chống DDoS, và giới hạn lưu lượng để loại bỏ rủi ro tài chính.
- Về mặt hiệu năng, CloudFront giúp giảm thời gian tải về cho máy chủ gốc (Origin) bằng cách hỗ trợ tải nhiều luồng (HTTP/3 multiplexing) và nén dữ liệu HTTP, giúp giảm tối 81% thời gian phản hồi và 82% dung lượng.
- Sử dụng CloudFront kết hợp với Origin Access Control (OAC) hoặc Custom Headers giúp che giấu máy chủ gốc (Origin cloaking), tăng cường độ bảo mật cho hệ thống.


### 5. Anh Đức Đào — Tính phi định tính (Non-Determinism) của LLM
- Dù đã cài đặt thông số nhiệt độ về 0 (Temperature = 0) với lý thuyết sẽ mang lại kết quả đầu ra luôn giống nhau, các mô hình LLM trên thực tế vẫn có sự sai số.
- Nguyên nhân kỹ thuật sâu xa đến từ kiến trúc phần cứng (toán học dấu phẩy động trên GPU) và cơ chế gom nhóm xử lý (Inference batching) từ các nhà cung cấp API để tối ưu chi phí.
- Các kỹ thuật khắc phục bao gồm: Chạy prompt nhiều lần và lấy kết quả phổ biến nhất (Majority voting), ép buộc mô hình trả về dữ liệu có cấu trúc (JSON mode, Regex), hoặc tự lưu trữ mô hình.


### 6. Chị Vy Lam — Hệ thống Đa Tác tử cấp Doanh nghiệp (Enterprise-Grade Multi-Agent)
- Các mô hình đơn giản đã từng dùng truyền thống thường thất bại khi áp dụng cho các Startup vì thời hồi đáp chậm, dữ liệu phân tán và biến động không nhanh.
- Kiến trúc Đa Tác tử (Multi-Agent) giải quyết vấn đề này bằng cách thiết lập một "Hội đồng tin tưởng ảo", nơi các AI chuyên biệt (Phân tích tài chính, Phân tích thị trường, Đánh giá rủi ro...) làm việc song song và kiểm chéo lẫn nhau.
- Hệ thống cấp doanh nghiệp đòi hỏi các tiêu chuẩn khắt khe về bảo mật (Mạng VPC, Quản lý IAM, mã hóa dữ liệu) và các cơ chế kiểm soát rào chắn (Guardrails) ở các đầu vào, quá trình xử lý và đầu ra.
- Việc ứng dụng kiến trúc này mang lại mức ROI không lờ: giảm 95% thời gian xử lý, tiết kiệm 95% chi phí cho quyết định và tăng tỷ lệ duyệt hồ sơ.


## IV. Giá Trị Động Lắm

- Về Tối ưu hóa Hệ thống: Hiểu được tầm quan trọng của việc che giấu Origin và sử dụng mạng biên (Edge computing) để vừa giảm chi phí tài nguyên, vừa chống lại các cuộc tấn công DDoS.
- Về AI & Kỹ nghệ Prompt: Nhận thức rõ ràng rằng không gì là chắc chắn tuyệt đối 100% trong AI (kể cả khi Temperature = 0). Cung cấp ngữ cảnh (Context) sạch, gọn và có cấu trúc quan trọng hơn việc nhồi nhét dữ liệu vào prompt.
- Về Tư duy Phát triển: Trong tương lai, sự khác biệt trong sự nghiệp không nằm ở việc "Người đối với AI", mà là "Người biết dùng AI" đối với "Người không biết dùng". Xây dựng AI cho doanh nghiệp không chỉ là làm cho nó chạy được, mà phải bảo mật, tin cậy và có thể mở rộng (Scale).


## V. Kế Hoạch Ứng Dụng Vào Thực Tế

- Thay đổi cách làm việc với LLM: Áp dụng tư duy thiết kế hệ thống lường trước số (Design for variance) bằng cách chuẩn hóa các định dạng đầu ra (như JSON) thay vì phụ thuộc hoàn toàn vào văn bản tự do của mô hình.
- Ứng dụng thiết lập "Guardrails" (Rào chắn) và nguyên tắc phân quyền tối thiểu (Least privilege) khi triển khai các dự án Backend/Cloud để đảm bảo an toàn ngay từ khâu thiết kế kiến trúc.
- Tối ưu hóa các dự án thực tập và lab AWS: Thiết lập CloudFront làm lớp đệm bắt buộc trước các máy chủ EC2 hoặc S3, cấu hình nén tự động để giảm băng thông và cải thiện tốc độ phản hồi cho frontend.
- Xây dựng hệ thống "Second Brain" cho cá nhân để lưu trữ, truy xuất các tài liệu kỹ thuật, mã nguồn và kiến thức AWS một cách có hệ thống.


## VI. Cảm Nhận Cá Nhân

Sự kiện thứ hai mang tính kỹ thuật chuyên sâu và mở rộng tâm nhìn kiến trúc để những cái khác biệt. Mình đặc biệt ấn tượng với đề "Non-Determinism" vì nó giải thích rõ ràng vì sao có những lỗi không được định mà mình từng gặp phải khi test API của LLM. Bài trình bày về Multi-Agent và CloudFront cũng cung cấp các best-practices thực chiến rất giá trị, giúp mình định hình rõ ràng hơn về cách các doanh nghiệp lớn vận hành bảo mật hạ tầng và tích hợp AI an toàn, tối ưu chi phí cho các dự án phần mềm.


## VII. Một Số Hình Ảnh Từ Sự Kiện

<img src="/images/Event2/z7969075645797_c6232463de54c809944d4c1fc251693b.jpg" alt="AWS & Generative AI Event Photo 1" class="blog-image" />
<img src="/images/Event2/z7969075646427_3bd1c651ae7b793d115fa3c37c78272f.jpg" alt="AWS & Generative AI Event Photo 2" class="blog-image" />
