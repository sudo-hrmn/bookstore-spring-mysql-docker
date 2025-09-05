# Spring Boot Book Store Management System

A containerized Spring Boot book store management system with MySQL database using Docker Compose for local development and deployment.

## Architecture Diagram

![Architecture Diagram](architect%20diagram.png)

## Features
- Add, view, and manage book inventory
- Author and pricing management
- Responsive web interface with Thymeleaf templates
- MySQL database integration with JPA/Hibernate
- Containerized deployment with Docker

## Tech Stack
- **Backend:** Spring Boot 2.3.8, Spring Data JPA, Hibernate
- **Frontend:** Thymeleaf, HTML, CSS, Bootstrap
- **Database:** MySQL 5.7
- **Containerization:** Docker, Docker Compose
- **Build Tool:** Maven

## Quick Start

### Prerequisites
- Docker & Docker Compose
- Java 11+ (for local development)
- Maven (for local development)

### Running the Application

1. Clone the repository:
```bash
git clone https://github.com/sudo-hrmn/bookstore-spring-mysql-docker.git
cd bookstore-spring-mysql-docker
```

2. Start the application:
```bash
docker-compose up -d
```

3. Access the application:
```
http://localhost:8080
```

### Stopping the Application
```bash
docker-compose down
```

## Project Structure
```
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── in/ashokit/
│   │   │       ├── Application.java
│   │   │       ├── controller/BookController.java
│   │   │       ├── binding/Book.java
│   │   │       └── repository/BookRepository.java
│   │   └── resources/
│   │       ├── application.yml
│   │       └── templates/
│   │           ├── index.html
│   │           └── success.html
├── Dockerfile
├── docker-compose.yml
└── pom.xml
```

## Database Schema
- **Database:** sbms
- **Table:** book
  - book_id (Primary Key)
  - book_name
  - author_name
  - book_price

## Contact
**Harman Singh**  
Contact: [LinkedIn](https://www.linkedin.com/in/harmansinghsudo/)
