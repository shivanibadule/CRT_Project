# Flight Service Platform

A full-stack web application designed for searching, managing, and booking flights. This project features a robust Spring Boot backend (Java 21) communicating with a MySQL database, paired with a modern React UI.

## Technologies Used

### Backend
- **Java 21**: Core language for the backend.
- **Spring Boot 4.0.x**: Rapid application development framework.
- **Spring Data JPA**: For database interactions and ORM.
- **MySQL**: Relational database.
- **Springdoc OpenAPI (Swagger)**: For auto-generating API documentation and testing capabilities.
- **Maven**: Build and dependency management.

### Frontend
- **React**: Modern component-based UI library.
- **CSS / Flexbox / Grid**: For responsive design and sophisticated layouts matching modern aesthetics.
- **Axios / fetch**: For executing requests against the REST API.
- **NPM Package Manager**: Managing frontend dependencies.

## Project Structure

- `/src/main/java`: Backend source code including Controllers, Services, and Repositories.
- `/src/test/java`: Backend integration and unit tests.
- `/frontend`: The React frontend application.
- `pom.xml`: Maven configuration for the backend.

## Prerequisites

- **Java Development Kit (JDK) 21** or later
- **Maven 3.8+**
- **Node.js (v18+) and npm**
- **MySQL Database Server**

## Getting Started

### 1. Database Setup
Create a new MySQL database named `flightdb` (or as configured in your `application.properties`/`application.yml`).

```

Update your `src/main/resources/application.properties` with your database credentials:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/db_name
spring.datasource.username=username
spring.datasource.password=your_password
```

### 2. Running the Backend (Spring Boot)
Open your terminal in the project root directory and run:

```bash
mvn spring-boot:run
```
Alternatively, just run the main application file from your preferred standard IDE (Eclipse, IntelliJ IDEA, or VS Code). The API by default will run on `http://localhost:8080`.

**API Documentation:**
Once running, you can interact with the Swagger documentation by navigating to:
`http://localhost:8080/swagger-ui.html`

### 3. Running the Frontend (React)
Open a new terminal window, navigate to the `frontend` directory, and start the development server:

```bash
cd frontend
npm install
npm start
```
The application will open in development mode at `http://localhost:3000`.

## Features
- Search for flights based on various criteria (e.g., origin, destination, dates).
- Fetch details of a specific flight carrier or price.
- Dynamic responsive UI that adapts to both desktop and mobile views.
- Dedicated modular React components for adding, listing, and filtering available flights.
