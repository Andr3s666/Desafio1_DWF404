## 📚 Book API - Letras Vivas

This is a basic REST API developed with Spring Boot for the fictional publishing house **"Letras Vivas"**, as part of the practical challenge for the subject **Web Application Development with Frameworks**.

## 🚀 Features

- List all books
- Add a new book
- Search books by title
- Delete a book by ID

## 🛠️ Technologies

- Java 17
- Spring Boot 3.2.4
- Maven
- Spring Web
- Spring Data JPA
- H2 In-Memory Database

## 📁 Project structure

The code follows a layered architecture:
- `model`: Book class
- `repository`: BookRepository interface
- `service`: BookService class
- `controller`: BookController class

## ⚙️ Configuration

The `application.properties` includes:

```properties
server.port=8080
spring.datasource.url=jdbc:h2:mem:booksdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true
spring.jpa.hibernate.ddl-auto=update
