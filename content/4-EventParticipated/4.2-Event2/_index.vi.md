---
title: "Event 2 Offline"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---


# Bài Thu Hoạch: AWS First Cloud Journey 06/06

## Mục Tiêu Của Sự Kiện

* **Bảo mật chuyên sâu:** Nắm bắt phương pháp kết hợp **AWS WAF** và **Machine Learning (NIDS)** để nâng cao năng lực phòng thủ mạng.
* **Công nghệ đóng gói:** Hiểu rõ về **Containerization (Docker)** và lý do nó vượt trội hơn mô hình Virtualization truyền thống.
* **Định hướng nghề nghiệp:** Lắng nghe kinh nghiệm thực chiến và lộ trình thăng tiến từ vị trí **IT Helpdesk** lên **Cloud/DevOps**.
* **Ứng dụng Real-time Cloud:** Khám phá cách xây dựng hệ thống **Multiplayer Game** trên nền tảng Cloud sử dụng **Godot** và **AWS WebSockets**.
* **Kỹ năng mềm:** Nâng cao kỹ năng **làm việc nhóm (Teamwork)** thông qua các nguyên tắc vàng và áp dụng công cụ số.
* **AI & Knowledge Graph:** Tiếp cận kiến trúc **GraphRAG** kết hợp **Amazon Bedrock** và **Amazon Neptune** để giải quyết bài toán suy luận phức tạp.

---

## Danh Sách Diễn Giả

| Diễn giả | Vai trò / Tổ chức | Chủ đề chia sẻ |
| :--- | :--- | :--- |
| **Lê Hoàng Gia Đại** | Sinh viên năm cuối ĐH HUTECH / AWS G3 | Machine Learning-based NIDS on AWS |
| **Bảo Huỳnh** | Junior Cloud Native Developer, Endava Vietnam | Docker – A Containerization Technology |
| **Trần Trung Vinh** | System Administrator, Central Retail Group | From IT Helpdesk to Senior Sysadmin |
| **Nguyễn Quốc Bảo** | Cloud Engineer / Game Dev | Multiplayer in the Cloud (Godot & AWS) |
| **Trương Huy Phước** | Technical Lead / Mentor | The Art of Effective Teamwork |
| **Viết Phát** | Sinh viên AI, Swinburne University | Build GraphRAG applications with Bedrock & Neptune |

---

## Nội Dung Nổi Bật

### 1. Machine Learning-based NIDS on AWS
> **Diễn giả:** Lê Hoàng Gia Đại

* **Vấn đề của WAF truyền thống:** Các hệ thống dựa trên quy tắc (*Rule-based*) chỉ ngăn chặn được rủi ro đã biết, dễ bị vượt qua bởi các tấn công **Zero-day** hoặc các hành vi bất thường không theo mẫu cố định.
* **Giải pháp ML & NIDS:** Xây dựng hệ thống học hành vi mạng thực tế để chủ động và tự động phát hiện xâm nhập (**NIDS - Network Intrusion Detection System**).
* **Quá trình huấn luyện:** 
  * Sử dụng bộ dữ liệu chuẩn `CSE-CIC-IDS2018`.
  * Nhấn mạnh tầm quan trọng của việc **làm sạch** và **cân bằng dữ liệu** (Data balancing) giúp mô hình **LightGBM** nhận diện chính xác các cuộc tấn công.
* **Kiến trúc Cloud:** Tích hợp chuỗi dịch vụ **AWS WAF**, **EC2**, **ALB**, **Amazon Kinesis** và **AWS Security Hub** để thu thập log, giám sát và phát cảnh báo theo thời gian thực.

---

### 2. Docker – A Containerization Technology
> **Diễn giả:** Bảo Huỳnh

* **Virtual Machine (VM) vs Container:**
  * *Virtual Machine:* Cồng kềnh vì phải khởi chạy toàn bộ một hệ điều hành riêng (**Guest OS**), tiêu tốn nhiều tài nguyên hạ tầng.
  * *Container:* Tối ưu và siêu nhẹ do dùng chung nhân OS với máy host (**Shared Kernel**) và chỉ đóng gói những dependency thực sự cần thiết.
