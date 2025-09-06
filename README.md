# Patient Management System

A system for patient administration built with a production-ready microservices architecture.
Currently, the core `patient-service` is implemented, providing fundamental CRUD operations.

## Current Features

- **RESTful Microservice**: A robust `patient-service` built with Java and Spring Boot.
- **Data Persistence**: Uses PostgreSQL for production environments and H2 for local development and
  testing.
- **API Documentation**: Integrated Swagger UI for easy exploration and testing of the REST API
  endpoints.
- **Containerized**: Fully containerized with Docker for consistent development and deployment
  environments.

## Tech Stack (Current)

- **Backend**: Java 21, Spring Boot
- **API**: REST
- **Database**: PostgreSQL, H2 (for local development)
- **Containerization**: Docker

## Prerequisites

Ensure you have the following installed:

- Java Development Kit (JDK 21 LTS)
- Docker

## Running Locally

1. **Clone the repository**:
   ```bash
   git clone https://github.com/josealvarezz/patient-management
   cd patient-management
   ```

2. **Navigate to the service directory**:
   ```bash
   cd patient-service
   ```

3. **Run with Docker**:
   The project is configured to run easily using Docker. Make sure Docker is running on your machine
   and then execute the necessary commands to build and run the container (details to be added).

   *(Note: Further instructions on running with Docker Compose or individual Docker commands will be
   added here.)*

---

## Project Roadmap & Future Features

This project is under active development. The vision is to expand it into a complete, event-driven
microservices ecosystem. Here are the features planned for the future:

- **API Gateway**: Implement Spring Cloud Gateway to act as a single entry point for all services,
  handling routing and load balancing.
- **gRPC Communication**: Introduce gRPC for efficient, high-performance inter-service communication
  alongside REST.
- **Secure Authentication**: Develop a dedicated authentication service to secure the APIs using JWT
  Bearer tokens.
- **Event-Driven Architecture**: Integrate Apache Kafka to enable asynchronous messaging between
  services, making the system more resilient and scalable.
- **Cloud Deployment**: Create infrastructure scripts to deploy the entire system to an AWS
  environment simulated with **LocalStack**, including services like ECS, RDS, and MSK.
- **Comprehensive Testing**: Expand the automated testing suite to include integration and
  end-to-end tests for the entire microservices landscape.