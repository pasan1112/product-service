# Product Service Microservice

IT Number: IT22189776  
Module: SE4010 – Current Trends in Software Engineering  
Lab: DevOps Lab 03  

---

## 📌 Project Overview

This project is a simple Spring Boot RESTful microservice built as part of DevOps Lab 03.

It demonstrates:

- CRUD REST APIs
- Spring Data JPA
- In-memory H2 Database
- Swagger (OpenAPI) documentation

The service manages `Product` entities with:

- id
- name
- price

---

## 🛠️ Technologies Used

- Java 17
- Spring Boot 3.5.10
- Spring Web
- Spring Data JPA
- H2 Database (In-Memory)
- Springdoc OpenAPI (Swagger UI)
- Maven

---

## ▶️ How to Run the Application

### Option 1 – Using IDE
Run the main class:

ProductServiceApplication.java


### Option 2 – Using Maven

```bash
mvn spring-boot:run
The application runs on:

http://localhost:8080
📡 Available REST Endpoints
Base URL:

http://localhost:8080/products
Method	Endpoint	Description
POST	/products	Create a new product
GET	/products	Get all products
GET	/products/{id}	Get product by ID
DELETE	/products/{id}	Delete product by ID
🧪 Swagger UI (API Documentation)
Access Swagger UI at:

http://localhost:8080/swagger-ui/index.html
Swagger allows testing all REST APIs directly from the browser.

🗄️ H2 Database Console
Access H2 Console at:

http://localhost:8080/h2-console
Use the following configuration:

JDBC URL: jdbc:h2:mem:testdb

Username: sa

Password: (leave blank)

To verify table:

SELECT * FROM PRODUCT;
📂 Project Structure
com.sliit.productservice
│
├── controller
│   └── ProductController.java
│
├── model
│   └── Product.java
│
├── repository
│   └── ProductRepository.java
│
└── ProductServiceApplication.java

🎯 Expected Learning Outcome
This lab demonstrates how to:
Build a Spring Boot microservice
Implement REST APIs
Use JPA for data persistence
Configure and use an in-memory database
Document APIs using Swagger

🔗 GitHub Repository
https://github.com/pasan1112/product-service