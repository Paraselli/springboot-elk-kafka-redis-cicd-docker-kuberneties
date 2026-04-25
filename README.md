# 🚀 Spring Boot ELK Kafka Redis CI/CD Docker Kubernetes

<div align="center">

![Java](https://img.shields.io/badge/Java-17-orange?style=for-the-badge\&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-green?style=for-the-badge\&logo=springboot)
![Kafka](https://img.shields.io/badge/Apache_Kafka-Event_Driven-black?style=for-the-badge\&logo=apachekafka)
![Redis](https://img.shields.io/badge/Redis-Cache-red?style=for-the-badge\&logo=redis)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue?style=for-the-badge\&logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestrated-326CE5?style=for-the-badge\&logo=kubernetes)
![Jenkins](https://img.shields.io/badge/Jenkins-CI/CD-D24939?style=for-the-badge\&logo=jenkins)
![ELK](https://img.shields.io/badge/ELK-Logging-005571?style=for-the-badge\&logo=elasticstack)

### ⚡ Production-grade Spring Boot microservice with Kafka, Redis, ELK, Docker, Kubernetes & Jenkins CI/CD

</div>

---

## 📌 Overview

This project is a **production-style Spring Boot microservice** designed to demonstrate modern backend engineering and DevOps practices in one end-to-end system.

It combines:

* **Spring Boot REST APIs**
* **Apache Kafka** for event-driven messaging
* **Redis** for caching
* **Docker** for containerization
* **Kubernetes** for orchestration
* **Jenkins** for CI/CD automation
* **ELK Stack** for centralized logging & monitoring

This repository is built as a **portfolio-grade backend + DevOps showcase** for real-world enterprise architecture.

---

## 🏗️ Architecture

```text id="85b9l5"
                            +----------------------+
                            |      Client/API      |
                            +----------+-----------+
                                       |
                                       v
                            +----------------------+
                            |  Spring Boot App     |
                            |  REST Microservice   |
                            +----+-----+-----+-----+
                                 |     |     |
                                 |     |     |
                                 v     v     v
                            +------+ +------+ +------+
                            | Redis| |Kafka | | ELK  |
                            |Cache | |Queue | |Logs  |
                            +------+ +------+ +------+
                                 |
                                 v
                           +------------------+
                           |   Docker Image   |
                           +------------------+
                                 |
                                 v
                           +------------------+
                           | Kubernetes (K8s) |
                           +------------------+
                                 |
                                 v
                           +------------------+
                           | Jenkins CI/CD    |
                           +------------------+
```

---

## ✨ Features

* ✅ Spring Boot REST API
* ✅ Apache Kafka integration
* ✅ Redis caching
* ✅ Docker containerization
* ✅ Jenkins CI/CD pipeline
* ✅ Kubernetes deployment
* ✅ ELK centralized logging
* ✅ Portfolio-ready enterprise architecture

---

## 🛠️ Tech Stack

| Technology   | Purpose                 |
| ------------ | ----------------------- |
| Java 17      | Core language           |
| Spring Boot  | Backend framework       |
| Apache Kafka | Event streaming         |
| Redis        | Distributed caching     |
| Docker       | Containerization        |
| Kubernetes   | Container orchestration |
| Jenkins      | CI/CD automation        |
| ELK Stack    | Logging & monitoring    |
| Maven        | Build tool              |

---

## 📂 Project Structure

```bash id="68u3m2"
springboot-elk-kafka-redis-cicd-docker-kubernetes/
│── DemoApplication.java
│── TestController.java
│── Dockerfile
│── Jenkinsfile
│── deployment.yaml
│── service.yaml
│── docker-compose.yml
│── pom.xml
└── README.md
```

---

## ⚙️ Setup & Run

### 1️⃣ Clone Repository

```bash id="x4g71f"
git clone https://github.com/Paraselli/springboot-elk-kafka-redis-cicd-docker-kubernetes.git
cd springboot-elk-kafka-redis-cicd-docker-kubernetes
```

### 2️⃣ Run with Docker Compose

```bash id="h0s4t6"
docker-compose up -d
```

This starts:

* Spring Boot App
* Kafka
* Redis
* Zookeeper

### 3️⃣ Run Locally

```bash id="6okm4v"
mvn spring-boot:run
```

---

## 📬 API Endpoint

### Health Check API

```http id="4ukw1o"
GET /test
```

### Response

```json id="8cm4fa"
"Application is running successfully"
```

---

## 🔁 Application Flow

1. Client sends request
2. Spring Boot processes request
3. Redis handles caching
4. Kafka handles async events
5. ELK captures logs
6. Docker packages app
7. Jenkins builds & deploys
8. Kubernetes runs production workload

---

## 🐳 Docker

This project includes:

* Dockerfile for container image creation
* Docker Compose for local multi-service setup

Build manually:

```bash id="wulj0v"
docker build -t springboot-app .
```

Run container:

```bash id="sh2nyo"
docker run -p 8080:8080 springboot-app
```

---

## ☸️ Kubernetes

Kubernetes manifests included:

* `deployment.yaml`
* `service.yaml`

Deploy to Kubernetes:

```bash id="s6n0u1"
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

---

## 🔄 Jenkins CI/CD

The `Jenkinsfile` automates:

* Build
* Test
* Docker image creation
* Deployment pipeline

Typical flow:

```text id="n7slb8"
Code Push → Jenkins Build → Docker Image → Kubernetes Deploy
```

---

## 📊 ELK Logging

ELK Stack integration enables:

* Centralized application logs
* Log aggregation
* Monitoring & observability
* Easier debugging in distributed environments

---

## 🎯 Why This Project Matters

This project demonstrates **real-world enterprise backend + DevOps engineering**:

* Microservice architecture
* Event-driven communication
* Distributed caching
* CI/CD automation
* Containerization
* Kubernetes orchestration
* Centralized logging

Perfect for:

* Backend Developer portfolio
* DevOps portfolio
* Resume showcase
* Enterprise interview discussions

---

## 👨‍💻 Author

---

### Ram Paraselli

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2?style=for-the-badge\&logo=linkedin)](https://www.linkedin.com/in/ram-paraselli/)

[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge\&logo=github)](https://github.com/Paraselli)

---

## ⭐ Support

If this project helped you, consider giving it a **star** ⭐ on GitHub.
