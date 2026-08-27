# ServiceHub - Eureka Server

## 📌 Overview

The **Eureka Server** provides service discovery for the ServiceHub microservice architecture.

It maintains a registry of available ServiceHub services and allows services to discover each other dynamically.

---

## 👨‍🎓 Student Information

| Information | Details |
|---|---|
| Student Name | Yashoda Gunawardhana |
| Student ID | 241711077 |
| Project | ServiceHub |
| Component | Eureka Server |
| GCP Project ID | project-a6d8ea92-fb5d-4ed6-99d |

---

## 🛠️ Technology Stack

- Java 25
- Spring Boot
- Spring Cloud Netflix Eureka
- Maven

---

## 🏗️ Architecture

```
                 Eureka Server
                    :8761
                       |
        +--------------+--------------+
        |              |              |
        v              v              v
   API Gateway    User Service    Request Service
      :8080           :8081           :8082
                                       |
                                       v
                                Provider Service
                                      :8083
```

---

## 🔎 Service Discovery

The following services register with Eureka:

- API Gateway
- User Service
- Request Service
- Provider Service

Eureka provides the service registry used by the microservices and API Gateway.

---

## 🔌 Service Information

| Property | Value |
|---|---|
| Service Name | eureka-server |
| Port | 8761 |
| Type | Service Registry |

---

## 🚀 Running the Server

**Windows**

```bash
.\mvnw.cmd spring-boot:run
```

### Build

```bash
.\mvnw.cmd clean package
```

### Run Tests

```bash
.\mvnw.cmd test
```

---

## 🌐 Eureka Dashboard

When running locally:

http://localhost:8761

---

## 🔗 GitHub Repository

https://github.com/yashodha-gunawardana/eureka-server

---

## 📌 Project Status

- Java 25: ✅
- Eureka Server: ✅
- GitHub Repository: ✅
- GCP Deployment: ⏳

---
