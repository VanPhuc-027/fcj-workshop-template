---
title: "Event 2 Offline"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---

# Harvest Report: AWS First Cloud Journey 06/06

## Event Objectives

* **Advanced Security:** Master methods combining **AWS WAF** and **Machine Learning (NIDS)** to elevate network defense capabilities.
* **Packaging Technology:** Thoroughly understand **Containerization (Docker)** and why it surpasses traditional Virtualization models.
* **Career Path:** Gain practical industry insights and career progression paths from **IT Helpdesk** to **Cloud/DevOps** roles.
* **Real-time Cloud Applications:** Explore how to build **Multiplayer Games** on Cloud infrastructure using **Godot** and **AWS WebSockets**.
* **Soft Skills:** Enhance **Teamwork** skills through golden principles and digital collaboration tools.
* **AI & Knowledge Graphs:** Discover the **GraphRAG** architecture combining **Amazon Bedrock** and **Amazon Neptune** to solve complex reasoning problems.

---

## Speaker List

| Speaker | Role / Organization | Topic |
| :--- | :--- | :--- |
| **Le Hoang Gia Dai** | Senior Student at HUTECH University / AWS G3 | Machine Learning-based NIDS on AWS |
| **Bao Huynh** | Junior Cloud Native Developer, Endava Vietnam | Docker – A Containerization Technology |
| **Tran Trung Vinh** | System Administrator, Central Retail Group | From IT Helpdesk to Senior Sysadmin |
| **Nguyen Quoc Bao** | Cloud Engineer / Game Dev | Multiplayer in the Cloud (Godot & AWS) |
| **Truong Huy Phuoc** | Technical Lead / Mentor | The Art of Effective Teamwork |
| **Viet Phat** | AI Student, Swinburne University | Build GraphRAG Applications with Bedrock & Neptune |

---

## Highlighted Content

### 1. Machine Learning-based NIDS on AWS
> **Speaker:** Le Hoang Gia Dai

* **The Problem with Traditional WAF:** Rule-based systems only mitigate known risks and are easily bypassed by **Zero-day** attacks or abnormal behaviors that do not fit predefined patterns.
* **ML & NIDS Solution:** Building a system that learns real network behaviors to proactively and automatically detect intrusions (**NIDS - Network Intrusion Detection System**).
* **Training Process:** 
  * Utilized the benchmark dataset `CSE-CIC-IDS2018`.
  * Emphasized the importance of **data cleaning** and **data balancing** to enable the **LightGBM** model to accurately identify cyberattacks.
* **Cloud Architecture:** Integrated a service pipeline consisting of **AWS WAF**, **EC2**, **ALB**, **Amazon Kinesis**, and **AWS Security Hub** to collect logs, monitor, and dispatch alerts in real time.

---

### 2. Docker – A Containerization Technology
> **Speaker:** Bao Huynh

* **Virtual Machine (VM) vs Container:**
  * *Virtual Machine:* Heavyweight because it requires running an entire separate guest operating system (**Guest OS**), consuming significant infrastructure resources.
  * *Container:* Optimized and lightweight by sharing the host OS kernel (**Shared Kernel**) and packaging only the necessary dependencies.
* **Core Components:**
  * Standardized methods for writing `Dockerfile`.
  * Mechanics of creating and managing **Docker Images** along with the lifecycle of **Docker Containers**.
  * Leveraging **Layer Caching** to significantly speed up image build times.
* **Practical Applications:** Deploying **CI/CD** pipelines, designing **Microservices** architectures, and applying Cloud-native standards under the philosophy of *"Build once, run anywhere"*.

---

### 3. From IT Helpdesk to Senior Sysadmin
> **Speaker:** Tran Trung Vinh

* **Career Progression:**
  $$\text{IT Helpdesk (End-user support)} \longrightarrow \text{Linux \& Networking} \longrightarrow \text{System Administrator} \longrightarrow \text{AWS Cloud \& DevOps (IaC)}$$
* **Practical Operational Mindset:**
  * Always configure **Monitoring & Alerting** systems before incidents occur.
  * Automate repetitive tasks.
  * **Biggest Misconduct:** The golden rule *"Never test directly on Production environments"*.
* **Interview Insights & Advice:**
  * Focus on proving competence through real-world projects, troubleshooting skills, and architectural understanding rather than pursuing purely theoretical certifications.
  * Deeply master **1–2 core skills** before expanding to avoid learning too broadly without focus.

---

### 4. Multiplayer in the Cloud (Godot & AWS)
> **Speaker:** Nguyen Quoc Bao

