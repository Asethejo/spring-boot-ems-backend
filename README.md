# Employee Management System (EMS) – Spring Boot Backend

This project is a **Spring Boot REST API backend** for an **Employee Management System (EMS)**.  
It is built using **Spring Boot, Spring Data JPA, Hibernate, and PostgreSQL**, following a clean **3-layer architecture**.

The application supports basic employee management operations and is tested using **Postman** with database verification through **pgAdmin**.

---

## 📌 Project Overview

The project follows a standard layered backend architecture:

- **Controller Layer**  
  Handles incoming HTTP requests and exposes REST APIs.
- **Service Layer**  
  Contains business logic and data processing.
- **Repository Layer**  
  Communicates with the PostgreSQL database using Spring Data JPA.

---

## 🚀 Features

- Create employee
- Fetch all employees
- PostgreSQL database integration
- RESTful API design
- Layered architecture (Controller, Service, Repository)
- JPA & Hibernate ORM

---

## 🛠️ Tech Stack

- Java 17  
- Spring Boot  
- Spring Web  
- Spring Data JPA  
- Hibernate  
- PostgreSQL  
- Maven  

---

## 🧰 Tools & IDE Used

- **Visual Studio Code (VS Code)**
- **VS Code Extensions**
  - Spring Boot Extension Pack  
  - Java Extension Pack  
  - Maven for Java  
- **Postman** – API testing  
- **pgAdmin 4** – PostgreSQL database management  
- **Git & GitHub** – Version control  
- **Maven Wrapper (`mvnw`)** – Build & dependency management  

---

## 📂 Project Structure

```text
src/main/java/com/example/demo
│
├── controller        → REST controllers
├── service
│   ├── impl          → Service implementations
│   └── EmployeeService.java
├── repository        → JPA repositories
├── entity            → JPA entities
├── dto               → Data Transfer Objects
├── mapper            → Entity ↔ DTO mapping
└── DemoApplication.java

⚙️ Database Configuration
Create Database
sql
Copy code
CREATE DATABASE ems;
Configure application.properties
properties
Copy code
spring.datasource.url=jdbc:postgresql://localhost:5432/ems
spring.datasource.username=postgres
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

▶️ Steps to Run the Project!!

1️⃣ Clone the Repository

git clone https://github.com/<your-username>/spring-boot-ems-backend.git
cd spring-boot-ems-backend
2️⃣ Open in VS Code
Open the project folder in VS Code

Ensure Java & Spring extensions are installed

3️⃣ Start PostgreSQL
Start PostgreSQL server

Verify database connection in pgAdmin

4️⃣ Run the Application
Using VS Code:

Open DemoApplication.java

Click Run

OR using terminal:

./mvnw spring-boot:run
5️⃣ Verify Application
Open browser:

http://localhost:8080/employees
Expected response:
[]

🔌 API Endpoints
➕ Create Employee
POST
http://localhost:8080/employees
Request Body

{
  "firstName": "Jothika",
  "lastName": "Jo",
  "email": "jothikajo63@example.com"
}
📄 Get All Employees
GET
http://localhost:8080/employees
🧪 API Testing
APIs tested using Postman

Verified responses for POST & GET requests

Data persistence confirmed using pgAdmin

⚠️ Challenges Faced & Learnings
❌ 1. Database Connection Issues
Faced incorrect database and credential configurations

Learned how JDBC URL, username, and password work together

❌ 2. Table & Schema Confusion
Encountered relation does not exist errors

Learned the difference between database, schema, and table names

❌ 3. Application Startup & Port Issues
Faced localhost refused to connect

Learned how to analyze Spring Boot logs and verify Tomcat port usage

❌ 4. Maven & Dependency Errors
Faced build and reload issues after updating pom.xml

Learned how to reload Maven projects and use Maven Wrapper

❌ 5. REST API Testing Errors
Incorrect URLs and HTTP methods caused failures

Learned correct usage of GET, POST, and request bodies

❌ 6. Tool & Environment Setup Issues
Faced issues configuring VS Code extensions, Maven reload, and PostgreSQL in pgAdmin

Learned how different tools (VS Code, Postman, pgAdmin) work together in a backend project

✅ Key Learnings
1.Built a real-world Spring Boot REST API

2.Understood layered backend architecture

3.Hands-on experience with PostgreSQL & JPA

4.Practical debugging and troubleshooting

5.Confidence in backend development workflow

👩‍💻 Author
Jothika
Java | Spring Boot | Backend Developer

