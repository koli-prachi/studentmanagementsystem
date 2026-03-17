# 🎓 Student Management System

A Spring Boot based CRUD web application to manage student records efficiently. This project demonstrates the use of Spring Boot, Spring MVC, Spring Data JPA, Thymeleaf, and MySQL.

---

## 🚀 Features

- Add new students  
- View all students  
- Update student details  
- Delete student records  
- Persistent storage using MySQL  
- Web interface using Thymeleaf  

---

## 🛠️ Tech Stack

- Java  
- Spring Boot  
- Spring MVC  
- Spring Data JPA (Hibernate)  
- MySQL  
- Thymeleaf  
- Maven  

---

## 📂 Project Structure

student-management-system  
│  
├── controller        (Handles HTTP requests)  
├── entity            (JPA Entity - Student)  
├── repository        (JpaRepository interface)  
├── service           (Business logic layer)  
├── templates         (Thymeleaf HTML files)  
├── application.properties  
└── main class  

---

## ⚙️ Setup Instructions

### 1. Clone Repository
git clone https://github.com/your-username/student-management-system.git  
cd student-management-system  

---

### 2. Create Database

Run this in MySQL:

CREATE DATABASE studentdb;

---

### 3. Configure application.properties

spring.datasource.url=jdbc:mysql://localhost:3306/studentdb  
spring.datasource.username=root  
spring.datasource.password=root  

---

### 4. Run Application

Using Maven:
mvn spring-boot:run  

OR run the main class:
StudentManagementSystemApplication.java  

---

### 5. Open in Browser

http://localhost:8081/students  

---

## 🔗 Endpoints

GET     /students              -> View all students  
GET     /students/new          -> Show create form  
POST    /students              -> Save student  
GET     /students/edit/{id}    -> Show edit form  
POST    /students/{id}         -> Update student  
GET     /students/{id}         -> Delete student  

---

## ⚠️ Notes

- Default port: 8081  
- MySQL must be running  
- Hibernate auto updates tables (ddl-auto=update)  

---

## 📈 Future Improvements

- Add validation  
- Add authentication (Spring Security)  
- Pagination and search  
- REST API version  

---

## 👩‍💻 Author

Prachi Koli  
BE IT Student  


