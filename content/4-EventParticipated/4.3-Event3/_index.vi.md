---
title: "Event 3 online 27/06/2026"
date: 2026-06-27
weight: 1
chapter: false
pre: " <b> 4.3. </b> "
---

# FCAJ Community Day (Data Driven, AI Risen)

## Mục Tiêu Của Sự Kiện

* **AgenticOps & Autonomic Cloud:** Khám phá mô hình tự động hóa vận hành đám mây và cấu trúc của Deep Response Engine.
* **Voice AI Enterprise:** Nắm bắt xu hướng Voice Agents và cách triển khai hệ thống AI đàm thoại quy mô lớn trong doanh nghiệp.
* **DevOps Automation:** Trải nghiệm AWS DevOps Agent cùng chiến lược tối ưu hóa bằng hệ thống Multi-Agent.
* **AI trong HR & Planning:** Đánh giá tác động của AI trong mảng Quản trị nhân sự (Workforce Planning) thông qua giải pháp Amazon Quick.
* **Bảo mật & Zero Trust:** Thực hành cấu hình bảo mật kết nối riêng tư cho giao thức MCP (Model Context Protocol).

---

## Danh Sách Diễn Giả

| Diễn giả | Vai trò / Tổ chức | Chủ đề chia sẻ |
| :--- | :--- | :--- |
| **Steve Tran** | CTO/Founder, CloudThinker | Áp dụng AgenticOps cho hệ thống Cloud |
| **Trung Vu** | CEO, Revve AI | Triển khai Voice Agent quy mô lớn |
| **Nghi Danh** | AI Engineer, Renova Cloud | Triển khai Voice Agent & Bảo mật MCP |
| **Kiet Tran** | AI Engineer, AWS Student Builder Group | Triển khai Voice Agent quy mô lớn |
| **Nguyen Nguyen** | Cloud Engineer, Cloud Kinetics | AWS DevOps Agent: Trợ lý vận hành đắc lực |
| **Bao Phan** | Cloud Engineer, Cloud Kinetics | AWS DevOps Agent: Trợ lý vận hành đắc lực |
| **Truong Tran** | AI Solution Sales, Noventiq | Quy hoạch nhân sự bằng AI (Workforce Planning) |
| **Anh Dang** | Solution Sales, Noventiq | Quy hoạch nhân sự bằng AI (Workforce Planning) |
| **Toan Nguyen** | AWS Security Builder | Thiết lập MCP bảo mật riêng tư cho Amazon Quick |

---

## Nội Dung Nổi Bật
### 1. Áp dụng AgenticOps cho hệ thống Cloud
> **Diễn giả:** Steve Tran

* **Thực trạng vận hành:** Quá trình chuyển đổi lên Platform Engineering khiến số lượng công cụ tăng gấp 4 lần và đội ngũ kỹ sư tăng gấp 3 lần, nhưng thời gian phục hồi sự cố (**MTTR**) vẫn không cải thiện. Kỹ sư bị kẹt trong "bức tường phức tạp" của hạ tầng.
* **Hướng giải quyết với AgenticOps:** Đưa vào vận hành một hệ thống gồm nhiều AI Agent chuyên biệt (dành cho K8s, Cloud, Database) được quản lý bởi một Super Agent, giúp tự động xử lý các công việc phức tạp.
* **Triết lý vận hành:** Hệ thống giám sát (*Observability*) truyền thống chỉ để nhìn, còn **AgenticOps** là để chủ động hành động và tự học hỏi (*"CloudThinker acts on it, learn it"*).
* **Hiệu quả thực tế:** Xử lý tự động **70%** lỗi, kéo giảm MTTR tới **87%**, tiết kiệm **25%** tài nguyên đám mây và loại bỏ **40%** các tác vụ lặp đi lặp lại.

---

### 2. Triển khai Voice Agent quy mô lớn
> **Diễn giả:** Trung Vu, Nghi Danh, Kiet Tran

* **Khác biệt cốt lõi:** Voice Agent yêu cầu khả năng giao tiếp luồng đôi (*bidirectional audio*) theo thời gian thực thay vì mô hình hỏi-đáp văn bản thông thường.
* **Lựa chọn kiến trúc:** Lựa chọn *Cascaded Pipeline (STT $\rightarrow$ LLM $\rightarrow$ TTS)* thay vì *Speech-to-speech* nguyên khối. Điều này giúp kiểm soát nội dung (*guardrails*), gọi công cụ (*tool calling*) chính xác và xử lý ngữ điệu tiếng Việt tốt hơn.
* **Tối ưu độ trễ:** Áp dụng phương pháp streaming, sinh văn bản đón đầu (*preemptive generation*) và khởi tạo kết nối sớm (*warm-up*) để cuộc hội thoại diễn ra tự nhiên.
* **Kỹ thuật luân phiên (Turn-taking):** Huấn luyện mô hình tiếng Việt với độ chính xác **81%** để AI nhận biết khi người dùng nói xong. Kết hợp State Machine và RAG để triệt tiêu hiện tượng "ảo giác" (*hallucination*).
* **Go-live:** Trải qua kiểm thử có sự tham gia của con người (*Human-in-the-loop*), theo dõi sát sao và tích hợp trực tiếp vào hệ thống tổng đài doanh nghiệp (**SIP/WebRTC**).

---

### 3. AWS DevOps Agent: Trợ lý vận hành đắc lực
> **Diễn giả:** Nguyen Nguyen, Bao Phan

