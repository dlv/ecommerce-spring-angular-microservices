 # ecommerce-spring-angular-microservices - Educational Project

 ## 🎯 Project Overview

 Full-stack ecommerce platform using Spring Boot microservices for the backend
and Angular for the frontend. This repository demonstrates microservices
architecture, distributed systems patterns, and modern development practices
for both Java (Spring Boot) and Angular applications.

## 📚 Learning Objectives

- Understand microservices design patterns
- Service discovery and communication
- Distributed data management and consistency patterns
- Event-driven architecture and messaging
- API gateway and routing patterns
- Containerization and orchestration (Docker, Kubernetes)
- Build integration between Angular frontend and Spring Boot backend

## 🏗️ Core Microservices

### User Service
- User registration and authentication
- Profile management
- JWT token generation and security

### Product Service
- Product catalog management
- Inventory tracking
- Search and filtering

### Order Service
- Order creation and lifecycle management
- Order status tracking and history
- Shopping cart functionality

### Payment Service
- Simulated payment processing
- Transaction history
- Multiple payment method hooks

### Notification Service
- Email notifications for orders and events
- Order confirmations and promotional messages

## 🛠️ Infrastructure Components

- Service Discovery: Eureka (service registration)
- API Gateway: Spring Cloud Gateway for routing and filters
- Configuration: Spring Cloud Config Server for centralized configuration
- Monitoring: Spring Boot Actuator, Sleuth/Zipkin for tracing
- Logging & Metrics: centralized logging and metrics collection

## 📊 Data Management

- Each microservice owns its own database
- Recommended: PostgreSQL for transactional data
- Redis for caching and session/fast lookups
- Message broker for events: RabbitMQ or Kafka

## 🚀 Advanced Features

- Circuit breaker patterns (Hystrix or Resilience4j)
- Asynchronous messaging with RabbitMQ/Kafka
- Docker containerization and Kubernetes deployment manifests
- CI/CD pipeline examples (GitHub Actions / Jenkins)

## 🌐 Angular Frontend

### Core Features
- Product browsing and search
- Shopping cart and checkout flow
- User authentication and profile management
- Order history and tracking

### Technical Implementation
- Angular with standalone components
- Angular Material for UI components
- Reactive forms and validation
- State management (Signals or other patterns)
- JWT authentication handling with HTTP interceptors

## 🧰 Technology Stack

### Backend
- Java 21+
- Spring Boot 3.x
- Spring Cloud components (Eureka, Gateway, Config)
- Spring Security for auth
- PostgreSQL, Redis
- RabbitMQ / Kafka
- Docker & Kubernetes

### Frontend
- Angular 20+
- TypeScript
- Angular Material

## ⚙️ Progressive Implementation Plan

1. Phase 1: Basic CRUD services (User, Product, Order) + Angular skeleton
2. Phase 2: Service communication, API Gateway, and frontend integration
3. Phase 3: Event-driven patterns, messaging, and async flows
4. Phase 4: Monitoring, observability, and containerized deployment
5. Phase 5: Scalability, performance tuning, and production hardening

## 🏁 Getting Started (development)

1. Clone the repo
2. Start required services (PostgreSQL, Redis, RabbitMQ)
3. Build and run microservices (Maven/Gradle)
4. Start Angular frontend (Angular CLI)

Example (Linux/macOS / adapt commands for Windows):

```bash
# backend (each microservice)
./mvnw spring-boot:run -pl user-service
./mvnw spring-boot:run -pl product-service

# frontend
cd frontend
npm install
ng serve
```

## Contributing

Contributions are welcome. Open issues or PRs with proposed changes,
architecture improvements, or documentation updates.

## License

This project is provided for educational purposes. Check the original
repository for license details.
