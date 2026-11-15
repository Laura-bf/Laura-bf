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
![Astro](https://img.shields.io/badge/Astro-7-BC52EE?logo=astro)
![TypeScript](https://img.shields.io/badge/TypeScript-6-3178C6?logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4-06B6D4?logo=tailwindcss)
![Sanity](https://img.shields.io/badge/Sanity-Headless%20CMS-F03E2F?logo=sanity)
![Cloudflare Pages](https://img.shields.io/badge/Cloudflare%20Pages-Hosting-F38020?logo=cloudflarepages)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI-2088FF?logo=githubactions)


<h1>Laura Benito Fernández</h1>

<h2>Project Portfolio</h2>

<h3>A curated collection of projects: a freelance client website and backend Java work demonstrating progressive growth from fundamentals to enterprise-level architecture.</h3>

</div>

<div align="center">

---

<h3> Index </h3>

[Clara Martínez Website](#clara-martínez-hernández--portfolio-website)                             
[ITAcademy_Java](#itacademy_java)                             
[BusinessAssistantBCN](#businessassistantbcn---backend)       
[backendDevTest](#backenddevtest)      

</div>
                
---
## [Clara Martínez Hernández — Portfolio Website](https://github.com/cvclaramh-oss/clara-martinez-website)

  > **Role:** Sole developer (design & development) | **Context:** Freelance client project (2 weeks, September 2026; pre-launch)

  > **Stack:** Astro 7, TypeScript, Tailwind CSS 4, SCSS, Sanity 6 (GROQ, Portable Text), Cloudflare Pages, GitHub Actions, Web3Forms

A bilingual (Catalan/Spanish) static website for a social educator and trainer. Every catalog item, the bio and the site settings are edited by the client in Sanity Studio; the site is rebuilt from that content into 118 static pages. Accessibility-first (WCAG 2.2 AA).

### What This Demonstrates

**Content Modeling for a Non-Technical Editor:**
- One `catalogItem` document type covers four sections (projects, materials, trainings, workshops), so one card template and one detail template serve the whole site
- Schema validations prevent broken content: slugs locked once published (shared URLs keep working), video as URL *or* file, button as link *or* download, required alt text, safe link schemes only
- Tags migrated from free text to bilingual documents, removing duplicates and enabling a tag filter in both languages ([ADR 0019](https://github.com/cvclaramh-oss/clara-martinez-website/blob/dev/docs/adr/0019-etiquetes-com-a-document.md))
- Studio in the editor's language, with help text, a curated desk structure and free "sections" for new information without code changes

**Bilingual Static Architecture:**
- A single `getStaticPaths` router generates static pages, paginated listings, tag pages and item pages in both languages from a table of translated route segments
- Typed i18n dictionary: `t()` only accepts existing keys, so a missing translation is a type error caught by `astro check`
- Content fetched at build time in batches; the language switcher resolves the translated slug of each item through the CMS

**Accessibility & Design System:**
- WCAG 2.2 AA baseline: semantic HTML, skip link, keyboard-friendly menus, visible focus, contrast checked in both themes
- Design tokens in CSS custom properties with `light-dark()` for dark mode, fluid type and spacing scale (Utopia), self-hosted fonts

**Code Quality & Refactoring:**
- Clear principles written down from day one: DRY, KISS and YAGNI, consistent naming conventions, configuration through environment variables (12-Factor), and no silent error handling
- The final iteration was devoted to refactoring and cleanup: a full audit of the codebase against the starter, shared components instead of duplicated markup, custom Tailwind utilities, link styles moved to the base layer removing every `!important`, and dead starter code deleted
- Refactors verified with automated before/after style comparisons on key pages, so cleanup never changed the design by accident
- Type safety end to end: typed translation keys and CMS query results, with `astro check` passing clean in CI

**Engineering Practice:**
- Small pull requests into `dev` with GitHub Actions CI (`astro check` + build) and a Cloudflare Pages preview per branch, protected with Cloudflare Access
- 24 Architecture Decision Records, including the decisions that were later superseded and why
- Two-level documentation: ADRs for the stable decisions, and a private session journal for the process, which also serves as the agent's memory between sessions, resumed through a custom `/retomar` command
- Client handover: a 13-page guide written for a non-technical client — a task-based walkthrough of the Studio with screenshots, what's done and what's still pending (grouped by what unblocks each step), account ownership and running costs. Kept private as a client deliverable.
- AI-assisted, human-led: development with Claude Code under a written protocol ([AGENTS.md](https://github.com/cvclaramh-oss/clara-martinez-website/blob/dev/AGENTS.md)) — explain before changing, ask before touching configuration, no commits without approval — with project knowledge in versioned skills

### Outcome & Learning

**A First, End to End:** In two weeks I designed and built my first production website on a stack that was entirely new to me (TypeScript, Astro, Sanity, Tailwind CSS 4 and Cloudflare Pages), coming from a Java backend background, working solo across every layer: content model, architecture, design system, accessibility, CI/CD and documentation.

**AI Raised the Ceiling, and the Workload:** Working with an AI agent made a far more ambitious first project possible: without it I would have shipped something simpler, likely a template. But higher speed also expands what feels achievable, and I chose to stay in control of every piece rather than accept code I didn't understand. That meant reviewing, questioning and documenting at the agent's pace, across a much larger scope: harder than building without AI, and the reason the result is production-quality. Every design and architecture decision stayed mine, recorded in 24 ADRs.

**Fast for Visitors, Simple for the Client:** The result is a fully static site, plain HTML served from Cloudflare's network with about 16 KB of JavaScript in total and no client-side framework, and an editing experience reduced to what the client actually needs: fill in a form in her own language, publish, done.

>[!TIP]
>**Start Here:** [README](https://github.com/cvclaramh-oss/clara-martinez-website#readme), [Content model](https://github.com/cvclaramh-oss/clara-martinez-website/blob/dev/studio/CONTENT-MODEL.md) or [Architecture Decision Records](https://github.com/cvclaramh-oss/clara-martinez-website/tree/dev/docs/adr)

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
| Clara Martínez Website | Freelance client project | Content modeling, i18n, accessibility, CI/CD | 118 static pages, 2 languages, 24 ADRs |
| ITAcademy_Java | Bootcamp Portfolio | Full Java stack, design patterns, testing | 36 projects, 5 phases |
| BusinessAssistantBCN | Professional | Microservices, resilience, team collaboration | 23 contributors, production |
| backendDevTest | Take-home | Reactive programming, performance | Single service, benchmarked |

---

## Connect

- **LinkedIn:** [linkedin.com/in/laura-benito-fernández](https://www.linkedin.com/in/laura-benito-fernández/)
- **Email:** [laura.dev.bcn@gmail.com](mailto:laura.dev.bcn@gmail.com)
