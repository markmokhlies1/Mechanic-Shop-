# Mechanic Shop Management System
A production‑ready, full‑stack mechanic shop management system built with ASP.NET Core, Blazor, and SQL Server, following Clean Architecture, DDD, and modern backend engineering best practices.

This project simulates a real automotive workshop environment and demonstrates how to build secure, scalable, and maintainable backend systems used in real‑world applications



# Why This Project Matters
This is not a CRUD demo.

It demonstrates how a professional backend system is designed, secured, tested, deployed, and maintained, including:
```
Clean Architecture with strict boundaries.

JWT‑based authentication & role‑based authorization

Domain Events for business workflows

Background jobs for asynchronous processing

Caching for performance optimization

Dockerized services & CI/CD pipeline

Comprehensive unit testing across all layers
```

# What This Project Demonstrates
```
Clean Architecture & SOLID principles

 Domain‑Driven Design (DDD)

 CQRS (Commands & Queries separation)

 Repository & Unit of Work patterns

 Result Pattern for explicit success/failure handling

 JWT Authentication & Role‑Based Access Control (RBAC)

 Domain Events & asynchronous messaging

 Background job processing

 Caching strategies

 RESTful API design

 Docker & CI/CD automation

 Enterprise‑level testing strategy
```

# Architecture Overview
The project strictly follows Clean Architecture, keeping business rules independent from frameworks and infrastructure.
```text

├── Domain
│   ├── Entities
│   ├── ValueObjects
│   ├── DomainEvents
│   ├── ResultPattern
│   └── Interfaces
|
│
├── Application
│   ├── UseCases (CQRS)
│   ├── Commands & Queries
│   ├── DTOs
│   ├── Validators
│   ├── Authorization Policies
│   └── EventHandlers
│
├── Infrastructure
│   ├── Persistence (EF Core / SQL Server)
│   ├── Repositories & UnitOfWork
│   ├── Identity & JWT
│   ├── Background Jobs
│   ├── Caching (In‑Memory / Distributed)
│   ├── SMS Notification Service
│   └── Logging & Monitoring
│
├── Presentation
│   ├── ASP.NET Core REST API
│   └── Blazor Frontend
│
├── Tests
│   ├── Domain.Tests
│   ├── Application.Tests
│   └── Infrastructure.Tests
```

# Technology Stack
```md
Backend


C#
ASP.NET Core
REST API
Entity Framework Core
SQL Server
MediatR
FluentValidation
JWT Authentication
Role‑Based Authorization
Result Pattern
Domain Events


Frontend

Blazor

Infrastructure & DevOps

Background Jobs (e.g. hosted services / Hangfire‑style processing)
Caching (In‑Memory / Distributed)
Docker & Docker Compose
CI/CD Pipeline (Build, Test, Lint)

Testing & Tooling

xUnit / NUnit
Moq
Swagger / OpenAPI
Global Exception Handling
Structured Logging
```
#  Security
```
JWT‑based authentication
Role‑based authorization 
Secure API endpoints using authorization policies
Token expiration and refresh handling
```
# Performance & Caching
```
Frequently accessed data cached to reduce database load
Cache invalidation handled on state changes
Improves response times and system scalability
```
# Testing Strategy
```
Unit tests for every Clean Architecture layer
 Domain logic tested independently
Application use cases tested with mocks
Infrastructure components tested separately
Tests executed automatically in CI pipeline
```
# Docker & CI/CD
```
Application containerized using Docker
Environment‑specific configurations supported
CI/CD pipeline automatically:
Builds the solution
Runs unit tests
Validates code quality
```











