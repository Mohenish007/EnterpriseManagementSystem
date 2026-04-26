📌 About the Project

This is a backend Enterprise Management System (EMS) built using a microservices architecture with Spring Boot and Node.js.
It enables HR professionals to efficiently manage employees, departments, recruitment processes, job positions, payroll, and leave records within a scalable and modular system.

The application allows HR agents to:

View and filter employee data (e.g., by department)
Create, update, and delete employee records
Manage job postings and applicants
Handle payroll and salary information
Track employee leaves and holidays
🚀 Key Features

The system consists of 5 core microservices, each handling a specific HR function:

Employee Service
Manages employee and candidate information such as hiring date, email, role, and personal details.
Recruitment Service
Handles job postings, applications, and recruitment workflows.
Position Service
Manages job roles, departments, and organizational structure.
Payroll Service
Handles employee salary and payroll-related data.
Leave/Holiday Service
Manages employee leaves and company holidays.
🏗️ Technical Architecture

This system follows a microservices-based architecture with the following core modules:

Gateway Service
Acts as the entry point for all client requests (API Gateway).
Config Service
Centralized configuration management using Spring Cloud Config.
Discovery Service
Service registry using Netflix Eureka for dynamic service discovery.
Employee Service
Handles CRUD operations for employee data.
Payroll Service
Manages payroll data and communicates with other services.
Recruitment Service
Manages recruitment-related operations.
Position Service
Handles job roles and department-related data.
Leave/Holiday Service
Manages leave requests and holiday data.
🔐 Authentication Flow
Users must register via the Auth Service
A token is generated upon successful authentication
All requests pass through the Gateway Service
The gateway validates the token before granting access to microservices
🛠️ Tech Stack
Backend: Spring Boot, Node.js
Databases: MySQL, MongoDB
Containerization: Docker, Docker Compose
Architecture: Microservices, REST APIs
Cloud Tools: Spring Cloud, Netflix OSS
⚡ Getting Started
📋 Prerequisites

Make sure you have installed:

Java (JDK 8 or above)
Maven
Docker
🧑‍💻 Installation
Clone the repository
git clone https://github.com/your-username/your-repo-name.git
Build all microservices
mvn clean package
Run the application using Docker
docker-compose up
🌐 Access the Application

Open your browser and visit:

http://localhost:8761

👉 This will open the Eureka Dashboard, where all services are registered.

📈 Roadmap
✅ Phase 1
Setup Discovery Service (Eureka)
Setup Gateway Service (Zuul)
Setup Config Server
✅ Phase 2
Implement core microservices:
Employee Service
Recruitment Service
Position Service
Payroll Service
Leave/Holiday Service
