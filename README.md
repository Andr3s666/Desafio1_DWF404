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

## ▶️ How to run
Clone the repository:

git clone https://github.com/your-user/bookapi.git
cd bookapi
Open the project in IntelliJ IDEA

Run the BookapiApplication.java main class

Access:

API: http://localhost:8080/api/books

H2 Console: http://localhost:8080/h2-console

## 🧪 Test with Postman
1. Get all books
GET http://localhost:8080/api/books

2. Add a book
POST http://localhost:8080/api/books

json
Copiar
Editar
{
  "title": "Clean Code",
  "author": "Robert C. Martin",
  "publicationYear": 2008
}
3. Search books
GET http://localhost:8080/api/books/search?title=code

4. Delete book
DELETE http://localhost:8080/api/books/1
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true
spring.jpa.hibernate.ddl-auto=update

## 👨‍🎓 Authors
Andres Eduardo Navidad Flores (NF220677)
