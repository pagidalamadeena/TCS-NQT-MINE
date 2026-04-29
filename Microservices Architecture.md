**Microservices Architecture:-**





\## 1. Fundamentals of Microservices Architecture



&#x20; Definition of Microservices



\*   Architectural style where application is split into  small, independent services

\*   Each service focuses on a  single business capability

\*   Services communicate over  network (HTTP/messaging)



&#x20;



&#x20; Characteristics of Microservices



\*   Independently deployable

\*   Loosely coupled

\*   Technology‑agnostic

\*   Own database per service

\*   Decentralized governance



&#x20;



&#x20; Monolithic vs Microservices Architecture



\*    Monolithic :

&#x20;   \*   Single codebase

&#x20;   \*   Tightly coupled components

&#x20;   \*   Hard to scale and deploy

\*    Microservices :

&#x20;   \*   Multiple small services

&#x20;   \*   Independent scaling and deployment

&#x20;   \*   Better fault isolation



&#x20;



&#x20; Benefits of Microservices



\*    Scalability :

&#x20;   \*   Scale individual services

\*    Modularity :

&#x20;   \*   Easy to develop and maintain

\*    Fault Isolation :

&#x20;   \*   Failure in one service doesn’t crash whole system

\*    Independent Deployment :

&#x20;   \*   Faster releases



&#x20;



&#x20; Key Principles of Microservices



&#x20;# Decoupling of Services



\*   Services are independent

\*   Minimal shared dependencies

\*   Changes in one service don’t affect others



&#x20;



&#x20;# API‑Based Communication



\*   Services communicate via APIs

\*   Usually REST or messaging

\*   Clear service contracts



&#x20;



&#x20;# Data Decentralization



\*   Each service owns its data

\*   No shared database

\*   Improves autonomy and scalability



&#x20;



&#x20;# Domain‑Driven Design (DDD) Basics



\*   Business logic divided into domains

\*   Each microservice aligns with a  bounded context

\*   Focus on business requirements



&#x20;



\## 2. Designing Microservices with ASP.NET Core



&#x20; Setting up ASP.NET Core for Microservices



\*   Use  ASP.NET Core Web API

\*   Lightweight and cross‑platform

\*   Supports containerization and cloud deployment



&#x20;



&#x20; Creating Modular Services



\*   Separate services like:

&#x20;   \*   Product Service

&#x20;   \*   Order Service

&#x20;   \*   User Service

\*   Each service has its own project



&#x20;



&#x20; Service Boundaries and Responsibilities



\*   Each service handles  one business capability

\*   No overlapping responsibilities

\*   Clear ownership of logic and data



&#x20;



&#x20; Dependency Injection and Configuration Management



\*   Built‑in DI container

\*   Services registered in `Program.cs`

\*   Configuration via `appsettings.json` and environment variables



&#x20;



&#x20; Using Entity Framework Core in Microservices



\*   EF Core used per service

\*   Separate DbContext per microservice

\*   Code‑First approach common



&#x20;



&#x20; Implementing RESTful APIs



\*   Controllers with HTTP verbs

\*   Stateless communication

\*   JSON‑based request/response



&#x20;



\## 3. Inter‑Service Communication



&#x20; REST API Communication



\*   Synchronous communication

\*   Uses HTTP/HTTPS

\*   Simple and widely used



&#x20;



&#x20; HTTP Clients in ASP.NET Core



\*   Use  HttpClientFactory

\*   Manages connection pooling

\*   Prevents socket exhaustion



&#x20;



&#x20; API Gateway Basics (Ocelot)



\*   Single entry point for clients

\*   Routes requests to microservices

\*   Handles authentication, logging, rate limiting



&#x20;



&#x20; Service Discovery (Intro)



\*   Automatically finds service locations

\*   Examples:

&#x20;   \*   Consul

&#x20;   \*   Eureka

\*   Useful in dynamic environments



&#x20;



&#x20; Message‑Based Communication



\*   Asynchronous communication

\*   Loose coupling

\*   Improves resilience



&#x20;



&#x20; Introduction to Asynchronous Messaging



\*   Producer sends message

\*   Consumer processes message later

\*   No direct dependency



&#x20;



&#x20; Event‑Driven Architecture



\*   Services publish events

\*   Other services subscribe

\*   Promotes scalability and decoupling



&#x20;



&#x20; Using RabbitMQ with ASP.NET Core



\*   Message broker

\*   Supports queues and exchanges

\*   Reliable asynchronous messaging



&#x20;



&#x20; Using Azure Service Bus



\*   Cloud‑native messaging service

\*   Supports queues and topics

\*   Used in Azure‑based microservices



&#x20;



&#x20; Publishing and Subscribing to Events



\*   Publisher emits event

\*   Subscribers react to event

\*   No direct service‑to‑service call



&#x20;



\## 4. Microservices Deployment and Scalability



&#x20; Containerization with Docker



\*   Each service packaged as a container

\*   Ensures consistent runtime environment

\*   Simplifies deployment



&#x20;



&#x20; Independent Deployment of Services



\*   Deploy services separately

\*   No need to redeploy entire system

\*   Enables continuous delivery



&#x20;



&#x20; Orchestration Basics (Kubernetes Overview)



\*   Manages containers

\*   Handles scaling, load balancing, and failures

\*   Automates deployment and monitoring



&#x20;



&#x20; Scaling Services Individually



\*   Scale only high‑load services

\*   Optimizes resource usage

\*   Improves performance



&#x20;



&#x20; Health Checks



\*   Endpoint to verify service health

\*   Used by orchestrators

\*   Detects unhealthy services



&#x20;



&#x20; Resilience Patterns



\*    Retry :

&#x20;   \*   Automatically retry failed requests

\*    Circuit Breaker :

&#x20;   \*   Stops calls to failing service

&#x20;   \*   Prevents cascading failures



&#x20;

