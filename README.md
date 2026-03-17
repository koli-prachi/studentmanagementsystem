# 🎓 Student Management System

A robust and scalable **Spring Boot CRUD application** designed to manage student records efficiently. This project follows a clean **layered architecture (MVC pattern)** and demonstrates best practices in backend development using Java.

---

## 📌 Project Description

The Student Management System enables users to perform complete **CRUD operations** on student data through a user-friendly web interface.

It is built to showcase:
- Clean code structure
- Separation of concerns
- Database integration using JPA
- Server-side rendering using Thymeleaf

---

## 🏗️ Architecture

The application follows a **3-layer architecture**:

1. **Controller Layer**
   - Handles HTTP requests
   - Maps URLs to business logic

2. **Service Layer**
   - Contains core business logic
   - Acts as an intermediary between controller and repository

3. **Repository Layer**
   - Handles database operations
   - Uses Spring Data JPA for abstraction

---

## 🚀 Features

- Create new student records  
- Retrieve and display all students  
- Update existing student details  
- Delete student entries  
- Server-side rendering with Thymeleaf  
- Persistent storage with MySQL  
- Clean and maintainable project structure  

---

## 🛠️ Technology Stack

| Layer        | Technology Used              |
|-------------|-----------------------------|
| Language     | Java                        |
| Framework    | Spring Boot                |
| Web Layer    | Spring MVC                 |
| ORM          | Hibernate (JPA)            |
| Database     | MySQL                      |
| View Engine  | Thymeleaf                  |
| Build Tool   | Maven                      |

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

