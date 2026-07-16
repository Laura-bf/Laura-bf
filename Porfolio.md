<div align="center">

![Java](https://img.shields.io/badge/Java-11%2F17-ED8B00?logo=openjdk)
![SQL](https://img.shields.io/badge/SQL-MySQL-4479A1?logo=databricks)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-2.5–2.6-6DB33F?logo=springboot)
![Spring Data JPA](https://img.shields.io/badge/Spring%20Data%20JPA-JPA-6DB33F?logo=spring)
![Spring WebFlux](https://img.shields.io/badge/Spring%20WebFlux-Reactive-6DB33F?logo=spring)
![JUnit 5](https://img.shields.io/badge/JUnit-5-25A162?logo=junit5)
![Mockito](https://img.shields.io/badge/Mockito-Mocking-25A162?logo=mockito)
![Resilience4J](https://img.shields.io/badge/Resilience4J-Resilience-000000?logo=java)
![MySQL](https://img.shields.io/badge/MySQL-8-4479A1?logo=mysql)
![MongoDB](https://img.shields.io/badge/MongoDB-5-47A248?logo=mongodb)
![Maven](https://img.shields.io/badge/Maven-3-C71A36?logo=apachemaven)
![Gradle](https://img.shields.io/badge/Gradle-7-02303A?logo=gradle)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?logo=docker)
![JWT](https://img.shields.io/badge/JWT-Auth-000000?logo=jsonwebtokens)
![Swagger](https://img.shields.io/badge/Swagger-3-85EA2D?logo=swagger)


<h1>Laura Benito Fernández</h1>

<h2>Project Portfolio</h2>

<h3>A curated collection of backend Java projects demonstrating progressive growth from fundamentals to enterprise-level architecture.</h3>

</div>

<div align="center">

---

<h3> Index </h3>

[ITAcademy_Java](#itacademy_java)                             
[BusinessAssistantBCN](#businessassistantbcn---backend)       
[backendDevTest](#backenddevtest)      

</div>
                
---
## [ITAcademy_Java](https://github.com/Laura-bf/ITAcademy_Java)

  > **Context:** 5-month intensive bootcamp portfolio (Barcelona, 2021)

  > **Stack:** Java 11/17, Spring Boot 2.5-2.6, JPA/Hibernate, MySQL, MongoDB, Swagger/OpenAPI 3, JWT, JUnit 5, Mockito

A comprehensive showcase of 36 backend Java projects progressing from console fundamentals to enterprise-level Spring Boot microservices with JWT authentication, dual persistence (JPA + MongoDB), and comprehensive testing.

### What This Demonstrates

**Growth Trajectory:** The repository traces a complete learning arc from zero Java knowledge to production-grade Spring Boot microservices. Each phase builds on previous skills:

| Phase | Focus | Key Takeaways |
|-------|-------|---------------|
| **Phase 1: Foundations** (M1-M4) | Variables, arrays, loops, console I/O, custom exceptions | Core Java fundamentals, error handling patterns |
| **Phase 2: Databases** (M5, S2) | MySQL schemas, SQL queries, MongoDB document models | Relational vs. document database design |
| **Phase 3: OOP & Patterns** (M6-M8, M11) | Inheritance, polymorphism, MVC, Factory, Command patterns | Clean architecture, design pattern application |
| **Phase 4: Concurrency** (M9-M10) | Multi-threaded simulation, Lambdas, Streams API | Parallel execution, functional programming |
| **Phase 5: Spring Boot** (S4-S5) | REST APIs, JPA, Swagger, JWT security, testing | Enterprise Java, production-ready concerns |

**Technical Highlights:**

- **JWT Authentication from Scratch:** Implemented custom filters, token utilities, and stateless session management in S502.DiceGame
- **Dual Persistence Architecture:** Same service layer operating over both JPA (MySQL) and MongoDB via Spring profiles
- **Design Patterns in Production:** Factory (M6), Command (M11), MVC (M8/M9/M11), Repository (M8/S4/S5), DTO (M8/S502)
- **Comprehensive Testing:** 37+ unit/integration tests covering controller, service, repository, and DTO layers using JUnit 5, Mockito, and Spring Boot Test

>[!TIP]
>**Start Here:** [Final Project - S502.DiceGame](https://github.com/Laura-bf/ITAcademy_Java/tree/master/S502.DiceGame.Nivel3) or [S501.SpringRESTapi](https://github.com/Laura-bf/ITAcademy_Java/tree/master/S501.SpringRESTapi.nivel3)

---

## [BusinessAssistantBCN - Backend](https://github.com/IT-Academy-BCN/BusinessAssistantBCN-backend)

> **Role:** Primary Contributor (Opendata Module) | **Context:** Collaborative project (23 contributors)

> **Stack:** Java 17, Spring Boot, Spring WebFlux, Resilience4J, Docker, JUnit 5

A Spring Boot microservices ecosystem powering a business-assistant tool for entrepreneurs, aggregating public open-data sources.

### What This Demonstrates

**Professional Collaboration:** Contributed to a multi-developer codebase following enterprise practices (Gitflow, code reviews, CI/CD).

**Resilient Architecture:**
- Designed a layered service proxying and normalizing Barcelona open-data datasets under a uniform, paginated API
- Implemented resilient communication using **Resilience4J `@CircuitBreaker`** to prevent downstream API outages from degrading availability
- Used **Spring WebFlux (Mono/Flux)** with non-blocking WebClient for data aggregation workflows


---

## [backendDevTest](https://github.com/Laura-bf/backendDevTest)

> **Context:** Technical take-home challenge

> **Stack:** Java 17, Spring Boot 2.6, Spring WebFlux, WebClient, Docker

A reactive product aggregation service consuming multiple upstream APIs concurrently, built within a provided benchmarking environment (Docker + k6 + InfluxDB + Grafana) to validate performance under concurrent load.

### What This Demonstrates

**Reactive Programming:** Built for performance under concurrent load, demonstrating understanding of non-blocking I/O and reactive streams.

**Key Implementation:**
- Exposed a unified REST endpoint that concurrently queries separate upstream services to stream aggregated data contracts
- Used reactive WebClient to call the provided upstream APIs efficiently, built with focus on the evaluation criteria: code clarity, performance, and resilience under concurrent load


---

## Summary

| Project | Type | Key Skills | Scale |
|---------|------|------------|-------|
| ITAcademy_Java | Bootcamp Portfolio | Full Java stack, design patterns, testing | 36 projects, 5 phases |
| BusinessAssistantBCN | Professional | Microservices, resilience, team collaboration | 23 contributors, production |
| backendDevTest | Take-home | Reactive programming, performance | Single service, benchmarked |

---

## Connect

- **LinkedIn:** [linkedin.com/in/laura-benito-fernández](https://www.linkedin.com/in/laura-benito-fernández/)
- **Email:** [laura.dev.bcn@gmail.com](mailto:laura.dev.bcn@gmail.com)
