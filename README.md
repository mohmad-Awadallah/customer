Project Description: CRUD API for Customer Entity
Short description
Project Description: CRUD API for Customer Entity
README
Updated Project Description with Redis Integration
This project implements a production-level RESTful API for managing customer data using Java, Spring Boot, and Redis as a caching layer. The API supports CRUD operations (Create, Read, Update, Delete) for customer records, with H2 as the primary in-memory database. The application follows best practices, including layered architecture, exception handling, validation, and caching for optimized performance.

How to Run the Project
Clone the repository:
Clone the project repository to your local machine and navigate to the project directory.

Build the project:
Compile the project and package it as a JAR:

mvn clean package
Run the Spring Boot application:
Start the application locally using Gradle:

./gradlew bootRun
Run Redis with Docker:
Start a Redis instance using Docker:

docker-compose -f docker-compose.yaml up
Access the API:

Use tools like Postman or Curl to test the endpoints.
Base URL: http://localhost:8080
Optional: Access the H2 database:

Navigate to the H2 Console at: http://localhost:8080/h2-console.
Use the JDBC URL, username, and password configured in application.properties.
Features Added by Redis
Caching: Frequently accessed customer data is cached to reduce latency.
Reduced Database Load: Fewer direct queries to the H2 database.
TTL (Time-to-Live): Cache entries are configured to expire after a set duration to ensure data freshness.
Future Enhancements
Add security using Spring Security with JWT for authentication and authorization.
Integrate a production-grade database like MySQL or PostgreSQL for persistent storage.
Implement pagination and sorting for customer listing endpoints.
Extend Docker Compose to manage the entire application stack.
Include Redis Cluster or Sentinel for high availability in production environments.