* **Thành phần cốt lõi:**
  * Phương pháp viết `Dockerfile` chuẩn hóa.
  * Cơ chế tạo và quản lý **Docker Images** cùng vòng đời của **Docker Containers**.
  * Tận dụng tối đa cơ chế **Layer Caching** để tăng tốc độ build image.
* **Ứng dụng thực tiễn:** Triển khai môi trường **CI/CD**, thiết kế hệ thống dạng **Microservices**, ứng dụng tiêu chuẩn Cloud-native với triết lý *"Build once, run anywhere"*.

---

### 3. From IT Helpdesk to Senior Sysadmin
> **Diễn giả:** Trần Trung Vinh

* **Hành trình phát triển:**
  $$\text{IT Helpdesk (End-user support)} \longrightarrow \text{Linux \& Networking} \longrightarrow \text{System Administrator} \longrightarrow \text{AWS Cloud \& DevOps (IaC)}$$
* **Tư duy vận hành thực chiến:**
  * Luôn thiết lập hệ thống giám sát (**Monitoring & Alerting**) trước khi sự cố xảy ra.
  * Tự động hóa các tác vụ lặp đi lặp lại.
  * **Tắc trách lớn nhất:** Nguyên tắc vàng *"Không bao giờ test trực tiếp trên môi trường Production"*.
* **Kinh nghiệm phỏng vấn & Lời khuyên:**
  * Tập trung chứng minh năng lực qua dự án thực tế, tư duy giải quyết sự cố (**Troubleshooting**) và hiểu biết về kiến trúc hơn là chạy theo bằng cấp/chứng chỉ thuần lý thuyết.
  * Đi sâu làm chủ **1–2 kỹ năng cốt lõi** trước khi mở rộng, tránh việc học quá dàn trải.

---

### 4. Multiplayer in the Cloud (Godot & AWS)
> **Diễn giả:** Nguyễn Quốc Bảo

* **So sánh các kiến trúc mạng trong Game:**

  | Giao thức | Ưu điểm | Nhược điểm | Trường hợp sử dụng phù hợp |
  | :--- | :--- | :--- | :--- |
  | **UDP / ENet** | Độ trễ cực thấp | Khó quản lý trạng thái | Game FPS, Racing, Fighting |
  | **HTTP Polling** | Đơn giản, dễ cài đặt | Độ trễ cao, tốn tài nguyên | Game Turn-based chậm, Quiz |
  | **WebSocket** | Giao tiếp 2 chiều Real-time | Cần duy trì kết nối | Game Lobby, Card Game, Turn-based |

* **Thiết kế hạ tầng trên AWS:**
  * **API Gateway (WebSocket):** Quản lý kết nối thời gian thực và trạng thái luồng (`$connect`, `$disconnect`, `$default`).
  * **AWS Lambda:** Xử lý logic ghép cặp phòng chơi (**Matchmaking**) và xử lý sự kiện ngắn hạn.
  * **Amazon DynamoDB:** Lưu trữ thông tin trạng thái session và ID người chơi.
* **Kỹ thuật phía Client (Godot):** Sử dụng `WebSocketPeer` để thiết lập kết nối và trao đổi dữ liệu dạng **JSON payload** nhằm đồng bộ trạng thái game.
* **Thách thức & Giải pháp:**
  * Xử lý kết nối rác (*Stale connections*).
  * Tối ưu chi phí bằng cách hạn chế dùng thao tác `Scan` trên DynamoDB.
  * Với game thời gian thực yêu cầu xử lý logic phức tạp (Stateful), cân nhắc nâng cấp lên giải pháp chuyên dụng **AWS GameLift**.

---

### 5. The Art of Effective Teamwork
> **Diễn giả:** Trương Huy Phước

