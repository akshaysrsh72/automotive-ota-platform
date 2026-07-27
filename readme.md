# 🚗 Automotive OTA Platform

A production-inspired microservices platform for managing connected vehicles and delivering Over-The-Air (OTA) software updates.

This project is being built from scratch to gain hands-on experience with modern Java backend development, distributed systems, cloud-native technologies, and automotive software architecture.

---

# 🎯 Project Goals

- Secure authentication using JWT
- Manage connected vehicles
- Create and manage fleets
- Schedule OTA campaigns
- Deliver firmware updates
- Collect vehicle telemetry
- Event-driven communication using Kafka
- Device communication using MQTT
- Deploy with Docker & Kubernetes
- Host on AWS
- Implement CI/CD using Jenkins
- Monitor with Prometheus & Grafana

---

# 🏗 High-Level Architecture

```text
React Admin UI
        |
        |
Spring Cloud Gateway
        |
Authentication (JWT)
        |
+-------------------------------+
|       Eureka Server           |
+-------------------------------+
        |
---------------------------------------------------------
|        |          |         |         |               |
Auth   Vehicle    Fleet   Campaign    OTA     Notification
                                           |
                                         Kafka
                                           |
                                   MQTT Publisher
                                           |
                                      MQTT Broker
                                           |
                               Connected Vehicles
```

---

# 🛠 Technology Stack

| Category | Technology |
|----------|------------|
| Language | Java 21 |
| Framework | Spring Boot |
| Security | Spring Security, JWT |
| Gateway | Spring Cloud Gateway |
| Discovery | Eureka |
| Configuration | Spring Cloud Config |
| Database | PostgreSQL |
| Messaging | Apache Kafka |
| IoT Communication | MQTT (EMQX) |
| Build Tool | Maven |
| Containerization | Docker |
| Orchestration | Kubernetes |
| Cloud | AWS |
| CI/CD | Jenkins |
| Monitoring | Prometheus, Grafana |
| Logging | ELK / Loki |
| Tracing | OpenTelemetry |

---

# 📂 Repository Structure

```text
automotive-platform/
│
├── infrastructure/
│   ├── eureka-server/
│   ├── config-server/
│   └── gateway-service/
│
├── services/
│   ├── auth-service/
│   ├── vehicle-service/
│   ├── fleet-service/
│   ├── campaign-service/
│   ├── ota-service/
│   ├── notification-service/
│   ├── telemetry-service/
│   └── audit-service/
│
├── docker/
├── kubernetes/
├── docs/
├── README.md
└── .gitignore
```

---

# 🚀 Development Roadmap

## Phase 1 - Infrastructure

- [ ] Eureka Server
- [ ] Config Server
- [ ] API Gateway

## Phase 2 - Security

- [ ] Authentication Service
- [ ] JWT Authentication
- [ ] Role-Based Access Control

## Phase 3 - Core Services

- [ ] Vehicle Service
- [ ] Fleet Service
- [ ] Campaign Service

## Phase 4 - Messaging

- [ ] Kafka
- [ ] OTA Service
- [ ] Notification Service

## Phase 5 - IoT

- [ ] MQTT Broker
- [ ] Vehicle Simulator
- [ ] Telemetry Service

## Phase 6 - Cloud

- [ ] Docker
- [ ] Kubernetes
- [ ] AWS Deployment
- [ ] Jenkins CI/CD

## Phase 7 - Monitoring

- [ ] Prometheus
- [ ] Grafana
- [ ] OpenTelemetry

---

# 📖 Learning Objectives

This project focuses on learning:

- Microservice Architecture
- Distributed Systems
- Event-Driven Architecture
- Secure REST APIs
- Spring Security
- Kafka Messaging
- MQTT Communication
- OTA Update Workflow
- Cloud Deployment
- Kubernetes
- CI/CD Pipelines
- Java Concurrency

---

# 📄 License

This project is for educational purposes.