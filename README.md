# Student Data Access Layer using Spring Boot & JPA

## 📌 Project Description

This project demonstrates the implementation of a Data Access Layer (DAL) using Spring Boot and Spring Data JPA. It provides REST APIs to retrieve student records based on conditions like department and age.

## 🚀 Technologies Used

* Java 17
* Spring Boot
* Spring Data JPA
* MySQL
* Maven
* Eclipse IDE
* Postman

## 📂 Project Structure

com.example.studentdal
│── controller
│   └── StudentController.java
│── service
│   └── StudentService.java
│── repository
│   └── StudentRepository.java
│── model
│   └── Student.java

## ⚙️ Configuration

application.properties

spring.datasource.url=jdbc:mysql://localhost:3306/studentdb
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

## 📡 API Endpoints

Get Students by Department
GET /students/department/{dept}

Get Students by Age
GET /students/age/{age}

Get Students Older Than Age
GET /students/age/greater/{age}

Filter by Department & Age
GET /students/filter?department=CSE&age=20

## 🧪 Sample Output

[
{
"id": 1,
"name": "Naveen",
"department": "CSE",
"age": 20
}
]

## 🛠️ How to Run

1. Clone the repository
   git clone https://github.com/your-username/student-dal-springboot-jpa.git

2. Open in Eclipse

3. Configure MySQL database

4. Run the application

5. Test APIs using browser or Postman

## 📊 Database Query

SELECT * FROM student;

## 🎯 Features

* Spring Data JPA Repository
* Custom Query Methods
* REST API Implementation
* MySQL Integration

## 👨‍💻 Author

Naveen