* **4 Nguyên tắc Vàng (Golden Rules):**
  1. **Clear & Shared Goals:** Xác định mục tiêu rõ ràng và đảm bảo toàn bộ thành viên đều thấu hiểu.
  2. **Right Person, Right Job:** Bố trí đúng người vào đúng vị trí dựa trên thế mạnh cá nhân.
  3. **Open Communication:** Giao tiếp cởi mở, minh bạch và chủ động lắng nghe (**Active Listening**).
  4. **Personal Accountability:** Đề cao tính trách nhiệm cá nhân đối với công việc được phân công.
* **Hệ sinh thái công cụ số hỗ trợ:**
  * **Quản lý tác vụ:** Trello, ClickUp.
  * **Tương tác & Trao đổi:** Slack, Discord, Google Workspace.

---

### 6. Build GraphRAG Applications with Bedrock & Neptune
> **Diễn giả:** Viết Phát

* **Giới hạn của RAG thông thường:** Hệ thống RAG dựa trên Vector Database truyền thống gặp hạn chế khi xử lý các câu hỏi mang tính chất **suy luận đa bước (Multi-hop reasoning)** hoặc truy xuất mối quan hệ chéo giữa các đối tượng.
* **Sức mạnh của GraphRAG:** Biểu diễn tri thức dưới dạng **Đồ thị (Graph với Nodes & Edges)** giúp định nghĩa rõ ràng ngữ cảnh và mối quan hệ ràng buộc, cho phép LLM dễ dàng truy xuất thông tin chính xác.
* **Mô hình kiến trúc triển khai trên AWS:**
  * **Hướng Fully Managed:** Kết hợp trực tiếp **Amazon Bedrock Knowledge Bases** với **Amazon Neptune Analytics**.
  * **Hướng Custom:** Sử dụng **LlamaIndex** tự xây dựng Data Pipeline, dùng **Amazon Neptune** lưu trữ đồ thị tri thức và thực thi truy vấn qua ngôn ngữ **Cypher**.

---

## Những gì học được

* Sự kiện cung cấp cái nhìn toàn diện từ **Hạ tầng, Bảo mật, Đóng gói ứng dụng, Xây dựng hệ thống Real-time** cho đến các công nghệ tiên phong như **AI GraphRAG**.
* Tiếp thu được nhiều kinh nghiệm thực chiến có giá trị cao từ các diễn giả, áp dụng trực tiếp vào quá trình tối ưu hóa các dự án và định hướng con đường phát triển sự nghiệp trong mảng **Cloud / DevOps**.

## Ứng Dụng Vào Công Việc
* Áp dụng kiến thức Docker vào việc chuẩn hóa `Dockerfile` cho các project cá nhân và nhóm. Tận dụng tối đa cơ chế **Layer Caching** để giảm thời gian build image.
* Đóng gói mã nguồn và đẩy (push) các container image lên **Amazon ECR**, sẵn sàng cho việc tự động hóa triển khai trên **Amazon ECS / EC2**.
* Thay đổi tư duy triển khai hạ tầng: Luôn cấu hình **CloudWatch Logs** và thiết lập cơ chế giám sát/cảnh báo (*Monitoring & Alerting*) ngay từ giai đoạn khởi tạo thay vì đợi sự cố phát sinh.

---

## Trải Nghiệm Trong Event
* Dù ban đầu có chút nhầm lẫn về mặt lịch trình cá nhân, tuy sẽ không được tính vào 1 buổi event nhưng may mắn vẫn được các anh chị trong BTC tạo điều kiện hỗ trợ cho phép tham dự. Đây là cơ hội vô cùng quý giá giúp bản thân không bỏ lỡ một buổi chia sẻ chất lượng.
* Buổi event diễn ra trong không khí vô cùng cởi mở, nhiệt huyết. Các diễn giả không chỉ trình bày lý thuyết suông mà đi thẳng vào các **bài toán thực chiến**, những sai lầm từng gặp và cách khắc phục trên môi trường thực tế.
* Có cơ hội gặp gỡ, trao đổi trực tiếp với các diễn giả giàu kinh nghiệm cùng các bạn học viên có chung định hướng Cloud/DevOps.

## Một số hình ảnh tham gia sự kiện