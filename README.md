# QuizApp - Microservices Application 🧠🛠️

This is a **Microservices-based Quiz Application** developed using **Spring Boot**, demonstrating core microservice architecture principles including service decomposition, inter-service communication, centralized routing with API Gateway, and service discovery using Eureka.

---

## 📌 Features

- 🚀 Microservices Architecture (User, Quiz, Question Services)
- 🔀 REST Communication between services
- 🌐 API Gateway for routing and centralized entry point
- 🧭 Eureka Discovery Server for service registration/discovery
- 🧪 Sample quiz creation and result retrieval
- 🧰 Spring Boot 3, Spring Web, Spring Data JPA, Spring Cloud
- 🗃️ H2 In-Memory Database (easily switchable to MySQL/PostgreSQL)

---

## 🧱 Microservices Breakdown

| Service        | Port | Description                                |
|----------------|------|--------------------------------------------|
| **API Gateway** | 8080 | Central routing point for all services     |
| **User Service** | 8081 | Manages quiz users                         |
| **Question Service** | 8082 | Manages questions bank                   |
| **Quiz Service** | 8083 | Creates quizzes and retrieves quiz data    |
| **Eureka Server** | 8761 | Service registry and discovery server     |

---

## 📁 Project Structure

quizapp-microservices-application/
├── api-gateway/
├── eureka-server/
├── user-service/
├── question-service/
└── quiz-service/


Each module is a separate Spring Boot application with its own configurations.

---

## ⚙️ Technologies Used

- Java 17
- Spring Boot 3.x
- Spring Cloud (Eureka, Gateway)
- Spring Web
- Spring Data JPA
- H2 Database
- Maven

---

## 🚦 How to Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/VamsiKrishnaAlapati31/QuizApp-Microservices-Application.git
   cd QuizApp-Microservices-Application
2.Start Eureka Server

Navigate to eureka-server/ and run the application.

3.Start All Services

Run api-gateway/, user-service/, question-service/, and quiz-service one by one from your IDE or using:
bash : 
mvn spring-boot:run

Access Services

Eureka Dashboard: http://localhost:8761

API Gateway (entry point): http://localhost:8080

🔍 Sample Endpoints
Get all users: GET http://localhost:8080/user

Get all questions: GET http://localhost:8080/question

Get all quizzes: GET http://localhost:8080/quiz

📝 Author
Vamsi Krishna Alapati
Java | Spring Boot | Microservices 
📧 vamsialapati1431@gmail.com

🌟 Star this repo if it helped you!


