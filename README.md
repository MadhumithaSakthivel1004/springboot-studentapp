## PROJECT STRUCTURE:
springboot-studentapp
 ┣ 📄 pom.xml
 ┣ 📄 application.properties
 ┣ 📄 StudentappApplication.java
 ┣ 📄 Student.java
 ┣ 📄 StudentRepository.java
 ┣ 📄 StudentService.java
 ┗ 📄 StudentController.java

## FEATURES:
-CRUD operations for student records
-Layered architecture (Controller → Service → Repository → Entity)
-Automatic schema generation with Hibernate
-Easy testing with Postman or browser

Student Management API (Spring Boot + MySQL)

## WHAT IS THIS PROJECT?
This is a **Spring Boot REST API** for managing student records.  
It demonstrates a clean layered architecture:
- **Entity** → Student.java (maps to database table)
- **Repository** → StudentRepository.java (data access layer)
- **Service** → StudentService.java (business logic)
- **Controller** → StudentController.java (REST endpoints)

The project uses **MySQL** as the database and **Spring Data JPA** for ORM

## HOW TO RUN:
1. Create the Database name it as **student_db**
This creates the database where student records will be stored.
2. RUN THE MAIN FILE
**StudentappApplication.java**
This starts the Spring Boot server on http://localhost:8080

## TO TEST API:
Use browser or Postman:
GET - http://localhost:8080/students → fetch all students
POST - http://localhost:8080/students → add a new student
PUT - http://localhost:8080/students/{id} → update student details
DELETE - http://localhost:8080/students/{id} → delete a student

## VERIFY IN DATABASE:
After each operation, refresh the student_db in MySQL.
You’ll see records added, updated, or deleted based on your API calls.

### QUICK FLOW RECAP:
1. Create DB → student_db
2. Configure application.properties
3. Run StudentappApplication.java
4. Test endpoints in browser/Postman
5. Refresh DB to confirm changes