* **Nỗi đau vận hành:** Việc khắc phục sự cố thủ công tiêu tốn nhiều thời gian (chỉ số MTTD/MTTR cao) do dữ liệu phân mảnh và thiếu ngữ cảnh hệ thống, khiến đội Ops rơi vào thế bị động.
* **Giải pháp DevOps Agent:** AI Agent hoạt động độc lập giúp điều tra và phòng ngừa sự cố trên đa môi trường (AWS, Azure, On-premise).
* **Vòng đời sự cố 4 bước:**
  $$\text{Triage (Tiếp nhận)} \longrightarrow \text{Investigate (Phân tích)} \longrightarrow \text{Mitigate (Khắc phục)} \longrightarrow \text{Prevent (Phòng ngừa)}$$
* **Tính năng nổi bật:** Tự học sơ đồ kiến trúc (*topology*) của ứng dụng, không cần cài đặt hạ tầng cồng kềnh, tương tác trực tiếp qua Slack hoặc ServiceNow.
* **Kết quả:** Giúp các doanh nghiệp thực tế (như WGU, ZENCHEF) giảm hơn **75%** thời gian xử lý sự cố.

---

### 4. Quy hoạch nhân sự bằng AI (Workforce Planning)
> **Diễn giả:** Truong Tran, Anh Dang

* **Thách thức:** Quy trình sàng lọc CV thủ công chậm chạp, dễ bị cảm tính chi phối, ảnh hưởng đến chất lượng nhân sự và tiến độ kinh doanh.
* **Sức mạnh của Amazon Quick Suite:** Tự động hóa quy trình HR dựa trên AI. Hệ thống tích hợp bảo mật nghiêm ngặt (*Guardrails*) và kết nối đa nguồn dữ liệu (SaaS, Database) thông qua engine SPICE.
* **Quy trình 5 bước tuyển dụng tự động:**
  1. **Connect:** Tự động thu thập dữ liệu từ các nền tảng tuyển dụng.
  2. **Automate:** AI chấm điểm CV và đề xuất mức lương tối ưu.
  3. **Visualize:** Hiển thị phễu tuyển dụng dạng Dashboard trực quan.
  4. **Decide:** Tự động chuyển trạng thái và tạo thư mời nhận việc (*Offer letter*).
  5. **Track:** Hệ thống tự động sắp xếp lịch phỏng vấn với ứng viên.

---

### 5. Thiết lập MCP bảo mật riêng tư cho Amazon Quick
> **Diễn giả:** Toan Nguyen, Nghi Danh

* **Khái niệm MCP:** *Model Context Protocol* là giao thức chuẩn hóa giúp các Client (như Amazon Quick) kết nối an toàn với MCP Servers để truy xuất dữ liệu.
* **Lỗ hổng bảo mật:** Kết nối mặc định của Amazon Quick thường qua Internet (*Public Endpoint*), vi phạm nguyên tắc an toàn Zero Trust trong doanh nghiệp.
* **Kiến trúc VPC Connection:** Ép buộc toàn bộ luồng kết nối đi qua card mạng nội bộ (**Private-IP ENI**) kết hợp với hệ thống phân giải tên miền riêng (**Route 53 Resolver**).
* **Đường đi dữ liệu an toàn:**
  $$\text{Amazon Quick} \xrightarrow{\text{VPC Connection}} \text{Internal ALB (HTTPS)} \xrightarrow{\text{Private Network}} \text{MCP Server (HTTP)}$$
  Luồng dữ liệu hoàn toàn khép kín nội bộ, không tiếp xúc với Internet công cộng.

---

## Những gì học được

* **FCAJ Community Day** đã mang lại một bức tranh toàn cảnh về sự kết hợp mạnh mẽ giữa **Data Driven** và **AI Risen**.
* Tiếp thu được nhiều giải pháp kiến trúc hạ tầng tân tiến, tư duy vận hành hiện đại và kiến thức bảo mật chuyên sâu để trực tiếp áp dụng vào công việc quản trị hệ thống và phát triển các giải pháp trên nền tảng Cloud.

## Ứng Dụng Vào Công Việc
* Áp dụng nguyên tắc **Zero Trust** cho các luồng truyền nhận dữ liệu giữa các dịch vụ.

* Khi triển khai kết nối API hoặc giao thức dữ liệu (như MCP), ưu tiên sử dụng cấu trúc **VPC Endpoints**, **Internal ALB** và **Route 53 Private Hosted Zones** để giữ trọn vẹn luồng dữ liệu trong mạng nội bộ.

* Tận dụng các công cụ phân tích dữ liệu như **Amazon Quick** kết hợp AI để xây dựng các phễu theo dõi công việc tự động, giúp giảm thiểu tác vụ thủ công và đưa ra quyết định dựa trên dữ liệu (*Data-driven*).



## Trải Nghiệm Trong Event

* **Cập nhật xu hướng AI thực chiến:** 
  Sự kiện không chỉ dừng lại ở lý thuyết LLM đơn thuần mà mang đến cái nhìn rất sâu về **AI Agents**, **Voice AI** và **AgenticOps** – những công nghệ đang thực sự giải quyết các bài toán hạ tầng và vận hành của doanh nghiệp.
* **Chất lượng chuyên môn cao:** 
  Các diễn giả đều là những chuyên gia, kỹ sư dày dạn kinh nghiệm thực chiến. Các phần trình bày về kiến trúc hệ thống, đường đi dữ liệu (*data flow*) và giải pháp khắc phục lỗi (*troubleshooting*) cực kỳ chi tiết, mang lại giá trị tham khảo chuyên môn cao.

## Một số hình ảnh tham gia sự kiện