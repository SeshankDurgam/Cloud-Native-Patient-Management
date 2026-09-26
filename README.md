# 🏥 Production-Ready Patient Management System (Java Microservices + Spring Boot + AWS)

This is a **Production-Ready Patient Management System** built using **Java**, **Spring Boot**, and **Microservices Architecture**, and deployed with **AWS**. It is designed to be scalable, maintainable, and secure — providing a real-world use case of a healthcare system where patients, doctors, and appointments are managed using decoupled microservices.

---

## 📌 Project Architecture

This project follows a distributed microservices architecture with the following components:

- **API Gateway** – Entry point for all clients, implemented using Spring Cloud Gateway
- **Config Server** – Centralized configuration for all microservices
- **Eureka Server** – Service discovery and registration
- **Auth Service** – Handles user registration, login, and JWT-based authentication
- **Patient Service** – Manages patient information
- **Doctor Service** – Manages doctor data
- **Appointment Service** – Schedules and manages appointments
- **Notification Service** – Sends email/SMS notifications (optional)
- **Database** – Uses MySQL and MongoDB
- **Deployment** – Configured for cloud deployment on AWS EC2 or ECS

---

## 🚀 Features

- ✅ Microservices-based modular architecture
- ✅ RESTful APIs for communication
- ✅ Java + Spring Boot for robust backend services
- ✅ Spring Security with JWT authentication and role-based authorization
- ✅ Spring Cloud Gateway for routing and security
- ✅ Centralized configuration using Spring Cloud Config
- ✅ Service Registry and Discovery with Netflix Eureka
- ✅ Resilience with Circuit Breakers (using Resilience4j or Netflix Hystrix)
- ✅ Load balancing with Ribbon
- ✅ Dockerized for containerized deployment
- ✅ AWS integration for deployment and scalability
- ✅ Swagger for API documentation

---

## 📂 Project Structure

.
├── api-gateway
├── config-server
├── discovery-server (Eureka)
├── auth-service
├── patient-service
├── doctor-service
├── appointment-service
├── notification-service (optional)
├── common-utils
├── docker-compose.yml
└── README.md



---

## 🛠️ Tech Stack

- **Language:** Java 17
- **Framework:** Spring Boot, Spring Cloud
- **Security:** Spring Security, JWT
- **Databases:** MySQL, MongoDB
- **Service Registry:** Eureka
- **Gateway:** Spring Cloud Gateway
- **Config Server:** Spring Cloud Config
- **Containerization:** Docker
- **Deployment:** AWS EC2, AWS ECS, Docker Compose
- **DevOps:** CI/CD pipeline (GitHub Actions or similar - if configured)
- **API Docs:** Swagger/OpenAPI

---

## 🖥️ How to Run Locally

### Prerequisites

- Java 17+
- Maven
- Docker & Docker Compose
- MySQL and MongoDB running (or use Docker)

### Steps

1. Clone the repo

```bash
git clone https://github.com/Abhisheksur123/Production-Ready-Patient-Management-System-with-Microservices-Java-Spring-Boot-AWS.git
cd Production-Ready-Patient-Management-System-with-Microservices-Java-Spring-Boot-AWS


Build each service:

bash
Copy
Edit
mvn clean install
Run using Docker Compose:

bash
Copy
Edit
docker-compose up --build
Access Services:

Gateway: http://localhost:8080

Eureka Dashboard: http://localhost:8761

Swagger UI (per service): http://localhost:<service-port>/swagger-ui/index.html

🔐 Authentication
JWT-based authentication system via auth-service

Roles: ADMIN, DOCTOR, PATIENT

Each user gets a token on successful login

Include Authorization: Bearer <token> in headers to access protected endpoints

🧪 API Documentation
Swagger is enabled in all microservices for easy testing and documentation.

Example:
http://localhost:<port>/swagger-ui/index.html

☁️ Deployment on AWS
You can deploy each service on:

AWS EC2 (manual setup or with Docker Compose)

AWS ECS (using containerized microservices)

AWS RDS for MySQL

AWS S3 (optional for storage)

AWS CloudWatch (for logs and monitoring)

📈 Future Enhancements
✅ Frontend Integration (React.js or Angular)

🔄 Kafka-based Event-Driven communication

📦 CI/CD pipeline using GitHub Actions or Jenkins

📊 Monitoring using Prometheus + Grafana

🔒 OAuth2 or SSO integration

📱 Mobile App support

🤝 Contributing
Contributions are welcome! Feel free to open issues or submit PRs to improve the codebase.

📄 License
This project is open-source and available under the MIT License.

🙋‍♂️ Author
Abhishek Sur
📧 abhisheksur99@gmail.com