* **Comparison of Game Networking Architectures:**

  | Protocol | Advantages | Disadvantages | Best Use Cases |
  | :--- | :--- | :--- | :--- |
  | **UDP / ENet** | Ultra-low latency | Difficult state management | FPS, Racing, Fighting games |
  | **HTTP Polling** | Simple, easy to implement | High latency, resource-intensive | Turn-based strategy, Quiz games |
  | **WebSocket** | Real-time bi-directional | Requires persistent connections | Game Lobbies, Card games, Turn-based |

* **AWS Infrastructure Design:**
  * **API Gateway (WebSocket):** Manages real-time connections and connection lifecycle states (`$connect`, `$disconnect`, `$default`).
  * **AWS Lambda:** Handles matchmaking logic and short-lived event processing.
  * **Amazon DynamoDB:** Stores session state information and player IDs.
* **Client-Side Implementation (Godot):** Uses `WebSocketPeer` to establish connections and exchange data via **JSON payloads** for game state synchronization.
* **Challenges & Solutions:**
  * Handling stale connections.
  * Optimizing costs by avoiding full `Scan` operations on DynamoDB.
  * For real-time games with complex stateful logic, consider upgrading to dedicated solutions like **AWS GameLift**.

---

### 5. The Art of Effective Teamwork
> **Speaker:** Truong Huy Phuoc

* **4 Golden Rules:**
  1. **Clear & Shared Goals:** Establish unambiguous objectives and ensure full team alignment.
  2. **Right Person, Right Job:** Assign roles based on individual strengths.
  3. **Open Communication:** Encourage transparent communication and **Active Listening**.
  4. **Personal Accountability:** Foster strong personal ownership for assigned tasks.
* **Digital Ecosystem Support Tools:**
  * **Task Management:** Trello, ClickUp.
  * **Communication & Collaboration:** Slack, Discord, Google Workspace.

---

### 6. Build GraphRAG Applications with Bedrock & Neptune
> **Speaker:** Viet Phat

* **Limitations of Traditional RAG:** Standard RAG relying on Vector Databases struggles with **multi-hop reasoning** queries or retrieving cross-entity relationships.
* **The Power of GraphRAG:** Representing knowledge as a **Graph (Nodes & Edges)** explicitly defines context and relational constraints, enabling LLMs to retrieve precise answers.
* **AWS Architectural Patterns:**
  * **Fully Managed Approach:** Natively integrating **Amazon Bedrock Knowledge Bases** with **Amazon Neptune Analytics**.
  * **Custom Approach:** Building custom Data Pipelines using **LlamaIndex**, storing knowledge graphs in **Amazon Neptune**, and executing queries via **Cypher**.

---

## Key Takeaways

* Provided a comprehensive overview ranging from **Infrastructure, Security, Containerization, Real-time Systems** to cutting-edge technologies like **AI GraphRAG**.
* Acquired high-value practical insights from experienced speakers to directly apply toward optimizing projects and mapping out a career path in **Cloud / DevOps**.

## Practical Application
* Applied Docker concepts to standardize `Dockerfile` configurations for personal and group projects while utilizing **Layer Caching** to reduce build times.
* Containerized application source code and pushed container images to **Amazon ECR**, preparing for automated deployments on **Amazon ECS / EC2**.
* Transformed infrastructure mindsets: Always configuring **CloudWatch Logs** and setting up monitoring/alerting mechanisms right from the initialization phase instead of reacting after production issues arise.

---

## Event Experience
* Despite a minor personal scheduling mix-up—meaning this session technically could not count toward official attendance credit—the event organizers kindly accommodated and allowed me to attend. This was an invaluable opportunity to catch a top-tier sharing session.
* The event took place in an open, highly enthusiastic environment. Speakers skipped abstract theory and dove directly into **real-world production challenges**, past mistakes, and remediation techniques.
* Gained great networking opportunities to interact directly with veteran speakers and peers who share common goals in Cloud and DevOps.

## Event Photos

![Slide Docker Intro - Docker, not a full intro, fun and interactive](/images/4-EventParticipated/4.2-Event2/event2-slide1-docker-intro-anime.jpg?featherlight=false&width=90pc)

![Slide WAF + ML for Cyber Attack Detection - NIDS on AWS](/images/4-EventParticipated/4.2-Event2/event2-slide2-waf-ml-cyber-attack.png?featherlight=false&width=90pc)

![Slide From IT Helpdesk to Senior Sysadmin - Tran Trung Vinh](/images/4-EventParticipated/4.2-Event2/event2-slide3-it-helpdesk-to-sysadmin.png?featherlight=false&width=90pc)

![Slide Docker - A Containerization Technology - ITea LAB](/images/4-EventParticipated/4.2-Event2/event2-slide4-docker-containerization-iteab.png?featherlight=false&width=90pc)