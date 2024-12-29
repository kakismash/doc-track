<div align="center" id="top"> <img src="./.github/app.gif" alt="Doc Track" />
 

<!-- <a href="https://doctrack.netlify.app">Demo</a> --> </div> <h1 align="center">Doc Track</h1> <p align="center"> <img alt="Github top language" src="https://img.shields.io/github/languages/top/{{YOUR_GITHUB_USERNAME}}/doc-track?color=56BEB8"> <img alt="Github language count" src="https://img.shields.io/github/languages/count/{{YOUR_GITHUB_USERNAME}}/doc-track?color=56BEB8"> <img alt="Repository size" src="https://img.shields.io/github/repo-size/{{YOUR_GITHUB_USERNAME}}/doc-track?color=56BEB8"> <img alt="License" src="https://img.shields.io/github/license/{{YOUR_GITHUB_USERNAME}}/doc-track?color=56BEB8"> </p> <p align="center"> <a href="#dart-about">About</a> &#xa0; | &#xa0; <a href="#sparkles-features">Features</a> &#xa0; | &#xa0; <a href="#rocket-technologies">Technologies</a> &#xa0; | &#xa0; <a href="#gear-architecture">Architecture</a> &#xa0; | &#xa0; <a href="#white_check_mark-requirements">Requirements</a> &#xa0; | &#xa0; <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0; <a href="#memo-license">License</a> &#xa0; | &#xa0; <a href="https://github.com/{{YOUR_GITHUB_USERNAME}}" target="_blank">Author</a> </p> <br>
:dart: About
Doc Track is an example of a modern microservices architecture application. It demonstrates the integration of multiple microservices with modern tools and frameworks, including an API Gateway, AuthService, Eureka Server, various domain-specific microservices, and a frontend built using Ionic.

The application is reactive, using Spring Boot and PostgreSQL, showcasing scalability, modularity, and real-world practices for building distributed systems.

:sparkles: Features
:heavy_check_mark: Reactive Spring Boot microservices;
:heavy_check_mark: Centralized API Gateway for routing and security;
:heavy_check_mark: AuthService with JWT-based authentication;
:heavy_check_mark: Service discovery using Eureka Server;
:heavy_check_mark: Modular microservices architecture;
:heavy_check_mark: Frontend integration using Ionic framework;
:heavy_check_mark: Postgres for persistent storage;
:heavy_check_mark: Built-in examples for extensibility.

:rocket: Technologies
The following tools were used in this project:

Backend:

Spring Boot (Reactive)
PostgreSQL
Spring Cloud Gateway (API Gateway)
Eureka Server
Spring Security
Frontend:

Ionic
Angular
Other Tools:

JWT (Authentication)
Flyway (Database migrations)
:gear: Architecture
Microservices
API Gateway:

Central entry point for routing requests to microservices.
Handles cross-cutting concerns like security (JWT) and load balancing.
AuthService:

Manages user authentication and authorization.
Issues JWT tokens for secure communication.
Eureka Server:

Service discovery for dynamic microservice registration and lookup.
Domain Microservices:

Independent services, each responsible for a specific domain.
Communicate with other services via API Gateway.
Ionic Frontend:

User-facing application interacting with the API Gateway.
Database
Uses PostgreSQL as the primary database for all microservices.
Each microservice manages its own schema.
Reactive Design
Implements reactive programming with Spring WebFlux for non-blocking and asynchronous communication.
:white_check_mark: Requirements
Before starting :checkered_flag:, ensure you have the following installed:

Git
Node.js
PostgreSQL
Java Development Kit (JDK 11 or later)
Maven or Gradle (depending on your build tool preference)
:checkered_flag: Starting
Follow these steps to set up and run the project:

1. Database Setup
Ensure PostgreSQL is running on your system.
Create databases for each microservice:
sql
Copy code
CREATE DATABASE api_gateway;
CREATE DATABASE auth_service;
CREATE DATABASE other_service; -- Repeat for each microservice
Update the application.properties or application.yml files in each microservice with the database connection details.
2. Start Backend Services
Navigate to each backend module (e.g., api-gateway, auth-service, etc.).
Build and start each service:
bash
Copy code
mvn clean install
mvn spring-boot:run
3. Start Eureka Server
Navigate to the eureka-server module.
Build and start the Eureka Server:
bash
Copy code
mvn clean install
mvn spring-boot:run
4. Start Frontend (Ionic)
Navigate to the frontend directory:

bash
Copy code
$ cd frontend
Install dependencies:

bash
Copy code
$ npm install
Start the Ionic development server:

bash
Copy code
$ ionic serve
Access the application at http://localhost:8100.

5. Verify the Setup
API Gateway: http://localhost:8080
Eureka Server: http://localhost:8761
Frontend: http://localhost:8100
:memo: License
This project is under license from MIT. For more details, see the LICENSE file.

Made with :heart: by <a href="https://github.com/{{YOUR_GITHUB_USERNAME}}" target="_blank">{{YOUR_NAME}}</a>

 

<a href="#top">Back to top</a>