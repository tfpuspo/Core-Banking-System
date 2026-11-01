
## Core Banking System — Spring Webflux, Microservices, GraphQL, gRPC, Kafka 


### A Core Banking System built on Spring Webflux, Microservices, GraphQL, gRPC, Kafka (Work-in-progress)

CBS Application Video Recording Link: https://drive.google.com/drive/folders/1PUa2bbuZyb0PKn6EBXFBtXdK4DFlnmks?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto

<div align="center">
  <h3>Part 1</h3>
  <a href="https://github.com/user-attachments/assets/e8d9de4e-56cd-4470-b595-c7c9ad51e22e">
    <img src="records/backend_team.png" width="700" height="400" alt="Part 1 - backend_team demo">
  </a>
</div>



<div align="center">
  <h3>Part 2</h3>
  <a href="https://github.com/user-attachments/assets/ddcce9cd-56c7-46c9-b07a-27d7015122fc">
    <img src="records/customer.png"
         width="700"
         height="400"
         alt="Part 2 - Customer demo">
  </a>
</div>


Tools & Technology:
 - Java 23, Spring Boot 3.5 (Spring WebFlux — reactive, non-blocking)
 - Spring Data R2DBC + PostgreSQL (isolated database per service)
 - GraphQL via Netflix DGS (auth-service)
 - gRPC + Protocol Buffers (internal service-to-service calls)
 - Apache Kafka (planned — Saga/Outbox pattern for transfers)
 - Kong API Gateway (planned)
 - Docker Compose (planned — local orchestration)
- React + TypeScript + Tailwind CSS (frontend)




Completed Features:
- Developed a microservice-based core banking platform using Spring WebFlux to serve both customers and backend
banking teams while gaining an in-depth understanding of core banking processes
- Implemented customer self-registration with account-based identity verification and Redis-backed SMS OTP, with
Kafka outbox notifications
- Designed and developed JWT based authentication with a dynamic RBAC (roles, permissions, per-user overrides and
permission-driven menus) managed by admins at runtime
- Implemented an all-or-nothing account-opening flow across three services using saga-style compensating rollback, so
a failure at any step leaves no partial data
- Implemented inter-service communication and event-driven processing using GraphQL, gRPC, WebClient, and
Apache Kafka with the Outbox Pattern
 

