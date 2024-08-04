# JAM Bookstore

## Overview

JAM Bookstore is a Spring Boot application designed to manage a collection of books. It features basic CRUD (Create, Read, Update, Delete) operations and uses an H2 in-memory database for data storage. The application also includes a simple web interface built with Thymeleaf for managing book records.

## Features

- **Book Management**: Add, edit, and delete books.
- **H2 Database**: Uses H2 in-memory database for storing book data.
- **Web Interface**: Simple and intuitive user interface for book management.

## Technologies Used

- **Spring Boot**: Framework for building the application.
- **H2 Database**: In-memory database for development and testing.
- **Thymeleaf**: Server-side template engine for rendering web pages.
- **Spring Security**: Configured to permit access to the H2 console and disable CSRF protection for testing purposes.

## Getting Started

### Prerequisites

- Java 21 SDK
- Maven or Gradle (depending on your build tool)

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/jam-bookstore.git
   cd jam-bookstore
   ```

2. **Build the Project**

   Using Maven:

   ```bash
   mvn clean install
   ```

   Or using Gradle:

   ```bash
   ./gradlew build
   ```

3. **Run the Application**

   Using Maven:

   ```bash
   mvn spring-boot:run
   ```

   Or using Gradle:

   ```bash
   ./gradlew bootRun
   ```

4. **Access the Application**

   Open a web browser and go to `http://localhost:8080`.

### Usage

- **View Books**: Navigate to `http://localhost:8080/books` to see the list of books.
- **Add Book**: Go to `http://localhost:8080/books/add` to add a new book.
- **Edit Book**: Click "Edit" next to a book in the list to modify its details.
- **Delete Book**: Click "Delete" next to a book in the list to remove it.

### Access H2 Console

To access the H2 database console:

1. Open `http://localhost:8080/h2-console` in your web browser.
2. Use the following credentials:
   - **JDBC URL**: `jdbc:h2:mem:bookstoredb`
   - **User Name**: `Mohammadh2`
   - **Password**: `passwordhtwo`

### Configuration

- **Database**: Configured to use an H2 in-memory database. See `src/main/resources/application.properties` for details.
- **Security**: Spring Security is configured to permit access to the H2 console and disable CSRF protection for testing.

## Contributing

Feel free to submit issues or pull requests to improve the project.

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and test thoroughly.
4. Submit a pull request with a description of your changes.

## Acknowledgments

- [Spring Boot](https://spring.io/projects/spring-boot)
- [H2 Database](https://www.h2database.com/)
- [Thymeleaf](https://www.thymeleaf.org/)

---