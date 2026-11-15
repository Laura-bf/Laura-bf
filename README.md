<div align="center">

![Java](https://img.shields.io/badge/Java-11%2F17-ED8B00?logo=openjdk)
![SQL](https://img.shields.io/badge/SQL-MySQL-4479A1?logo=databricks)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-2.5–2.6-6DB33F?logo=springboot)
![Spring Batch](https://img.shields.io/badge/Spring%20Batch-Batch-6DB33F?logo=spring)
![Spring Data JPA](https://img.shields.io/badge/Spring%20Data%20JPA-JPA-6DB33F?logo=spring)
![Spring WebFlux](https://img.shields.io/badge/Spring%20WebFlux-Reactive-6DB33F?logo=spring)
![JUnit 5](https://img.shields.io/badge/JUnit-5-25A162?logo=junit5)
![Mockito](https://img.shields.io/badge/Mockito-Mocking-25A162?logo=mockito)
![Resilience4J](https://img.shields.io/badge/Resilience4J-Resilience-000000?logo=java)
![MySQL](https://img.shields.io/badge/MySQL-8-4479A1?logo=mysql)
![MongoDB](https://img.shields.io/badge/MongoDB-5-47A248?logo=mongodb)
![Maven](https://img.shields.io/badge/Maven-3-C71A36?logo=apachemaven)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?logo=docker)
![JWT](https://img.shields.io/badge/JWT-Auth-000000?logo=jsonwebtokens)
![Swagger](https://img.shields.io/badge/Swagger-3-85EA2D?logo=swagger)
![Astro](https://img.shields.io/badge/Astro-7-BC52EE?logo=astro)
![TypeScript](https://img.shields.io/badge/TypeScript-6-3178C6?logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4-06B6D4?logo=tailwindcss)
![Sanity](https://img.shields.io/badge/Sanity-Headless%20CMS-F03E2F?logo=sanity)
![Cloudflare Pages](https://img.shields.io/badge/Cloudflare%20Pages-Hosting-F38020?logo=cloudflarepages)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI-2088FF?logo=githubactions)

</div>

---

<div align="center">

<h1 style="margin-bottom: 0">Laura Benito Fernández</h1>
<h3 style="margin-top: 0">Backend Java Developer | Spring Boot & Enterprise Java</h3>

> Backend Java Developer with enterprise experience building REST APIs and batch processing systems. Currently strengthening my backend engineering foundations while exploring AI-assisted development workflows and developer tooling.

</div>



---

## Technical Stack & Focus

**Professional experience (Capgemini, client project):**

| Category                      | Technologies                                                 |
| :---------------------------- | :----------------------------------------------------------- |
| **Languages**                 | Java 17, SQL                                                 |
| **Frameworks**                | Spring Boot, Spring Batch, Spring Data JPA                   |
| **Testing & Quality**         | JUnit, Mockito, SonarQube, code coverage                     |
| **Tools & CI/CD**             | Git, Jenkins, Maven, Jira                                    |
| **Methodologies & Practices** | Agile, Clean Code, SOLID, refactoring, Pull Request workflow |

**Freelance client project (Clara Martínez Hernández website):**

| Category                      | Technologies                                                                 |
| :---------------------------- | :--------------------------------------------------------------------------- |
| **Languages**                 | TypeScript, HTML, CSS/SCSS                                                   |
| **Frameworks**                | Astro 7, Tailwind CSS 4                                                      |
| **CMS & Data**                | Sanity (headless CMS, GROQ, Portable Text)                                   |
| **Infrastructure & CI/CD**    | Cloudflare Pages, GitHub Actions                                             |
| **Quality**                   | Clean code (DRY, KISS, YAGNI), refactoring, WCAG 2.2 AA accessibility, `astro check`, Architecture Decision Records |
| **AI-assisted Workflow**      | Claude Code working under a written agent protocol (AGENTS.md + skills)      |

**Personal & collaborative projects (bootcamp portfolio, BusinessAssistantBCN, backendDevTest):**

| Category                 | Technologies                                                                                                            |
| :----------------------- | :---------------------------------------------------------------------------------------------------------------------- |
| **Languages**            | Java 11/17, SQL, Bash                                                                                                   |
| **Frameworks**           | Spring Boot, Spring Data JPA, Spring WebFlux                                                                            |
| **Testing & Resilience** | JUnit 5, Mockito, Resilience4J                                                                                          |
| **Databases**            | MySQL, MongoDB, H2                                                                                                      |
| **Developer Tools**      | Git, Maven, Gradle, Docker, Linux, Shell scripting                                                                      |
| **Currently Exploring**  | AI-assisted Development, LLM Integration, Prompt Engineering, RAG, Agentic AI Engineering, MCP, Spec-Driven Development |

---

## Featured Projects

>[!NOTE]
>For detailed project breakdowns, architecture decisions, and learning outcomes **[View Full Portfolio →](https://github.com/Laura-bf/Laura-bf/blob/main/Portfolio.md)**

### [Clara Martínez Hernández — Portfolio Website](https://github.com/cvclaramh-oss/clara-martinez-website)

> **Role:** Sole developer (design & development) | **Context:** Freelance client project (2 weeks, September 2026; pre-launch)

A bilingual (Catalan/Spanish) static website for a social educator and trainer, with all content editable by the client in a headless CMS. Accessibility-first (WCAG 2.2 AA).

- Modeled the content in **Sanity** with a single document type and schema validations that keep the editor from breaking the site: slugs locked after publishing, link-or-download buttons, required alt text, bilingual tag documents.
- Built a **single `getStaticPaths` router** that generates every page in both languages with translated URLs, plus a typed i18n dictionary checked at build time.
- Implemented a **design system on CSS tokens** with `light-dark()` dark mode and a fluid type and spacing scale, on top of an accessible Astro starter.
- Delivered through **small PRs with GitHub Actions CI** and Cloudflare Pages previews, documenting decisions in **24 ADRs**; AI-assisted development (Claude Code) under a written agent protocol, with design decisions kept human.
- _Stack: Astro 7, TypeScript, Tailwind CSS 4, SCSS, Sanity 6 (GROQ), Cloudflare Pages, GitHub Actions, Web3Forms._

### [BusinessAssistantBCN - Backend](https://github.com/IT-Academy-BCN/BusinessAssistantBCN-backend)

> **Role:** Primary Contributor (Opendata Module) | **Context:** Collaborative project (23 contributors)

A Spring Boot microservices ecosystem powering a business-assistant tool for entrepreneurs, aggregating public open-data sources.

- Designed a layered service proxying and normalizing Barcelona open-data datasets under a uniform, paginated API.
- Implemented resilient communication using **Resilience4J `@CircuitBreaker`** to prevent downstream API outages from degrading availability.
- Used **Spring WebFlux (Mono/Flux)** with non-blocking WebClient for data aggregation workflows.
- _Stack: Java 17, Spring Boot, Spring WebFlux, Resilience4J, Docker, JUnit 5, Trello._

### [ITAcademy_Java](https://github.com/Laura-bf/ITAcademy_Java)

> **Context:** 5-month intensive bootcamp portfolio (Barcelona, 2021)

A comprehensive showcase of 36 backend Java projects progressing from console fundamentals to enterprise-level Spring Boot microservices with JWT authentication, dual persistence (JPA + MongoDB), and comprehensive testing.

- Built a **growth-driven portfolio** spanning 5 phases: Foundations → Databases → OOP & Patterns → Concurrency → Spring Boot REST APIs
- Implemented **JWT authentication from scratch** with custom filters, token utilities, and stateless session management in [S502.DiceGame](https://github.com/Laura-bf/ITAcademy_Java/tree/master/S502.DiceGame.Nivel3)
- Designed **dual persistence architecture** operating over both JPA (MySQL) and MongoDB via Spring profiles ([S502.DiceGame](https://github.com/Laura-bf/ITAcademy_Java/tree/master/S502.DiceGame.Nivel3))
- Applied **design patterns** in practice, not just labeled: Factory (M6), Command (M11), MVC (M8/M9/M11), Repository (M8/S4/S5), DTO (M8/S502)
- Developed **37+ unit/integration tests** covering controller, service, repository, and DTO layers using JUnit 5, Mockito, and Spring Boot Test.
- Created **Swagger/OpenAPI documentation** for all Spring Boot REST endpoints (S402, S502)
- **Final Project:** [S502.DiceGame](https://github.com/Laura-bf/ITAcademy_Java/tree/master/S502.DiceGame.Nivel3)
- _Stack: Java 11/17, Spring Boot 2.5-2.6, JPA/Hibernate, Thymeleaf, MySQL, H2, MongoDB, Swagger/OpenAPI 3, JWT, JUnit 5, Mockito, Postman, Java Swing_

### [backendDevTest](https://github.com/Laura-bf/backendDevTest)

> **Context:** Technical take-home challenge

A reactive product aggregation service consuming multiple upstream APIs concurrently, built within a provided benchmarking environment (Docker + k6 + InfluxDB + Grafana) to validate performance under concurrent load.

- Exposed a unified REST endpoint that concurrently queries separate upstream services to stream aggregated data contracts.
- Used reactive WebClient to call the provided upstream APIs efficiently, built with focus on the evaluation criteria: code clarity, performance, and resilience under concurrent load.
- _Stack: Java 17, Spring Boot 2.6, Spring WebFlux, WebClient, Docker._

---

## Professional Trajectory

- **Freelance Web Project (September 2026, 2 weeks):** Designed and built a bilingual client website end to end on a stack entirely new to me (TypeScript, Astro, Sanity) — content model, static architecture, accessibility and deployment — working in small reviewed PRs with CI and documenting every architectural decision as an ADR.
- **Enterprise Experience (1.5+ Years):** Developed REST APIs and automated batch processing (**Spring Batch**) within a layered architecture closely aligned with Hexagonal principles, on top of a client-owned corporate framework. Executed deployments to testing environments via **Jenkins** pipelines, actively participated in the Pull Request review process, and handled client-facing technical discussions.
- **Intensive Foundations:** 5-month full-time Java Backend Track at IT Academy Barcelona (2021), covering core concurrency through secure REST microservices with **JWT** authentication.

> [!NOTE]
> **Current Focus & Upskilling**
> After a professional pause, I'm reinforcing core Java fundamentals and algorithmic problem-solving for technical assessments, with a growing focus on system architecture (Hexagonal Architecture, distributed systems) and Agentic AI engineering (RAG Pipelines, MCP, Spec-Driven Development).

---

## Connect with Me

- **Email:** [laura.dev.bcn@gmail.com](mailto:laura.dev.bcn@gmail.com)
- **LinkedIn:** [linkedin.com/in/laura-benito-fernández](https://www.linkedin.com/in/laura-benito-fernández/)
