Dim readmeContent As String = "
FrontEnd for this Project: https://github.com/sakshi-j-alt/Job-Application-Front-End

# 💼 Job Portal Application (Spring Boot)

A **robust and scalable backend system** for a job portal, developed using **Spring Boot**. It supports user roles (**Admin**, **Recruiter**, and **Job Seeker**), **secure authentication via JWT**, **job posting**, **application tracking**, and more.

---

## 🔧 Technologies Used

| Layer         | Stack                          |
|---------------|-------------------------------|
| Language      | Java 17+                       |
| Framework     | Spring Boot                    |
| ORM           | Hibernate, Spring Data JPA     |
| Security      | Spring Security (JWT)          |
| Database      | MySQL / H2 (for testing)       |
| Build Tool    | Maven                          |
| Project Tools | Lombok, Swagger (optional)     |

---

## ✅ Features

### 🔐 User Roles
- **Admin**: Manage all jobs and users
- **Recruiter**: Post jobs, manage applications
- **Job Seeker**: Apply for jobs, track status

### 💼 Job Management
- Post, update, delete jobs (Recruiter)
- View all jobs (All roles)
- Apply for jobs (Job Seeker)

### 🔒 Security
- JWT-based authentication
- Password encryption (BCrypt)
- Role-based access control

### 🛠 Developer Features
- Exception Handling
- Clean Code with DTOs
- Configurable with external database (MySQL)
- Swagger support (optional)

---

## ⚙️ Getting Started

### Prerequisites
- Java 17+
- Maven 3.6+
- MySQL (or use H2 for local testing)

### Steps

1. Clone the Repository
git clone https://github.com/ParikshitJ06/job-portal-application.git
cd job-portal-application/job-application


2. Configure Database
Edit `src/main/resources/application.properties`:
MySQL example
spring.datasource.url=jdbc:mysql://localhost:3306/job_portal
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update


---

## 🔗 API Endpoints

| Method | Endpoint                | Description                     |
| ------ | ----------------------- | ------------------------------- |
| POST   | /auth/register          | Register new user               |
| POST   | /auth/login             | Login and receive JWT           |
| GET    | /jobs                   | View all job listings           |
| POST   | /jobs                   | Create new job (Recruiter only) |
| DELETE | /jobs/{id}              | Delete job (Recruiter/Admin)    |
| POST   | /jobs/{id}/apply        | Apply to job (Job Seeker only)  |
| GET    | /applications/user/{id} | View user’s applications        |

---

## 📂 Folder Overview

- controllers/ – REST endpoints for jobs, users, applications
- services/ – Business logic and validation
- repositories/ – JPA repositories for DB operations
- entities/ – JPA entity models
- dtos/ – Clean data transfer objects
- security/ – JWT filters, configs, and utils

---

## 🧪 Testing

Use tools like Postman, Swagger, or any REST client to test the endpoints.

---

## 🧠 Future Enhancements
- Frontend integration
- Resume upload feature
- Email notifications
- Admin dashboard with analytics
- Job search/filter by category, location, salary

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

Parikshit Jadhav
📧 jadhavparikshit0510@gmail.com
"

