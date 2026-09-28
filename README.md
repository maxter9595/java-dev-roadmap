# Roadmap Java-разработчика

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Roadmap для системного изучения **Backend на Java/Spring Boot** и **Frontend** с выходом на уровень **Fullstack**.

<img src="assets/images/silicon-valley-gilfoyle.png" alt="It's coding time" width="100%">

## Структура Roadmap

```
Backend
↗ Language Fundamentals and Tools
↗ Backend Development 
↗ Architecture and Infrastructure
↗ Distributed Systems

Frontend
↗ Fundamentals
↗ React Development
↗ Architecture & Security
↗ Testing & Deployment

Backend → Fullstack Capstone ← Frontend

Parallel Career Track
↗ English
↗ Agile / Scrum / Kanban
↗ CV / Portfolio
↗ Interview Preparation
```

## Как пользоваться roadmap

1. Начни с [чек-листа навыков](#чек-лист-навыков-java-backend--fullstack-разработчика).
2. Отметь для каждой строки статус: не знаю / плаваю / знаю уверенно.
3. Работай сначала только с P0, пока не закроешь его полностью.
4. P1 добирай параллельно.
5. P2 — не раньше, чем закроешь P0 и большую часть P1.
6. Раз в 3–6 месяцев сверяйся с 20–30 вакансиями и корректируй приоритеты.
7. Для каждого раздела выполняй практику, не только читай теорию.

## Оглавление

### Backend

#### Основы языка и работы с инструментами

1. [Java](#1-java)
2. [Git / GitHub](#2-git--github)
3. [Сборка проектов: Maven и Gradle](#3-сборка-проектов-maven-и-gradle)
4. [Принципы и паттерны проектирования](#4-принципы-и-паттерны-проектирования)
5. [Алгоритмы и структуры данных](#5-алгоритмы-и-структуры-данных)

#### Backend-разработка

6. [Web и компьютерные сети](#6-web-и-компьютерные-сети)
7. [SQL / PostgreSQL](#7-sql--postgresql)
8. [Spring / Spring Boot](#8-spring--spring-boot)
9. [Spring Security](#9-spring-security)
10. [Spring Testing](#10-spring-testing)

#### Архитектура и инфраструктура

11. [Backend-архитектура](#11-backend-архитектура)
12. [Linux](#12-linux)
13. [Docker + Docker Compose](#13-docker--docker-compose)
14. [CI/CD (GitHub Actions)](#14-cicd-github-actions)
15. [Инфраструктурные компоненты](#15-инфраструктурные-компоненты)
16. [Observability basics](#16-observability-basics)
17. [Нагрузочное тестирование](#17-нагрузочное-тестирование)

#### Распределённые системы

18. [Cloud Basics](#18-cloud-basics)
19. [System Design (HLD)](#19-system-design-hld)
20. [Микросервисы и распределённые системы](#20-микросервисы-и-распределённые-системы)
21. [DevOps (Nginx, Kubernetes, Terraform)](#21-devops-nginx-kubernetes-terraform)

### Frontend

#### Основы Frontend

22. [HTML5 + CSS3](#22-html5--css3)
23. [JavaScript](#23-javascript)
24. [TypeScript](#24-typescript)

#### Разработка на React

25. [Frontend Build / Tooling](#25-frontend-build--tooling)
26. [React + Next.js](#26-react--nextjs)
27. [OpenAPI / Documentation / Contracts](#27-openapi--documentation--contracts)
28. [State Management + API Integration](#28-state-management--api-integration)

#### Архитектура и безопасность Frontend

29. [Архитектура фронтенд-приложений](#29-архитектура-фронтенд-приложений)
30. [Web Security](#30-web-security)
31. [WebSockets / SSE](#31-websockets--sse)

#### Тестирование и развёртывание Frontend

32. [Frontend Testing](#32-frontend-testing)
33. [Frontend CI/CD + Docker](#section-33)

### Fullstack Capstone
34. [Fullstack Capstone + Containerization + CI/CD](#34-fullstack-capstone--containerization--cicd)

### Карьера и поиск работы
35. [Английский язык](#35-английский-язык)
36. [Методологии разработки: Agile, Scrum, Kanban](#36-методологии-разработки-agile-scrum-kanban)
37. [Резюме, портфолио и собеседования](#37-резюме-портфолио-и-собеседования)

## Чек-лист навыков Java Backend / Fullstack-разработчика

**Легенда:**

- **P0** — обязательно для уверенной самостоятельной работы на соответствующем уровне.
- **P1** — желательно для усиления профиля и расширения зоны ответственности.
- **P2** — продвинутое углубление для Senior, DevOps, Fullstack и специализации.
- **Критерий готовности** — конкретный практический навык, по которому можно проверить готовность.

| # | Раздел | P0 — обязательно | P1 — желательно | P2 — позже | Критерий готовности |
|---|--------|------------------|-----------------|------------|---------------------|
| 1 | **Java** | OOP, Collections, Exceptions, Generics, Stream API, Optional, базовая многопоточность | JVM, JMM, GC базово, CompletableFuture, Virtual Threads, records, sealed, pattern matching | JIT, глубокий GC tuning, Structured Concurrency, JVM internals | Пишет, читает и объясняет современный Java-код; понимает race condition, deadlock, visibility; решает задачи на concurrency |
| 2 | **Git / GitHub** | commit, branch, merge, pull/push, PR, разрешение конфликтов | rebase, cherry-pick, reset/revert, tags, Conventional Commits | Git internals, advanced workflows | Работает в команде через PR, самостоятельно разрешает конфликты, ведёт ветки |
| 3 | **Maven / Gradle** | Maven lifecycle, dependencies, scopes, plugins, profiles, Wrapper | multi-module, dependencyManagement / BOM, Gradle обзорно | Сложные multi-module builds, custom plugins | Собирает, тестирует и упаковывает Java-проект без IDE; разбирает dependency:tree |
| 4 | **Design Principles & Patterns** | OOP, SOLID, composition over inheritance, основные GoF | GRASP, UML, refactoring, anti-patterns, распознавание в JDK/Spring | Глубокий DDD, архитектурные паттерны | Объясняет архитектурное решение, выбирает паттерн и аргументированно избегает лишнего |
| 5 | **Algorithms & Data Structures** | Big O, Collections, search, sorting, trees, graphs, BFS/DFS, basic DP | Dijkstra, greedy, sliding window, two pointers, prefix sums | Advanced DP, segment tree, Fenwick tree, вычислительная геометрия | Решает medium LeetCode, объясняет time/space complexity, сравнивает альтернативы |
| 6 | **Web & Networks** | HTTP, HTTPS, REST, headers, status codes, JSON, DNS, TCP/IP basics | HTTP/2, WebSockets, proxies, TLS details, Socket | Глубокие network internals | Объясняет полный путь HTTP-запроса, диагностирует типичные сетевые проблемы |
| 7 | **SQL / PostgreSQL** | CRUD, JOIN, GROUP BY, transactions, indexes, constraints, schema design | CTE, window functions, EXPLAIN ANALYZE, MVCC, locks, isolation levels | Partitioning, replication, глубокая оптимизация | Проектирует БД, пишет сложный SQL, находит причину медленного запроса через EXPLAIN |
| 8 | **Spring / Spring Boot** | DI/IoC, REST, MVC, DTO, validation, exception handling, JPA, @Transactional, configuration | Hibernate performance, N+1, JOIN FETCH, Flyway/Liquibase, OpenAPI | Spring internals, Spring Modulith, WebFlux | Разрабатывает production-like REST API с PostgreSQL, миграциями и обработкой ошибок |
| 9 | **Spring Security** | Authentication, Authorization, PasswordEncoder, roles/authorities, JWT/session, CORS/CSRF базово | OAuth2/OIDC, Method Security, security headers, refresh tokens | Advanced IAM, OAuth2 internals | Реализует и объясняет безопасную authentication/authorization-схему, понимает OAuth2 ≠ JWT |
| 10 | **Spring Testing** | JUnit 5, Mockito, unit/integration tests, MockMvc, @DataJpaTest, @SpringBootTest | Testcontainers + PostgreSQL, Spring Security Test, test slices | Mutation testing, advanced test architecture | Покрывает backend unit- и integration-тестами, диагностирует падение теста |
| 11 | **Backend Architecture** | Layered Architecture, Modular Monolith, dependency direction, coupling/cohesion | Clean/Hexagonal, DDD базово, package-by-feature, ADR | CQRS, Event-Driven Architecture, advanced DDD | Выбирает архитектуру под требования и объясняет trade-offs, разделяет слои |
| 12 | **Linux** | CLI, filesystem, permissions, processes, SSH, systemd, logs, networking базово | Bash, diagnostics, deployment без Docker, firewall | Advanced administration, kernel internals | Деплоит Java-приложение на Linux-сервер, диагностирует через systemctl/journalctl |
| 13 | **Docker / Compose** | images, containers, Dockerfile, volumes, networks, Compose, env variables | multi-stage builds, healthchecks, registry, security | Swarm, advanced networking/security | Контейнеризирует Spring Boot + PostgreSQL, диагностирует проблемы контейнера |
| 14 | **CI/CD** | GitHub Actions: build, test, package, Docker build | registry, staging, deployment, smoke tests, rollback, environments, secrets | reusable workflows, self-hosted runners, OIDC | Настраивает pipeline от commit/PR до deployment с секретами и проверками |
| 15 | **Infrastructure Components** | Redis basics (cache-aside, TTL), message broker concepts | Redis caching/invalidation, Kafka **или** RabbitMQ, retries, DLQ, idempotency, Outbox | Elasticsearch, Debezium/CDC, второй брокер | Интегрирует Redis + один брокер в Spring Boot, понимает назначение каждого компонента |
| 16 | **Observability** | structured logs, health checks, metrics, Actuator | Micrometer, Prometheus, Grafana, tracing, OpenTelemetry, centralized logs | SLI/SLO, error budgets, alerting architecture | Обнаруживает и локализует production-like проблему по logs/metrics/traces |
| 17 | **Load Testing** | latency, throughput/RPS, p95/p99, load/stress testing | k6 **или** JMeter **или** Gatling, profiling, JFR/JMC, bottleneck analysis | Capacity planning, performance engineering | Проводит нагрузочный тест, находит bottleneck, исправляет и сравнивает результаты |
| 18 | **Cloud Basics** | VM, networking, managed PostgreSQL, object storage, IAM, secrets | containers, registry, CDN, load balancer, managed Kubernetes | Serverless, advanced cloud architecture, FinOps | Разворачивает Spring Boot в облаке на одном провайдере |
| 19 | **System Design (HLD)** | requirements, capacity, API, DB, cache, queues, scaling, reliability | replication, sharding, rate limiting, failure scenarios, trade-offs | Multi-region, advanced distributed architecture | Проектирует систему на HLD-уровне, объясняет ключевые архитектурные решения |
| 20 | **Microservices / Distributed Systems** | service boundaries, REST/messaging, retries, timeouts, idempotency, eventual consistency | Kafka, Outbox, Saga, Circuit Breaker, distributed tracing | Consensus, Raft/Paxos, advanced distributed algorithms | Понимает partial failures, проектирует устойчивое взаимодействие нескольких сервисов |
| 21 | **DevOps** | Nginx как reverse proxy, базовые Kubernetes concepts | Deployment/Service/Ingress/ConfigMap/Secret/probes, Terraform basics | HPA/VPA, NetworkPolicy, advanced Terraform/Kubernetes | Разворачивает приложение через Nginx/Kubernetes, описывает инфраструктуру в Terraform |
| 22 | **HTML / CSS** | semantic HTML, forms, Flexbox, Grid, responsive design | accessibility, BEM, Sass, modern CSS | Advanced CSS architecture | Верстает адаптивный интерфейс по макету |
| 23 | **JavaScript** | language fundamentals, DOM, events, async/await, Promise, Fetch, modules | Event Loop, closures, prototypes, generators, browser APIs, AbortController | Advanced JS internals | Понимает JavaScript runtime, реализует интерактивное приложение |
| 24 | **TypeScript** | types, interfaces, unions, generics, narrowing, strict mode | utility/conditional/mapped types, Zod, advanced generics | Сложная type-level programming | Типизирует полноценное React-приложение без систематического `any` |
| 25 | **Frontend Tooling** | npm, Vite, ESLint, Prettier, TypeScript build | Husky, lint-staged, GitHub Actions, bundle optimization | Webpack internals, Module Federation | Настраивает production build и автоматические quality checks |
| 26 | **React / Next.js** | components, props, state, hooks, routing, forms, REST API | Next.js App Router, Server/Client Components, caching, Server Actions, Proxy | Advanced Next.js rendering/caching architecture | Разрабатывает production-like React/Next.js приложение |
| 27 | **OpenAPI / API Contracts** | OpenAPI, schemas, status codes, Swagger UI | code generation, mock server, contract testing, compatibility, versioning | Advanced API governance | Поддерживает API contract и синхронизирует frontend/backend через OpenAPI |
| 28 | **State Management / API Integration** | React state, Context, server state, API layer | Redux Toolkit, TanStack Query, optimistic updates, caching, auth refresh | Advanced state architecture | Разделяет UI/server/URL/auth state без дублирования данных |
| 29 | **Frontend Architecture** | component/feature architecture, boundaries, dependency direction | modular architecture, ADR, performance, monorepo | Microfrontends, Module Federation | Проектирует структуру frontend-приложения, объясняет trade-offs |
| 30 | **Web Security** | XSS, CSRF, CORS, cookies, HTTPS, auth boundaries | CSP, security headers, dependency security, clickjacking, Trusted Types | Advanced browser security | Определяет attack surfaces frontend-приложения, устраняет типовые уязвимости |
| 31 | **WebSockets / SSE** | WebSocket/SSE basics, lifecycle, reconnect, authentication | STOMP, heartbeat, reconnect strategy, multi-instance basics | Advanced realtime architecture | Реализует realtime-функциональность, обрабатывает disconnect/reconnect |
| 32 | **Frontend Testing** | unit/component/integration testing | React Testing Library, MSW, Playwright, E2E, CI | Advanced test architecture, visual testing | Строит устойчивую frontend test pyramid и запускает её в CI |
| 33 | **Frontend CI/CD + Docker** | production build, Docker, Nginx, CI | registry, staging/prod, HTTPS, rollback, security headers | Advanced CDN/cache/edge architecture | Собирает, контейнеризирует, публикует и разворачивает frontend |
| 34 | **Fullstack Capstone** | Spring Boot + PostgreSQL + React/Next.js + Docker + CI/CD | Security, OpenAPI, realtime, observability, tests, staging | Kafka/Redis/microservices/cloud production architecture | Доводит fullstack-проект от кода до production-like deployment |
| 35 | **English** | чтение технической документации, базовое общение | B1–B2, speaking, IT vocabulary, technical interviews | C1, свободное профессиональное общение | Читает docs без переводчика, объясняет техническую проблему на английском |
| 36 | **Agile / Scrum / Kanban** | основные термины и процесс разработки | Scrum events/roles/artifacts, Kanban, WIP, refinement, estimation | Advanced Agile practices | Понимает командный процесс и корректно описывает свою работу в нём |
| 37 | **CV / Portfolio / Interviews** | CV, GitHub, portfolio, HR interview, Java/SQL/algorithms basics | System Design, mock interviews, STAR, negotiation | Advanced interview preparation | Презентует опыт и проекты, проходит HR + technical screening |
| **—** | **Финальный уровень** | **Все ключевые P0 закрыты** | **Большинство P1 закрыто** | P2 изучается по необходимости | **Самостоятельно разрабатывает, тестирует, контейнеризирует, деплоит и сопровождает production-like fullstack-приложение; объясняет технические решения и диагностирует типовые проблемы** |

## Основы языка и работы с инструментами

### 1. Java

Цель: освоить язык Java — синтаксис, современные возможности (records, sealed classes, Pattern Matching), JVM, concurrency, Java Memory Model и Generics.

#### Ресурсы для изучения

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 1.1 | JavaRush — основной курс                                                                                 | [JavaRush](https://javarush.com/courses/java)                                                                       |
| 1.2 | Ablazzing. Java с нуля                                                                                           | [YouTube](https://www.youtube.com/watch?v=FR7vWoCWOMM&list=PLw265NhvhLXHptSyZ93dFd_7AoPnJTF1T)                      |
| 1.3 | JavaGuru. Java Core с нуля, полный курс | [YouTube](https://www.youtube.com/playlist?list=PLt91xr-Pp57T4tvQ4if78_I83QytkUhmG)                      |
| 1.4 | Андрей Сумин. Java: полный курс с нуля + подготовка к собеседованию | [Stepik](https://stepik.org/course/118518/promo)                                                                    |

#### Самостоятельно изучаем следующие темы

- **Современный Java:**

  - record
  - sealed class / sealed interface
  - Pattern Matching
  - switch expressions
  - var (не современная фича, но нужен для Legacy-кода)
  - Text Blocks (появились до Java 17, но знать нужно)
  - Optional — практическое владение
  - Stream API — углублённо
  - CompletableFuture
  - современный HttpClient
  - Virtual Threads (Java 21+)
  - базовое понимание изменений Java 17 → 21 → 25
- **JVM и выполнение Java-программ:**

  - устройство JVM
  - Heap / Stack / Metaspace
  - Class Loading и ClassLoader
  - Bytecode — базовое понимание
  - JIT-компиляция
  - Garbage Collector и управление памятью
  - основные принципы работы GC
  - G1 GC — концептуально
  - Stop-the-World
  - причины и базовые сценарии утечек памяти в Java
- **Concurrency и Java Memory Model:**

  - Thread
  - Runnable / Callable
  - ExecutorService
  - Thread Pool
  - synchronized
  - Lock / ReentrantLock
  - volatile
  - Atomic-классы
  - Concurrent Collections
  - Java Memory Model (JMM)
  - happens-before
  - visibility / atomicity / ordering
  - race condition
  - deadlock
  - starvation
  - CompletableFuture
  - Virtual Threads
  - базовое понимание Structured Concurrency
- **Generics:**

  - generic classes / methods
  - bounded type parameters
  - wildcards
  - extends / super
  - PECS
  - type erasure

#### Дополнительная литература

- Cay S. Horstmann — «Java. Библиотека профессионала. Том 1. Основы» → основная книга для систематизации Java
- Joshua Bloch — «Effective Java» → после освоения основ — учимся писать Java правильно и качественно
- Bruce Eckel — «Философия Java» → углубление понимания ООП и самой модели Java. Многие темы будут уже знакомы, поэтому читать её можно выборочно
- Brian Goetz и др. — «Java Concurrency in Practice» → отдельный углублённый блок по многопоточности и concurrency
- Kathy Sierra, Bert Bates — «Head First Java» → не обязательная книга после JavaRush. Скорее дополнительная для объяснения фундаментальных концепций другим способом

### 2. Git / GitHub

Цель: освоить систему контроля версий — ветвление, работа с историей, rebase, разрешение конфликтов и совместная разработка на GitHub.

#### Ресурсы для изучения

| #   | Ресурс                                                                                                            | Ссылка                                        |
| --- | ----------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 2.1 | Pragmatic Programmer. Git + GitHub. Полный курс                                                               | [Stepik](https://stepik.org/course/214865/promo)       |
| 2.2 | Иван Черняков. Git, GitHub, GitLab. Полный актуальный гайд за полтора часа | [YouTube](https://www.youtube.com/watch?v=0Y-fneoUIO8) |
| 2.3 | Артём Шумейко. Git — простым языком на понятном примере | [YouTube](https://www.youtube.com/watch?v=cG-8NnH4x94) |
| 2.4 | Богдан Стащук. Git - полный курс Git и GitHub для начинающих | [YouTube](https://www.youtube.com/watch?v=O00FTZDxD0o) |

#### Самостоятельно изучаем следующие темы

- rebase
- cherry-pick
- reset vs revert
- merge vs rebase
- HEAD / detached HEAD
- tag
- remote
- fetch vs pull
- Conventional Commits

#### Дополнительная литература

- Scott Chacon, Ben Straub — «Pro Git» → основная книга для глубокого и системного понимания Git. Особенно полезна после прохождения курса: branching, merging, rebasing, remote repositories, Git internals и работа с историей
- Jon Loeliger, Matthew McCullough — «Version Control with Git» → углубление понимания Git и системы контроля версий. Хорошо подходит после освоения базовых команд и рабочих сценариев
- Ryan Hodson — «Ry's Git Tutorial» → практическое руководство по Git. Подходит для закрепления команд и типовых рабочих сценариев разработки
- Travis Swicegood — «Pragmatic Version Control Using Git» → практическое применение Git в реальной разработке: workflow, ветки, история изменений и совместная работа в команде
- Richard E. Silverman — «Git Pocket Guide» → справочник по Git для быстрого повторения команд, параметров и основных операций. Не обязательно читать последовательно — удобно для точечных обращений

### 3. Сборка проектов: Maven и Gradle

Цель: научиться собирать Java-проекты через Maven и Gradle — управление зависимостями, lifecycle, плагины и multi-module проекты.

#### Ресурсы для изучения

| #   | Ресурс                                                                       | Ссылка                                                                                                         |
| --- | ---------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| 3.1 | Игорь Судакевич. Apache Maven: глубокое знакомство | [Stepik](https://stepik.org/course/268853/promo?search=9837193047)                                                      |
| 3.2 | OnFreeTube (EvgMel). Java Tutorials. Сборщик Maven                          | [YouTube](https://www.youtube.com/watch?v=MrTSmslo6i0&list=PL1zJrLkuWT67KutVoHZ3EhGswNkMcRIX2)                          |
| 3.3 | JavaGuru. Maven, сборщик проектов                                   | [Часть 1](https://www.youtube.com/watch?v=w28rwYgiuj8) · [Часть 2](https://www.youtube.com/watch?v=km4HtlDg9Ss) |
| 3.4 | JavaGuru. Gradle. Сборщик проектов                                  | [YouTube](https://www.youtube.com/watch?v=-b3X0F1oObY)                                                                  |
| 3.5 | Том Грегори. Gradle tutorial for complete beginners                      | [YouTube](https://www.youtube.com/watch?v=-dtcEMLNmn0)                                                                  |
#### Самостоятельно изучаем следующие темы

- **Maven:**

  - Maven CLI и Lifecycle: `clean`, `validate`, `compile`, `test`, `package`, `verify`, `install`, `deploy`; понимать phases, goals и порядок выполнения
  - POM: groupId, artifactId, version, packaging, properties, dependencies, plugins, profiles
  - Dependencies: прямые и транзитивные зависимости, конфликты версий, `dependency:tree`
  - Dependency Scopes и Dependency Management: compile, provided, runtime, test, dependencyManagement, parent, BOM
  - Repositories: local, Maven Central, remote repositories; понимать, откуда Maven получает зависимости и куда устанавливает артефакты
  - Properties и Profiles: `${...}`, централизованное управление версиями и профили dev / test / prod
  - Plugins: понимать связь plugin → goal → execution и назначение основных Maven-плагинов
  - Packaging и Artifacts: jar, war, создание и использование артефактов; install vs deploy
  - Multi-module projects: parent, modules, inheritance и aggregation
  - Maven Wrapper и settings.xml: `mvnw`, `mvnw.cmd`, `.mvn/`, назначение `settings.xml`
  - Maven + JUnit + Git/CI: запуск тестов и сборки через Maven, базовая цепочка Git → CI → Maven → test → package
  - **Практика:** самостоятельно создать Maven-проект, подключить зависимости, написать JUnit-тесты, собрать JAR, разобраться с `dependency:tree` и разместить проект на GitHub
- **Gradle:**

  - Основы Gradle: `build.gradle` / `build.gradle.kts`, `settings.gradle`, структура проекта и принцип работы Gradle
  - Gradle Wrapper: `gradlew`, `gradlew.bat` и зачем фиксировать версию Gradle в проекте
  - CLI и основные задачи: `./gradlew clean`, `build`, `test`, `check`, `assemble`
  - Dependencies: dependencies, repositories, configurations и транзитивные зависимости
  - Tasks: понимание task, зависимостей между задачами и Task Graph
  - Plugins: применение Java-плагина и понимание роли Gradle plugins
  - Multi-module projects: `settings.gradle`, subprojects и зависимости между модулями
  - **Практика:** самостоятельно собрать небольшой Java-проект через Gradle Wrapper, подключить зависимость, запустить тесты и сравнить структуру `build.gradle` с Maven `pom.xml`

#### Дополнительная литература

- Sonatype — «Maven: The Definitive Guide» → хорошая систематизация Maven: POM, lifecycle, dependencies, plugins, repositories, multi-module
- Sonatype — «Maven: The Complete Reference» → сильный справочник по Maven. Использовать выборочно, а не читать полностью
- Benjamin Muschko — «Gradle in Action» → хорошая книга для понимания модели Gradle, tasks, plugins, dependency management и multi-project builds. Учитывать возраст книги и сверять команды с современной документацией
- Gradle User Manual / Gradle Build Tool Documentation → для Gradle предпочтительнее официальная документация, а не книга: Gradle развивается быстро. Для Java-проектов особое внимание разделам про Wrapper, Java Plugin, dependencies, testing и multi-project builds

### 4. Принципы и паттерны проектирования

Цель: научиться проектировать код на уровне классов и модулей — SOLID, GRASP, GoF, рефакторинг и работа с архитектурными анти-паттернами.

#### Ресурсы для изучения

| #   | Ресурс                                                                                          | Ссылка                                        |
| --- | ----------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 4.1 | Евгений Сулейманов. Шаблоны проектирования на языке Java | [YouTube](https://www.youtube.com/watch?v=k6oh9C_71mE) |
| 4.2 | Builder Line. Паттерны проектирования программ на языке Java | [YouTube](https://www.youtube.com/playlist?list=PLKP3l9fd3KUFbrccxZMI0z3CgRdBDCp-g) |
| 4.3 | Иван Андрианов. Паттерны проектирования на Java                  | [Stepik](https://stepik.org/course/294677/promo)       |

#### Самостоятельно изучаем следующие темы

- **ООП и принципы проектирования:**

  - Composition over Inheritance
  - Programming to an Interface
  - Encapsulate What Varies
  - Prefer Delegation over Inheritance
  - Dependency Inversion
  - Law of Demeter — понимать принцип
  - Tell, Don't Ask — понимать принцип
- **SOLID:**

  - SRP
  - OCP
  - LSP
  - ISP
  - DIP
- **GRASP:**

  - Information Expert
  - Creator
  - Controller
  - Low Coupling
  - High Cohesion
  - Polymorphism
  - Pure Fabrication
  - Indirection
  - Protected Variations
- **GoF:**

  - знать назначение и решаемую проблему всех 23 паттернов
  - понимать структуру и взаимодействие участников паттерна
  - понимать преимущества и недостатки
  - понимать основные trade-offs
  - уметь определить, когда паттерн применять не следует
  - уметь распознавать паттерны в существующем Java-коде
  - уметь находить паттерны в JDK и Spring
  - ключевые для Java Backend паттерны уметь самостоятельно реализовать на Java
- **Практика проектирования:**

  - для заданной проблемы выбирать подходящий паттерн
  - объяснять, почему выбран именно этот паттерн
  - сравнивать паттерн с альтернативным решением без него
  - реализовывать ключевые паттерны самостоятельно на Java
  - рефакторить существующий код с применением подходящего паттерна
  - распознавать и устранять overengineering
  - находить God Object, Spaghetti Code, Golden Hammer и другие типичные design smells
  - оценивать coupling / cohesion после рефакторинга
  - проектировать взаимодействие нескольких классов и интерфейсов
  - читать и создавать UML class diagrams на базовом уровне
- **Практика на Java:**

  - реализовать несколько небольших задач, каждая из которых требует выбора паттерна
  - для каждой задачи подготовить минимум два решения и сравнить их
  - использовать interfaces, composition, polymorphism и dependency injection
  - написать тесты для разработанных решений
  - отдельно разобрать реальные примеры применения паттернов в JDK и Spring
- **Итоговая практика:**

  - получить исходный код намеренно плохо спроектированного Java-приложения
  - определить основные design problems
  - определить применимые SOLID / GRASP / GoF-подходы
  - выполнить последовательный рефакторинг
  - объяснить каждое архитектурное решение
  - сравнить код до и после рефакторинга
  - оформить итоговый проект на GitHub

#### Дополнительная литература

- Craig Larman — «Applying UML and Patterns» → один из лучших источников по object-oriented analysis and design, ответственности объектов, GRASP, UML и проектированию взаимодействия объектов. Особенно полезна для расширения раздела LLD за пределы GoF
- Erich Gamma, Richard Helm, Ralph Johnson, John Vlissides — «Design Patterns: Elements of Reusable Object-Oriented Software» → фундаментальный источник по 23 паттернам GoF. Использовать как справочник и первоисточник, а не как книгу для обязательного последовательного прочтения
- Robert C. Martin — «Clean Code» → практическая база по качеству кода, именованию, функциям, классам, зависимостям и рефакторингу. Хорошо связывает принципы проектирования с повседневной разработкой
- Robert C. Martin — «Agile Software Development, Principles, Patterns, and Practices» → глубокое дополнение к SOLID, принципам проектирования, паттернам и эволюционному дизайну. Особенно полезна для понимания связи принципов и архитектурных решений

### 5. Алгоритмы и структуры данных

Цель: освоить базовые алгоритмы, структуры данных и оценку сложности — для собеседований, оптимизации кода и решения практических задач.

#### Ресурсы для изучения

| #   | Ресурс                                                                                                                                                                     | Ссылка                                                                                                                                                                                                                           |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 5.1 | Алексей Ковальчук. Алгоритмы и структуры данных: курс для профессионалов (практику решать на Java) | [Stepik](https://stepik.org/course/184350/promo)                                                                                                                                                                                          |
| 5.2 | Ulbi TV. Алгоритмы и структуры данных. Фундаментальный курс от А до Я. Графы, деревья, хеш-таблицы       | [YouTube](https://www.youtube.com/watch?v=hXYHZVMHec0)                                                                                                                                                                                    |
| 5.3 | JavaRush, Константин. Что спрашивают на собеседовании: обзор алгоритмов                                                     | [Часть 1](https://javarush.com/groups/posts/3021-chto-sprashivajut-na-sobesedovanii-obzor-algoritmov-chastjh-1) · [Часть 2](https://javarush.com/groups/posts/3022-chto-sprashivajut-na-sobesedovanii-obzor-algoritmov-chastjh-2) |
| 5.4 | Илья Круковский. Алгоритмы и структуры данных                                                                                             | [YouTube](https://www.youtube.com/watch?v=BlwiPA9rx8w)                                                                                                     
#### Обязательно изучаем

- оценка сложности алгоритмов (Big O)
- анализ времени и памяти
- линейный и бинарный поиск
- переборные алгоритмы
- бинарный поиск по ответу
- сортировки
- жадные алгоритмы
- метод двух указателей
- динамическое программирование
- LinkedList
- Stack
- Queue
- Deque
- Heap
- Priority Queue
- деревья
- DFS
- BFS
- Dijkstra
- базовые графовые алгоритмы
- битовые операции
- базовые числовые алгоритмы

#### Для каждой обязательной задачи уметь объяснить

- алгоритм
- выбранную структуру данных
- Time Complexity
- Space Complexity
- альтернативное решение

#### Темы олимпиадного уровня (выборочно, без требования полного освоения)

- дерево отрезков
- дерево Фенвика
- сложная геометрия
- выпуклая оболочка
- продвинутые числовые алгоритмы

#### Обязательная самостоятельная практика на Java

- ArrayList vs LinkedList
- HashMap / HashSet
- TreeMap / TreeSet
- Queue / Deque
- PriorityQueue
- Comparator / Comparable
- бинарный поиск
- бинарный поиск по ответу
- сортировки
- рекурсия
- Two Pointers
- Sliding Window
- Prefix Sum
- алгоритмы на основе Stack
- BFS / DFS
- базовые графы
- Dijkstra
- Dynamic Programming
- жадные алгоритмы
- битовые операции
- оценка Time Complexity / Space Complexity

#### Статьи на Хабре

- **Big O и сложность алгоритмов:**

  - [Alex_BBB. Big O](https://habr.com/ru/articles/444594/)
  - [Open-JS. Сложность алгоритмов. Разбор Big O](https://habr.com/ru/articles/782608/)
- **Поиск и Two Pointers:**

  - [Open-JS. Бинарный поиск](https://habr.com/ru/articles/783848/)
  - [ddk-0310. O(log n) или O(n)? Разбор алгоритмов поиска](https://habr.com/ru/articles/1017108/)
  - [Artur_frontDev. Зная эти паттерны, ты решишь 60% задач на собеседовании](https://habr.com/ru/articles/1020222/)
- **Сортировки:**

  - [techno_mot. Это база. Алгоритмы сортировки для начинающих](https://habr.com/ru/companies/selectel/articles/851206/)
  - [OMS7. Описание алгоритмов сортировки и сравнение их производительности](https://habr.com/ru/articles/335920/)
- **Структуры данных:**

  - [Александр Чепайкин. Структуры данных для подготовки к собеседованиям по алгоритмам](https://habr.com/ru/articles/879914/)
  - [dcct0r. Шпаргалка по структурам данных в Java](https://habr.com/ru/articles/751648/)
  - [yetanothercoder. Алгоритмы и структуры данных JDK](https://habr.com/ru/articles/182776/)
- **Heap / Priority Queue:**

  - [awolf. Структуры данных: двоичная куча (binary heap)](https://habr.com/ru/articles/112222/)
- **Деревья:**

  - [akozyrenko. Бинарные деревья — решение алгоритмических задач, часть 1](https://habr.com/ru/articles/835706/)
  - [Procs. Бинарные деревья поиска и рекурсия — это просто](https://habr.com/ru/articles/267855/)
  - [nickme. АВЛ-деревья](https://habr.com/ru/articles/150732/)
- **Графы:**

  - [tonitaga. Базовые алгоритмы на графах](https://habr.com/ru/companies/timeweb/articles/751762/)
  - [aio350. Обход графа: поиск в глубину и поиск в ширину простыми словами](https://habr.com/ru/articles/504374/)
  - [yastrebdev. Алгоритмы поиска путей на пальцах. Часть 1: Поиск в ширину](https://habr.com/ru/articles/856138/)
  - [yastrebdev. Алгоритмы поиска путей на пальцах. Часть 2: Алгоритм Дейкстры](https://habr.com/ru/articles/856166/)
- **Динамическое программирование:**

  - [cybrid. Динамическое программирование. Классические задачи](https://habr.com/ru/articles/113108/)
  - [Frommi. Всё, что вы хотели знать о динамическом программировании, но боялись спросить](https://habr.com/ru/articles/191498/)
- **Жадные алгоритмы:**

  - [Rustam. Жадные алгоритмы](https://habr.com/ru/articles/120343/)
  - [nikolaysmartynov. Совершенный алгоритм. Жадные алгоритмы и динамическое программирование](https://habr.com/ru/articles/674352/)
- **Битовые операции:**

  - [malkovsky. Алгоритмы манипуляций с битами](https://habr.com/ru/articles/886182/)
  - [Bright_Translate. Откройте для себя весь потенциал побитовых операторов. Без математики](https://habr.com/ru/companies/ruvds/articles/735668/)

#### Дополнительная литература

- Thomas H. Cormen, Charles E. Leiserson, Ronald L. Rivest, Clifford Stein — «Introduction to Algorithms» (CLRS) → главная фундаментальная книга по алгоритмам и структурам данных. Охватывает асимптотику, сортировки, структуры данных, деревья, графы, жадные алгоритмы, динамическое программирование и многие другие темы. Главная справочная книга, а не книга для последовательного чтения от корки до корки
- Robert Sedgewick, Kevin Wayne — «Algorithms» → отличное практическое дополнение к CLRS: алгоритмы и структуры данных объясняются прикладным образом, с большим количеством реализаций и анализа производительности. Особенно полезна для перехода от теории к программированию
- Aditya Bhargava — «Grokking Algorithms» → самое доступное объяснение основных алгоритмов. Хорошо использовать как дополнительное объяснение, если какая-то тема из основного курса или CLRS оказалась слишком абстрактной. Не заменяет фундаментальную литературу
- Steven S. Skiena — «The Algorithm Design Manual» → сильная книга именно по проектированию алгоритмов и выбору подходящего решения. Особенно полезна для развития алгоритмического мышления: как распознать тип задачи, какую технику применить и как оценить решение. Хорошо соответствует требованию объяснять альтернативное решение
- Jon Kleinberg, Éva Tardos — «Algorithm Design» → углублённое изучение алгоритмического проектирования: жадные алгоритмы, divide and conquer, динамическое программирование, графы и другие алгоритмические парадигмы. Читать выборочно после основного курса для более глубокого понимания

## Backend-разработка

### 6. Web и компьютерные сети

Цель: понять, как работает интернет и HTTP, и научиться работать с сетью из Java — HttpClient, Socket, сервлеты, Tomcat.

#### Ресурсы для изучения

**Теоретическая часть:**

| #   | Ресурс                                                                                                                               | Ссылка                                                                                         |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- |
| 6.1 | Ulbi TV. Что такое REST API (HTTP)? SOAP? GraphQL? WebSockets? RPC (gRPC, tRPC). Клиент — сервер. Вся теория | [YouTube](https://www.youtube.com/watch?v=XaTwnKLQi4A)                                                  |
| 6.2 | Sriniously. Understanding HTTP for Backend Engineers                                                                                       | [YouTube](https://www.youtube.com/watch?v=a3C1DMswClQ)                                                  |
| 6.3 | Хабр. Как работает интернет + Taydvax. Как работает Интернет                                     | [Хабр](https://habr.com/ru/articles/840116/) · [YouTube](https://www.youtube.com/watch?v=aSPCTGhmxdI) |
| 6.4 | Хабр. Протокол HTTP                                                                                                            | [Хабр](https://habr.com/ru/articles/813395/)                                                        |

**JavaRush — работа с сетью:**

| #    | Ресурс                                                                        | Ссылка                                                                                                       |
| ---- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| 6.5  | JavaRush. Устройство сети                                             | [JavaRush](https://javarush.com/quests/lectures?quest=QUEST_JSP_SERVLETS&level=8)                                     |
| 6.6  | JavaRush. Протокол HTTP                                                     | [JavaRush](https://javarush.com/quests/lectures?quest=QUEST_JSP_SERVLETS&level=9)                                     |
| 6.7  | JavaRush. HttpClient                                                                | [JavaRush](https://javarush.com/quests/lectures?quest=QUEST_JSP_SERVLETS&level=10)                                    |
| 6.8  | Сергей Симонов (JavaRush). Классы Socket и ServerSocket в Java | [JavaRush](https://javarush.com/groups/posts/654-klassih-socket-i-serversocket-ili-allo-server-tih-menja-slihshishjh) |
| 6.9  | JavaRush. Tomcat                                                                    | [JavaRush](https://javarush.com/quests/lectures?quest=QUEST_JSP_SERVLETS&level=11)                                    |
| 6.10 | JavaRush. Сервлеты                                                          | [JavaRush](https://javarush.com/quests/lectures?quest=QUEST_JSP_SERVLETS&level=12)                                    |

**JavaGuru:**

| #    | Ресурс                                                                                        | Ссылка                                                                                        |
| ---- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| 6.11 | JavaGuru. Networking, основы работы с сетями в Java                             | [YouTube](https://www.youtube.com/watch?v=26Kq69J9iCQ&list=PLt91xr-Pp57QEnGJPuI4R_VqEXikn2a76&index=4) |
| 6.12 | JavaGuru. Apache Tomcat, сервер приложений и контейнер сервлетов | [YouTube](https://www.youtube.com/watch?v=tyyQw0a0KgU&list=PLt91xr-Pp57QEnGJPuI4R_VqEXikn2a76&index=5) |
| 6.13 | JavaGuru. Servlet API, технология сервлетов                                      | [YouTube](https://www.youtube.com/watch?v=A4y7UP_pTzA&list=PLt91xr-Pp57QEnGJPuI4R_VqEXikn2a76&index=6) |

#### Обязательная самостоятельная практика

- **HTTP через Java HttpClient** — написать Java-проект, работающий с публичным REST API:

  - выполнить GET-запрос
  - разобрать HTTP status code
  - прочитать response headers
  - получить JSON из response body
  - выполнить POST с JSON-телом
  - выполнить PUT
  - выполнить DELETE
  - передавать собственные HTTP headers
  - настроить timeout
  - реализовать обработку ошибок HTTP и сетевых исключений
  - выполнить один из запросов асинхронно через `sendAsync()`
- **Socket / ServerSocket** — простой консольный клиент-сервер на Java:

  - `ServerSocket` запускает сервер и ожидает подключения
  - `Socket` подключается к серверу
  - клиент отправляет текстовое сообщение
  - сервер принимает сообщение и отправляет ответ
  - корректно закрывать соединения и ресурсы
  - обработать ситуацию, когда клиент отключился
  - добавить поддержку нескольких клиентов
- **HTTP-инструменты** — для одного из REST API выполнить те же запросы через `curl` или Postman:

  - GET
  - POST
  - PUT
  - DELETE

  Сравнить HTTP-запрос, HTTP-ответ, headers, status code, body.
- **Итоговая мини-практика** — доработать HTTP-клиент из первого задания:

  - вынести URL и настройки в конфигурацию
  - преобразовывать JSON в Java-объекты и обратно с использованием Jackson
  - реализовать отдельные методы/классы для работы с API
  - корректно обрабатывать успешные и ошибочные HTTP-ответы
  - обработать сетевые ошибки и timeout
  - использовать `sendAsync()` хотя бы для одного запроса
  - проверить работу клиента через `curl` или Postman
  - оформить проект как небольшой самостоятельный Java-проект

#### Дополнительная литература

- James F. Kurose, Keith W. Ross — «Computer Networking: A Top-Down Approach» → главная книга для систематизации компьютерных сетей. Последовательно изучает сетевые протоколы сверху вниз: прикладной уровень, HTTP, DNS, транспортный уровень, TCP/UDP, сетевой уровень, IP, маршрутизация, канальный уровень и основы сетевой безопасности. Лучше всего дополняет теоретическую часть и помогает сформировать целостное понимание того, как работает интернет
- Elliotte Rusty Harold — «Java Network Programming» → главная практическая книга именно по сетевому программированию на Java. Подробно рассматривает Socket, ServerSocket, TCP/IP, UDP, URL/URI, HTTP, сетевые потоки и другие возможности Java
- David Gourley, Brian Totty, Marjorie Sayer, Anshu Aggarwal, Sailu Reddy — «HTTP: The Definitive Guide» → глубокое дополнение к изучению HTTP. Подробно разбирает HTTP-сообщения, методы, status codes, headers, cookies, authentication, caching, proxies и другие механизмы протокола. Книга ориентирована преимущественно на HTTP/1.1, поэтому использовать её для фундаментального понимания HTTP, а не как руководство по HTTP/2 и HTTP/3
- Sam Newman — «Building Microservices» → практическое дополнение для понимания взаимодействия backend-сервисов в современной архитектуре. Рассматривает API, синхронное и асинхронное взаимодействие, REST, messaging, service discovery, отказоустойчивость, наблюдаемость и другие аспекты распределённых систем. Хорошо связывает фундаментальные знания с последующим изучением Spring Boot, микросервисов, Docker и Kubernetes

### 7. SQL / PostgreSQL

Цель: освоить SQL и PostgreSQL — запросы, индексы, EXPLAIN, транзакции, MVCC и проектирование схемы БД для backend-приложений.

#### Ресурсы для изучения

| #   | Ресурс                                                                                                                                                                                       | Ссылка                                                                                                                                                                                                         |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 7.1 | Shultais Education. Программа «SQL с нуля до PRO» (фундамент SQL на примере MySQL)                                                                             | [Stepik](https://stepik.org/course/61247/promo)                                                                                                                                                                         |
| 7.2 | Артём Санников. Погружение в базы данных PostgreSQL                                                                                                              | [Stepik](https://stepik.org/course/204101/promo)                                                                                                                                                                        |
| 7.3 | JavaGuru. SQL                                                                                                                                                                                      | [Часть 1](https://www.youtube.com/watch?v=4pe16In1Byc&list=PLt91xr-Pp57QEnGJPuI4R_VqEXikn2a76&index=8) · [Часть 2](https://www.youtube.com/watch?v=vAecKsvjL2M&list=PLt91xr-Pp57QEnGJPuI4R_VqEXikn2a76&index=9) |
| 7.4 | freeCodeCamp.org. Learn PostgreSQL Tutorial — Full Course for Beginners                                                                                                                           | [YouTube](https://www.youtube.com/watch?v=qw--VYLpxG4)                                                                                                                                                                  |
| 7.5 | Диджитализируй! База по оптимизации PostgreSQL: схема, индексы, чтение EXPLAIN, методы доступа и соединения, тюнинг | [YouTube](https://www.youtube.com/watch?v=gA3A_epB3So) |

#### Самостоятельно изучаем следующие темы

- **PostgreSQL на практике:**

  - `psql`, DBeaver, создание БД и пользователей
  - типы данных: UUID, JSONB, ARRAY, ENUM, TIMESTAMP, DATE, NUMERIC
  - идентификаторы: `GENERATED ... AS IDENTITY`, sequences
- **SQL — базовый уровень:**

  - CRUD: INSERT, UPDATE, DELETE, SELECT
  - `RETURNING`
  - `ON CONFLICT` / UPSERT
  - JOIN: INNER, LEFT, RIGHT, FULL
  - GROUP BY / HAVING
  - подзапросы и CTE (WITH)
  - рекурсивные CTE — понимать принцип
  - Window Functions
  - VIEW / MATERIALIZED VIEW
- **Индексы и производительность:**

  - индексы: B-tree, Hash, GIN, GiST, BRIN
  - составные, уникальные, частичные индексы
  - EXPLAIN / EXPLAIN ANALYZE
  - почему запрос медленный, как найти проблему и как индекс влияет на план выполнения
- **Транзакции и конкурентность:**

  - транзакции: BEGIN, COMMIT, ROLLBACK
  - ACID
  - уровни изоляции и MVCC
  - блокировки и deadlocks
  - `SELECT ... FOR UPDATE`
- **Проектирование БД:**

  - нормализация: 1NF, 2NF, 3NF; когда допустима денормализация
  - проектирование схемы: таблицы, PK/FK, ограничения, связи 1:1, 1:N, N:M
  - резервное копирование: базовое понимание `pg_dump` / `pg_restore`
- **Практика:** самостоятельно спроектировать PostgreSQL-БД для Java-проекта и написать набор реальных SQL-запросов к ней

#### Дополнительная литература

- Markus Winand — «SQL Performance Explained» → главная книга по производительности SQL. Индексы, execution plans, JOIN, сортировки, диапазонные запросы и оптимизация. Читать после освоения базового SQL
- Regina Obe, Leo Hsu — «PostgreSQL: Up and Running» → практическое знакомство именно с PostgreSQL. Хорошо использовать как дополнительный справочник при работе с PostgreSQL
- Hans-Jürgen Schönig — «Mastering PostgreSQL 17» → углубление PostgreSQL: типы данных, SQL, индексы, запросы, транзакции, производительность и внутренние механизмы
- Alex Petrov — «Database Internals: A Deep Dive into How Distributed Data Systems Work» → понимание того, как работают базы данных внутри: storage engines, B-Tree, LSM-tree, индексы, WAL, репликация, распределённые системы. Читать после уверенного освоения SQL/PostgreSQL
- Martin Kleppmann — «Designing Data-Intensive Applications» → архитектура систем, работа с данными, репликация, partitioning, transactions, consistency, distributed systems, Kafka и другие инструменты. Это переход от обычной работы с БД к архитектуре backend-систем

### 8. Spring / Spring Boot

Цель: научиться разрабатывать полноценный REST API на Spring Boot с PostgreSQL, Spring Data JPA, Hibernate, DTO, валидацией, обработкой ошибок и миграциями.

#### Ресурсы для изучения

| #   | Ресурс                                                                                           | Ссылка                                        |
| --- | ------------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 8.1 | Заур Трегулов. Spring для начинающих                                          | [Stepik](https://stepik.org/course/115372/promo)       |
| 8.2 | Заур Трегулов. JPA & Hibernate                                                             | [Stepik](https://stepik.org/course/233204/promo)       |
| 8.3 | Павел Сорокин. Основной практический материал по Spring Boot | [YouTube](https://www.youtube.com/watch?v=KDrNL-uw3oc) |
| 8.4 | Павел Сорокин. Обзорный материал по всему Java Backend              | [YouTube](https://www.youtube.com/watch?v=vW9O_FIg_70) |

#### Самостоятельно изучаем следующие темы

- **Spring Boot:**

  - структура приложения, `@SpringBootApplication`, configuration, profiles, `application.yml`
- **Spring MVC и REST API:**

  - `@RestController`, `@RequestMapping`, `@GetMapping`, `@PostMapping`, `@PutMapping`, `@DeleteMapping`
  - HTTP methods, status codes, ресурсы, pagination, PUT vs PATCH, идемпотентность HTTP-операций
- **JSON / Jackson:**

  - serialization / deserialization, `@JsonProperty`, `@JsonIgnore`, `ObjectMapper`
- **DTO и валидация:**

  - Entity ≠ DTO, mapping Entity ↔ DTO
  - `@Valid`, `@NotNull`, `@NotBlank`, `@Size`, `@Email`, собственные constraints
- **Обработка ошибок:**

  - `@ExceptionHandler`, `@ControllerAdvice`, единый формат ошибок
- **Spring Data JPA:**

  - `JpaRepository`, derived queries, `@Query`, pagination / sorting, `EntityManager`
- **JPA / Hibernate — производительность:**

  - LAZY / EAGER, JOIN FETCH, EntityGraph, N+1 и способы его устранения
- **Spring + PostgreSQL:**

  - datasource, подключение PostgreSQL, JPA / Hibernate configuration
- **Транзакции:**

  - `@Transactional`, propagation, rollback, readOnly, isolation
  - понимать связь Spring Transaction Management → JPA → Hibernate → PostgreSQL
- **Database migrations:**

  - базовое применение Flyway или Liquibase
- **OpenAPI / Swagger:**

  - документирование REST API
- **Практика:** самостоятельно разработать полноценный Spring Boot REST API с PostgreSQL, DTO, Validation, Exception Handling, Spring Data JPA, Hibernate и Transactions

#### Дополнительная литература

- Craig Walls — «Spring in Action» → основная книга для систематизации Spring / Spring Boot, включая Core, Boot, MVC, REST и Data
- Laurentiu Spilca — «Spring Start Here» → углубление Spring Core: IoC, DI, beans, scopes, lifecycle, AOP
- Vlad Mihalcea — «High-Performance Java Persistence» → глубокое изучение JPA / Hibernate и производительности persistence layer: fetching, batching, transactions, caching, N+1, SQL
- Christian Bauer, Gavin King, Gary Gregory — «Java Persistence with Hibernate» → фундаментальный справочник по JPA / Hibernate и продвинутому mapping
- Martin Fowler — «Patterns of Enterprise Application Architecture» → архитектура enterprise-приложений: Repository, Unit of Work, Data Mapper, Service Layer, DTO и другие паттерны

### 9. Spring Security

Цель: освоить аутентификацию и авторизацию в Spring-приложениях — JWT, OAuth2, роли, permissions, Method Security и защиту REST API.

#### Ресурсы для изучения

| #   | Ресурс                                                                                                            | Ссылка                                        |
| --- | ----------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 9.1 | Иван Андрианов. Spring Security: архитектура безопасности Java-приложений | [Stepik](https://stepik.org/course/278484/promo)       |
| 9.2 | CodeSnippet. Master Spring Security in One Shot 2026 (JWT + OAuth2 + Authorization, Roles & More)                       | [YouTube](https://www.youtube.com/watch?v=eYCOzPx3ht8) |

#### Самостоятельно изучаем следующие темы

- **Security Core:**

  - SecurityFilterChain и последовательность обработки запроса
  - SecurityContext, Authentication, Principal
  - Authentication vs Authorization
- **UserDetails и пароли:**

  - UserDetails, UserDetailsService, PasswordEncoder
  - Password storage и BCryptPasswordEncoder / современный PasswordEncoder
- **Roles и Authorities:**

  - Roles vs Authorities
  - `hasRole()` vs `hasAuthority()`
  - URL-based authorization
- **Method Security:**

  - `@PreAuthorize`, `@PostAuthorize`
- **CSRF, CORS, Security Headers:**

  - CSRF: зачем нужен и когда отключается для REST API
  - CORS: preflight, origins, methods, headers
  - Security headers
  - logout
- **Аутентификация: сессии vs JWT:**

  - Session-based vs stateless authentication
  - JWT: header / payload / signature, access token, expiration
  - JWT authentication flow
  - JWT + SecurityFilterChain
  - refresh token — на уровне архитектуры и принципа
- **OAuth 2.0 и OpenID Connect:**

  - OAuth 2.0: роли Resource Owner / Client / Authorization Server / Resource Server
  - OpenID Connect — понимать отличие от OAuth 2.0
  - OAuth2 Resource Server — хотя бы базовая практическая настройка
- **Обработка ошибок и защита REST API:**

  - authentication / authorization errors: AuthenticationEntryPoint, AccessDeniedHandler
  - защита REST API: HTTPS, secure headers, rate limiting, secrets management
  - Security Testing — базово
- **Практика:** защитить собственный Spring Boot REST API

#### Дополнительная литература

- Laurentiu Spilca — «Spring Security in Action» → главная книга по Spring Security: authentication, authorization, password storage, CSRF, OAuth2, JWT, method security
- Badr Nasslahsen — «Spring Security: Effectively secure your web apps, RESTful services, cloud apps, and microservice architectures» (4th ed., Packt, 2024) → современное практическое руководство, охватывающее широкий спектр тем, от основ до микросервисов
- Craig Walls — «Spring in Action» (см. раздел 8) → в этом разделе полезен как связка Security с остальным Spring-стеком: Core, Boot, MVC, REST
- Vlad Mihalcea — «High-Performance Java Persistence» (см. раздел 8) → не книга непосредственно по Security, но важна для понимания защищённого приложения на уровне persistence: transactions, Hibernate, SQL, fetching, performance
- Martin Fowler — «Patterns of Enterprise Application Architecture» (см. раздел 8) → архитектурная база: Service Layer, DTO, Unit of Work, Data Mapper и другие паттерны, которые помогают правильно проектировать security boundary в enterprise-приложении

### 10. Spring Testing

Цель: научиться тестировать Spring Boot приложения — unit, integration и repository-тесты, MockMvc, Testcontainers и Spring Security Test.

#### Ресурсы для изучения

| #    | Ресурс                                                                                               | Ссылка                                        |
| ---- | ---------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 10.1 | Евгений Сулейманов. Тестирование ПО глазами разработчика | [YouTube](https://www.youtube.com/watch?v=9GOs-QQcVRA) |
| 10.2 | Think Constructive. Master Unit Testing Java Spring Boot REST API Application in One Shot                  | [YouTube](https://www.youtube.com/watch?v=HqiEM5HQsZs) |
| 10.3 | SivaLabs. Java Testing Made Easy: Learn writing Unit, Integration, E2E & Performance Tests | [YouTube](https://www.youtube.com/playlist?list=PLuNxlOYbv61jtHHFHBOc9N7Dg5jn013ix) |
| 10.4 | Java coding interview. Тестирование (включая нагрузочное) | [YouTube](https://www.youtube.com/playlist?list=PLk9a6fpk-pjv8W6lQTVuAUlExHmU9N3B1) |

#### Самостоятельно изучаем следующие темы

- **JUnit 5:**

  - `@Test`
  - `@BeforeEach`, `@AfterEach`, `@BeforeAll`, `@AfterAll`
  - Assertions: `assertEquals`, `assertNotNull`, `assertTrue`, `assertFalse`, `assertThrows`, `assertAll`
  - `@ParameterizedTest`
  - `@ValueSource`, `@CsvSource`, `@MethodSource`
  - `@Nested`
  - `@DisplayName`
  - `@Tag`
  - жизненный цикл тестов
- **AssertJ:**

  - `assertThat`
  - fluent assertions
  - assertions для объектов и коллекций
  - `contains`, `containsExactly`, `containsExactlyInAnyOrder`
  - `extracting`
  - проверка исключений
- **Mockito:**

  - `@Mock`
  - `@InjectMocks`
  - `@Spy`
  - `when(...).thenReturn(...)`
  - `thenThrow(...)`
  - `verify(...)`
  - `times(...)`
  - `never()`
  - `ArgumentCaptor`
  - mock vs spy vs real object
  - что следует мокировать, а что — нет
- **Основы unit-тестирования:**

  - unit-тесты vs integration-тесты
  - AAA / Given–When–Then
  - happy path
  - edge cases
  - error cases
  - тестирование исключений
  - читаемые и поддерживаемые тесты
  - test fixtures
  - flaky tests
  - принцип изоляции unit-тестов
- **Spring Boot Test:**

  - `@SpringBootTest`
  - `@WebMvcTest`
  - `@DataJpaTest`
  - Test Slices
  - Spring Test Context
  - `@ActiveProfiles`
  - `application-test.yml`
  - отличие обычного unit-теста от Spring-теста
- **Тестирование Controller:**

  - MockMvc
  - GET / POST / PUT / DELETE
  - HTTP status codes
  - headers
  - JSON request / response
  - JSONPath
  - DTO
  - Bean Validation
  - обработка ошибок
  - тестирование `@ControllerAdvice`
  - проверка 400 / 404 / 409 / 500
  - тестирование защищённых endpoint'ов
- **Тестирование Service:**

  - unit-тестирование бизнес-логики
  - Mockito
  - проверка взаимодействия с зависимостями
  - verify
  - ArgumentCaptor
  - позитивные и негативные сценарии
  - граничные случаи
- **Тестирование Repository:**

  - `@DataJpaTest`
  - derived queries
  - JPQL / native queries
  - проверка сохранения и получения данных
  - constraints
  - тестирование транзакций
  - H2 vs PostgreSQL
- **Интеграционное тестирование:**

  - `@SpringBootTest`
  - полный Spring Application Context
  - Controller → Service → Repository
  - интеграционные тесты REST API
  - test profile
  - подготовка и очистка тестовых данных
  - транзакции в интеграционных тестах
- **Testcontainers:**

  - Docker + Testcontainers
  - `@Testcontainers`
  - `@Container`
  - PostgreSQL container
  - lifecycle контейнеров
  - интеграционные тесты с реальным PostgreSQL
  - H2 vs Testcontainers + PostgreSQL
  - Testcontainers + Spring Boot
- **Интеграция с миграциями БД:**

  - Testcontainers + PostgreSQL
  - Flyway / Liquibase в тестах
  - проверка миграций
  - проверка реальной схемы БД
  - тестирование SQL / JPA на PostgreSQL
- **Spring Security Test:**

  - тестирование защищённых REST endpoint'ов
  - MockMvc + Spring Security
  - `@WithMockUser`
  - authentication / authorization
  - проверка 401 / 403
  - roles / authorities
  - тестирование JWT-защищённых endpoint'ов
- **Современное мокирование Spring Beans:**

  - `@MockitoBean` — современный подход (Spring Boot 3.4+)
  - `@MockBean` — legacy-подход в старых проектах
  - отличие `@MockitoBean` от `@Mock`
  - понимание того, когда нужен Spring Context, а когда достаточно Mockito
- **Практика:** покрыть тестами Spring Boot REST API из раздела 8:

  - написать unit-тесты для Service layer
  - написать тесты Controller через MockMvc
  - написать тесты Repository через `@DataJpaTest`
  - написать integration tests через `@SpringBootTest`
  - поднять PostgreSQL через Testcontainers
  - подключить Flyway / Liquibase в тестах
  - протестировать Security через Spring Security Test
  - проверить 401 / 403
  - протестировать validation и обработку ошибок
  - выполнить integration-тесты полного сценария Controller → Service → Repository → PostgreSQL
  - разместить тесты на GitHub

#### Дополнительная литература

- Vladimir Khorikov — «Unit Testing Principles, Practices, and Patterns» → главная книга для систематизации unit-тестирования: качественные unit-тесты, изоляция, test doubles, mock vs stub vs fake, интеграционные тесты, test design и maintainability тестового кода
- Roy Osherove — «The Art of Unit Testing» → практическое руководство по проектированию и написанию поддерживаемых unit-тестов: isolation, test doubles, mocks / stubs, тестируемость кода, работа с legacy-кодом и организация тестового набора
- Andrew Hunt, David Thomas — «The Pragmatic Programmer» → не книга исключительно про тестирование, но полезна как дополнение по качеству разработки: DRY, design for change, defensive programming, automation, debugging и поддерживаемость кода
- Cătălin Tudose — «JUnit in Action» (3rd ed., Manning, 2025) → практическое углубление в JUnit 5: lifecycle, assertions, parameterized tests, nested tests, extensions, test organization и современные возможности фреймворка. Включает главы по тестированию Spring и Spring Boot приложений
- Ken Kousen — «Mockito Made Clear» (Pragmatic Bookshelf, 2023) → практическое руководство по Mockito и test doubles: mock / spy, stubbing, verification, ArgumentCaptor, взаимодействие с зависимостями и применение Mockito в unit-тестах на JUnit 5

## Архитектура и инфраструктура

### 11. Backend-архитектура

Цель: изучить архитектурные стили (Layered, Clean, Hexagonal, Modular Monolith), принципы проектирования и DDD для backend-систем.

#### Ресурсы для изучения

**Теоретические основы архитектуры**

| #    | Ресурс                                                                                                                                                         | Ссылка                                  |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| 11.1 | JavaGuru. Паттерны микросервисной архитектуры | [YouTube](https://www.youtube.com/playlist?list=PLt91xr-Pp57TN4-UN1F6JqqwhaI1T6E0b) |
| 11.2 | Big Data. Java для мидлов (Модуль 18 - архитектура) | [Stepik](https://stepik.org/course/294073/promo) |
| 11.3 | mpanaryin. Разбираем архитектуру. Часть 1. Чистая архитектура и её корни: история и взаимосвязи | [Хабр](https://habr.com/ru/articles/905148/) |
| 11.4 | mpanaryin. Разбираем архитектуру. Часть 2. Чистая архитектура на примере FastAPI-приложения             | [Хабр](https://habr.com/ru/articles/908082/) |

**Практическая архитектура backend — гексагональная архитектура:**

| #    | Ресурс                                                                                                                      | Ссылка                                                        |
| ---- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| 11.5 | Bifurcated. Реализация гексагональной архитектуры на Java                                    | [Хабр](https://habr.com/ru/articles/985156/)                       |
| 11.6 | Tom Hombergs. Hexagonal Architecture with Java and Spring                                                                         | [Reflectoring](https://reflectoring.io/spring-hexagonal/)              |
| 11.7 | Уголок сельского джависта. Гексагональная архитектура и микросервисы | [YouTube](https://www.youtube.com/watch?v=V1xP5LVr4fY)                 |
| 11.8 | Organizing Layers Using Hexagonal Architecture, DDD, and Spring                                                                   | [Baeldung](https://www.baeldung.com/hexagonal-architecture-ddd-spring) |

**Практическая архитектура backend — Modular Monolith:**

| #    | Ресурс                                                                           | Ссылка                                                                                                                  |
| ---- | -------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| 11.9 | Dan Vega. Introduction to Spring Modulith — Modular Monoliths in Spring Boot          | [YouTube](https://www.youtube.com/watch?v=xHlDyKVyvig)                                                                           |
| 11.10 | Siva Katamreddy. Migrating to Modular Monolith using Spring Modulith and IntelliJ IDEA | [JetBrains Blog](https://blog.jetbrains.com/idea/2026/02/migrating-to-modular-monolith-using-spring-modulith-and-intellij-idea/) |

**Критическое мышление и trade-offs:**

| #     | Ресурс                                                                              | Ссылка                                  |
| ----- | ----------------------------------------------------------------------------------------- | --------------------------------------------- |
| 11.11 | jdev. Вам не нужна чистая архитектура. Скорее всего | [Хабр](https://habr.com/ru/articles/888428/) |

#### Самостоятельно изучаем следующие темы

- **Architectural characteristics / quality attributes:**

  - maintainability
  - scalability
  - performance
  - reliability
  - availability
  - security
  - testability
  - deployability
  - observability
- **Архитектурные стили:**

  - Layered Architecture
  - Modular Monolith
  - Clean Architecture
  - Hexagonal Architecture / Ports & Adapters
  - Onion Architecture
  - package-by-layer vs package-by-feature
- **Принципы проектирования:**

  - Dependency Rule
  - Dependency Inversion
  - Separation of Concerns
  - coupling / cohesion
- **Слои и границы:**

  - domain / application / infrastructure / presentation
  - business logic vs application / orchestration logic
  - границы модулей и направление зависимостей
- **Модели и абстракции:**

  - DTO / Command / Domain Model / Persistence Model
  - Repository / Gateway / Adapter
  - Domain Service / Application Service
- **DDD:**

  - Ubiquitous Language
  - Entity, Value Object, Aggregate
  - Domain Service, Application Service
  - Repository, Domain Event
  - Bounded Context, Context Map
- **Продвинутые паттерны:**

  - CQRS и Event-Driven Architecture на концептуальном уровне
- **Trade-offs и анти-паттерны:**

  - архитектурные trade-offs
  - overengineering / YAGNI / KISS
  - architectural smells: God Module, Big Ball of Mud, cyclic dependencies, leaky abstractions, misplaced business logic, excessive coupling
  - выбор архитектуры в зависимости от требований, сложности и ожидаемых изменений

#### Дополнительная литература

- Robert C. Martin — «Clean Architecture» → основная книга по архитектурным границам, Dependency Rule, слоям и направлению зависимостей
- Martin Fowler — «Patterns of Enterprise Application Architecture» (см. разделы 8–9) → фундаментальный справочник по архитектурным паттернам прикладных систем: Domain Model, Service Layer, Repository, Unit of Work, Data Mapper, DTO, Gateway и др.
- Eric Evans — «Domain-Driven Design: Tackling Complexity in the Heart of Software» → классическая книга по DDD: Ubiquitous Language, Entity, Value Object, Aggregate, Repository, Bounded Context и стратегическому проектированию домена
- Vaughn Vernon — «Implementing Domain-Driven Design» → практическое продолжение Evans с акцентом на реализацию DDD, bounded contexts, aggregates, domain events, repositories и интеграцию между контекстами
- Mark Richards, Neal Ford — «Fundamentals of Software Architecture» → систематизация архитектурного мышления: архитектурные стили, характеристики качества, coupling / cohesion, modularity, trade-offs, архитектурные решения и эволюция архитектуры

### 12. Linux

Цель: научиться работать с Linux-сервером и разворачивать Java-приложения без Docker — systemd, права, логи, SSH, Bash.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                          | Ссылка                                                                     |
| ---- | --------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| 12.1 | Константин Варнали. Linux-Мастер: Администрирование, Bash-скрипты, SSH | [Stepik](https://stepik.org/course/260221/promo)                                    |
| 12.2 | Новая образовательная система. Администрирование Linux                    | [YouTube](https://www.youtube.com/playlist?list=PLYl91BhaOf-kkXWweBzgOw555he6S7SUs) |
| 12.3 | freeCodeCamp.org. Introduction to Linux — Full Course for Beginners                                                  | [YouTube](https://www.youtube.com/watch?v=sWbUDq4S6Y8)                              |

#### Самостоятельно изучаем следующие темы

- **systemd:**

  - назначение systemd
  - units, services, targets
  - `systemctl status` / `start` / `stop` / `restart` / `enable` / `disable`
  - автозапуск сервисов
  - создание собственного `.service`
  - `systemctl daemon-reload`
  - зависимости сервисов
  - базовое понимание жизненного цикла systemd-сервиса
- **Деплой Java-приложения без Docker:**

  - установка JDK на Linux-сервер
  - создание отдельного пользователя для приложения
  - создание каталога приложения
  - настройка владельца и прав доступа
  - размещение JAR-файла
  - конфигурация через environment variables
  - запуск Spring Boot-приложения как systemd-сервиса
  - автоматический запуск приложения после перезагрузки
  - graceful shutdown / restart
  - обновление JAR-файла и перезапуск приложения
- **Логи:**

  - `journalctl`
  - `journalctl -u <service>`
  - `journalctl -f`
  - просмотр логов конкретного сервиса
  - фильтрация логов по времени
  - поиск ошибок
  - связь systemd ↔ application logs
- **Диагностика Java-приложения:**

  - `ps`, `top`, `htop`, `free`, `df`, `du`, `uptime`
  - `kill`
  - SIGTERM (`kill -15`)
  - SIGKILL (`kill -9`)
  - понимание PID
  - CPU / RAM / disk usage
  - поиск Java-процесса
  - базовая диагностика приложения, которое перестало отвечать
- **Сетевая диагностика:**

  - `ip`, `ss`, `ping`, `curl`, `wget`
  - проверка открытых портов
  - проверка доступности Spring Boot REST API
  - диагностика проблем localhost / 0.0.0.0
  - базовое понимание firewall на сервере
- **Файловая система и права:**

  - `chmod`, `chown`, `chgrp`
  - владельцы файлов
  - права пользователя / группы / остальных
  - правильные права для JAR, конфигурации и логов
  - каталоги приложения и их permissions
  - почему Java-приложение не следует запускать от root
- **Переменные окружения:**

  - `env`, `printenv`, `export`, `PATH`
  - передача конфигурации Spring Boot через environment variables
  - различие shell variables и environment variables
  - базовое понимание `/etc/environment` и systemd `Environment` / `EnvironmentFile`
- **SSH для работы с сервером:**

  - SSH-ключи
  - `~/.ssh`, `authorized_keys`, `~/.ssh/config`
  - aliases для серверов
  - `scp`
  - `rsync` — базовое понимание
  - безопасная работа с удалённым сервером
- **Bash для автоматизации:**

  - написать Bash-скрипт для проверки состояния Spring Boot-приложения
  - проверять HTTP endpoint через `curl`
  - проверять наличие Java-процесса
  - выводить понятный статус
  - использовать exit codes
  - передавать параметры скрипту
  - обрабатывать ошибки
  - базовое использование `set -euo pipefail`
  - базовое использование скриптов для deployment / maintenance

#### Итоговая практика

Самостоятельно развернуть Spring Boot REST API из раздела 8 на Ubuntu Server без Docker:

- создать Ubuntu Server VM
- подключиться к серверу по SSH
- настроить SSH-аутентификацию по ключу
- создать отдельного пользователя для приложения
- установить JDK
- скопировать JAR на сервер
- настроить environment variables
- создать systemd service
- настроить автозапуск
- запустить приложение
- проверить REST API через `curl`
- проверить открытый порт через `ss`
- посмотреть логи через `journalctl`
- выполнить `start` / `stop` / `restart`
- выполнить обновление JAR и перезапуск приложения
- проверить graceful shutdown через SIGTERM
- проверить использование CPU и RAM
- намеренно сломать конфигурацию приложения
- самостоятельно найти причину проблемы по `systemctl status` и `journalctl`
- исправить проблему и восстановить приложение
- написать Bash health-check script
- проверить работу health-check script

#### Дополнительная литература

- William Shotts — «The Linux Command Line» → лучшая дополнительная книга для систематизации работы с командной строкой, Bash, файлами, процессами, permissions и shell scripting
- Brian Ward — «How Linux Works» → для понимания того, как Linux работает внутри: процессы, загрузка, устройства, файловая система, networking и system services. Читать после основного курса
- Michael Kerrisk — «The Linux Programming Interface» → очень глубокая книга о Linux API, процессах, памяти, IPC, файловой системе, signals и networking. Для Java Backend — справочная литература, полностью читать не требуется
- Nemeth, Snyder, Hein, Whaley, Mackin — «UNIX and Linux System Administration Handbook» → большой справочник по администрированию Linux / Unix. Использовать выборочно как справочник
- Carl Albing, JP Vossen — «bash Cookbook» → практический справочник по Bash-скриптам. Особенно полезен для автоматизации deployment и рутинных серверных операций

### 13. Docker + Docker Compose

Цель: освоить контейнеризацию Java-приложений и локальный запуск инфраструктуры (PostgreSQL, Redis, Kafka) через Docker Compose.

#### Ресурсы для изучения

| #    | Ресурс                                                                                           | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 13.1 | Антон Ларичев. Docker + Ansible — с нуля, деплой и управление Swarm | [Stepik](https://stepik.org/course/103647/promo)       |
| 13.2 | RomNero. Docker с 0 до 100%. Всё, что нужно знать                                   | [YouTube](https://www.youtube.com/watch?v=O8N1lvkIjig) |
| 13.3 | freeCodeCamp. Learn Docker — Full DevOps Course for Deploying Containerized Apps                      | [YouTube](https://www.youtube.com/watch?v=rjjES5IsPdg) |

#### Самостоятельно изучаем следующие темы

- **Основы Docker:**

  - container vs image
  - Docker Engine, Docker CLI, Docker Desktop
  - архитектура Docker: Client → Docker Daemon → Registry
  - Docker Hub и private registry — базовое понимание
  - жизненный цикл контейнера
  - immutable infrastructure — понимать принцип
- **Docker CLI:**

  - `docker run`, `docker ps`, `docker stop` / `start` / `restart`, `docker rm`
  - `docker exec`, `docker logs`, `docker inspect`, `docker stats`, `docker cp`
  - `docker pull` / `push`, `docker image ls` / `rm`
  - `docker container prune` / `image prune` / `system prune`, `docker system df`
- **Images:**

  - layers, image ID и tags, digest
  - Dockerfile, build context, `.dockerignore`
  - `docker build`, `docker buildx` — базовое понимание
  - cache при сборке, multi-stage builds
  - разница между image и container
  - почему контейнеры должны быть максимально небольшими
- **Dockerfile:**

  - `FROM`, `RUN`, `COPY`, `ADD` — понимать отличие от `COPY`
  - `WORKDIR`, `ENV`, `ARG`, `EXPOSE`, `USER`
  - `ENTRYPOINT`, `CMD`, `HEALTHCHECK`
  - порядок инструкций и влияние на cache
  - запуск приложения от non-root пользователя
- **Containers:**

  - foreground / detached mode
  - port mapping
  - environment variables
  - container filesystem, writable layer
  - restart policies, healthcheck, graceful shutdown
  - PID 1 и обработка сигналов — базовое понимание
- **Storage:**

  - volumes, bind mounts, tmpfs
  - `docker volume create` / `inspect` / `rm`
  - persistent data
  - почему данные БД нельзя хранить только внутри container filesystem
- **Networking:**

  - bridge network, host network — понимать назначение
  - container-to-container communication
  - DNS внутри Docker network
  - ports и `EXPOSE` — понимать разницу
  - published ports, custom networks
  - frontend / backend network
  - service discovery в Compose
- **Логи и диагностика:**

  - `docker logs`, `docker inspect`, `docker stats`
  - container exit codes, restart loops, healthcheck failures
  - проблемы с ports, volumes, networks
  - image / container debugging
  - базовый алгоритм поиска проблем в контейнеризированном приложении
- **Docker Compose:**

  - `compose.yaml` / `docker-compose.yml`
  - services, image, build, ports, environment, env_file
  - volumes, networks, depends_on, healthcheck, restart
  - profiles, secrets, configs — базовое понимание
  - `docker compose up` / `up -d` / `down`
  - `docker compose build`, `docker compose up --build`
  - `docker compose ps`, `logs`, `exec`, `run`, `restart`, `pull`, `config`, `start` / `stop`
- **Docker + Spring Boot + PostgreSQL:**

  - Java / Spring Boot application, PostgreSQL
  - отдельные networks
  - persistent volume для PostgreSQL
  - environment variables, application configuration
  - healthcheck, корректный порядок запуска сервисов
  - локальная разработка через Docker Compose
  - создание Docker image для Spring Boot application
  - multi-stage build с Maven
  - запуск JAR внутри контейнера
  - конфигурация через environment variables
  - Spring Profiles: dev / test / prod
  - подключение Spring Boot к PostgreSQL в Docker network
  - настройка `server.port`, graceful shutdown
  - healthcheck для Spring Boot Actuator — базовое понимание
  - правильное хранение secrets и credentials
- **Docker Security:**

  - запуск container от non-root пользователя
  - минимальные base images
  - не хранить passwords / API keys в Dockerfile
  - `.dockerignore`, secrets
  - базовое понимание image vulnerabilities
  - принцип least privilege
  - почему container isolation ≠ полноценная виртуальная машина
- **Docker Registry:**

  - Docker Hub
  - `docker login`, `docker tag`, `docker push`, `docker pull`
  - private registry — базовое понимание
  - image tags vs immutable digest
- **Docker Swarm:**

  - Swarm architecture, manager / worker nodes
  - `docker swarm init` / `join` / `leave`
  - node, service, task, replica
  - `docker service create` / `ls` / `ps` / `inspect` / `logs` / `scale` / `update` / `rm`
  - replicated vs global services
  - overlay networks, service discovery, load balancing
  - desired state / reconciliation
  - rolling updates, rollback
  - resource limits и reservations, placement constraints
  - Docker secrets, Docker configs, stacks
  - `docker stack deploy` / `services` / `ps` / `rm`
  - связь Compose file → Docker Swarm stack
  - понимать, чем Docker Compose отличается от Docker Swarm
  - знать, что в индустрии доминирует Kubernetes, а Swarm используется в небольших проектах и для обучения
- **Docker + Ansible:**

  - базовое понимание роли Ansible в автоматизации Docker-инфраструктуры
  - inventory, playbook, task, module, variables, handlers, idempotency
  - управление Docker-хостами через Ansible
  - автоматизация установки и настройки Docker
  - автоматизация deployment
  - понимать отличие Ansible от Docker и Docker Swarm
- **Практика:** самостоятельно контейнеризировать Spring Boot REST API:

  - подключить PostgreSQL через Docker Compose
  - создать production-like Dockerfile с multi-stage build
  - настроить environment variables и Spring profiles
  - настроить Docker networks и persistent volume для PostgreSQL
  - добавить healthcheck
  - проверить запуск, остановку, перезапуск и диагностику контейнеров
  - собрать Docker image и разместить его в Docker Hub
  - развернуть приложение в Docker Swarm
  - выполнить scaling, rolling update и rollback
  - использовать Docker Secrets
  - автоматизировать часть deployment через Ansible
  - разместить итоговый проект на GitHub
  - проверить работу REST API после контейнеризации
  - выполнить integration-тесты против PostgreSQL в Docker

#### Дополнительная литература

- Nigel Poulton — «Docker Deep Dive» (5th ed., 2025) → основная книга для систематизации Docker. Контейнеры, images, Dockerfile, networking, storage, security, Docker Compose и Swarm. Лучший выбор как основная книга после прохождения курса
- Sean P. Kane, Karl Matthias — «Docker: Up & Running» (3rd ed., 2023) → практическое руководство по Docker и контейнеризации. Полезно для закрепления рабочих сценариев и понимания Docker в production. Включает современные возможности: BuildKit, multi-stage builds, security
- Ian Miell, Aidan Hobson Sayers — «Docker in Practice» (2nd ed., 2019) → более 100 практических рецептов по работе с Docker: от базовых операций до сложных сценариев развёртывания и отладки. Хорошо дополняет теоретические книги
- Elton Stoneman — «Learn Docker in a Month of Lunches» (2nd ed., 2025) → практическое введение в Docker в формате коротких уроков. Подходит для быстрого старта и закрепления CLI-команд и Docker Compose

### 14. CI/CD (GitHub Actions)

Цель: освоить непрерывную интеграцию и доставку с помощью GitHub Actions — автоматизация сборки, тестирования, публикации Docker-образов и деплоя приложений.

| #    | Ресурс                                                                                                                                                                  | Ссылка                                        |
| ---- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 14.1 | Павел Сорокин. Почему каждый разработчик должен знать CI/CD в 2026? | [YouTube](https://www.youtube.com/watch?v=AxG9dA72IJQ) |
| 14.2 | Быть Программистом. Полный курс по GitHub Actions — автоматизация CI/CD на GitHub с нуля до продвинутого уровня (на примере WordPress) | [YouTube](https://www.youtube.com/playlist?list=PL2CKgzoZxvxUgafrEtnzBcr7SBMfTBH80) |
| 14.3 | La Tecnología Avanza. CI/CD desde cero con GitHub Actions y Spring Boot (Guía completa) — звуковую дорожку настраиваем на английский | [YouTube](https://www.youtube.com/watch?v=m9zY0nZI3dI) |
| 14.4 | Ali Bouali. Production Deployment On VPS Using Docker & Github Actions pipeline | [YouTube](https://www.youtube.com/watch?v=QI7ZAlwJ2rY) |

#### Самостоятельно изучаем следующие темы

- Основы CI/CD:
  - Что такое Continuous Integration?
  - Что такое Continuous Delivery?
  - Что такое Continuous Deployment?
  - Отличие CI / CD / CD
  - Зачем нужен CI/CD pipeline?
  - Этапы pipeline: build → test → package → deploy
  - Обратная связь и раннее обнаружение проблем
  - Автоматизация vs ручные проверки
- GitHub Actions — основы:
  - workflow
  - event / trigger
  - job
  - step
  - action
  - runner
  - контекст и переменные окружения
  - секреты
  - артефакты
  - кэширование
- Workflow:
  - .github/workflows/*.yml
  - name, on, jobs, steps
  - runs-on
  - uses, with, run
  - env, secrets
  - if, needs
  - strategy / matrix
  - concurrency
  - permissions
- Triggers:
  - push
  - pull_request
  - workflow_dispatch
  - schedule
  - release
  - фильтрация по веткам и путям
- Jobs и Steps:
  - параллельные и последовательные jobs
  - зависимости между jobs (needs)
  - matrix builds
  - reusable workflows
  - composite actions
  - условия выполнения
- Java / Maven в GitHub Actions:
  - checkout репозитория
  - установка JDK (actions/setup-java)
  - Maven dependency cache
  - mvn test
  - mvn verify
  - mvn package
  - запуск integration tests
  - Testcontainers в CI
  - публикация test reports
- Docker в GitHub Actions:
  - сборка Docker image
  - multi-stage build в CI
  - docker build
  - docker buildx
  - кэширование слоёв
  - публикация image в GitHub Container Registry (GHCR) / Docker Hub
  - тегирование images
- Сикреты и безопасность:
  - GitHub Secrets
  - environment secrets
  - repository secrets
  - organization secrets
  - OIDC и аутентификация без долгоживущих секретов — концептуально
  - принцип least privilege
  - защита от утечек секретов
  - secrets в логах
- Артефакты:
  - сохранение build artifacts
  - test reports
  - coverage reports
  - Docker images как artifacts
  - срок хранения artifacts
- CI pipeline для Java Backend:
  - checkout
  - установка JDK
  - Maven dependency cache
  - mvn test
  - integration tests
  - Testcontainers в CI
  - mvn package
  - сборка Docker image
  - публикация Docker image
  - static analysis
- CD — Continuous Deployment:
  - deployment в staging
  - deployment в production
  - environment-specific configuration
  - secrets management
  - health checks после deployment
  - smoke tests
  - rollback при неудачном deployment
  - ручное подтверждение для production
  - GitHub Environments
- Продвинутые темы:
  - reusable workflows
  - composite actions
  - self-hosted runners — концептуально
  - caching strategies
  - matrix builds
  - concurrency control
  - workflow dispatch с параметрами
  - scheduled workflows
- Мониторинг и observability CI:
  - статус workflow
  - логи jobs
  - уведомления о падении
  - анализ времени выполнения pipeline
  - оптимизация pipeline
- Troubleshooting CI:
  - почему workflow падает?
  - проблемы с кэшем
  - проблемы с секретами
  - проблемы с Docker build в CI
  - проблемы с Testcontainers в CI
  - проблемы с зависимостями
  - проблемы с permissions

#### Обязательная самостоятельная практика

- GitHub Actions — базовый pipeline. На собственном Spring Boot + Maven проекте:
  - создать GitHub repository
  - настроить workflow
  - запускать CI на push и Pull Request
  - выполнять mvn test
  - выполнять integration tests
  - настроить Maven dependency cache
  - разделить workflow на несколько jobs
  - использовать зависимости между jobs
  - использовать GitHub Secrets
  - настроить автоматическую сборку JAR
  - добиться полностью рабочего CI pipeline
- Docker + GitHub Actions:
  - написать production-oriented Dockerfile
  - использовать multi-stage build
  - запускать приложение от non-root пользователя
  - передавать настройки через environment variables
  - добавить healthcheck
  - собрать Docker image
  - запустить приложение локально
  - проверить logs, inspect, exec, stats
  - опубликовать image в container registry
  - добавить сборку Docker image в GitHub Actions
- CD pipeline:
  - deployment в staging
  - smoke tests
  - ручное подтверждение для production
  - deployment в production
  - health checks после deployment
  - rollback при неудачном deployment
- Troubleshooting. Намеренно сломать конфигурацию и самостоятельно восстановить. Для каждой проблемы определить: симптом → диагностика → причина → исправление → проверка. Список кейсов:
  - GitHub Actions workflow
  - Docker build
  - Docker networking
  - PostgreSQL connection
  - Docker healthcheck
  - deployment
  - secrets
  - permissions

#### Дополнительная литература
- Gene Kim, Jez Humble, Patrick Debois, John Willis — «The DevOps Handbook» → для понимания DevOps-подхода целиком: CI/CD, automation, deployment, feedback loops, monitoring и культура эксплуатации. Не технический справочник, а книга для формирования системного понимания DevOps
- Jez Humble, David Farley — «Continuous Delivery» → Фундаментальная книга по Continuous Integration, Continuous Delivery, deployment pipelines, automated testing, environments и снижению рисков релизов. Особенно полезна для понимания того, почему CI/CD pipeline строится именно как последовательность автоматизированных проверок и deployment stages
- Nigel Poulton — «Docker Deep Dive» (5th ed., 2025) → основная книга для систематизации Docker. Контейнеры, images, Dockerfile, networking, storage, security, Docker Compose и Swarm. Лучший выбор как основная книга после прохождения курса
- Matthew Skelton, Manuel Pais — «Team Topologies» → Полезна для понимания организации delivery-процессов, взаимодействия development и operations и принципов эффективного software delivery
- Brent Laster — «Learning GitHub Actions: Automation and Integration of CI/CD with GitHub» → практическое руководство именно по GitHub Actions: workflows, triggers, jobs, steps, actions, secrets, artifacts, caching, matrix builds, reusable workflows, безопасность, построение CI/CD pipeline и интеграция с Docker и deployment. Хорошо закрывает инструментальную часть раздела, дополняя книги по DevOps-культуре и Continuous Delivery.

### 15. Инфраструктурные компоненты

Цель: освоить Redis, RabbitMQ, Kafka и Elasticsearch — их назначение, паттерны применения и интеграцию с Spring Boot.

#### Ресурсы для изучения

**Redis:**

| #    | Ресурс                                                                          | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 15.1 | Евгений Сулейманов. Основы Redis                               | [YouTube](https://www.youtube.com/watch?v=Tw_-3sHDeyA) |
| 15.2 | Файсал Мемон. Redis Masterclass for Spring Boot Developers                 | [YouTube](https://www.youtube.com/watch?v=Pvc3DIr3Q1g) |
| 15.3 | DavinchiCoder. Domina Redis con Java 25 y Spring Boot 4: Cache, Locks, Streams y más | [YouTube](https://www.youtube.com/watch?v=48ZRIY-LyCs) |

**RabbitMQ:**

| #    | Ресурс                                                                                      | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 15.4 | Кирилл Сачков. RabbitMQ: полный гайд для разработчика (2026) | [YouTube](https://www.youtube.com/watch?v=7rxOg8mV1PE) |
| 15.5 | Файсал Мемон. Очереди сообщений с RabbitMQ                            | [YouTube](https://www.youtube.com/watch?v=dBdw1vN1WQE) |
| 15.6 | Java Guides. Spring Boot RabbitMQ Tutorial — Consumer, Producer, Crash Course 2025               | [YouTube](https://www.youtube.com/watch?v=0--Ll3WHMTQ) |

**Kafka:**

| #     | Ресурс                                                                                              | Ссылка                                        |
| ----- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 15.7  | Влад Мишустин. Лучший гайд по Kafka для начинающих за 1 час     | [YouTube](https://www.youtube.com/@fakng-engineer)     |
| 15.8  | JavaGuru. Apache Kafka | [YouTube](https://www.youtube.com/watch?v=64ZBMgnXTow&list=PLt91xr-Pp57Q50WsXz9r-zmxy5ceu_hp_)     |
| 15.9  | Java Techie. Apache Kafka Crash Course with Spring Boot 3.0.x                                             | [YouTube](https://www.youtube.com/watch?v=c7LPlWvxZcQ) |
| 15.10  | Файсал Мемон. Apache Kafka Course for Beginners with Spring Boot Project, Spring Cloud Streams | [YouTube](https://www.youtube.com/watch?v=NWLwGtkBrkQ) |
| 15.11 | Олег Тодор. Apache Kafka Java: продвинутый                                            | [Stepik](https://stepik.org/course/243796/promo)       |

**Elasticsearch:**

| #     | Ресурс                                                                                            | Ссылка                                                                                |
| ----- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 15.12 | Денис Сучков. Elasticsearch: всё, что нужно знать за 30 минут         | [YouTube](https://www.youtube.com/watch?v=vxE1aGTEnbE)                                         |
| 15.13 | EnggAdda. Elasticsearch                                                                                 | [YouTube](https://www.youtube.com/watch?v=FeUAT7PhTXk&list=PLoNChWlyFPxcB-jY277teAoJXtNNCcifM) |
| 15.14 | Lilium Code. Mastering Spring Data Elasticsearch: A Comprehensive Guide to Integration with Spring Boot | [YouTube](https://www.youtube.com/watch?v=XNAyiX6_shQ&list=PLXy8DQl3058P-mqOmuVu98HLhohnP_hz1) |

#### Обязательная самостоятельная практика

Создать интеграционный проект, объединяющий Java + Spring Boot + PostgreSQL + Redis + RabbitMQ + Kafka + Elasticsearch.

- **Архитектура проекта:**

  - Spring Boot REST API
  - PostgreSQL — основная транзакционная БД и Source of Truth
  - Redis — кэширование и распределённые механизмы
  - RabbitMQ — асинхронные команды / очереди задач
  - Kafka — событийная передача данных и Event Streaming
  - Elasticsearch — поисковая проекция данных
  - Docker Compose — запуск всей инфраструктуры
- **Redis:**

  - реализовать Cache-Aside
  - настроить TTL
  - реализовать cache invalidation
  - использовать Redis для кэширования результатов REST API
  - реализовать распределённую блокировку
  - изучить проблему cache stampede и способы её предотвращения
  - проверить поведение приложения при недоступности Redis
- **RabbitMQ:**

  - реализовать Producer и Consumer
  - создать Exchange, Queue, Binding и Routing Key
  - использовать Direct / Topic / Fanout
  - реализовать manual ACK / NACK
  - настроить prefetch
  - реализовать retry
  - реализовать Dead Letter Exchange / Dead Letter Queue
  - обеспечить idempotency Consumer
  - настроить publisher confirms
  - проверить поведение при падении Consumer и RabbitMQ
- **Kafka:**

  - создать несколько Topics
  - реализовать Producer и Consumer
  - использовать Partition
  - настроить Consumer Groups
  - изучить Offset и Commit
  - проверить ordering
  - реализовать несколько Consumer
  - реализовать retry / DLT
  - использовать idempotent producer
  - изучить базовый сценарий exactly-once / transactional processing
  - проверить масштабирование Consumer Group
- **Transactional Outbox Pattern:**

  - проблема dual write
  - запись изменения в PostgreSQL + запись события в outbox в одной транзакции
  - публикация событий из outbox
  - retry
  - idempotency
  - eventual consistency
  - понимание роли Debezium / CDC — концептуально
- **Elasticsearch:**

  - создать Index
  - определить Mapping
  - реализовать первоначальную индексацию
  - реализовать incremental indexing
  - реализовать обновление и удаление документов
  - реализовать полнотекстовый поиск
  - реализовать фильтрацию
  - реализовать сортировку
  - реализовать пагинацию
  - реализовать autocomplete
  - реализовать aggregations
  - использовать aliases
  - реализовать reindex
  - проверить refresh и eventual consistency
- **Интеграция PostgreSQL → Messaging → Elasticsearch:**

  - PostgreSQL остаётся Source of Truth
  - изменение данных в PostgreSQL должно приводить к публикации события
  - передать событие через RabbitMQ и / или Kafka
  - Consumer обновляет Elasticsearch
  - реализовать обработку Create / Update / Delete
  - обеспечить idempotency
  - реализовать retry
  - обработать потерю / повторную доставку сообщения
  - реализовать восстановление Elasticsearch из PostgreSQL
  - реализовать полную повторную индексацию
  - продемонстрировать eventual consistency между PostgreSQL и Elasticsearch
- **Отказоустойчивость и диагностика:**

  - остановить Redis и проверить поведение приложения
  - остановить RabbitMQ
  - остановить Kafka
  - остановить Elasticsearch
  - проверить retry и DLQ / DLT
  - проверить повторную обработку сообщений
  - проверить идемпотентность
  - проверить потерю и восстановление соединения
  - добавить структурированные логи
  - добавить correlation / request ID
  - использовать Actuator для health-check
  - проверить состояние всех инфраструктурных компонентов

#### Дополнительная литература

- Josiah L. Carlson — «Redis in Action» → практическая книга по Redis: структуры данных, кэширование, очереди, публикация / подписка и практические паттерны применения Redis. Использовать как справочник, а не читать целиком от начала до конца
- Alvaro Videla, Jason J. W. Williams — «RabbitMQ in Action» → хорошая фундаментальная книга по AMQP, exchanges, queues, routing, acknowledgements и построению приложений с RabbitMQ. Издание старое, поэтому современные особенности RabbitMQ сверять с актуальной документацией
- Gwen Shapira, Todd Palino, Rajini Sivaram, Krit Petty — «Kafka: The Definitive Guide» → основной дополнительный источник по архитектуре Kafka: topics, partitions, replication, consumer groups, delivery semantics и эксплуатация. Хорошо дополняет продвинутый курс Олега Тодора
- Clinton Gormley, Zachary Tong — «Elasticsearch: The Definitive Guide» → сильный источник для понимания индексов, mappings, анализаторов, поиска, relevance, aggregations и внутренней модели Elasticsearch. Использовать преимущественно как справочник по фундаментальным концепциям; актуальные возможности Elasticsearch сверять с современной документацией
- Martin Kleppmann, Chris Riccomini — «Designing Data-Intensive Applications» (2nd ed.) → главная дополнительная книга не по конкретному инструменту, а по архитектуре распределённых систем: репликация, партиционирование, транзакции, консистентность, очереди, event streams, отказоустойчивость и обработка данных. Особенно полезна для понимания того, зачем в реальной системе одновременно могут использоваться PostgreSQL, Redis, RabbitMQ, Kafka и Elasticsearch

### 16. Observability basics

**Цель:** научиться наблюдать за работой production-like приложения, собирать и анализировать logs, metrics и traces, находить причины проблем и настраивать базовый monitoring, alerting и SLI/SLO.

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 16.01 | Уголок сельского джависта. Actuator, Micrometer, Victoria Metrics, Grafana - Мониторинг Spring Boot | [YouTube](https://www.youtube.com/watch?v=EMQN5Vr837o)        |
| 16.02 | José Cruz (IT Architect). Mastering Micrometer in Spring Boot: Metrics, Prometheus & Observability Explained | [YouTube](https://www.youtube.com/watch?v=kcUYneEVtEI)        |
| 16.03 | kirya522. Сбор метрик Spring Boot приложения c помощью Prometheus и Grafana | [Хабр](https://habr.com/ru/articles/548700/)        |
| 16.04 | sproshchaev. Как настроить observability в Spring Boot 3 | [Хабр](https://habr.com/ru/companies/otus/articles/1031290/)        |
| 16.05 | sproshchaev. Spring Boot Actuator: полный гайд по мониторингу в 2026 | [Хабр](https://habr.com/ru/companies/otus/articles/1008360/)        |

#### Самостоятельно изучаем следующие темы

- Observability:
  - что такое observability?
  - monitoring vs observability
  - logs / metrics / traces
  - три основных сигнала observability
  - как observability помогает находить и диагностировать проблемы?

- Logging:
  - уровни логирования: TRACE / DEBUG / INFO / WARN / ERROR
  - structured logging
  - JSON logs
  - correlation ID / request ID
  - что следует и что не следует писать в logs?
  - log rotation и retention
  - centralized logging

- Metrics:
  - что такое metrics?
  - counter / gauge / histogram / timer
  - latency
  - throughput
  - error rate
  - JVM / system / application metrics
  - custom metrics

- Spring Boot:
  - Spring Boot Actuator
  - health checks
  - liveness / readiness
  - application / JVM metrics
  - Micrometer
  - custom metrics
  - безопасность Actuator endpoints

- Prometheus + Grafana:
  - Prometheus
  - scraping
  - exporters
  - PromQL
  - Grafana
  - dashboards
  - alerts

- Distributed Tracing:
  - trace / span
  - parent / child spans
  - trace ID / span ID
  - context propagation
  - OpenTelemetry
  - distributed tracing в микросервисах

- Centralized Logging:
  - зачем централизовать logs?
  - ELK / Elastic Stack
  - Loki
  - log aggregation
  - поиск и фильтрация logs
  - correlation ID для поиска запроса между сервисами

- Alerting:
  - зачем нужны alerts?
  - alert conditions
  - error rate
  - latency
  - availability
  - resource utilization
  - actionable alerts
  - alert fatigue

- SLI / SLO:
  - SLI — Service Level Indicator
  - SLO — Service Level Objective
  - SLA — Service Level Agreement
  - availability SLI
  - latency SLI
  - error rate SLI
  - error budget
  - различия SLI / SLO / SLA

- Troubleshooting:
  - поиск проблем по logs
  - поиск проблем по metrics
  - поиск проблем по traces
  - correlation ID / trace ID при расследовании ошибок
  - связь между logs, metrics и traces

#### Практика

Реализовываем observability для Spring Boot-приложения:
- создать или использовать существующее Spring Boot-приложение
- подключить Spring Boot Actuator
- настроить health / liveness / readiness checks
- подключить Micrometer
- добавить application metrics
- добавить custom metric
- поднять Prometheus через Docker Compose
- настроить сбор metrics с Spring Boot-приложения
- подключить Grafana
- создать dashboard с основными метриками:
  - request rate
  - error rate
  - response time / latency
  - JVM memory
  - CPU
  - active requests
- добавить structured logging
- добавить correlation ID / request ID
- поднять централизованный сбор logs через Loki
- подключить logs к Grafana
- подключить OpenTelemetry для traces
- настроить distributed tracing и context propagation
- связать trace ID с logs
- создать несколько alerts:
  - высокий error rate
  - высокая latency
  - недоступность приложения
- искусственно создать:
  - HTTP 5xx ошибки
  - повышенную latency
  - недоступность PostgreSQL
- найти и диагностировать проблемы:
  - по logs
  - по metrics
  - по traces
- сформулировать 2–3 SLI и SLO для приложения
- проверить работу observability после перезапуска контейнеров
- описать, какие данные помогают обнаружить проблему и какие — установить её причину

#### Дополнительная литература

- Charity Majors, Liz Fong-Jones, George Miranda — «Observability Engineering: Achieving Production Excellence, 2nd Edition» → Современное системное руководство по observability: logs, metrics, traces, debugging production systems, observability-driven development и диагностике проблем распределённых систем. Особенно полезна как основная дополнительная книга к разделу. Второе издание вышло в 2026 году.
- Cindy Sridharan — «Distributed Systems Observability» → Короткое, но концентрированное введение в observability распределённых систем: monitoring vs observability, alerting, logs, metrics, tracing и debugging. Хорошо подходит для закрепления концептуальной части раздела.
- Betsy Beyer, Chris Jones, Christof Leng, David Huska, Jennifer Petoff, Niall Richard Murphy — «Site Reliability Engineering: How Google Runs Production Systems, 2nd Edition» → Системное руководство по эксплуатации надёжных production-систем: monitoring, SLO, alerting, troubleshooting, incident management, load balancing и работа с перегрузками. Второе издание вышло в 2026 году.
- Betsy Beyer, Niall Richard Murphy, David K. Rensin, Kent Kawahara, Stephen Thorne — «The Site Reliability Workbook» → Практическое продолжение SRE Book: SLI/SLO, error budgets, monitoring, alerting, troubleshooting и реальные примеры внедрения SRE-практик. Особенно полезно для перехода от теории observability к эксплуатации production-систем.
- Brian Brazil, Julius Volz — «Prometheus: Up & Running» → Практическое изучение Prometheus: сбор metrics, exporters, PromQL, monitoring и построение системы мониторинга. Использовать как дополнительную литературу к части Prometheus + Grafana.

### 17. Нагрузочное тестирование

**Цель:** научиться проверять производительность Spring Boot-приложения под нагрузкой, измерять RPS, latency, p95/p99 и error rate, находить bottleneck'и на уровне приложения, JVM и PostgreSQL и оценивать влияние изменений на производительность.

**В целом**

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 17.01 | Алексей Рагозин. Теория и практика нагрузочного тестирования | [YouTube](https://www.youtube.com/watch?v=KxlbwLVrujU)        |

**Apache Jmeter**

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 17.02 | Иван Стрелка. Apache Jmeter - Нагрузочное тестирование | [YouTube](https://www.youtube.com/playlist?list=PLwgnAPg_hK1W6z4JHGvdWd_Su9g5J-gms)        |
| 17.03 | Testing Funda by Zeeshan Asghar. Master Apache JMeter Full Course | [YouTube](https://www.youtube.com/watch?v=Gz57tS1a47g)        |

**Gatling**

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 17.04 | James Willett. Gatling Load Testing - Ultimate Crash Course Tutorial For Beginners | [YouTube](https://www.youtube.com/watch?v=NzqO6AOKjeg)        |
| 17.05 | Code&Test. Gatling. Нагрузочное тестирование | [YouTube](https://www.youtube.com/playlist?list=PLmrN-SZCRElswc_hj53JJ0Gg46STtBfSM)        |

**K6**

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 17.06 | Automation Step by Step. k6 Beginner Tutorials | [YouTube](https://www.youtube.com/playlist?list=PLhW3qG5bs-L9EF8wFBxBY4RU4WzG9X6gd)        |
| 17.07 | Mike Møller Nielsen. K6 Load Impact Insight and Spring Boot | [YouTube](https://www.youtube.com/watch?v=arHiXoS-Keg)        |
| 17.08 | Java holic club. Нагрузочное тестирование K6, grafana c нуля | [YouTube](https://www.youtube.com/watch?v=hsIVOJ6mIm4)        |

#### Самостоятельно изучаем следующие темы

- Основы нагрузочного тестирования:
  - что такое performance testing?
  - load / stress / spike / soak testing
  - volume testing
  - scalability testing
  - отличие load testing от stress testing
  - когда и зачем проводить нагрузочные тесты?

- Нагрузочная модель:
  - virtual users / concurrent users
  - requests per second (RPS)
  - throughput
  - ramp-up / ramp-down
  - duration теста
  - постоянная и ступенчатая нагрузка
  - realistic workload

- Основные метрики:
  - response time / latency
  - average latency
  - min / max latency
  - p5 0 / p90 / p95 / p99
  - throughput / RPS
  - error rate
  - concurrent requests
  - saturation

- Инструменты:
  - Apache JMeter
  - Gatling
  - k6
  - основные различия инструментов
  - когда использовать JMeter, Gatling или k6?

- REST API:
  - нагрузочное тестирование HTTP GET / POST / PUT / DELETE
  - headers
  - query parameters
  - request body
  - authentication
  - сценарии с последовательностью запросов
  - проверка HTTP status codes
  - parameterization / test data

- Java / Spring Boot под нагрузкой:
  - влияние нагрузки на Spring Boot application
  - Tomcat / web server thread pool
  - connection pool
  - database bottlenecks
  - JVM memory
  - Garbage Collector
  - CPU utilization
  - влияние количества concurrent requests

- Поиск bottleneck:
  - CPU-bound vs I/O-bound
  - CPU
  - RAM
  - GC
  - threads
  - connection pool
  - PostgreSQL
  - slow SQL queries
  - network
  - external services
  - как определить компонент, ограничивающий производительность?

- Profiling под нагрузкой:
  - зачем профилировать приложение во время load test?
  - Java Flight Recorder (JFR)
  - Java Mission Control (JMC)
  - thread dumps
  - CPU hotspots
  - memory allocation
  - GC activity
  - blocked / waiting threads
  - связь результатов profiling с результатами нагрузочного теста

- Анализ результатов:
  - как читать результаты load test?
  - построение графиков latency / RPS / error rate
  - анализ p95 / p99
  - поиск деградации производительности
  - сравнение результатов разных запусков
  - определение capacity приложения
  - поиск точки saturation
  - формулирование выводов по результатам тестирования

- Нагрузочное тестирование в CI:
  - запуск тестов в отдельном окружении
  - запуск k6 / JMeter из CI
  - хранение результатов
  - базовые performance thresholds
  - автоматическое обнаружение деградации производительности
  - почему полноценные load tests не всегда запускают на каждом commit?

#### Практика

Реализовываем нагрузочное тестирование Spring Boot REST API:
- создать или использовать существующее Spring Boot-приложение
- подготовить REST API для тестирования
- запустить приложение вместе с PostgreSQL через Docker Compose
- выбрать один из инструментов: JMeter / Gatling / k6
- создать сценарий нагрузочного тестирования REST API
- протестировать GET / POST запросы
- добавить authentication, если она используется приложением
- настроить concurrent users
- выполнить load test
- измерить RPS / throughput / latency / error rate
- проанализировать p95 / p99
- провести load test с постепенным увеличением нагрузки
- провести stress test до появления деградации
- провести короткий spike test
- определить bottleneck приложения
- проверить CPU / RAM / JVM / GC
- проверить connection pool
- проверить PostgreSQL и slow queries
- выполнить profiling приложения под нагрузкой
- использовать JFR / JMC для поиска проблем JVM
- исправить найденный bottleneck
- повторить тест и сравнить результаты до и после оптимизации
- сохранить результаты тестирования
- сформулировать performance baseline
- определить допустимые thresholds для latency / error rate / RPS
- запустить нагрузочный тест в CI или отдельном окружении
- описать результаты тестирования и выявленные ограничения системы

#### Дополнительная литература

- Scott Oaks — «Java Performance: The Definitive Guide» → Производительность Java-приложений: performance testing, throughput, response time, JVM, garbage collection, memory, threads и методы поиска узких мест. Особенно полезна для понимания того, что происходит внутри Spring Boot / JVM под нагрузкой.
- Brendan Gregg — «Systems Performance: Enterprise and the Cloud, 2nd Edition» → Системный подход к анализу производительности: CPU, memory, disks, network, applications, benchmarking, Linux performance tools и методология поиска bottleneck. Использовать выборочно для глубокого понимания причин деградации системы.
- Bayo Erinle — «Performance Testing with JMeter 3: Enhance the Performance of Your Web Application» → Практическое руководство по JMeter: performance testing fundamentals, создание тестовых сценариев, анализ результатов, resource monitoring и distributed testing. Использовать как дополнительную литературу именно к JMeter.
- Ian Molyneaux — «The Art of Application Performance Testing» → Методология performance testing: определение целей, построение workload, performance baseline, проведение load/stress tests, анализ результатов и выявление проблем производительности. Использовать для понимания процесса нагрузочного тестирования целиком.
- Michael T. Nygard — «Release It!, 2nd Edition» → Практика проектирования production-систем, устойчивых к нагрузке и отказам: stability patterns, timeouts, circuit breakers, bulkheads, cascading failures и capacity-related проблемы. Читать выборочно в контексте связи нагрузочного тестирования с надёжностью backend-систем.

## Распределённые системы

### 18. Cloud basics

**Цель:** получить базовое понимание облачной инфраструктуры и научиться самостоятельно разворачивать Spring Boot-приложение в облаке с использованием VM, Docker, managed PostgreSQL, networking, secrets, monitoring и базовых cloud-сервисов.

**GCP / AWS / Azure:**

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 18.01 | freeCodeCamp. Google Cloud Associate Cloud Engineer Course | [YouTube](https://www.youtube.com/watch?v=jpno8FSqpc8)        |
| 18.02 | freeCodeCamp. AWS Solutions Architect Associate Full Course | [YouTube](https://www.youtube.com/watch?v=c3Cn4xYfxJY)        |
| 18.03 | Tech Tutorials with Piyush. AZ-900 Azure Fundamentals | [YouTube](https://www.youtube.com/watch?v=-pX5PjIYTJs)        |

**Yandex Cloud:**

| #   | Ресурс                                                                                                          | Ссылка                                                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 18.04 | Yandex Cloud. about:cloud — infrastructure | [YouTube](https://www.youtube.com/watch?v=XNRVbfUMkS0)        |
| 18.05 | Azzrael Code. Yandex Cloud Functions. Что это и как использовать? (на примере Python) | [YouTube](https://www.youtube.com/watch?v=SYwIFlXg-3w)        |

#### Самостоятельно изучаем следующие темы

- Cloud Computing:
  - что такое облачные вычисления?
  - преимущества и недостатки облака
  - IaaS / PaaS / SaaS — различия и примеры
  - public / private / hybrid cloud
  - shared responsibility model

- Cloud providers:
  - AWS / GCP / Azure / Yandex Cloud
  - основные аналоги сервисов между провайдерами:
    - Compute
    - Object Storage
    - Managed PostgreSQL
    - VPC / Networking
    - IAM
    - Container Registry
    - Kubernetes
    - Serverless

- Compute:
  - VM — виртуальные машины и их основные характеристики
  - containers — контейнеры и отличие от VM
  - serverless / FaaS — когда применять
  - autoscaling и load balancing
  - managed vs self-managed infrastructure

- Storage:
  - object storage — S3-подобное хранилище
  - block storage — диски для VM
  - file storage — файловые системы
  - различия и сценарии использования
  - durability, availability и backup
  - lifecycle policies и versioning

- Managed Databases:
  - что такое managed database?
  - managed PostgreSQL vs PostgreSQL на собственной VM
  - backups, replication, scaling и high availability
  - подключение приложения к managed database

- Networking:
  - VPC / Virtual Network
  - subnet
  - public / private subnet
  - IP-адреса и маршрутизация
  - security groups / firewall rules
  - load balancer
  - DNS
  - NAT
  - базовое понимание ingress / egress traffic

- IAM и безопасность:
  - IAM
  - users / service accounts / roles
  - permissions и policies
  - principle of least privilege
  - authentication vs authorization
  - secrets и secrets management
  - зачем нельзя хранить credentials в Git

- CDN:
  - что такое CDN?
  - edge locations
  - caching
  - зачем CDN используется вместе с object storage и web-приложениями?

- Kubernetes:
  - зачем Kubernetes нужен в облаке?
  - managed Kubernetes vs самостоятельная установка
  - cluster / node / pod / service
  - зачем использовать EKS / GKE / AKS / Managed Kubernetes?
  - когда Kubernetes избыточен для проекта?

- Pricing и Cost Awareness:
  - за что платят в облаке?
  - compute / storage / network costs
  - pay-as-you-go
  - free tier
  - reserved / committed usage
  - как контролировать расходы?
  - budgets, billing alerts и cost monitoring

- Deployment:
  - основные этапы deployment приложения в облако
  - container registry
  - build → containerize → push image → deploy → configure networking → connect database
  - environment variables и secrets
  - logs и monitoring
  - rollback и обновление приложения

- Monitoring:
  - logs
  - metrics
  - health checks
  - alerts
  - базовый monitoring облачных ресурсов и приложения

#### Практика

Реализовываем базовый deployment Spring Boot-приложение в облаке:
- создать VM
- настроить VPC / firewall / security groups
- установить Docker
- собрать Spring Boot-приложение
- создать Docker image
- загрузить image в container registry
- запустить container на VM
- подключить managed PostgreSQL
- настроить environment variables / secrets
- настроить HTTP/HTTPS
- проверить logs / health checks
- проверить доступность API
- проверить работу приложения после перезапуска
- проверить подключение к managed PostgreSQL и сохранность данных
- удалить неиспользуемые ресурсы и проверить расходы

#### Дополнительная литература
- Thomas Erl, Eric Barcelo Monroy — «Cloud Computing: Concepts, Technology, Security, and Architecture» → Системное введение в cloud computing: IaaS / PaaS / SaaS, deployment models, cloud architecture, security, virtualization и orchestration. Использовать для формирования общего понимания облачной инфраструктуры независимо от конкретного провайдера
- Cornelia Davis — «Cloud Native Patterns» → Паттерны разработки и эксплуатации cloud-native приложений: statelessness, scaling, configuration, service discovery, resilience, routing, distributed tracing и взаимодействие сервисов. Особенно полезна для понимания того, как меняется архитектура приложения при переносе в облако.
- Justin Domingus, John Arundel — «Cloud Native DevOps with Kubernetes, 2nd Edition» → Практическое руководство по cloud-native подходу, контейнерам, Kubernetes, DevOps и эксплуатации приложений в облачной среде. Читать выборочно после освоения Docker и базовых Kubernetes-концепций.
- Brendan Burns, Joe Beda, Kelsey Hightower, Lachlan Evenson — «Kubernetes: Up and Running, 3rd Edition» → Практическое введение в Kubernetes: containers, cluster, pods, services, networking, health checks, resource limits, scaling, deployment и monitoring. Использовать как дополнительную литературу к базовому Kubernetes из раздела Cloud.
- J.R. Storment, Mike Fuller — «Cloud FinOps, 2nd Edition» → Понимание стоимости облачной инфраструктуры: cloud billing, cost allocation, forecasting, optimization, контейнерные расходы и взаимодействие разработчиков с FinOps. Использовать для развития практического понимания Cloud Cost Awareness.

### 19. System Design (HLD)

Цель: освоить высокоуровневое проектирование распределённых систем — capacity planning, выбор компонентов, масштабирование, надёжность и trade-offs.

**HLD (High-Level Design)** — высокоуровневое проектирование архитектуры системы: выбор компонентов, их взаимодействие, масштабирование, надёжность и trade-offs. Противопоставляется **LLD (Low-Level Design)** — проектированию на уровне классов и модулей.

**Основные ресурсы**

| #    | Ресурс                                                                                                              | Ссылка                                               |
| ---- | ------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| 19.1 | Иван Зинченко. C нуля до проектирования систем уровня senior-инженера | [Stepik](https://stepik.org/course/240911/promo)              |
| 19.2 | JavaGuru. Микросервисная архитектура | [YouTube](https://www.youtube.com/watch?v=7EPZzA79Xww&list=PLt91xr-Pp57T4kKLdavnQ0gV1X427frC2&index=48)              |
| 19.3 | Антон Назаров. Все про System Design | [YouTube](https://www.youtube.com/watch?v=HHQTVvMXadE)        |
| 19.4 | donnemartin. The System Design Primer                                                                                     | [GitHub](https://github.com/donnemartin/system-design-primer) |

**Статьи на Хабре**

| #    | Ресурс                                                                                                                                                                                                                   | Ссылка                                   |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------- |
| 19.5 | koreandr94. System Design для самых маленьких. Reference к интервью                                                                                                                                  | [Хабр](https://habr.com/ru/articles/747112/)  |
| 19.6 | polyakovin. Конспект по архитектуре ПО и System Design                                                                                                                                                 | [Хабр](https://habr.com/ru/articles/888202/)  |
| 19.7 | AndrewDeveloper. System Design на практике: создаём систему сокращения ссылок от проектирования архитектуры до развёртывания в облаке | [Хабр](https://habr.com/ru/articles/1052938/) |
| 19.8 | offiziellen. Шардирование баз данных: проблемы, альтернативы, практические рекомендации                                                                       | [Хабр](https://habr.com/ru/articles/916394/)  |
| 19.9 | pahomovda. Проектирование эффективной системы кэширования для высоконагруженной системы                                                                  | [Хабр](https://habr.com/ru/articles/804205/)  |

#### Самостоятельная практика System Design

Для каждой задачи проходить полный цикл проектирования:

- **Requirements:**

  - functional requirements
  - non-functional requirements
  - ограничения и out of scope
  - приоритеты требований
- **Capacity Planning:**

  - DAU / MAU
  - RPS / QPS
  - read / write ratio
  - peak load
  - storage
  - network bandwidth
  - приблизительная оценка ресурсов
- **API и основные сценарии:**

  - основные API / endpoints
  - ключевые user flows
  - требования к latency и consistency
- **HLD:**

  - Client
  - Load Balancer
  - API Gateway / BFF при необходимости
  - application services
  - cache
  - databases
  - queues / brokers
  - external systems
- **Data Design:**

  - выбор типа хранилища
  - основные сущности и access patterns
  - индексы
  - replication
  - partitioning / sharding при необходимости
- **Scalability:**

  - vertical / horizontal scaling
  - load balancing
  - caching
  - replication
  - sharding
  - asynchronous processing
- **Reliability:**

  - single points of failure
  - timeout / retry
  - idempotency
  - rate limiting
  - graceful degradation
  - backup / recovery
  - observability
  - failure scenarios
- **Trade-offs:**

  - почему выбран именно этот подход
  - какие есть альтернативы
  - какие новые проблемы создаёт выбранное решение

**Обязательные System Design задачи:**

1. **URL Shortener** — спроектировать сервис сокращения ссылок наподобие Bitly
2. **Notification Service** — спроектировать сервис отправки Email / SMS / Push-уведомлений с очередями, retry, idempotency и защитой от дублирования
3. **Social Network Feed** — спроектировать ленту социальной сети с большим количеством пользователей и высокой нагрузкой на чтение
4. **Hotel Booking System** — спроектировать систему бронирования отелей с поиском, проверкой доступности, конкурентными запросами и защитой от двойного бронирования
5. **File Storage / Image Hosting** — спроектировать сервис хранения и раздачи файлов / изображений с object storage, CDN, caching и масштабированием

Для задач №3–5 дополнительно проработать:

- capacity planning
- replication / sharding
- caching
- очереди и асинхронную обработку
- rate limiting
- failure scenarios
- graceful degradation
- multi-region / disaster recovery на концептуальном уровне

Для каждой задачи подготовить:

- архитектурную схему
- API
- краткое письменное обоснование решений
- список bottlenecks
- список trade-offs
- 2–3 альтернативных архитектурных решения

Цель практики — научиться самостоятельно проходить путь: **требования → оценки → API → архитектура → данные → масштабирование → надёжность → trade-offs**.

#### Дополнительная литература

- Alex Xu — «System Design Interview: An Insider's Guide, Vol. 1» → практическая база по System Design Interview: требования, capacity planning, API, storage, caching, queues, scaling, load balancing и reliability. Большое количество типовых задач позволяет отработать сам алгоритм проектирования
- Alex Xu, Sahn Lam — «System Design Interview: An Insider's Guide, Vol. 2» → продолжение Vol. 1 с более сложными системами и архитектурными trade-off. Полезно после освоения базового подхода для расширения практики и усложнения System Design задач
- Martin Kleppmann, Chris Riccomini — «Designing Data-Intensive Applications» (2nd ed.) → главная книга для глубокого понимания data-intensive и distributed systems: storage, replication, partitioning, transactions, consistency, consensus, batch / stream processing и trade-off архитектурных решений. Переход от HLD к глубокому пониманию того, как работают распределённые системы
- Mark Richards, Neal Ford — «Fundamentals of Software Architecture» (2nd ed.) → систематизация архитектурного мышления: architectural characteristics, архитектурные стили и паттерны, coupling, cohesion, компоненты, partitioning и принятие архитектурных решений. Особенно хорошо связывает System Design с разделом Backend Architecture
- Neal Ford, Mark Richards, Pramod Sadalage, Zhamak Dehghani — «Software Architecture: The Hard Parts» → продвинутый разбор сложных архитектурных компромиссов: service boundaries, distributed architecture, data ownership, consistency, coupling и evolutionary architecture. Главная ценность книги — умение принимать архитектурные решения там, где нет одного правильного варианта

### 20. Микросервисы и распределённые системы

Цель: научиться проектировать и реализовывать микросервисные системы — Saga, Outbox, Kafka, идемпотентность, отказоустойчивость.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                                   | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 20.1 | Евгений Сулейманов. Микросервисы и распределённые системы                   | [YouTube](https://www.youtube.com/watch?v=V4oFJ3LbW9s) |
| 20.2 | Павел Сорокин. Пишем Яндекс.Еду за 2 часа — архитектура микросервисов | [YouTube](https://www.youtube.com/watch?v=qkz5EFwKZuI) |
| 20.3 | Григорий Кислин. Микросервисы, Docker, Kafka, Spring Cloud, реактивный стек            | [Stepik](https://stepik.org/course/213010/promo)       |
| 20.4 | Programming Techie. Spring Boot Microservice Project Full Course in 6 Hours                                                    | [YouTube](https://www.youtube.com/watch?v=mPPhcU7oWDU) |

**Статьи на Хабре:**

| #    | Ресурс                                                                                                                                                        | Ссылка                                   |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| 20.5 | ivankov_timofei. Основные паттерны микросервисной архитектуры: Strangler Fig, API Gateway, Service Mesh и другие    | [Хабр](https://habr.com/ru/articles/904954/)  |
| 20.6 | offiziellen. Взаимодействие микросервисов: проблемы, решения, практические рекомендации           | [Хабр](https://habr.com/ru/articles/933110/)  |
| 20.7 | ivankov_timofei. Распределённые транзакции в микросервисах: от SAGA до Two-Phase Commit                                   | [Хабр](https://habr.com/en/articles/906484/)  |
| 20.8 | MiSta1984. Паттерн Transactional Outbox на примере двух микросервисов на Java                                                    | [Хабр](https://habr.com/ru/articles/991934/)  |
| 20.9 | tquality. Как тестировать распределённые системы: тайм-ауты, дубликаты, Saga и частичные отказы | [Хабр](https://habr.com/ru/articles/1070068/) |

#### Самостоятельная практика: учебная микросервисная система

Реализовать систему на Java / Spring Boot из 3–5 сервисов:

- API Gateway
- Order Service
- Payment Service
- Inventory Service
- Notification Service

**Архитектура должна включать:**

- отдельную БД для каждого сервиса (Database per Service)
- REST для синхронного взаимодействия
- Kafka для асинхронного взаимодействия
- Transactional Outbox
- идемпотентность consumer'ов
- timeout + retry
- Circuit Breaker
- Saga
- централизованные логи
- distributed tracing
- metrics
- integration tests с Testcontainers

**Обязательно реализовать и проверить следующие failure scenarios:**

1. недоступность одного из сервисов
2. timeout при межсервисном вызове
3. потеря ответа после успешного выполнения операции
4. повторная доставка сообщения
5. получение сообщения в неожиданном порядке
6. недоступность Kafka
7. падение consumer
8. ошибка на одном из шагов Saga
9. ошибка компенсационной операции
10. восстановление сервиса после отказа и обработка накопившихся сообщений

Для каждого сценария проверить не только техническое поведение системы, но и бизнес-инварианты:

- один заказ не может быть оплачен дважды
- повторная доставка сообщения не должна повторно выполнять бизнес-операцию
- отказ Notification Service не должен ломать оплату заказа
- временная недоступность Kafka не должна приводить к потере бизнес-событий
- после восстановления consumer'а сообщения должны быть обработаны корректно
- Saga должна либо успешно завершиться, либо корректно компенсироваться
- неисправность одного сервиса не должна приводить к неконтролируемому каскадному отказу всей системы

**Для проекта подготовить:**

- архитектурную схему
- описание границ и ответственности сервисов
- API основных сервисов
- схему взаимодействия через REST
- схему событий Kafka
- описание Saga
- описание механизма Outbox
- перечень failure scenarios
- integration / fault tests
- краткое описание trade-offs выбранной архитектуры

Цель практики — не просто собрать несколько Spring Boot сервисов, а научиться понимать поведение распределённой системы при нормальной работе, задержках, дубликатах, частичных отказах и восстановлении.

#### Углубление в Distributed Systems

**Статья:**

| #     | Ресурс                                                                       | Ссылка                                  |
| ----- | ---------------------------------------------------------------------------------- | --------------------------------------------- |
| 20.10 | 0x0FFF. Консенсус в распределённых системах. Paxos | [Хабр](https://habr.com/ru/articles/222825/) |

**Дополнительно изучить концептуально:**

- Raft и replicated log
- leader election
- quorum
- consistency models
- replication
- partition tolerance
- CAP / PACELC
- clocks и ordering событий
- distributed locks
- failure detection
- recovery после частичных отказов

> На этом этапе не требуется самостоятельно реализовывать Paxos или Raft. Важнее понимать назначение механизмов, условия их применения и связанные trade-offs.

#### Контроль усвоения

После завершения раздела самостоятельно ответить на следующие вопросы:

- Почему микросервисы не всегда лучше модульного монолита?
- Как определить границы микросервиса?
- Что означает Database per Service?
- Почему сервисы не должны напрямую обращаться к БД друг друга?
- Когда использовать REST, а когда messaging?
- Какие проблемы создаёт distributed transaction?
- Как работает Saga?
- В чём разница между orchestration и choreography?
- Зачем нужен Transactional Outbox?
- Почему повторная доставка сообщений является нормальной ситуацией?
- Как обеспечить идемпотентность consumer'а?
- Для чего нужны timeout, retry, Circuit Breaker и Bulkhead?
- Что такое eventual consistency?
- Как возникают cascading failures?
- Как обнаруживать и исследовать partial failures?
- Что дают distributed tracing, metrics и centralized logging?
- Как тестировать распределённую систему при частичных отказах?
- Что такое quorum?
- Зачем распределённой системе нужен consensus?
- В чём основная идея Paxos / Raft?
- Какие trade-offs возникают между consistency, availability, latency, reliability и complexity?

#### Дополнительная литература

- Sam Newman — «Building Microservices» (2nd ed.) → главная практическая книга по микросервисной архитектуре: декомпозиция, границы сервисов, независимый deployment, межсервисное взаимодействие, тестирование, мониторинг, безопасность, данные и эксплуатация. Особенно ценна тем, что автор подробно рассматривает не только преимущества, но и стоимость сложности, которую создают микросервисы
- Chris Richardson — «Microservices Patterns» → практическая книга именно по архитектурным паттернам микросервисов с примерами на Java: Database per Service, API Gateway, Saga, transactional outbox, messaging, CQRS, event-driven architecture, service discovery и тестирование. Это одна из наиболее полезных книг для понимания того, как решать типовые проблемы распределённого приложения
- Martin Kleppmann, Chris Riccomini — «Designing Data-Intensive Applications» (2nd ed.) → главная книга раздела для глубокого понимания distributed data systems: replication, partitioning / sharding, transactions, consistency, consensus, distributed-system failures и streaming. Второе издание вышло в феврале 2026 года и содержит отдельные главы о проблемах распределённых систем, транзакциях, consistency / consensus и streaming
- Brendan Burns — «Designing Distributed Systems» (2nd ed.) → компактная практическая книга по паттернам распределённых систем: replication, scaling, communication, queues, event-based processing, coordination, health checks, idempotency и delivery semantics. Особенно хорошо подходит как переход от микросервисной практики к собственно distributed systems
- Roberto Vitillo — «Understanding Distributed Systems» (2nd ed.) → систематическое изучение фундаментальных механизмов распределённых систем: network failures, timeouts, consistency, replication, coordination, fault tolerance и другие базовые концепции. Хороший вариант именно для формирования теоретической модели того, почему распределённые системы сложнее обычного приложения

### 21. DevOps (Nginx, Kubernetes, Terraform)

Цель: освоить Nginx, Kubernetes и Terraform для автоматизации сборки, доставки и эксплуатации backend-приложений.

**Nginx:**

| #    | Ресурс                                                                                         | Ссылка                                        |
| ---- | ---------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 21.1 | NeuralNine. NGINX Crash Course: Web Server, Reverse Proxy & Load Balancer                            | [YouTube](https://www.youtube.com/watch?v=7FpSPSlJj-0) |
| 21.2 | Артём Шумейко. Nginx — простым языком на понятном примере | [YouTube](https://www.youtube.com/watch?v=2aoOEnZmCmQ) |

**Kubernetes:**

| #    | Ресурс                                                                               | Ссылка                                  |
| ---- | ------------------------------------------------------------------------------------------ | --------------------------------------------- |
| 21.3 | JavaGuru. Docker & Kubernetes | [YouTube](https://www.youtube.com/playlist?list=PLt91xr-Pp57SuhAN8GUQKysUTR_OoSJlv) |
| 21.4 | Rotoro Cloud. Certified Kubernetes Administrator (CKA) + практический опыт | [Stepik](https://stepik.org/course/184745/promo) |

**Terraform:**

| #    | Ресурс                                                                                                                                                         | Ссылка                                                                                |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 21.5 | Денис Астахов. Terraform с нуля до сертифицированного профессионала                                                | [YouTube](https://www.youtube.com/watch?v=R0CaxXhrfFE&list=PLg5SS_4L6LYujWDTYb-Zbofdl44Jxb2l8) |
| 21.6 | freeCodeCamp.org. Изучаем Terraform (и AWS) через создание среды разработки — полный курс для начинающих | [YouTube](https://www.youtube.com/watch?v=iRaai1IBlB0)                                         |

#### Самостоятельно изучаем следующие темы
- Nginx — основы:
  - назначение Nginx
  - web server vs reverse proxy
  - установка и базовая конфигурация
  - структура конфигурационного файла
  - server, location, upstream
  - proxy_pass
  - proxy_set_header
  - Host
  - X-Real-IP
  - X-Forwarded-For
  - X-Forwarded-Proto
  - access / error logs
  - HTTP → HTTPS
  - базовая TLS-конфигурация
- Nginx — балансировка нагрузки:
  - upstream
  - балансировочные алгоритмы
  - health checks
  - Nginx → Spring Boot #1 + Spring Boot #2
  - проверка load balancing
  - session affinity — концептуально
  - sticky sessions — концептуально
- Nginx — продвинутые темы:
  - caching
  - rate limiting
  - gzip
  - security headers — концептуально
  - static files — концептуально
- Kubernetes — основы:
  - зачем нужен Kubernetes?
  - container orchestration
  - cluster
  - node
  - control plane
  - worker nodes
  - desired state / reconciliation
  - declarative configuration
  - kubectl
- Kubernetes — Workloads:
  - Pod
  - ReplicaSet
  - Deployment
  - StatefulSet — концептуально
  - DaemonSet — концептуально
  - Job / CronJob — концептуально
  - Deployment → ReplicaSet → Pod
  - rolling update
  - rollback
  - scaling
  - self-healing
- Kubernetes — Service:
  - Service
  - ClusterIP
  - NodePort
  - LoadBalancer
  - ExternalName — концептуально
  - service discovery
  - DNS внутри кластера
- Kubernetes — ConfigMap и Secret:
  - ConfigMap
  - Secret
  - передача конфигурации в Pod
  - environment variables
  - volumes
  - обновление ConfigMap / Secret
  - безопасность Secret
- Kubernetes — Networking:
  - CNI — концептуально
  - Pod-to-Pod communication
  - Service networking
  - Ingress
  - Ingress Controller
  - Network Policies — концептуально
  - доступ к приложению извне кластера
- Kubernetes — Storage:
  - Volume
  - PersistentVolume (PV)
  - PersistentVolumeClaim (PVC)
  - StorageClass
  - StatefulSet и storage
  - подключение PostgreSQL
  - persistent storage
- Kubernetes — Health checks:
  - liveness probe
  - readiness probe
  - startup probe
  - настройка probes
  - влияние на rolling update
  - self-healing
- Kubernetes — Resource management:
  - resource requests
  - resource limits
  - CPU / memory
  - QoS classes — концептуально
  - Horizontal Pod Autoscaler (HPA) — концептуально
  - Vertical Pod Autoscaler (VPA) — концептуально
- Kubernetes — Namespaces:
  - Namespace
  - изоляция ресурсов
  - квоты — концептуально
  - RBAC — концептуально
- Kubernetes — Troubleshooting:
  - kubectl get
  - kubectl describe
  - kubectl logs
  - kubectl exec
  - kubectl port-forward
  - kubectl events
  - диагностика Pod
  - диагностика Deployment
  - диагностика Service
  - диагностика Ingress
  - диагностика ConfigMap / Secret
  - диагностика probes
  - диагностика rollout
- Terraform — основы:
  - Infrastructure as Code (IaC)
  - декларативный подход
  - Terraform vs Ansible
  - установка Terraform
  - HCL
  - providers
  - resources
  - data sources
  - variables
  - outputs
  - state
  - remote state
  - modules
  - workspaces
  - environments
  - dependency management
  - terraform init / plan / apply / destroy
  - terraform fmt / validate
  - terraform state
  - terraform import
- Terraform — практика:
  - создание VM
  - создание сети
  - создание security groups
  - создание managed PostgreSQL
  - создание object storage
  - создание Kubernetes cluster — концептуально
  - построение переиспользуемой инфраструктуры
  - модули
  - remote state
  - environments dev / staging / prod

#### Обязательная самостоятельная практика

- **Nginx #1.** Настроить Nginx → Spring Boot и отработать:

  - server
  - location
  - `proxy_pass`
  - upstream
  - `proxy_set_header`
  - Host
  - `X-Real-IP`
  - `X-Forwarded-For`
  - `X-Forwarded-Proto`
  - access / error logs
  - HTTP → HTTPS
  - базовую TLS-конфигурацию
- **Nginx #2.** После Nginx #1 настроить балансировку:
  - Nginx → Spring Boot #1 + Spring Boot #2
  - проверить load balancing
- **Kubernetes — базовая практика.** Развернуть Spring Boot-приложение в локальном Kubernetes-кластере. Отработать:
  - Namespace
  - Pod
  - Deployment
  - Service
  - ConfigMap
  - Secret
  - readiness probe
  - liveness probe
  - resource requests / limits
  - `kubectl get`
  - `kubectl describe`
  - `kubectl logs`
  - `kubectl exec`
- **Kubernetes — развёртывание.** Практически выполнить:
  - развёртывание нескольких replicas
  - обновление приложения через rolling update
  - проверку rollout
  - rollback
  - масштабирование
  - обновление и использование ConfigMap / Secret
  - проверку self-healing
  - подключение PostgreSQL
  - persistent storage
  - Ingress
  - доступ к приложению извне кластера
- **Примечание по Kubernetes Workloads:**
  - ReplicaSet — Kubernetes-контроллер, управляющий количеством Pod'ов; обычно создаётся и управляется через Deployment
  - вручную создавать ReplicaSet в рамках практики не требуется, но необходимо понимать его роль в цепочке Deployment → ReplicaSet → Pod
- Terraform — практика:
  - установить Terraform
  - настроить provider
  - создать VM
  - создать сеть
  - создать security groups
  - создать managed PostgreSQL
  - создать object storage
  - вынести конфигурацию в variables
  - использовать outputs
  - вынести код в modules
  - настроить remote state
  - создать environments dev / staging / prod
  - применить terraform plan / apply / destroy
  - проверить созданную инфраструктуру
  - удалить инфраструктуру через terraform destroy
- **Troubleshooting.** Намеренно сломать конфигурацию и самостоятельно восстановить. Для каждой проблемы определить: **симптом → диагностика → причина → исправление → проверка**. Список кейсов:
  - Docker build
  - Docker networking
  - PostgreSQL connection
  - Docker healthcheck
  - Nginx `proxy_pass`
  - Nginx upstream
  - Kubernetes Deployment
  - ConfigMap
  - Secret
  - Service
  - readiness / liveness probe
  - Ingress
  - rollout
  - `kubectl logs` / `describe` / `get`
  - Terraform state
  - Terraform apply

#### Дополнительная литература

- Nigel Poulton — «Docker Deep Dive» → лучшая дополнительная книга для систематизации Docker: images, containers, Dockerfile, networking, volumes, Compose, security и container lifecycle
- Brendan Burns, Joe Beda, Kelsey Hightower, Lachlan Evenson — «Kubernetes: Up & Running» → главная книга по Kubernetes для разработчика: Pods, Deployments, Services, ConfigMaps, Secrets, networking, storage, health checks и deployments. Читать после CKA, выборочно или полностью
- Benjamin Muschko — «Certified Kubernetes Administrator (CKA) Study Guide» → практический справочник именно по администрированию Kubernetes и подготовке к CKA. Полезен как справочник при выполнении практического блока из текущего раздела
- Derek DeJonghe — «NGINX Cookbook» → практический справочник по Nginx: reverse proxy, load balancing, SSL / TLS, caching, routing и настройке production-конфигураций. Читать выборочно, параллельно с практикой из текущего раздела
- Gene Kim, Jez Humble, Patrick Debois, John Willis — «The DevOps Handbook» → для понимания DevOps-подхода целиком: CI/CD, automation, deployment, feedback loops, monitoring и культура эксплуатации. Не технический справочник, а книга для формирования системного понимания DevOps
- Yevgeniy Brikman — «Terraform: Up & Running» → глубокое практическое руководство по Terraform: HCL, providers, resources, data sources, variables, outputs, modules, state, remote state, environments, dependency management и построение переиспользуемой инфраструктуры как кода (IaC)

## Основы Frontend

### 22. HTML5 + CSS3

Цель: освоить вёрстку и современный CSS — семантику, Flexbox, Grid, адаптивность, препроцессоры, доступность.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                                                   | Ссылка                                                                                |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 22.1 | Дмитрий Фокеев. Профессия веб-верстальщик. Пакет из 2 курсов по веб-разработке | [Stepik](https://stepik.org/course/121498/promo)                                               |
| 22.2 | SuperSimpleDev. HTML & CSS Full Course — Beginner to Pro                                                                                      | [YouTube](https://www.youtube.com/watch?v=G3e-cpL7ofc)                                         |
| 22.3 | freeCodeCamp.org. Introduction to Responsive Web Design — HTML & CSS Tutorial                                                                 | [YouTube](https://www.youtube.com/watch?v=srvUrASNj0s)                                         |
| 22.4 | Александр Ламков. Адаптивная вёрстка сайта с нуля для начинающих                        | [YouTube](https://www.youtube.com/watch?v=AUdW01JQFME&list=PL0MUAHwery4rqkzKF1mDBCIH_eZgjY6uN) |

#### Обязательная самостоятельная практика

Закрепить на практике:

- **HTML5:**

  - структура документа, семантические элементы
  - заголовки, списки, ссылки, изображения, таблицы
  - формы и HTML-валидация
- **CSS3:**

  - селекторы, каскад, наследование, специфичность
  - box model, размеры и единицы измерения
  - цвета, шрифты, позиционирование
- **Layout:**

  - display, Flexbox, CSS Grid
  - overflow, object-fit, aspect-ratio
- **Responsive Design:**

  - media queries, адаптивные единицы
  - mobile-first, breakpoints
  - построение адаптивных страниц для разных ширин viewport
- **Современный CSS:**

  - CSS Variables
  - `calc()`, `min()`, `max()`, `clamp()`
  - transitions, animations
- **BEM + SCSS/Sass:**

  - организация HTML/CSS
  - базовая работа с препроцессором
- **Accessibility:**

  - семантика, label, alt
  - keyboard navigation
  - базовые ARIA-атрибуты
- **DevTools:**

  - инспектирование HTML/CSS
  - box model, computed styles
  - responsive режим
  - поиск и исправление проблем
- **Практика по макетам:** сверстать несколько страниц по готовым дизайнам и адаптировать их под разные разрешения
- **Итоговый мини-проект:** адаптивный frontend для Task Management System — Login, Registration, Dashboard, список / создание / редактирование / просмотр задач, Profile, 404. На этом этапе — без JavaScript и backend

#### Дополнительная литература

- Jon Duckett — «HTML and CSS: Design and Build Websites» → очень доступное визуальное объяснение HTML и CSS. Хорошо подходит для закрепления фундаментальных концепций после основного курса
- Eric A. Meyer, Estelle Weyl — «CSS: The Definitive Guide» → глубокий справочник по CSS: cascade, selectors, box model, layout, Flexbox, Grid, positioning, responsive design и другим возможностям CSS. Использовать как справочник, а не читать обязательно целиком
- Jennifer Robbins — «Learning Web Design» → системное введение в web development: HTML, CSS, responsive design, accessibility и основы frontend-разработки. Хорошо подходит для закрытия пробелов после курса
- Rachel Andrew — «The New CSS Layout» → специализированное углубление в современный CSS layout, прежде всего Flexbox и Grid. Читать выборочно после освоения базового CSS
- Lea Verou — «CSS Secrets» → практические продвинутые приёмы CSS: responsive design, gradients, animations, визуальные эффекты и нестандартные решения. Использовать как дополнительный источник после уверенного освоения основ

### 23. JavaScript

Цель: изучить JavaScript — язык, объектную модель, асинхронность, DOM, Fetch API, модули и работу с состоянием приложения.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                                 | Ссылка                                        |
| ---- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 23.1 | Антон Ларичев. JavaScript с нуля — основы языка и практика для начинающих | [Stepik](https://stepik.org/course/122243/promo)       |
| 23.2 | Антон Ларичев. JavaScript Advanced — продвинутые концепции языка и ООП             | [Stepik](https://stepik.org/course/130339/promo)       |
| 23.3 | Владилен Минин. JavaScript с нуля — курс для начинающих с практикой            | [YouTube](https://www.youtube.com/watch?v=fcMcf_4PjfI) |
| 23.4 | SuperSimpleDev. JavaScript Tutorial Full Course — Beginner to Pro                                                           | [YouTube](https://www.youtube.com/watch?v=EerdGm-ehJQ) |

#### Обязательная самостоятельная практика

Закрепить на практике:

- **JavaScript Core:**

  - переменные, типы данных, Symbol, BigInt
  - операторы, функции, массивы, объекты
  - деструктуризация, spread / rest
  - современные конструкции ES
- **Выполнение кода:**

  - scope, lexical environment, execution context
  - hoisting, closures
  - this, `call`, `apply`, `bind`
- **Объектная модель:**

  - prototypes, prototype chain
  - classes, inheritance, encapsulation, polymorphism
- **Коллекции и итерации:**

  - Map, Set, WeakMap, WeakSet
  - iterators, generators
- **Регулярные выражения:**

  - создание RegExp
  - основные шаблоны
  - методы поиска и проверки строк
- **Работа с ошибками:**

  - `try` / `catch` / `finally`
  - собственные типы ошибок
  - корректная обработка ошибок
- **Асинхронность:**

  - callbacks, Promise, async / await
  - Promise API
  - параллельное и последовательное выполнение
  - обработка ошибок
  - Event Loop, microtasks / macrotasks
  - отмена асинхронных операций
- **Работа с HTTP API:**

  - Fetch API
  - HTTP-методы, headers, JSON, query parameters
  - обработка HTTP-ошибок
  - CORS
- **DOM:**

  - поиск и изменение элементов
  - создание / удаление элементов
  - атрибуты, классы, стили, формы
- **Events:**

  - обработчики событий
  - bubbling / capturing
  - event delegation
  - keyboard / mouse / form events
- **Browser API:**

  - `localStorage`, `sessionStorage`
  - URL / URLSearchParams, FormData
  - timers, AbortController
- **Модули:**

  - ES Modules (`import` / `export`)
  - организация JavaScript-кода по модулям
- **NPM:**

  - `package.json`
  - установка и использование зависимостей
  - npm scripts
- **DevTools:**

  - Console, Debugger, Network, Sources, Application
  - анализ HTTP-запросов и поиск ошибок
- **Код и архитектура:**

  - разделение ответственности
  - переиспользование функций / классов
  - разделение UI / state / API / utility-логики
  - работа с состоянием приложения

#### Практический проект

Продолжить Task Management System и превратить статическую HTML/CSS-вёрстку в полноценное интерактивное приложение на Vanilla JavaScript:

- Login / Registration с валидацией
- Dashboard
- CRUD-операции с задачами
- поиск, фильтрация, сортировка
- URL / query parameters
- управление состоянием
- loading / error / empty states
- localStorage
- ES Modules
- Fetch API
- обработка ошибок
- разделение API / state / UI / utility-логики
- сначала mock REST API
- затем подготовка приложения к подключению реального REST API Spring Boot

#### Дополнительная литература

- Современный учебник JavaScript → лучший русскоязычный справочник для систематизации и углубления JavaScript. Охватывает Core JavaScript, объекты и прототипы, классы, Promise, async / await, Event Loop, генераторы, модули, DOM, события, Fetch, WebSocket, Web Storage, Web Components, RegExp и другие возможности языка и браузера. Использовать как постоянный справочник, а не обязательно проходить целиком — [learn.javascript.ru](https://learn.javascript.ru/)
- Marijn Haverbeke — «Eloquent JavaScript» (4th ed., 2024) → хорошее системное объяснение самого языка JavaScript, программирования и работы с браузером. Особенно полезна для закрепления функций, объектов, массивов, замыканий, асинхронности, DOM и архитектуры небольших приложений
- David Flanagan — «JavaScript: The Definitive Guide» → один из лучших справочников по JavaScript. Глубоко рассматривает синтаксис и семантику языка, объекты, функции, классы, итераторы, генераторы, Promise, async / await, модули, регулярные выражения и браузерные API. Использовать прежде всего как справочник для сложных и редко используемых возможностей языка
- Kyle Simpson — «You Don't Know JS Yet» → серия книг для глубокого понимания внутренних механизмов JavaScript: типы и приведение, scope и closures, объекты и прототипы, this, async и другие особенности языка. Особенно полезна для понимания того, почему JavaScript работает именно так, а не только для запоминания синтаксиса
- Axel Rauschmayer — «JavaScript for Impatient Programmers» → продвинутое системное изучение современного JavaScript: современный синтаксис ES, функции, объекты, классы, коллекции, итераторы, модули, асинхронность и другие возможности языка. Хорошо использовать после основных курсов для закрытия пробелов и углубления Core JavaScript

### 24. TypeScript

Цель: освоить статическую типизацию поверх JavaScript — типы, generics, utility types, narrowing и безопасную работу с внешними данными.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                                      | Ссылка                                        |
| ---- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 24.1 | Роман Максимов. TypeScript с 0 до ПРО — решение задач по TS, разбор сложных тем | [Stepik](https://stepik.org/course/221935/promo)       |
| 24.2 | Ulbi TV. TypeScript ФУНДАМЕНТАЛЬНЫЙ КУРС от А до Я — вся теория + практика             | [YouTube](https://www.youtube.com/watch?v=LWtHl__oEWc) |
| 24.3 | Dave Gray. TypeScript Full Course for Beginners. Complete All-in-One Tutorial                                                     | [YouTube](https://www.youtube.com/watch?v=gieEQFIfgYc) |

#### Обязательная самостоятельная практика

После курса — **обязательный самостоятельный практический блок**.

Закрепить на практике:

- **TypeScript Core:**

  - типизация переменных, функций, объектов, массивов, tuples, `enum` и современные альтернативы (`union` / `literal types`)
- **Type aliases и interfaces:**

  - проектирование собственных типов и контрактов
- **Union / Intersection Types:**

  - объединение и композиция типов
- **`unknown`, `never`, `void`, `any`:**

  - понимание различий и правильное применение
- **Type narrowing:**

  - `typeof`, `instanceof`, `in`, пользовательские type guards, assertion functions
- **Type assertions:**

  - `as`, non-null assertion и понимание случаев, когда assertions следует избегать
- **Generics:**

  - generic functions, interfaces, classes, constraints, default types
- **Utility Types:**

  - `Partial`, `Required`, `Readonly`, `Pick`, `Omit`, `Record`, `Exclude`, `Extract`, `NonNullable`, `ReturnType`, `Parameters`, `Awaited`
- **Type operators:**

  - `keyof`, `typeof`, indexed access types
- **Advanced Types:**

  - conditional types, mapped types, template literal types, recursive types
- **Generic type inference:**

  - `infer`, `satisfies`, const type parameters
- **Function typing:**

  - optional / default / rest parameters, overloads, callbacks, generic functions
- **Classes:**

  - modifiers, abstract classes, inheritance, interfaces, generics, polymorphism
- **Modules:**

  - `import` / `export`, типизация модулей и организация TypeScript-кода
- **Declaration Files:**

  - понимание `.d.ts`, `declare`, `declare module`, типизация библиотек без встроенных типов
- **Configuration:**

  - `tsconfig.json`, `strict`, `noImplicitAny`, `strictNullChecks`, `target`, `module`, `moduleResolution`
- **Runtime vs compile-time:**

  - понимание различий между проверками TypeScript на этапе компиляции и runtime-проверками
  - runtime validation, type predicates, Zod или аналогичный schema-validation инструмент
- **Типизация внешних данных:**

  - API responses, формы, JSON и безопасная работа с данными, которым нельзя доверять
- **Практика с TypeScript Challenge:**

  - решение задач на conditional types, generics, mapped types, `infer` и другие возможности системы типов
- **Code Quality:**

  - устранение неоправданного `any`, проектирование устойчивых типов, переиспользование типов и уменьшение дублирования

#### Практический проект

**Мигрировать Task Management System с JavaScript на TypeScript:**

- Перевести весь проект с `.js` на `.ts`
- Типизировать модели приложения: `User`, `Task`, `Profile`, `Auth`, `ApiResponse`, `Pagination` и другие доменные сущности
- Типизировать состояние приложения и функции управления состоянием
- Типизировать формы `Login` / `Registration` / `Task Create` / `Task Edit`
- Создать типизированный API layer: request/response types, generic-обёртки над Fetch API, обработка ошибок и runtime validation внешних данных
- Описать типы успешных и ошибочных ответов REST API
- Реализовать безопасную обработку `unknown` при разборе внешних данных
- Типизировать query parameters и работу с `URLSearchParams`
- Типизировать DOM API и события: `HTMLElement`, `HTMLInputElement`, `HTMLFormElement`, `Event`, `MouseEvent`, `KeyboardEvent`, `SubmitEvent` и обработчики событий
- Типизировать фильтрацию, сортировку и поиск задач
- Создать переиспользуемые generic-типы и utility-типы там, где это действительно оправдано
- Настроить строгий режим TypeScript (`strict: true`) и устранить ошибки типизации с минимизацией использования `any`
- Разделить типы приложения по назначению: `domain` / `API` / `UI` / `utility`
- Подготовить архитектуру проекта к дальнейшей миграции на React + TypeScript
- Собрать production build и проверить проект без ошибок TypeScript

#### Дополнительная литература

- TypeScript Handbook — официальная документация TypeScript ([TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/))
  → Главный reference по TypeScript. Покрывает базовые типы, narrowing, функции, object types, generics, type manipulation, classes и modules. Особенно полезен как постоянный справочник при работе с языком.
- Josh Goldberg — «Learning TypeScript»
  → Системное введение в TypeScript для разработчиков, уже знакомых с JavaScript. Хорошо объясняет type system, narrowing, functions, generics, type manipulation и практическое применение TypeScript. Использовать как дополнительное последовательное чтение после основного курса.
- Dan Vanderkam — «Effective TypeScript», 2nd Edition
  → Одна из лучших книг именно для перехода от знания синтаксиса TypeScript к профессиональному использованию языка. Полезна для понимания типизации реального кода, проектирования типов, generics, type-level programming и практических trade-offs. Использовать 2-е издание 2024 года.
- Stefan Baumgartner — «TypeScript Cookbook»
  → Практический reference с более чем 100 рецептами: настройка проектов, type system, generics, conditional types, template literal types, variadic tuples, utility types, стандартная библиотека, classes, decorators, `satisfies`, тестирование сложных типов и runtime validation. Читать выборочно как практический справочник.
- Boris Cherny — «Programming TypeScript»
  → Системное и более глубокое рассмотрение TypeScript: compiler, type system, generics, advanced types, asynchronous programming, modules и применение TypeScript в реальных проектах. Книга старше остальных, поэтому использовать преимущественно для фундаментального понимания, а современные возможности сверять с официальной документацией.

## Разработка на React

### 25. Frontend Build / Tooling

Цель: освоить инструменты сборки frontend — npm, Vite, ESLint, Prettier, Husky и CI-проверки через GitHub Actions.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                                                                                                       | Ссылка                                        |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 25.1 | Александр Ламков. NPM для начинающих. Полный гайд: установка, команды, флаги, разбор package.json, версионирование | [YouTube](https://www.youtube.com/watch?v=IsRl03T9VMo) |
| 25.2 | Игорь Бабко. Vite — Быстрая Сборка JavaScript Проектов\| Полный курс                                                                                     | [YouTube](https://www.youtube.com/watch?v=evmIHSAn1AU) |
| 25.3 | Ulbi TV. Webpack ПОЛНЫЙ КУРС от А до Я. Вся конфигурация, Микрофронтенд, Монорепозиторий, Module Federation                             | [YouTube](https://www.youtube.com/watch?v=acAH2_YT6bs) |
| 25.4 | Александр Ламков. Линтеры и форматтеры в фронтенде: ESLint, Stylelint и Prettier без боли                                                       | [YouTube](https://www.youtube.com/watch?v=jwTwnI3hwig) |
| 25.5 | Syntax. Lint Like a Senior Developer w/ eslint + husky + lint staged + github actions                                                                                                              | [YouTube](https://www.youtube.com/watch?v=Kr4VxMbF3LY) |

#### Обязательная самостоятельная практика

После изучения материалов обязательно применить знания на практике в **Task Management System**:

- **Настроить npm и package.json:**

  - dependencies / devDependencies
  - npm scripts
  - development / production scripts
  - lock-файл зависимостей
- **Настроить Vite:**

  - dev server
  - HMR
  - aliases
  - environment variables
  - assets
  - plugins
  - production build
  - preview production build
- **Настроить TypeScript:**

  - TypeScript compiler (tsc)
  - type-check script
  - strict mode
  - отсутствие TypeScript-ошибок перед production build
- **Настроить ESLint:**

  - современная конфигурация
  - правила для TypeScript и React
  - npm scripts для lint / lint:fix
- **Настроить Prettier:**

  - единый стиль форматирования
  - конфигурация проекта
  - интеграция с ESLint
- **Настроить Husky + lint-staged:**

  - pre-commit hook
  - автоматическая проверка изменённых файлов
  - запуск ESLint / Prettier перед commit
- **Настроить GitHub Actions:**

  - установка зависимостей
  - TypeScript type-check
  - ESLint
  - production build
  - автоматический запуск pipeline при push / pull request
- **Изучить production optimization:**

  - code splitting
  - tree shaking
  - lazy loading
  - source maps
  - анализ размера bundle
- **Изучить Webpack на концептуальном уровне:**

  - entry / output
  - loaders
  - plugins
  - bundling
  - code splitting
  - tree shaking
  - Module Federation
- **Финальная задача:**

  - настроить полный frontend pipeline Task Management System
  - командами npm запускать development, lint, format, type-check и production build
  - перед commit автоматически выполнять проверки
  - GitHub Actions должен проверять проект
  - production build должен успешно собираться без ошибок
  - описать весь frontend toolchain в README

#### Дополнительная литература

- npm Documentation
  → Справочник по npm, package.json, npm scripts, зависимостям, версиям и конфигурации.
- Vite Documentation
  → Актуальная документация по Vite, конфигурации, dev server, HMR, environment variables, plugins и production build.
- Webpack Documentation
  → Справочник по концепциям Webpack: entry/output, loaders, plugins, code splitting, tree shaking и Module Federation.
- ESLint Documentation
  → Актуальная документация по конфигурации ESLint, правилам, TypeScript/React и интеграции с другими инструментами.
- Prettier Documentation
  → Документация по настройке Prettier, конфигурации проекта и интеграции с ESLint.

### 26. React + Next.js

Цель: научиться разрабатывать современные frontend-приложения на React и Next.js — компоненты, hooks, routing, state, SSR и Server Actions.

#### Ресурсы для изучения

**React:**

| #    | Ресурс                                                                                     | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 26.1 | Дмитрий Фокеев. Полный курс по React JS (Redux / Router / Tailwind CSS) | [Stepik](https://stepik.org/course/221235/promo)       |
| 26.2 | Ulbi TV. React JS фундаментальный курс от А до Я                        | [YouTube](https://www.youtube.com/watch?v=GNrdg3PzpJQ) |
| 26.3 | SuperSimpleDev. React Tutorial Full Course — Beginner to Pro (React 19, 2025)                   | [YouTube](https://www.youtube.com/watch?v=TtPXvEcE11E) |

**Next.js:**

| #    | Ресурс                                                                                         | Ссылка                                        |
| ---- | ---------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 26.4 | TeaCoder. Next.js — лучший React-фреймворк. Полный курс 2026               | [YouTube](https://www.youtube.com/watch?v=t72VITDy1vc) |
| 26.5 | Ankita Kulkarni. Next.js 16 Full Course — Build and Deploy a Production-Ready Full Stack App        | [YouTube](https://www.youtube.com/watch?v=tI_Nt32_4wM) |
| 26.6 | PedroTech. NextJS 16 Full Course 2026 — Build and Deploy a Production Ready Job Application Tracker | [YouTube](https://www.youtube.com/watch?v=vCIsrOGNhas) |

#### Обязательная самостоятельная практика

После курса — **обязательный самостоятельный практический блок**.

Продолжить сквозной проект **Task Management System**.

- **React + TypeScript:**

  - перенести UI с Vanilla JS на React
  - разбить приложение на переиспользуемые компоненты
  - использовать props, state, Hooks и Context API
  - реализовать формы и валидацию
  - реализовать маршрутизацию через React Router
  - реализовать управление глобальным состоянием через Redux Toolkit
  - реализовать loading / success / error / empty states
  - реализовать поиск, фильтрацию, сортировку и pagination
  - строго типизировать компоненты, события, формы, state и API
- **REST API:**

  - подключить приложение к реальному Spring Boot REST API
  - реализовать CRUD задач
  - реализовать регистрацию и авторизацию
  - обработать HTTP 401 / 403 / 404 / 409 / 422 / 500
  - реализовать корректную обработку loading / success / error состояний
  - реализовать взаимодействие с authentication API
  - работать с access / refresh token в соответствии с архитектурой, изученной в Spring Security и Frontend Security
- **Next.js:**

  - мигрировать React-приложение на Next.js
  - использовать App Router
  - организовать маршруты через App Router с использованием page, layout и nested routes
  - реализовать dynamic routes
  - использовать Server Components и Client Components осознанно, в зависимости от требований конкретной страницы
  - реализовать loading / error / not-found
  - реализовать серверную загрузку данных там, где это оправдано
  - изучить современную модель caching и revalidation в Next.js 16
  - понимать Cache Components, use cache и Partial Prerendering (PPR)
  - понимать revalidateTag / updateTag и базовые сценарии их применения
  - использовать Server Actions там, где они действительно уместны
  - при необходимости реализовать Route Handlers
  - работать с cookies / headers
  - реализовать metadata и базовое SEO
  - оптимизировать изображения и шрифты средствами Next.js
  - настроить environment variables
  - подготовить production build
  - выполнить deployment
- **Next.js Proxy (ранее Middleware):**

  - назначение Proxy в Next.js
  - понимать, что в Next.js 16 термин Middleware был переименован в Proxy
  - обработка входящего request до выполнения дальнейшей логики приложения
  - matcher: определение маршрутов, для которых применяется Proxy
  - redirects
  - rewrites
  - работа с cookies
  - работа с request / response headers
  - изменение и передача request / response metadata
  - предварительная обработка запросов
  - authentication: проверка наличия authentication state / session
  - protected routes
  - role-based route protection
  - redirect неавторизованного пользователя на страницу Login
  - redirect авторизованного пользователя с Login / Registration
  - работа с URL и query parameters на уровне Proxy
  - отличие Proxy от client-side route guards
  - отличие Proxy от Route Handlers
  - отличие Proxy от Server Actions
  - отличие Proxy от server-side authorization
  - security boundaries Next.js
  - понимать, что Proxy не заменяет backend authorization
  - backend остаётся окончательной границей доверия для authentication / authorization
  - ограничения Proxy и случаи, когда бизнес-логику не следует помещать в Proxy
  - runtime и ограничения среды выполнения — понимать концептуально
  - предотвращение циклических redirects
  - корректная работа с cookies и headers
  - обработка ошибок и edge cases
  - практика: реализовать защиту маршрутов Task Management System через Next.js Proxy
  - практика: закрыть Dashboard / Profile / Projects / Tasks для неавторизованных пользователей
  - практика: реализовать redirect на Login
  - практика: реализовать redirect авторизованного пользователя с Login / Registration
  - практика: реализовать базовую проверку роли пользователя для отдельных маршрутов
  - практика: проверить взаимодействие Proxy с authentication flow и backend authorization

#### Дополнительная литература

- Robin Wieruch — «The Road to React»
  → Системное изучение React: компоненты, JSX, state, Hooks, работа с API, управление состоянием и архитектура React-приложений. Хорошо подходит для последовательного закрепления React после основного курса.
- Alex Banks, Eve Porcello — «Learning React», 3rd Edition
  → Практическое и системное изучение современного React. Полезна для углубления компонентов, Hooks, state management, работы с API и архитектуры React-приложений.
- Stoyan Stefanov — «React: Up & Running», 2nd Edition
  → Практическое руководство по разработке React-приложений. Полезно для закрепления компонентов, JSX, state, props, Hooks и построения приложений от простых компонентов до более сложной архитектуры.
- Adam Boduch, Roy Derks — «React and React Native: A Complete Guide», 5th Edition
  → Более подробное справочное руководство по экосистеме React. Полезно для углубления Hooks, управления состоянием, производительности, архитектуры и практических паттернов.
- Robin Wieruch — «The Road to Next»
  → Практическое изучение Next.js и построения приложений поверх React. Использовать выборочно как дополнительный материал, а актуальные возможности Next.js обязательно сверять с официальной документацией.
- Next.js Documentation
  → Основной справочный источник по актуальному Next.js: App Router, Server Components, routing, data fetching, caching, revalidation, Server Actions, Route Handlers, metadata, deployment и другим возможностям фреймворка.

### 27. OpenAPI / Documentation / Contracts

Цель: освоить контрактный подход к API — OpenAPI, code generation, mock server и Contract Testing между frontend и backend.

#### Ресурсы для изучения

| #    | Ресурс                                                                             | Ссылка                                                                                |
| ---- | ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 27.1 | IT как Конструктор. OpenAPI и Swagger за 1 час                       | [YouTube](https://www.youtube.com/watch?v=z3lat1gzaKk&list=PL4MpKy3QjNp8IsepABrb_c6D867DFO6aR) |
| 27.2 | Максим Иванов. NodeJS Swagger API Documentation Tutorial Using Swagger JSDoc | [YouTube](https://www.youtube.com/watch?v=S8kmHtQeflo)                                         |
| 27.3 | Study Automation Academy. Swagger API                                                    | [YouTube](https://www.youtube.com/watch?v=gZnu0TBWRJk&list=PLD5mJXRPUUgsZ5qXWoosfUWw_IQfC79Jy) |
| 27.4 | Tomasz Buszewski. Generate an OpenAPI Client for React                                   | [YouTube](https://www.youtube.com/watch?v=3LIk2Tu1-9I)                                         |

#### Обязательная самостоятельная практика

После изучения материалов обязательно применить знания на практике в **Task Management System**.

- **Теоретическая часть:**

  - API contract: что такое контракт API и зачем он нужен
  - Contract-first / Design-first / Code-first подходы и их различия
  - OpenAPI Specification: назначение и структура
  - OpenAPI 3.x: `openapi`, `info`, `servers`, `paths`, `components`, `schemas`
  - Operations: GET, POST, PUT, PATCH, DELETE
  - Parameters: path, query, header, cookie
  - Request body и response body
  - DTO и JSON Schema: связь между DTO, JSON Schema и OpenAPI schemas
  - типы данных, required, null, enum, default и constraints
  - reusable schemas через `components`
  - `$ref` и переиспользование компонентов
  - HTTP status codes в API contract
  - единый формат ошибок API
  - authentication / authorization и `securitySchemes`
  - pagination, filtering и sorting как часть API contract
  - API versioning: URL, headers и другие подходы
  - backward compatibility / breaking changes
  - API evolution: как изменять контракт без поломки существующих клиентов
  - документация API: Swagger UI и Swagger Editor
  - mock server и использование OpenAPI contract до готовности backend
  - code generation: TypeScript types и API clients из OpenAPI
  - преимущества и ограничения generated client
  - интеграция generated client с React и TanStack Query
  - API contract как источник истины для frontend и backend
  - Contract Testing: проверка соответствия реализации API описанному контракту
- **Практическая часть:**

  - создать и поддерживать OpenAPI specification для Task Management System
  - описать основные endpoints, parameters, request / response schemas и ошибки
  - описать authentication / authorization и security schemes
  - описать pagination / filtering / sorting
  - организовать переиспользуемые schemas через `components` и `$ref`
  - подключить Swagger UI для просмотра и тестирования API
  - сгенерировать TypeScript types из OpenAPI
  - сгенерировать TypeScript API client для React
  - использовать generated client на frontend вместо ручного дублирования API-типов
  - при необходимости интегрировать generated client с TanStack Query
  - проверить типобезопасность запросов и ответов
  - внести изменение в API contract и обновить generated types / client
  - продемонстрировать совместимое и несовместимое изменение API
  - добавить mock API на основе OpenAPI contract
  - настроить Contract Testing
  - настроить проверку API contract в CI
  - документировать процесс работы с OpenAPI в README

#### Дополнительная литература

- Arnaud Lauret — «The Design of Web APIs» (2nd ed., 2025) → основная книга для современного API design: consumer-first подход, API contract, совместимость, versioning, эволюция API, OpenAPI и JSON Schema
- Joshua S. Ponelat, Lukas L. Rosenstock — «Designing APIs with Swagger and OpenAPI» (2022) → основная книга непосредственно по OpenAPI / Swagger: структура спецификации, Swagger Editor / UI, design-first, документация, code generation, frontend integration, pagination, error handling, versioning и breaking changes
- Mark Massé — «REST API Design Rulebook» → фундаментальные принципы REST API design: URI, HTTP methods, status codes, headers, representations и client concerns. Использовать именно как фундамент REST, а не как современное руководство по OpenAPI
- Leonard Richardson, Mike Amundsen, Sam Ruby — «RESTful Web APIs» → более глубокое понимание Web API design: ресурсы, representations, HTTP, hypermedia и взаимодействие клиента с API. Дополняет OpenAPI пониманием самого API design
- James Gough, Daniel Bryant, Matthew Auburn — «Mastering API Architecture» → архитектурный уровень: API как часть распределённой системы, API governance, design decisions, evolution, compatibility и эксплуатация долгоживущих API

### 28. State Management + API Integration

Цель: освоить управление состоянием frontend-приложения и интеграцию с backend API — client state vs server state, Redux Toolkit, TanStack Query, кэширование, инвалидация, optimistic updates, обработка ошибок и authentication flow.

| #    | Ресурс                                                                                                                                         | Ссылка                                        |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 28.1 | Ulbi TV. Redux | [YouTube](https://www.youtube.com/playlist?list=PL6DxKON1uLOHsBCJ_vVuvRsW84VnqmPp6) |
| 28.2 | Ulbi TV.  State management от А до Я. Управление состоянием. Server vs client state. Global vs module | [YouTube](https://www.youtube.com/watch?v=tnzjswnQ7So) |
| 28.3 | freeCodeCamp.org. React State Management – Intermediate JavaScript Course | [YouTube](https://www.youtube.com/watch?v=-bEzt5ISACA) |
| 28.4 | Ulbi TV.  Tanstack query (react query) полный курс от А до Я за 70 минут | [YouTube](https://www.youtube.com/watch?v=mg9Kq1YaENI) |
| 28.5 | Marius Espejo.  React Query: Fetch, cache, and update server data using queries and mutations | ReactJS Tutorial  | [YouTube](https://www.youtube.com/watch?v=aLQbVd-2tIo) |

#### Для самостоятельного изучения
- Альтернативы Redux:
  - Zustand
  - Valtio
  - Jotai
  - Recoil (концептуально)
  - MobX (концептуально)
  - критерии выбора между Redux Toolkit, Zustand, Jotai и Valtio
  - trade-offs: boilerplate, кривая обучения, размер bundle, devtools, ecosystem
  - когда Redux Toolkit избыточен
  - когда Zustand или Jotai предпочтительнее Redux
- React Query и React Location:
  - React Query для server state
  - React Location как альтернатива React Router (концептуально)
  - сравнение подходов к routing и data fetching
- Современный use hook:
  - назначение use в React 19+
  - работа с Promise и Context через use
  - отличие use от useEffect + useState
  - Suspense и use
  - ограничения и сценарии применения
  - связь с Server Components
- Практические рекомендаци:
  - когда использовать useState vs useReducer?
  - когда выносить состояние в Context?
  - когда писать custom hook?
  - когда подключать React Query?
  - когда переходить на глобальный store?
  - как не превратить приложение в «зоопарк» из библиотек?
  - принцип «начинать с простого решения»

#### Обязательная самостоятельная практика

После изучения материалов обязательно применить знания на практике в Task Management System:

- Разделение состояния по категориям:
  - определить, какие данные относятся к client state, а какие — к server state
  - составить таблицу: категория состояния → примеры → выбранный инструмент → обоснование
  - для каждой категории определить, где она должна храниться:
    - UI state (sidebar, theme, модальные окна) → React state / Context
    - form state → React Hook Form
    - server state (задачи, проекты, пользователи) → TanStack Query
    - URL state (фильтры, сортировка, pagination) → query parameters
    - authentication state → Redux Toolkit / Context + защищённое хранилище
  - устранить дублирование server state в клиентском store
  - устранить хранение derived state, которое можно вычислить
  - устранить prop drilling там, где уместен Context или custom hook
- API layer:
  - создать единый typed API client
  - вынести базовый URL и настройки в environment variables
  - реализовать request / response interceptors
  - использовать OpenAPI-generated types / client из раздела 27
  - реализовать типизированные методы для работы с backend
  - обработать HTTP 400 / 401 / 403 / 404 / 409 / 422 / 500
  - реализовать timeout и cancellation через AbortController
  - реализовать централизованную обработку network errors
  - реализовать логирование ошибок без утечки secrets
  - не логировать access tokens, passwords и другие чувствительные данные
- Server state через TanStack Query:
  - подключить TanStack Query
  - настроить QueryClient
  - реализовать useQuery для всех read-операций
  - реализовать useMutation для create / update / delete
  - настроить queryKey согласно структуре домена
  - настроить staleTime и gcTime
  - реализовать инвалидацию запросов после mutations
  - реализовать оптимистичные обновления с rollback при ошибке
  - реализовать pagination через useQuery
  - реализовать infinite scroll через useInfiniteQuery
  - реализовать dependent queries
  - реализовать prefetching для переходов между страницами
  - использовать placeholderData для плавного UX
  - настроить TanStack Query DevTools
  - разобраться, когда useQuery избыточен и достаточно useEffect + useState
- Client state через Redux Toolkit:
  - определить, какое состояние действительно должно жить в Redux
  - настроить store через configureStore
  - создать slices для клиентского состояния: ui, theme, sidebar, filters, modal
  - использовать createEntityAdapter для нормализации там, где это оправдано
  - реализовать typed useSelector и useDispatch
  - реализовать selectors и memoized selectors через createSelector
  - настроить Redux DevTools
  - не дублировать server state в Redux
  - обосновать, почему для конкретных данных выбран Redux, а не Context или Zustand
- Альтернативы Redux:
  - реализовать один и тот же функционал Task Management System минимум с двумя разными подходами:
    - React state + Context + custom hooks
    - Redux Toolkit
  - при желании реализовать третий вариант на Zustand или Jotai
  - сравнить подходы: объём кода, читаемость, тестируемость, производительность, DX
  - письменно обосновать, какой подход выбран для итогового проекта и почему
  - зафиксировать trade-offs в README
- Authentication flow:
  - реализовать login / logout
  - хранить authentication state
  - реализовать автоматическое обновление access token по 401
  - организовать refresh queue, чтобы не отправлять несколько refresh-запросов одновременно
  - выполнять logout при истечении refresh token
  - очищать кэш TanStack Query при logout
  - реализовать redirect на login
  - реализовать redirect авторизованного пользователя с login / registration
  - защитить маршруты на уровне state
  - интегрировать authentication flow с Spring Security backend
  - понимать, что frontend authentication ≠ backend authorization
- Формы:
  - использовать React Hook Form или аналогичный инструмент
  - типизировать формы через TypeScript
  - реализовать клиентскую валидацию
  - реализовать отображение server-side validation errors
  - реализовать loading state при отправке
  - реализовать сброс формы при успехе
  - обработать ошибки валидации 400 / 422
  - не дублировать form state в глобальном store
- URL state:
  - хранить фильтры, сортировку и pagination в query parameters
  - синхронизировать URL и состояние приложения
  - реализовать deep linking
  - реализовать back / forward navigation
  - использовать URL как источник истины для воспроизводимых состояний
- Loading / Error / Empty / Success:
  - реализовать единый подход к состояниям загрузки
  - реализовать skeleton screens
  - реализовать глобальный Error Boundary
  - реализовать локальную обработку ошибок
  - реализовать корректные пустые состояния для списков
  - обработать offline
  - различать initial loading и background refetching
- Realtime:
  - интегрировать TanStack Query с WebSocket / SSE
  - обновлять кэш по событиям через setQueryData
  - инвалидировать запросы по событиям через invalidateQueries
  - обеспечить консистентность между realtime и polling
  - не дублировать realtime-события в отдельном store
- Современный use hook и Suspense:
  - реализовать хотя бы один сценарий с use и Suspense
  - сравнить с эквивалентом на useEffect + useState
  - понять, в каких случаях use действительно упрощает код
  - разобраться в ограничениях use и его связи с Server Components
- Архитектура state:
  - разделить UI state / domain state / server state / URL state
  - определить границы между слоями
  - вынести бизнес-логику в отдельные модули / hooks
  - вынести API-логику в API layer
  - избегать дублирования server state в Redux
  - избегать prop drilling
  - избегать giant global store
  - обосновать, почему для конкретных данных выбран конкретный инструмент
- Производительность:
  - минимизировать ререндеры
  - использовать memo, useMemo, useCallback там, где это оправдано
  - использовать selector-based subscriptions
  - избежать лишних запросов
  - использовать prefetching
  - проанализировать приложение через React DevTools Profiler
  - проанализировать сетевые запросы через Network tab
  - устранить лишние ререндеры и лишние запросы
- Сравнение и рекомендации:
  - для каждой категории состояния определить подходящий инструмент
  - обосновать выбор
  - устранить дублирование состояния
  - устранить лишние ререндеры
  - устранить лишние запросы
  - сформулировать принцип «начинать с простого решения»
  - зафиксировать в README, почему не был выбран более сложный инструмент
- Финальная задача:
  - все данные Task Management System приходят через TanStack Query
  - клиентское состояние управляется через Redux Toolkit (или обоснованно выбранную альтернативу)
  - forms управляются через React Hook Form
  - filters / sorting / pagination живут в URL
  - authentication flow работает с автоматическим refresh
  - все состояния (loading / error / empty / success) корректно обрабатываются
  - realtime-события обновляют кэш
  - отсутствуют лишние запросы и лишние ререндеры
  - обосновать в README выбор инструментов state management и API integration
  - описать архитектуру state в README
  - добавить диаграмму потоков данных: UI → hooks → API layer → backend → cache → UI
  - подготовить минимум 3 ADR:
    - выбор TanStack Query для server state
    - выбор Redux Toolkit (или альтернативы) для client state
    - выбор подхода к authentication flow

#### Дополнительная литература
- Tobias Renholt — «Data Fetching with TanStack Query: Caching, Synchronization, and Server State for Modern Web Apps» (HiTeX Press, 2026) → Специализированное руководство именно по TanStack Query, написанное для опытных React-разработчиков, которые хотят архитектурного понимания server state, а не поверхностного знакомства с хуками. Книга рассматривает data fetching как системную проблему: синхронизацию, идентичность кэша, инвалидацию, жизненные циклы рендеринга и операционную корректность в production-условиях. Разбираются declarative queries, дисциплина query keys, freshness policies, background refetching, mutation workflows, targeted invalidation, pagination, infinite loading, prefetching, SSR hydration, persistence и offline behavior. Хорошо дополняет официальную документацию структурированным объяснением того, как проектировать query-архитектуру, которая масштабируется, и как осознанно выбирать trade-offs.
- Daishi Kato — «Micro State Management with React Hooks: Explore custom hooks libraries like Zustand, Jotai, and Valtio to manage global states» (Packt, 2022) → Системное сравнение библиотек управления состоянием в React: Context, Redux, Zustand, Jotai, Valtio, Recoil и других. Книга показывает, как разбивать состояние на части (micro state management), как переиспользовать логику через hooks и как выбирать библиотеку под конкретный домен — включая form state и server cache state. Особенно полезна для понимания того, почему разные библиотеки решают разные задачи и как выбирать инструмент осознанно, а не по привычке.
- Thomas Findlay — «React — The Road To Enterprise: JavaScript Edition» (2023) → Продвинутое практическое руководство по построению поддерживаемых, масштабируемых и производительных React-приложений на TypeScript. Книга последовательно разбирает scalable project architecture, API layer и управление async-операциями, state management patterns, Redux Toolkit, Zustand и Jotai, advanced component patterns и performance optimisation. Хорошо связывает выбор инструмента управления состоянием с архитектурой приложения в целом и показывает, как не превратить проект в набор несогласованных решений.
- Kieran West — «Mastering Modern State Management in React 19: A Pragmatic and In-depth Guide to Building Scalable, Type-Safe Applications in React with TypeScript» → Практическое руководство по современному управлению состоянием в React 19 с акцентом на Redux Toolkit и TypeScript. Книга ориентирована на написание масштабируемого, типобезопасного и предсказуемого кода и хорошо подходит для перехода от базового знания Redux к осознанному применению Redux Toolkit в production-приложениях. Дополняет материалы раздела практическим взглядом на то, как организовать client state так, чтобы он не конфликтовал с server state.
- «Frontend Architecture: Components, State, and DX for Large Web Apps» (2026) → Практическое руководство по архитектуре больших frontend-приложений, написанное для senior-инженеров, tech lead'ов и архитекторов. Книга показывает, как выбирать и структурировать state management без overengineering, как проводить чёткие границы между UI, доменной логикой и инфраструктурой и как предотвращать архитектурную деградацию по мере роста команды и кодовой базы. Особенно полезна тем, что рассматривает state management не изолированно, а как часть общей архитектуры приложения, и хорошо готовит к следующему разделу — «Архитектура фронтенд-приложений».

## Архитектура и безопасность Frontend

### 29. Архитектура фронтенд-приложений

Цель: изучить архитектурные подходы к построению frontend-приложений — модульность, слои, state, microfrontends, ADR и trade-offs.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                                                         | Ссылка                                        |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 29.1 | Ulbi TV. Архитектура современных FRONTEND приложений. 5 видов. Преимущества и недостатки | [YouTube](https://www.youtube.com/watch?v=c3JGBdxfYcU) |
| 29.2 | theSeniorDev. Every Frontend Architecture Pattern Explained in 23 Minutes                                                                            | [YouTube](https://www.youtube.com/watch?v=9-r0RuX0pqk) |
| 29.3 | Reactify. Эволюция Frontend Архитектуры: от Монолита до Microfrontends (Monorepo, Multirepo)                          | [YouTube](https://www.youtube.com/watch?v=zZYfLZcUJ7Y) |
| 29.4 | Егор Локи. Архитектура в React: правильная структура приложения [Frontend]                          | [YouTube](https://www.youtube.com/watch?v=pnMyvVK4B9E) |

#### Обязательная самостоятельная практика

После изучения материалов закрепить на практике:

- **Основы архитектурного мышления:**

  - что такое software architecture и чем она отличается от структуры папок и design patterns
  - функциональные и нефункциональные требования
  - scalability, performance, maintainability, security, testability
  - coupling и cohesion
  - separation of concerns
  - dependency direction
  - architectural boundaries
  - technical debt и architectural degradation
  - trade-offs и отсутствие «идеальной» архитектуры
- **Архитектурные стили frontend-приложений:**

  - frontend monolith
  - layered architecture
  - modular monolith
  - component-based architecture
  - feature-based architecture
  - domain-oriented architecture
  - MVC / MVP / MVVM — понимать основные идеи и исторический контекст
  - server-driven UI — понимать концепцию и trade-offs
  - microfrontends — назначение, преимущества, недостатки и критерии применения
- **Модульность и декомпозиция:**

  - как определять границы модулей и features
  - public / private API модулей
  - dependency graph
  - предотвращение circular dependencies
  - shared code и проблема чрезмерного переиспользования
  - shared UI / utilities / domain logic
  - barrel exports и их влияние на зависимости
  - как не превратить приложение в набор слишком мелких модулей
- **Архитектура React-приложения:**

  - component / feature / page / domain / infrastructure / shared
  - разделение UI, бизнес-логики, state и API
  - custom hooks
  - service layer
  - API layer
  - model / domain layer
  - state layer
  - routing layer
  - adapters: API → domain → UI
  - dependency inversion на frontend
  - data fetching / caching
- **Управление состоянием:**

  - local state vs global state
  - client state vs server state
  - UI state, form state и URL state
  - когда использовать React state / Context / Redux Toolkit / server-state libraries
  - derived state и selectors
  - нормализация состояния
  - immutable updates
  - типичные ошибки глобального state management
- **Архитектура API и данных:**

  - единый API client
  - transport / API / domain layers
  - DTO и domain models
  - обработка ошибок
  - authentication / authorization
  - access / refresh tokens как часть authentication architecture
  - caching и invalidation
  - optimistic updates
  - pagination / infinite scroll
  - cancellation и timeout
  - runtime validation внешних данных
  - REST / WebSocket / SSE — понимать, когда какой подход оправдан
- **Routing и URL:**

  - route hierarchy
  - nested routes
  - protected routes
  - dynamic routes
  - URL как источник состояния
  - query parameters
  - deep linking
  - 404 / unauthorized / forbidden
  - layouts и route-level data loading
- **UI Architecture:**

  - reusable components
  - composition
  - compound components
  - controlled / uncontrolled components
  - UI primitives
  - design tokens и основы design system
  - accessibility как архитектурное требование
  - единый подход к loading / error / empty / success states
- **Frontend Security:**

  - XSS
  - CSRF
  - CORS
  - clickjacking
  - CSP
  - cookies vs localStorage / sessionStorage
  - OAuth 2.0 / OpenID Connect — концептуально
  - frontend authorization ≠ backend authorization
  - почему frontend нельзя считать доверенной средой
- **Performance Architecture:**

  - code splitting и lazy loading
  - route-level splitting
  - tree shaking
  - bundle analysis
  - caching
  - preloading / prefetching
  - image optimization
  - rendering performance
  - minimizing unnecessary re-renders
  - virtualization
  - Core Web Vitals
  - DevTools / Lighthouse для анализа производительности
- **Testing Architecture:**

  - unit / integration / component / E2E
  - test boundaries
  - mocking и test doubles
  - API / contract testing — понимать концепцию
  - тестирование state и пользовательских сценариев
  - testability как архитектурное требование
- **Monorepo и управление frontend-проектом:**

  - monorepo vs multirepo
  - workspaces и shared packages
  - dependency graph
  - code ownership
  - build caching
  - границы пакетов
  - проблемы чрезмерного количества shared packages
  - monorepo ≠ microfrontends
- **Microfrontends:**

  - зачем появились microfrontends
  - organizational boundaries
  - independent deployment
  - runtime vs build-time integration
  - Module Federation
  - shared dependencies
  - communication между microfrontends
  - authentication, routing и design system
  - observability и failure isolation
  - основные проблемы: complexity, duplication, consistency, performance
  - когда microfrontends не нужны
- **Архитектурная документация:**

  - Architecture Decision Records (ADR)
  - Context / Decision / Consequences
  - C4 Model на базовом уровне
  - dependency diagrams
  - sequence diagrams
  - фиксация архитектурных решений и их причин
- **Эволюция архитектуры:**

  - начинать с простого решения
  - evolutionary architecture
  - incremental refactoring
  - technical debt
  - migration strategies
  - strangler pattern
  - feature flags
  - backward compatibility
  - premature architecture
  - постепенное выделение модулей из frontend-монолита
- **Итоговая архитектурная практика:**

  - определить ограничения проекта:
    - размер команды
    - количество разработчиков
    - ожидаемый масштаб приложения
    - требования к deployment
    - требования к производительности
    - требования к безопасности
    - требования к независимой разработке и релизам
  - провести архитектурный review Task Management System
  - определить функциональные и нефункциональные требования проекта
  - выбрать подходящую архитектуру и обосновать выбор
  - рассмотреть минимум 3 архитектурных варианта:
    - простой React-монолит
    - modular / feature-based frontend
    - microfrontend architecture
  - для каждого варианта определить:
    - структуру проекта
    - границы модулей
    - dependency graph
    - state management
    - API layer
    - routing
    - authentication
    - testing
    - deployment
    - плюсы и минусы
    - основные риски
    - условия применения
  - выбрать один вариант как основной и письменно объяснить выбор
  - создать минимум 5 ADR
  - построить C4 Context и Container diagrams
  - определить dependency rules и public API модулей
  - проверить circular dependencies
  - провести bundle / performance analysis
  - определить security boundaries
  - определить testing strategy
  - подготовить migration plan
  - провести итоговый architecture review после завершения проекта
  - отдельно обосновать, почему microfrontends для текущего проекта, скорее всего, преждевременны

#### Дополнительная литература

- Neal Ford, Mark Richards, Pramod Sadalage, Zhamak Dehghani — «Software Architecture: The Hard Parts»
  → Одна из самых полезных книг именно для формирования архитектурного мышления. Главная ценность — не набор готовых паттернов, а методика анализа trade-off'ов, coupling, modularity, decomposition, contracts и эволюции архитектуры. Особенно полезна после первых практических архитектурных решений.
- Neal Ford, Mark Richards — «Fundamentals of Software Architecture», 2nd Edition
  → Фундаментальная книга для понимания software architecture: architectural characteristics, architectural styles, modularity, coupling, architecture fitness functions и принятия архитектурных решений. Это скорее книга для формирования инженерного мышления, чем конкретно про React.
- Micah Godbolt — «Frontend Architecture for Design Systems»
  → Одна из наиболее непосредственно релевантных книг именно для frontend architecture. Рассматривает frontend как самостоятельную архитектурную дисциплину, включая организацию HTML/CSS/JavaScript, modular CSS, BEM, design systems и архитектурный процесс. Книга 2016 года, поэтому современные инструменты и React-подходы необходимо сверять с актуальной документацией, но фундаментальные идеи остаются полезными.
- Luca Mezzalira — «Building Micro-Frontends: Distributed Systems for the Frontend», 2nd Edition
  → Основная книга для темы microfrontends. Второе издание вышло в 2025 году и значительно лучше соответствует современному состоянию подхода. Рассматривает архитектуру, независимую разработку и deployment, границы команд, композицию frontend-систем и масштабирование организации.
- Martin Kleppmann, Chris Riccomini — «Designing Data-Intensive Applications», 2nd Edition
  → Несмотря на то что книга не про frontend, я бы добавил её именно на этом этапе как переход от frontend architecture к полноценному system design. Второе издание вышло в феврале 2026 года и рассматривает reliability, scalability, distributed systems, consistency, cloud architecture, microservices и архитектурные trade-off'ы. Это поможет понимать, что происходит за REST API, которое frontend использует, и принимать архитектурные решения уже на уровне всей системы.

### 30. Web Security

Цель: освоить безопасность web-приложений — XSS, CSRF, CORS, CSP, работа с cookies, secrets и security boundaries.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                                                                                                                   | Ссылка                                                                                |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 30.1 | Александр Ламков. Безопасность в React: защита от XSS и работа с чувствительными данными. Подсветка фрагмента поиска | [YouTube](https://www.youtube.com/watch?v=AwMFWuUJXnk)                                         |
| 30.2 | Feross. Stanford University. CS 253: Web Security                                                                                                                                                              | [YouTube](https://www.youtube.com/watch?v=5JJrJGZ_LjM&list=PL1y1iaEtjSYiiSGVlL1cHsXN_kvJOOhu-) |

#### Обязательная самостоятельная практика

После изучения материалов — **обязательная практическая часть**.

- **Browser Security Model**

  - понятие origin: scheme + host + port
  - Same-Origin Policy (SOP)
  - same-origin vs same-site
  - trust boundaries в браузере
  - почему frontend-код нельзя считать доверенным
  - модель угроз для SPA/React-приложения
  - основные поверхности атаки браузерного приложения
- **HTTPS / TLS**

  - зачем нужен HTTPS
  - TLS на концептуальном уровне
  - confidentiality, integrity, authentication
  - certificate validation
  - HTTP → HTTPS
  - Mixed Content
  - Strict-Transport-Security (HSTS)
  - почему все страницы и API должны работать через HTTPS
  - связь HTTPS, Secure Cookies и защиты от MITM
- **XSS**

  - Reflected XSS
  - Stored XSS
  - DOM-based XSS
  - источники и точки вывода пользовательских данных
  - безопасное отображение пользовательского HTML/текста
  - innerHTML, outerHTML, insertAdjacentHTML
  - dangerouslySetInnerHTML в React
  - escaping и output encoding
  - sanitization
  - DOMPurify и аналогичные подходы
  - Content Security Policy (CSP)
  - Trusted Types
  - XSS через URL, query parameters, hash и данные из API
  - самостоятельное обнаружение и исправление XSS в тестовом приложении
- **CSRF**

  - механизм CSRF
  - почему cookie-based authentication создаёт CSRF-риск
  - SameSite Cookies
  - CSRF-токены
  - проверка Origin / Referer
  - отличие CSRF от XSS
  - когда CSRF актуален для SPA
  - защита frontend-приложения при работе с cookie-based authentication
- **CORS**

  - отличие SOP от CORS
  - simple requests
  - preflight (OPTIONS)
  - Access-Control-Allow-Origin
  - Access-Control-Allow-Credentials
  - Access-Control-Allow-Headers
  - wildcard * и credentials
  - типичные ошибки конфигурации CORS
  - почему CORS не является механизмом аутентификации или авторизации
  - диагностика CORS через DevTools
- **Cookies**

  - Secure
  - HttpOnly
  - SameSite
  - Domain
  - Path
  - Max-Age / Expires
  - session cookies
  - cookie-based authentication
  - риски хранения чувствительных данных в cookies
  - отличие cookie от localStorage и sessionStorage
- **Web Storage и клиентское хранение данных**

  - localStorage
  - sessionStorage
  - IndexedDB — на уровне понимания
  - какие данные допустимо хранить на клиенте
  - почему наличие данных в localStorage не делает их защищёнными
  - риски хранения access/refresh tokens
  - чувствительные данные и клиентский storage
  - browser cache и риск утечки чувствительных данных
  - Cache-Control и no-store для чувствительных ответов
- **Безопасность frontend-аутентификации**

  - безопасная работа frontend с authentication state
  - обработка 401 Unauthorized
  - обработка истёкшей сессии
  - frontend refresh-flow на уровне взаимодействия с API
  - logout и очистка клиентского состояния
  - безопасная обработка cookies
  - почему frontend authentication state не является механизмом безопасности
  - backend остаётся окончательной границей доверия
- **Frontend Authorization**

  - protected routes
  - скрытие/отображение UI в зависимости от прав
  - 401 vs 403
  - защита маршрутов в React/Next.js
  - почему скрытие кнопки не является защитой
  - почему любые frontend-проверки authorization должны дублироваться backend-проверками
  - типичные ошибки реализации client-side authorization
- **Security Headers**

  Изучить назначение и практическое применение:

  - Content-Security-Policy (CSP)
  - Strict-Transport-Security (HSTS)
  - X-Content-Type-Options
  - Referrer-Policy
  - Permissions-Policy
  - X-Frame-Options
  - frame-ancestors в CSP
- **Clickjacking**

  - принцип атаки
  - iframe и embedding
  - X-Frame-Options
  - CSP frame-ancestors
  - защита чувствительных страниц и действий
- **Безопасность URL и навигации**

  - open redirect
  - небезопасные redirect URL
  - javascript: URLs
  - пользовательские URL
  - target="_blank" и rel="noopener noreferrer"
  - безопасная обработка callback/redirect URL
  - URL-параметры как источник недоверенных данных
- **Input / Output Security**

  - любой пользовательский ввод считается недоверенным
  - данные из URL, формы, localStorage, cookies и API нельзя автоматически считать безопасными
  - client-side validation не является security-механизмом
  - runtime validation данных от API
  - schema validation
  - безопасная обработка ошибок
  - предотвращение утечки чувствительных данных через UI и логи
- **Secrets и environment variables**

  - отличие public configuration от secrets
  - почему `.env` во frontend-приложении не делает значение секретным
  - попадание переменных окружения в production bundle
  - API keys и public keys
  - что никогда нельзя помещать во frontend bundle
  - правильное разделение frontend/backend secrets
- **Dependency Security**

  - npm supply-chain attacks
  - malicious packages
  - dependency confusion
  - typosquatting
  - lock-файлы
  - обновление зависимостей
  - npm audit
  - анализ транзитивных зависимостей
  - минимизация количества зависимостей
  - риски сторонних скриптов и библиотек
- **Third-Party JavaScript**

  - риски сторонних `<script>`
  - analytics, widgets, CDN scripts и tag managers
  - потеря контроля над изменениями third-party code
  - выполнение стороннего кода с привилегиями страницы
  - утечка чувствительных данных третьим сторонам
  - Subresource Integrity (SRI)
  - sandboxing через iframe
  - минимизация количества third-party scripts
  - контроль и обновление сторонних библиотек
- **WebSocket / SSE Security**

  - безопасность WebSocket-соединений
  - origin и authentication
  - authorization после установления соединения
  - валидация входящих сообщений
  - защита от утечки чувствительных данных
  - базовые security considerations для SSE
- **Безопасность работы с API**

  - безопасная передача credentials
  - обработка 401 / 403
  - timeout
  - retry
  - cancellation запросов
  - предотвращение повторной отправки чувствительных операций
  - безопасное логирование
  - отсутствие access tokens, passwords и других secrets в логах
  - корректная обработка ошибок API
- **Business Logic Security**

  - frontend не является источником истины для security-relevant данных
  - нельзя доверять userId, role, taskId и другим значениям, пришедшим от клиента
  - hidden fields не являются защищёнными
  - disabled fields не являются защищёнными
  - данные, установленные JavaScript, должны рассматриваться как пользовательский ввод
  - client-side validation не заменяет server-side validation
  - бизнес-правила должны проверяться на backend
  - проверка ownership и permissions должна выполняться на backend
  - защита от обхода последовательности бизнес-операций
  - frontend должен рассматриваться как средство UX, а не как security boundary
- **React / Next.js Security Boundaries**

  - безопасность React rendering model
  - опасность dangerouslySetInnerHTML
  - пользовательский HTML
  - Server Components vs Client Components с точки зрения security boundary
  - server-only и client-exposed environment variables в Next.js
  - cookies/headers
  - Route Handlers
  - Server Actions
  - защита server-side secrets
  - недопустимость переноса серверных секретов в client bundle
- **Security Testing**

  Провести базовый security review собственного **Task Management System**:

  - определить assets
  - определить trust boundaries
  - определить attack surfaces
  - составить threat model
  - проверить HTTPS/TLS и Mixed Content
  - проверить XSS
  - проверить CSRF
  - проверить CORS
  - проверить cookies
  - проверить authentication flow на frontend-уровне
  - проверить authorization
  - проверить security headers
  - проверить clickjacking
  - проверить open redirects
  - проверить sensitive data exposure
  - проверить third-party scripts
  - проверить dependency vulnerabilities
  - проверить business logic
  - проверить обработку ошибок
  - проверить WebSocket/API security при наличии соответствующих функций
- **Использовать:**

  - Browser DevTools
  - PortSwigger Web Security Academy
  - Burp Suite Community Edition
  - OWASP Web Security Testing Guide

#### Дополнительная литература

- Dafydd Stuttard, Marcus Pinto — «The Web Application Hacker's Handbook», 2nd Edition
  → Фундаментальная книга по безопасности web-приложений: HTTP, browser security, authentication, session management, XSS, CSRF, access control, injection и другим типичным уязвимостям. Несмотря на возраст книги, она остаётся важным фундаментальным источником и хорошо дополняет практику PortSwigger Web Security Academy. Сам PortSwigger рекомендует её как дополнительный материал.
- Michal Zalewski — «The Tangled Web: A Guide to Securing Modern Web Applications»
  → Глубокое объяснение внутренней модели безопасности Web: Same-Origin Policy, origins, cookies, HTTP, JavaScript, DOM, browser security и взаимодействие различных механизмов браузера. Особенно полезна именно для понимания того, почему Web Security работает так, а не просто для запоминания отдельных защитных механизмов. OWASP также включает книгу в рекомендуемую литературу.
- Malcolm McDonald — «Web Security for Developers: Real Threats, Practical Defense»
  → Практическая книга именно с позиции разработчика: XSS, CSRF, SQL injection, authentication, sessions и другие типичные угрозы с акцентом на безопасную реализацию. Хорошо подходит как более прикладное дополнение к фундаментальной «The Tangled Web».
- Tanya Janca — «Alice and Bob Learn Application Security»
  → Системное введение в application security и Secure Development Lifecycle. Рассматривает security fundamentals, security requirements, secure design, secure coding, common pitfalls, testing и deployment. Особенно полезна для формирования security mindset при разработке собственного приложения.
- PortSwigger — «Web Security Academy»
  → Главный практический ресурс раздела. Это не книга, а постоянно обновляемая интерактивная платформа с теорией и лабораториями по XSS, CSRF, CORS, Clickjacking, DOM-based vulnerabilities, WebSockets, Authentication, Access Control и другим web-уязвимостям. Использовать после теоретических материалов для практической отработки.

### 31. WebSockets / SSE

Цель: освоить realtime-коммуникацию — WebSocket, STOMP, SSE, reconnect, authentication и масштабирование соединений.

#### Ресурсы для изучения

| #    | Ресурс                                                                                                 | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 31.1 | Ulbi TV. Что такое WebSocket? WebSockets простыми словами                             | [YouTube](https://www.youtube.com/watch?v=SxMvxIHBahU) |
| 31.2 | Тихон Галактионов. SSE за 10 минут: как сервер сам шлёт данные  | [YouTube](https://www.youtube.com/watch?v=2Wv2MGqUN0E) |
| 31.3 | Ulbi TV. WebSockets React & Node.js — полный курс Paint Online & Canvas                           | [YouTube](https://www.youtube.com/watch?v=KVeMsy4qCdg) |
| 31.4 | Java Techie. Build Real-Time Notifications in Spring Boot Applications Using WebSocket                       | [YouTube](https://www.youtube.com/watch?v=sqYqyr6EpAU) |
| 31.5 | codingX krishna. Spring Boot WebSocket + React Tutorial for Beginners — Real-Time Chat App Explained Simply | [YouTube](https://www.youtube.com/watch?v=2iPBkOlIrpA) |

#### Обязательная самостоятельная практика

После изучения материалов обязательно самостоятельно изучить теоретическую часть:

- **WebSocket — основы:**

  - назначение, принцип работы и области применения
  - отличие WebSocket от обычного HTTP request / response
  - WebSocket handshake и переход от HTTP к WebSocket-соединению
  - WebSocket lifecycle
  - connection states: `CONNECTING`, `OPEN`, `CLOSING`, `CLOSED`
  - события `open`, `message`, `error`, `close`
  - graceful disconnect и обработка разрыва соединения
  - reconnect strategies
  - exponential backoff и ограничение количества попыток переподключения
  - heartbeat / keep-alive и обнаружение неактивного соединения
- **WebSocket — обмен сообщениями:**

  - двусторонняя передача данных через WebSocket
  - message format: JSON и структура сообщений
  - subscriptions и publish / subscribe
- **STOMP:**

  - назначение и отличие от WebSocket
  - STOMP frames: `CONNECT`, `SEND`, `SUBSCRIBE`, `MESSAGE`, `UNSUBSCRIBE`, `DISCONNECT`
  - destinations, topics и queues
  - routing сообщений в STOMP
- **WebSocket — безопасность и ошибки:**

  - authentication / authorization
  - обработка ошибок и disconnect на клиенте и сервере
- **SSE — основы:**

  - назначение и принцип работы
  - отличие SSE от WebSocket
  - однонаправленная модель Server → Client
  - EventSource API
  - SSE connection lifecycle
  - SSE events: `event`, `data`, `id`, `retry`
  - автоматическое переподключение SSE
  - Last-Event-ID и восстановление потока событий
  - ограничения SSE
  - authentication и ограничения браузерного EventSource
- **Выбор технологии:**

  - WebSocket vs SSE: критерии выбора
  - realtime notifications и SSE
  - bidirectional communication и WebSocket
  - типичные сценарии использования WebSocket
  - типичные сценарии использования SSE
- **React integration:**

  - WebSocket API
  - EventSource API
  - lifecycle соединения в React
  - `useEffect` и cleanup
  - хранение connection state
  - обработка incoming messages
  - reconnect
  - предотвращение утечек соединений
  - интеграция realtime-событий с состоянием приложения
- **Spring WebSocket integration:**

  - WebSocket configuration
  - WebSocket endpoints
  - STOMP integration
  - message mappings
  - destinations / topics
  - subscriptions
  - отправка сообщений клиентам
  - обработка подключений и отключений
- **Spring SSE integration:**

  - SSE endpoints
  - `SseEmitter`
  - отправка событий клиенту
  - обработка completion / timeout / error
  - управление активными подключениями
  - базовое понимание SSE через реактивный подход Spring WebFlux / `Flux`
- **Безопасность realtime-соединений:**

  - CORS и WebSocket / SSE
  - авторизация подписок и сообщений
  - передача JWT / cookies при установлении соединения
  - защита от несанкционированных подписок
- **Масштабирование realtime-соединений:**

  - stateful connections
  - несколько экземпляров backend
  - необходимость внешнего broker / shared state
  - базовое понимание Redis Pub/Sub как способа доставки событий между экземплярами

#### Практическая часть

После изучения материалов обязательно применить знания на практике в **Task Management System**:

- реализовать WebSocket-соединение между React и Spring Boot
- реализовать STOMP subscriptions
- реализовать отправку и получение сообщений
- реализовать connection states на frontend
- реализовать обработку `open` / `message` / `error` / `close`
- реализовать reconnect с exponential backoff
- реализовать heartbeat / keep-alive
- корректно закрывать соединение при unmount React-компонента
- реализовать realtime-уведомления в Task Management System через WebSocket
- реализовать SSE endpoint в Spring Boot
- подключить React через EventSource
- реализовать realtime-обновление данных через SSE
- обработать автоматический reconnect SSE
- реализовать authentication / authorization для realtime-соединений
- определить, какие события Task Management System передавать через WebSocket, а какие через SSE
- протестировать потерю соединения и последующее восстановление
- протестировать несколько одновременно подключённых клиентов
- проверить корректное освобождение ресурсов после disconnect
- реализовать базовую поддержку realtime-соединений при нескольких экземплярах backend
- документировать архитектуру WebSocket / SSE в README

#### Дополнительная литература

- Andrew Lombardi — «WebSocket: Lightweight Client-Server Communications» → главная специализированная книга по WebSocket. Охватывает WebSocket API, двусторонний обмен, STOMP over WebSocket, совместимость, безопасность, отладку и сам протокол. Очень хорошо соответствует теоретической части раздела
- Ilya Grigorik — «High Performance Browser Networking» → отличная фундаментальная книга по сетевым технологиям браузера. Отдельные главы посвящены SSE и WebSocket, включая EventSource, event stream, WebSocket API, handshake, WSS, производительность, overhead и deployment. Для понимания того, что происходит «под капотом», это одна из самых полезных книг
- Darren Cook — «Data Push Apps with HTML5 SSE» → специализированная книга по Server-Sent Events: EventSource, серверная и клиентская части, realtime-обновления, обработка ошибок и восстановление после проблем с соединением. Книга старая (2014), поэтому использовать её именно для глубокого понимания SSE, а не современных frontend-фреймворков
- Craig Walls — «Spring in Action» (6th ed.) (см. разделы 8–9) → не книга именно про WebSocket, но хорошее дополнение для понимания Spring-подхода к messaging, asynchronous communication и reactive applications. Использовать выборочно в контексте Spring-части roadmap. 6-е издание вышло в 2022 году и ориентировано на Spring 5.3 / Spring Boot 2.4, поэтому не воспринимать примеры как актуальную документацию для современного Spring Boot
- Claudio Eduardo de Oliveira — «Spring 5.0 By Example» → полезна именно для Spring-реализации SSE: в книге есть отдельный раздел по Server-Sent Events и сравнению SSE с WebSockets. Книга старая, поэтому использовать как дополнительный источник по концепциям и Spring API, а не как основное современное руководство

## Тестирование и развёртывание Frontend

### 32. Frontend Testing

Цель: научиться тестировать frontend — unit, component, integration и E2E через Vitest, React Testing Library, MSW и Playwright.

#### Ресурсы для изучения

| #    | Ресурс                                                                                         | Ссылка                                                                                |
| ---- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 32.1 | Михаил Непомнящий. Тестирование JavaScript и React приложений | [Stepik](https://stepik.org/course/200433/promo)                                               |
| 32.2 | Codevolution. React Testing Tutorial                                                                 | [YouTube](https://www.youtube.com/watch?v=T2sv8jXoP4s&list=PLC3y8-rFHvwirqe1KHFCHJ0RqNuN61SJd) |
| 32.3 | Cosden Solutions. React Testing with Playwright (Complete Tutorial)                                  | [YouTube](https://www.youtube.com/watch?v=3NW0Mz943_E)                                         |

#### Обязательная самостоятельная практика

После изучения материалов — **обязательный самостоятельный практический блок**.

Добавить полноценное тестирование для **Task Management System**:

- **Unit Testing:**

  - тестирование чистых функций и utility-логики
  - тестирование преобразования и валидации данных
  - тестирование фильтрации, сортировки и поиска задач
  - тестирование функций работы с датами, pagination и query parameters
  - тестирование обработки ошибок
  - использовать Vitest или Jest
- **React Component Testing:**

  - тестирование отдельных React-компонентов
  - проверка различных props и состояний компонентов
  - тестирование пользовательских взаимодействий
  - тестирование controlled / uncontrolled forms
  - тестирование валидации форм
  - тестирование loading / success / error / empty states
  - тестирование доступности основных элементов
  - ориентироваться на поведение, наблюдаемое пользователем, а не на внутреннюю реализацию компонентов
  - использовать React Testing Library
- **Integration Testing:**

  - тестирование взаимодействия нескольких React-компонентов
  - тестирование взаимодействия компонентов с state management
  - тестирование взаимодействия UI с API layer
  - тестирование authentication flow
  - тестирование CRUD-сценариев работы с задачами
  - использовать MSW для перехвата HTTP-запросов и изоляции frontend от реального backend
- **E2E Testing:**

  - настроить Playwright
  - тестировать приложение в реальном браузере
  - использовать устойчивые selectors
  - использовать assertions и auto-waiting
  - тестировать navigation и routing
  - тестировать Login / Registration
  - тестировать authentication flow
  - тестировать создание, редактирование и удаление задач
  - тестировать поиск, фильтрацию и сортировку
  - тестировать pagination
  - тестировать protected routes
  - тестировать обработку 404 / unauthorized / forbidden
  - тестировать loading / error / empty states
  - тестировать критические пользовательские сценарии целиком
- **API и E2E:**

  - использовать Playwright API testing для проверки REST API
  - подготовка и очистка тестовых данных
  - комбинировать API и UI в одном E2E-сценарии
  - использовать API для быстрого создания test data перед UI-тестом
  - проверять соответствие поведения UI и API
- **Test Data:**

  - разделить production / development / test data
  - создавать независимые тестовые данные
  - избегать зависимости тестов друг от друга
  - обеспечить повторяемость тестов
  - реализовать setup / teardown
  - не использовать реальные пользовательские данные
- **Mocking:**

  - понимать, когда использовать mock, stub и fake
  - мокировать внешние HTTP-зависимости на уровне component/integration tests
  - использовать MSW для перехвата API-запросов
  - не злоупотреблять mocking в E2E-тестах
  - понимать разницу между тестированием изолированной логики и реального пользовательского сценария
- **Test Architecture:**

  - разделить unit / component / integration / E2E тесты
  - определить границы каждого уровня тестирования
  - не дублировать один и тот же сценарий на всех уровнях без необходимости
  - вынести общие test utilities
  - организовать fixtures и test data
  - использовать Page Object / test helpers там, где это действительно оправдано
  - обеспечить читаемость и поддерживаемость тестов
- **Quality:**

  - проверять отсутствие flaky tests
  - не использовать ненадёжные selectors, зависящие от CSS-структуры
  - не использовать избыточные timeouts и искусственные delays
  - проверять независимость тестов
  - анализировать причины падения тестов
  - рефакторить дублирующийся test code
  - поддерживать тесты при изменении UI
  - избегать тестирования деталей реализации, не имеющих значения для пользователя
- **Coverage:**

  - понимать code coverage и test coverage
  - настроить coverage для unit/component tests
  - анализировать покрытие критической бизнес-логики
  - не стремиться к 100% coverage любой ценой
  - определить критические пользовательские сценарии, которые обязательно должны покрываться E2E
- **CI:**

  - запускать unit/component tests в CI
  - запускать Playwright E2E tests в CI
  - настроить GitHub Actions
  - сохранять test reports и screenshots при падении тестов
  - сохранять Playwright traces / videos при необходимости
  - разделить быстрые тесты и E2E-тесты
  - запускать полный набор тестов перед production deployment
- **Итоговая практика:**

  - добиться стабильного прохождения всех тестов локально
  - настроить автоматический запуск тестов через GitHub Actions
  - исправить flaky tests
  - получить итоговый test report
  - документировать testing strategy проекта
  - в README описать:
    - используемые виды тестирования
    - используемые инструменты
    - структуру тестов
    - команды запуска
    - запуск тестов в CI
    - основные покрытые пользовательские сценарии

#### Дополнительная литература

- Kent C. Dodds — «Testing JavaScript»
  → Один из наиболее полезных современных материалов по стратегии тестирования JavaScript-приложений. Рассматривает unit, integration и E2E testing, mocking, Jest, React Testing Library и практические принципы построения поддерживаемых тестов. Использовать как дополнительный углубляющий материал после основного курса.
- Kent C. Dodds — Epic Web / Testing resources
  → Практические материалы по современному тестированию JavaScript и React. Хорошо дополняют основной курс примерами и разбором testing philosophy, React Testing Library и E2E-подходов.
- Roy Osherove — «The Art of Unit Testing»
  → Фундаментальные принципы unit testing, isolation, mocks/stubs, maintainability и проектирование тестов.
- Vladimir Khorikov — «Unit Testing Principles, Practices, and Patterns»
  → Одна из наиболее полезных книг по архитектуре и качеству unit/integration tests. Особенно полезна для понимания границ unit-тестов, интеграционных тестов, mock'ов и поддерживаемости тестового кода.
- Steve Freeman, Nat Pryce — «Growing Object-Oriented Software, Guided by Tests»
  → Глубокое рассмотрение TDD, тестируемого дизайна и взаимодействия объектов. Не является frontend-специализированной книгой, но хорошо развивает инженерное мышление при проектировании тестируемого кода.

<a id="section-33"></a>
### 33. Frontend CI/CD + Docker

Цель: освоить полный цикл доставки frontend-приложения — CI, production build, Docker image, публикацию в registry, deployment в staging и production, rollback, security headers и эксплуатацию frontend в production-like окружении.

В этом разделе рассматривается именно frontend-специфика: сборка, контейнеризация, публикация и доставка frontend-приложения.

**Docker + React + VPS**

| #      | Ресурс                                                                                 | Ссылка                                             |
| ------ | -------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| 33.1 | Sanjeev Thiyagarajan.  Docker + ReactJS tutorial: Development to Production workflow + multi-stage builds + docker compose | [YouTube](https://www.youtube.com/watch?v=3xDAU5cvi5E) |
| 33.2 | Sarvin Style Coding. Dockerfile Tutorial for Beginners — Dockerize a React App from Scratch | [YouTube](https://www.youtube.com/watch?v=Kb2xfvmaaVo) |
| 33.3 | Net Ninja. Docker Crash Course — Dockerization React-приложения | [YouTube](https://www.youtube.com/watch?v=QePBbG5MoKk) |
| 33.4 | Code Explained. Узнайте как развернуть приложение React на VPS. Сервер Ubuntu 20.04 с Nginx | [YouTube](https://www.youtube.com/watch?v=w3RFk35synM) |

**Docker + Next.js + VPS**

| #      | Ресурс                                                                                 | Ссылка                                             |
| ------ | -------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| 33.5 | ByteGrad. Лучшая настройка Next.js: Next.js + Postgres + Docker (разработка / продакшн)  | [YouTube](https://www.youtube.com/watch?v=tm70Xa6igbY) |
| 33.6 | ByteGrad. Dockerize + Next.js 16 и развертывание приложения на VPS: пользовательский домен, SSL, CDN Cloudflare, Docker Compose) | [YouTube](https://www.youtube.com/watch?v=DCJiQBag6Fs) |

**GitHub Actions + Docker + Deploy**

| #      | Ресурс                                                                                 | Ссылка                                             |
| ------ | -------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| 33.7 |  Антон Ларичев. GitHub Actions для CI/CD | [YouTube](https://www.youtube.com/watch?v=zn5T7FkpaTA) |
| 33.8 | TechWorld with Nana. GitHub Actions Tutorial - Basic Concepts and CI/CD Pipeline with Docker | [YouTube](https://www.youtube.com/watch?v=R8_veQiYBjI) |
| 33.9 | Piyush Garg.  GitHub Actions Tutorial - Deploy Node.js Application with CI CD and GitHub Actions  | [YouTube](https://www.youtube.com/watch?v=y7S2oSjJ8PA) |

#### Самостоятельно изучаем следующие темы
- CI pipeline для frontend:
  - npm ci, кэш npm, matrix по Node.js
  - ESLint, Prettier check, tsc --noEmit
  - unit / component tests, E2E tests
  - production build
  - артефакты сборки и test reports
  - concurrency и отмена устаревших запусков
- Production build frontend:
  - отличие dev build от production build
  - code splitting, tree shaking, minification
  - source maps: private vs public
  - cache busting через хэши в именах файлов
  - build-time vs runtime configuration
  - VITE_* и NEXT_PUBLIC_* — что вшивается в bundle
  - Next.js output: 'standalone'
- Docker для frontend — SPA (React + Vite):
  - multi-stage build: node:22-alpine → nginx:alpine
  - .dockerignore
  - запуск от non-root
  - layer caching: package*.json → npm ci → остальной код
  - ARG для build-time переменных
  - HEALTHCHECK
- Docker для frontend — Next.js:
  - output: 'standalone' в next.config.js
  - multi-stage build
  - копирование standalone output
  - запуск node server.js
  - server-only env vs NEXT_PUBLIC_*
- Nginx для SPA:
  - try_files $uri /index.html — SPA fallback
  - location /api → proxy_pass
  - proxy_set_header Host / X-Real-IP / X-Forwarded-For / X-Forwarded-Proto
  - gzip
  - cache headers для assets и index.html
  - security headers
- Reverse proxy — альтернатива:
  - Traefik как альтернатива Nginx
  - Docker provider и labels
  - автоматический Let's Encrypt
  - сравнение Nginx и Traefik
- Docker Compose для frontend:
  - frontend service
  - networks, ports, env_file
  - healthcheck, depends_on
  - reverse proxy
- Публикация Docker image:
  - Docker Hub / GHCR / private registry
  - docker login, tag, push, pull
  - схема тегирования: sha-<commit>, latest, semver
  - docker/build-push-action, docker/metadata-action
  - GITHUB_TOKEN для GHCR
- CD для frontend:
  - варианты: Vercel / Netlify / Cloudflare Pages / VPS + Docker
  - staging и production
  - GitHub Environments, protection rules
  - environment-specific configuration
  - smoke tests после deployment
  - rollback: предыдущий image tag
- Домен, DNS и SSL/TLS:
  - DNS-записи: A, AAAA, CNAME
  - HTTPS / SSL/TLS
  - Let's Encrypt и автоматическое обновление
  - HTTP → HTTPS redirect, HSTS
  - Mixed Content
- Cache и CDN:
  - Cache-Control: no-cache для index.html
  - Cache-Control: public, max-age=31536000, immutable для assets
  - Cloudflare: DNS, proxy mode, SSL mode
  - cache invalidation при deployment
- Security frontend в production:
  - CSP, HSTS, X-Content-Type-Options, Referrer-Policy, Permissions-Policy, X-Frame-Options
  - private source maps
  - запрет секретов в bundle
  - npm audit, Dependabot
- Observability frontend:
  - Sentry / GlitchTip
  - Web Vitals: LCP, INP, CLS
  - source maps для stack traces
  - release versioning
- Troubleshooting frontend deployment:
  - белый экран после deployment
  - 404 на SPA-маршрутах
  - неправильный base path
  - CORS / Mixed Content
  - неправильные env на build
  - cache не инвалидируется
  - Docker image собирается, но контейнер падает
  - Nginx / Traefik не отдаёт assets
  - CSP блокирует inline scripts
  - SSL-сертификат не выпускается
  - DNS не резолвится
  - алгоритм: симптом → диагностика → причина → исправление → проверка

#### Обязательная самостоятельная практика

Выполняется на Task Management System (сквозной проект).

- Frontend CI:
  - workflow .github/workflows/frontend-ci.yml
  - триггеры: push, pull_request в main / develop
  - jobs: install, quality, test, build, e2e
  - needs, concurrency
  - загрузка dist и Playwright report как artifacts
  - pipeline падает при любой ошибке
- Production Docker image для SPA (React + Vite):
  - multi-stage Dockerfile
  - .dockerignore
  - Nginx от non-root
  - ARG для build-time переменных
  - HEALTHCHECK
  - собрать image, запустить контейнер, проверить через curl
  - проверить SPA fallback, cache headers, security headers
- Production Docker image для Next.js:
  - output: 'standalone'
  - multi-stage Dockerfile
  - runtime stage: node:22-alpine, non-root
  - HEALTHCHECK
- Nginx / Traefik:
  - настроить SPA fallback
  - location /api → backend
  - security headers, cache headers, gzip
  - проверить через curl -I
  - альтернативно — Traefik с Docker provider и Let's Encrypt
- Docker Compose для frontend:
  - frontend service
  - networks, ports, env_file, healthcheck, depends_on
  - docker compose up --build, проверить config, логи
- Публикация Docker image:
  - job docker в CI
  - docker/build-push-action, docker/metadata-action
  - теги: `sha-<commit>`, `latest`, `semver`
  - публикация в GHCR
  - docker/login-action
- Deployment на VPS:
  - SSH, установка Docker и Docker Compose
  - загрузка image из registry
  - запуск контейнера
  - автозапуск, перезапуск после reboot
  - firewall
- Домен, DNS и SSL/TLS:
  - DNS-записи → VPS
  - Let's Encrypt (Traefik или Certbot)
  - HTTP → HTTPS redirect
  - HSTS
- CDN с Cloudflare:
  - DNS в Cloudflare, proxy mode, SSL mode
  - cache invalidation при deployment
- CD — staging:
  - GitHub Environment staging
  - workflow frontend-cd-staging.yml
  - deployment на push в develop
  - smoke tests: /, /assets/*, /api/health, SPA fallback
- CD — production:
  - GitHub Environment production с protection rules
  - ручное подтверждение
  - deployment на push в main или через workflow_dispatch
  - health checks, smoke tests, HTTPS, security headers, cache headers
- Rollback:
  - стратегия: предыдущий image tag
  - rollback workflow
  - проверить на staging и production
  - задокументировать процедуру
- Security frontend в production:
  - CSP, HSTS, X-Content-Type-Options, Referrer-Policy, Permissions-Policy, X-Frame-Options
  - private source maps
  - проверка отсутствия секретов в bundle
  - Dependabot, npm audit
- Observability frontend:
  - Sentry + source maps
  - release versioning
  - Web Vitals
  - correlation ID между frontend и backend
- Cache и CDN:
  - no-cache для index.html
  - immutable для /assets/*
  - проверка через DevTools
- Troubleshooting:
  - намеренно сломать конфигурацию и восстановить
  - для каждой проблемы: симптом → диагностика → причина → исправление → проверка
  - кейсы: base path, 404 SPA, CORS, Mixed Content, env на build, cache, Docker image, Nginx/Traefik, CSP, SSL, DNS, smoke tests, rollback
- Документация:
  - frontend CI/CD pipeline в README
  - схема тегирования images
  - процедура deployment в staging и production
  - процедура rollback
  - security headers, cache strategy, troubleshooting
  - CI/CD pipeline diagram

#### Дополнительная литература

- Nigel Poulton — «Docker Deep Dive» (5th ed., 2025) → основная книга по Docker: images, containers, Dockerfile, multi-stage builds, networking, storage, security, Docker Compose. Использовать как основную книгу по контейнеризации frontend.
- Sean P. Kane, Karl Matthias — «Docker: Up & Running» (3rd ed., 2023) → практическое руководство по Docker в production: multi-stage builds, BuildKit, security.
- Brent Laster — «Learning GitHub Actions: Automation and Integration of CI/CD with GitHub» → практическое руководство по GitHub Actions: workflows, triggers, jobs, steps, secrets, artifacts, caching, matrix builds, reusable workflows, безопасность, интеграция с Docker и deployment. Хорошо закрывает инструментальную часть раздела.
- Jez Humble, David Farley — «Continuous Delivery» → фундаментальная книга по CI, Continuous Delivery, deployment pipelines, automated testing, environments и снижению рисков релизов. Полезна для понимания, почему pipeline строится как последовательность автоматизированных проверок и deployment stages.
- Gene Kim, Jez Humble, Patrick Debois, John Willis — «The DevOps Handbook» → для понимания DevOps-подхода целиком: CI/CD, automation, deployment, feedback loops, monitoring и культура эксплуатации.

## Fullstack Capstone

### 34. Fullstack Capstone + Containerization + CI/CD

Цель: объединить backend и frontend в полноценный fullstack-проект с контейнеризацией, CI/CD, staging и production deployment.

#### 34.1. Подготовка: Docker + CI/CD

Изучить до или параллельно с проектом.

| #      | Ресурс                                                                                 | Ссылка                                             |
| ------ | -------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| 34.1.1 | D. A. Engineering Hub. Automate Docker Deployment with GitHub Actions. CI/CD to Cloud | [YouTube](https://www.youtube.com/watch?v=nkVKze4-hdk&t=2s) |
| 34.1.2 | Docker + Docker Compose (материалы из раздела «Docker + Docker Compose») | [Docker + Docker Compose](#12-docker--docker-compose)                                               |
| 34.1.3 | CI/CD (GitHub Actions) (материалы из раздела «CI/CD (GitHub Actions)»)             | [CI/CD (GitHub Actions)](#14-cicd-github-actions) |
| 34.1.4 | Frontend CI/CD + Docker (материалы из раздела «Frontend CI/CD + Docker») | [Frontend CI/CD + Docker](#section-33) |

#### 34.2. Учебные fullstack-проекты

Для погружения в связку Spring Boot + React.

| #      | Ресурс                                                                                                                   | Ссылка                                                                                                                                                                      |
| ------ | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 34.2.1 | JAVA DEVELOPER. Spring Boot + React + PostgreSQL CRUD Full Stack Project\| Java Full Stack Tutorial                            | [YouTube](https://www.youtube.com/watch?v=7KCLItj09SQ)                                                                                                                               |
| 34.2.2 | Amigoscode. Spring Boot, React.js & AWS S3 Full Stack Development                                                              | [YouTube](https://www.youtube.com/watch?v=9i1gQ7w2V24)                                                                                                                               |
| 34.2.3 | Code With Zosh. Library Management System Java Full Stack\| Spring Boot, React & MySQL - 2026                                  | [Google Drive](https://drive.google.com/file/d/1EXzSg7IAUnurjACyz0C1ucD4Lv5jLSiC/view) / [YouTube](https://www.youtube.com/watch?v=jZojHz7jp5Q&list=PL7Oro2kvkIzIpLa5KwcGaCLQvQY1YxNe5) |
| 34.2.4 | Java Guides. Spring Boot React JS Full-Stack Project\| Employee Management System \| Spring Boot React JS Course               | [YouTube](https://www.youtube.com/watch?v=KuM6OtuaYRs)                                                                                                                               |
| 34.2.5 | Code With Arjun и Dev Mate. Full Stack Spring Boot and React CRUD 1.5 hours Course\| Full Stack Web App \| MySQL \| Hibernate | [YouTube](https://www.youtube.com/watch?v=4LZKnegAm4g&list=PLJLf67YAhhod0OMooE_QOYcU_D63d26_p)                                                                                       |
| 34.2.6 | freeCodeCamp.org. Full Stack Development with Java Spring Boot, React, and MongoDB – Full Course                              | [YouTube](https://www.youtube.com/watch?v=5PdEmeopJVQ)                                                                                                                               |

#### 34.3. Финальный проект — Task Management System

После изучения roadmap все предыдущие практические части объединить в один полноценный fullstack-проект.

### 34.3.1. Backend — Java / Spring Boot

- реализовать полноценный REST API на Spring Boot
- использовать архитектуру, изученную в разделе «Архитектура бэкенда»
- реализовать корректное разделение presentation / application / domain / infrastructure
- использовать DTO и mapper
- реализовать валидацию входных данных
- реализовать единый формат ошибок API
- реализовать authentication / authorization через Spring Security
- реализовать роли и permissions
- реализовать CRUD для пользователей, проектов и задач
- реализовать поиск, фильтрацию, сортировку и pagination
- реализовать optimistic locking там, где это необходимо
- реализовать транзакции
- использовать PostgreSQL
- использовать Flyway для миграций
- реализовать обработку ошибок и edge cases
- реализовать логирование
- реализовать health checks
- реализовать unit и integration tests
- использовать Testcontainers для интеграционных тестов
- подготовить OpenAPI-документацию

### 34.3.2. Frontend — React / TypeScript

- реализовать полноценный frontend на React + TypeScript
- использовать компонентную архитектуру
- реализовать routing
- реализовать управление состоянием
- реализовать authentication flow
- реализовать формы и клиентскую валидацию
- реализовать CRUD задач
- реализовать проекты и пользователей
- реализовать поиск, фильтрацию, сортировку и pagination
- реализовать loading / error / empty states
- реализовать обработку HTTP 401 / 403 / 404 / 409 / 422 / 500
- использовать типизированный API client
- использовать OpenAPI-generated types / client
- реализовать responsive UI
- реализовать frontend tests
- подготовить production build

### 34.3.3. API Contract

- поддерживать OpenAPI specification как единый контракт между backend и frontend
- документировать endpoints, request/response schemas и ошибки
- документировать authentication / authorization
- использовать generated TypeScript types / API client
- проверять совместимость frontend с изменениями backend API
- выполнять contract checks в CI

### 34.3.4. Realtime

- реализовать realtime-уведомления через WebSocket
- реализовать SSE там, где однонаправленная доставка событий является более подходящей
- реализовать reconnect
- обработать потерю соединения
- корректно освобождать realtime-соединения
- определить, какие события передавать через WebSocket, а какие через SSE

### 34.3.5. Frontend Toolchain

- настроить npm scripts
- настроить Vite
- настроить TypeScript type-check
- настроить ESLint
- настроить Prettier
- настроить Husky + lint-staged
- настроить production build
- проверить отсутствие TypeScript и lint ошибок перед сборкой

### 34.3.6. Docker

- создать production Dockerfile для frontend
- использовать multi-stage build
- использовать Node.js только на build stage
- использовать Nginx для frontend runtime
- настроить SPA fallback
- создать production Dockerfile для Spring Boot
- использовать multi-stage build для backend
- создать `.dockerignore`
- правильно организовать Docker images
- использовать отдельные configuration/environment variables для разных окружений

### 34.3.7. Docker Compose — deployment stack приложения

- Frontend container (React + Nginx)
- Spring Boot backend
- PostgreSQL
- необходимые infrastructure services
- Docker networks
- volumes
- environment variables
- secrets
- health checks
- dependency management между сервисами

**Итоговая архитектура deployment stack приложения:**

```text
                    Browser
                       │
                       ▼
                 Frontend container
                  (React + Nginx)
                   /       \
                  ▼         ▼
             static files  /api
                              │
                              ▼
                         Spring Boot
                              │
                              ▼
                         PostgreSQL
```

### 34.3.8. CI — Continuous Integration

Настроить GitHub Actions pipeline.

При Pull Request и push:

- checkout
- установка JDK
- установка Node.js
- установка зависимостей frontend
- `npm ci`
- ESLint
- TypeScript type-check
- frontend tests
- frontend production build
- Maven build
- backend unit tests
- backend integration tests
- Testcontainers
- static analysis
- проверка OpenAPI contract
- Docker image build

Pipeline должен завершаться ошибкой при:

- TypeScript errors
- ESLint errors
- failed tests
- failed integration tests
- failed Maven build
- failed frontend build
- failed Docker build
- нарушении API contract

### 34.3.9. Docker Registry

- создать Docker images frontend и backend
- использовать понятную схему тегирования
- публиковать images в container registry
- не хранить секреты в Dockerfile
- использовать GitHub Actions secrets
- разделять images для разных окружений при необходимости

### 34.3.10. CD — Continuous Deployment

Настроить deployment pipeline:

```text
Pull Request
      ↓
     CI
      ↓
    Build
      ↓
Docker images
      ↓
Container Registry
      ↓
   Staging
      ↓
Smoke / Integration Tests
      ↓
 Production
```

Реализовать:

- автоматический deployment в staging
- ручное или контролируемое продвижение в production
- environment-specific configuration
- secrets management
- health checks после deployment
- проверку доступности frontend
- проверку доступности backend
- проверку database connectivity
- rollback при неудачном deployment
- просмотр deployment logs

### 34.3.11. Staging

- Создать отдельное staging-окружение.
- Перед production deployment приложение должно успешно пройти staging verification.

Проверить:

- frontend
- backend
- PostgreSQL
- authentication
- REST API
- WebSocket / SSE
- migrations
- Docker Compose
- environment variables
- production build
- smoke tests

### 34.3.12. Production

Подготовить production deployment.

**Обязательно:**

- HTTPS
- production environment variables
- безопасная конфигурация Spring Boot
- безопасная конфигурация frontend
- Nginx reverse proxy
- database persistence
- health checks
- logging
- restart policies
- Docker image versioning
- backup strategy для PostgreSQL
- rollback strategy

### 34.3.13. Нагрузочная и эксплуатационная проверка

- проверить приложение под несколькими одновременно работающими пользователями
- проверить параллельное изменение задач
- проверить обработку конфликтов
- проверить reconnect WebSocket / SSE
- проверить отказ backend
- проверить перезапуск контейнера
- проверить восстановление после перезапуска PostgreSQL
- проверить корректность database migrations
- проверить frontend при недоступном backend
- проверить корректность error handling
- проверить основные API endpoints под нагрузкой

### 34.3.14. Финальная документация

Подготовить README проекта:

- описание проекта
- архитектура системы
- используемый стек
- структура backend
- структура frontend
- database schema
- API documentation
- authentication architecture
- WebSocket / SSE architecture
- Docker architecture
- Docker Compose
- CI/CD pipeline
- staging / production environments
- deployment instructions
- environment variables
- запуск проекта локально
- запуск тестов
- troubleshooting
- известные ограничения
- архитектурные решения и их обоснование

Добавить:

- архитектурную диаграмму
- ER-диаграмму
- sequence diagrams для ключевых сценариев
- CI/CD pipeline diagram
- screenshots интерфейса
- ссылку на deployed application
- ссылку на API documentation

### 34.3.15. Итоговые требования к проекту

Проект считается завершённым только после выполнения полного цикла:

```text
Code
  ↓
Git
  ↓
Pull Request
  ↓
Lint
  ↓
Type-check
  ↓
Unit Tests
  ↓
Integration Tests
  ↓
Build
  ↓
Docker Images
  ↓
Container Registry
  ↓
Staging
  ↓
Smoke Tests
  ↓
Production
  ↓
Monitoring / Logs
```

Главная цель проекта — не просто получить работающее приложение, а самостоятельно пройти полный жизненный цикл production-like Java fullstack-системы:

**разработка → тестирование → контейнеризация → CI → staging → deployment → production**

#### Дополнительная литература

- Nigel Poulton — «Docker Deep Dive» → Практическое системное руководство по Docker: images, containers, Dockerfile, networking, volumes, registries, security и container lifecycle. Использовать как основную дополнительную книгу по контейнеризации.
- Kelsey Hightower, Brendan Burns, Joe Beda — «Kubernetes: Up & Running» → Книга по Kubernetes и production orchestration. Для самого проекта читать выборочно; основная ценность появится после освоения Docker, Docker Compose и базового CI/CD
- Matthew Skelton, Manuel Pais — «Team Topologies» → Полезна для понимания организации delivery-процессов, взаимодействия development и operations и принципов эффективного software delivery. Не является книгой по GitHub Actions или Docker и используется именно как дополнительный источник по DevOps-культуре
- Jez Humble, David Farley — «Continuous Delivery» → Фундаментальная книга по Continuous Integration, Continuous Delivery, deployment pipelines, automated testing, environments и снижению рисков релизов. Особенно полезна для понимания того, почему CI/CD pipeline строится именно как последовательность автоматизированных проверок и deployment stages
- Gene Kim, Kevin Behr, George Spafford — «The Phoenix Project» → Художественно-практическое введение в DevOps и continuous delivery. Использовать для понимания процессов и проблем delivery, а не как техническое руководство

## Карьера и поиск работы

### 35. Английский язык

**Цель:** довести английский до уровня, достаточного для работы разработчиком: понимать техническую документацию и англоязычный контент, общаться с коллегами, читать профессиональную литературу и самостоятельно искать информацию на английском языке.

#### Быстрая справка

| #    | Ресурс                                                                                                                                                       | Ссылка                                                             |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| 35.1 | Диджитализируй!. Англо-русский словарик часто встречающихся ИТ-слов                                      | [GitHub](https://github.com/alexey-goloburdin/eng-ru-dictionary)            |
| 35.2 | Языковая школа Диалог. Технический английский для IT. Английские слова для программистов | [YouTube](https://www.youtube.com/watch?v=lKEnfEd62jw)                      |
| 35.3 | Clever English. 100+ Ключевых Слов для Программистов                                                                                   | [YouTube](https://www.youtube.com/watch?v=TqSyAjKHANU)                      |
| 35.4 | The University of Oxford. Oxford Learner's Dictionaries                                                                                                            | [Oxford Learners Dictionaries](https://www.oxfordlearnersdictionaries.com/) |

#### План изучения

| #    | Ресурс                                                                                | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 35.5 | Мэйхэм. Английский от A1 до C1. Четкий план изучения! | [YouTube](https://www.youtube.com/watch?v=2To6EqvVPYo) |

#### Уровень A1–A2 (Начальный)

##### Учим 1500 наиболее распространенных слов

| #    | Ресурс                                                                                                                             | Ссылка                                            |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------- |
| 35.6 | Quizlet — изучение и повторение 1500 наиболее распространённых английских слов | [Quizlet](https://quizlet.com/ru/863328515)                |
| 35.7 | TonePerfect — практика произношения слов из Quizlet                                                           | [TonePerfect](https://toneperfect.app/ru/english/practice) |
| 35.8 | Reverso Context — извлечение контекста из выученных слов                                              | [Reverso Context](https://context.reverso.net)             |

##### Осваиваем основы языка с [Александром Бебрисом](https://www.youtube.com/@englishplaylists)

| #     | Ресурс                                                                              | Ссылка                                                                                |
| ----- | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 35.9  | English Galaxy — приложение для изучения английского     | [Google Play](https://play.google.com/store/apps/details?id=ru.englishgalaxy&pli=1)            |
| 35.10 | Александр Бебрис. Английский язык за 20 уроков (А0) | [YouTube](https://www.youtube.com/watch?v=_dVF0SXgs0w&list=PLD6SPjEPomauv1JKSm7TNQPUkK9vpI-fN) |
| 35.11 | Александр Бебрис. Английский язык за 20 уроков (А1) | [YouTube](https://www.youtube.com/watch?v=etnC0Ay2iRs&list=PLD6SPjEPomavB5Xmu_3J8E5uTOBuJMPl2) |
| 35.12 | Александр Бебрис. Английский язык за 20 уроков (А2) | [YouTube](https://www.youtube.com/watch?v=J0DA8JB2vhQ&list=PLD6SPjEPomavd9p66Hme87w11KqPxthKV) |

##### Открываем Essential Grammar in Use с [Vlad_and_English](https://www.youtube.com/@vlad_and_english)

| #     | Ресурс                                                                                                                                | Ссылка                                                                     |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| 35.13 | Raymond Murphy. Essential Grammar in Use. Русская версия                                                                       | [Telegram](https://t.me/english_materia/2744)                                       |
| 35.14 | Vlad_and_English. Бесплатный курс английского с нуля до B1 за 25 часов по Essential Grammar in Use | [YouTube](https://www.youtube.com/playlist?list=PLF2u7WJC9Bw84ApFN0jBdlc65xsAle2G0) |

##### Практикуемся составлять предложения из выученных слов

- Учим новую порцию слов в [Quizlet](https://quizlet.com/ru/863328515) (например, 10–15 слов)
- Составляем с ними 5–7 предложений, используя метод «снежного кома»:
  - **Метод [«Снежного кома»](https://practicum.yandex.ru/blog-english/how-to-memorize-a-text-quickly/):** строим простое предложение и постепенно добавляем к нему новые слова и детали
- Проверяем предложения на корректность с помощью [Reverso Spell Checker](https://www.reverso.net/spell-checker/english-spelling-grammar/)
- Устно проговариваем составленные предложения, чтобы закрепить их в речи. В помощь — [TonePerfect](https://toneperfect.app/ru/english/practice).

##### Смотрим Extra English и фильм «Один дома» c [Мэйхэмом](https://www.youtube.com/@mayhemENG)

| #     | Ресурс                                                                            | Ссылка                                                 |
| ----- | --------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| 35.15 | Мэйхэм. Смотрим Extra English с Мэйхэмом                    | [YouTube](https://www.youtube.com/watch?v=s9Ik82fYb3Y)          |
| 35.16 | Мэйхэм. Смотрим фильм «Один дома» с Мэйхэмом | [YouTube](https://www.youtube.com/watch?v=s9Ik82fYb3Y&t=17517s) |

#### Уровень B1-B2 (Средний)

##### Расширяем словарный запас: продолжаем учить английские слова

| #     | Ресурс                                                                     | Ссылка                                        |
| ----- | -------------------------------------------------------------------------------- | --------------------------------------------------- |
| 35.17 | Мэйхэм. Выучим 3000 слов в английском языке      | [YouTube](https://www.youtube.com/watch?v=NefYfsMNOAo) |
| 35.18 | Александр Бебрис. Выучим 5000 английских слов | [YouTube](https://www.youtube.com/watch?v=hZIMC-N-nro) |

##### Продолжаем изучать правила языка с [Александром Бебрисом](https://www.youtube.com/@englishplaylists)

| #     | Ресурс                                                                             | Ссылка                                                                                |
| ----- | ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 35.19 | Александр Бебрис. Английский язык за 20 уроков (B1) | [YouTube](https://www.youtube.com/watch?v=muJBtdiGotk&list=PLD6SPjEPomavdV8S5p7dPaz8o45a-B-hg) |
| 35.20 | Александр Бебрис. Английский язык за 20 уроков (B2) | [YouTube](https://www.youtube.com/watch?v=ZVpZhzC5Ux0&list=PLKVXijgJyL3s)                      |

##### Открываем English Grammar in Use с [Vlad_and_English](https://www.youtube.com/@vlad_and_english)

| #     | Ресурс                                                                                                                                | Ссылка                                                           |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| 35.21 | Raymond Murphy. English Grammar In Use - 5th Edition                                                                                        | [Telegram](https://t.me/AmEnglish/8747)                                   |
| 35.22 | Vlad_and_English. Английский с A2 до B2 за 51 час по English Grammar in Use. Полный курс грамматики | [YouTube](https://www.youtube.com/watch?v=KHAQFIjPg5E&list=PLXnUNFvWzehA) |

##### Смотрим фильм «Пингвины мистера Поппера» с [Мэйхэмом](https://www.youtube.com/@mayhemENG)

| #     | Ресурс                                                                                                           | Ссылка                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| 35.23 | Мэйхэм. Смотрим фильм «Пингвины мистера Поппера» с Мэйхэмом | [YouTube](https://www.youtube.com/watch?v=s9Ik82fYb3Y&t=23385s) |

##### Смотрим и самостоятельно разбираем англоязычные фильмы из [WatchEnglish.tv](https://watchenglish.tv/)

- Смотрим фильмы дважды: cначала смотрим с английскими субтитрами для разбора фраз (новые слова записываем), а затем без них
- Охватить как минимум 5 фильмов из списка

| #     | Ресурс                                                                                                           | Ссылка                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| 35.24 | Самостоятельно изучаем лексику из фильма «Приключения Паддингтона» | [WatchEnglish.tv](https://watchenglish.tv/movies/paddington)          |
| 35.25 | Самостоятельно изучаем лексику из фильма «День сурка» | [WatchEnglish.tv](https://watchenglish.tv/movies/groundhog-day)          |
| 35.26 | Самостоятельно изучаем лексику из фильма «Назад в будущее» | [WatchEnglish.tv](https://watchenglish.tv/movies/back-to-the-future) |
| 35.27 | Самостоятельно изучаем лексику из фильма «Стажёр» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-intern)          |
| 35.28 | Самостоятельно изучаем лексику из фильма «Форрест Гамп» | [WatchEnglish.tv](https://watchenglish.tv/movies/forrest-gump)          |
| 35.29 | Самостоятельно изучаем лексику из фильма «Шоу Трумана» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-truman-show)          |
| 35.30 | Самостоятельно изучаем лексику из фильма «Зелёная книга» | [WatchEnglish.tv](https://watchenglish.tv/movies/green-book)          |
| 35.31 | Самостоятельно изучаем лексику из фильма «Гарри Поттер и философский камень» | [WatchEnglish.tv](https://watchenglish.tv/movies/harry-potter-and-the-philosophers-stone)          |
| 35.32 | Самостоятельно изучаем лексику из фильма «Король говорит!» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-kings-speech)          |
| 35.33 | Самостоятельно изучаем лексику из фильма «Дьявол носит Prada» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-devil-wears-prada)          |

##### Погружаемся в англоязычную среду
- По возможности ищем собеседника для англоязычного разговора: репетитор, друг по переписке и т.п.
- Смотрим англоязычные [YouTube-ролики](https://www.youtube.com/)

#### Уровень C1-C2 (Продвинутый)

##### Расширяем словарный запас: продолжаем учить английские слова

| #     | Ресурс                                                                                                           | Ссылка                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| 35.34 | Hopkins English. 900 слов на уровне Advanced | [YouTube](https://www.youtube.com/playlist?list=PL74qVjPol50qJBnMCJgmNAimttcKNpUvZ)          |
| 35.35 | Now English 24. 4 Hours of C1 Advanced and C2 Proficiency English Vocabulary | [YouTube](https://www.youtube.com/watch?v=O22-e9TNFRs)          |

##### Продолжаем изучать правила языка с [Александром Бебрисом](https://www.youtube.com/@englishplaylists)

| #     | Ресурс                                                                                                           | Ссылка                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| 35.36 | Александр Бебрис. Практический курс по приложению English Galaxy (C1) | [YouTube](https://www.youtube.com/watch?v=EqnKey6umHU&list=PLD6SPjEPomas3z_YSZTDDiiqUlaGiVKXJ)          |

##### Открываем Advanced Grammar in Use с [Еленой Вогнистой](https://www.youtube.com/@ok-english)

| #     | Ресурс                                                                                                           | Ссылка                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| 35.37 |  Martin Hewings. Advanced Grammar in Use - 3th Edition | [ispsn.org](https://www.ispsn.org/sites/default/files/documentos-virtuais/pdf/3-advanced_grammar_in_use_3rd_edition_martin_hewings.pdf)          |
| 35.38 |  Елена Вогнистая. Advanced English Grammar (C1-C2) | [YouTube](https://www.youtube.com/playlist?list=PLYB0SmefqEskabgi9CfLoYtXTA3U8VNKS)          |

##### Погружаемся в англоязычную среду
- Привыкаем гуглить фразы на английском
- Продолжаем смотреть англоязычные [YouTube-ролики](https://www.youtube.com/)

##### Смотрим англоязычные фильмы

- Привыкаем смотреть фильмы только на английском

| #     | Ресурс                                                                                                           | Ссылка                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| 35.39 | Смотрим фильм «Побег из Шоушенка» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-shawshank-redemption)        |
| 35.40 | Смотрим фильм «Поймай меня, если сможешь» | [WatchEnglish.tv](https://watchenglish.tv/movies/catch-me-if-you-can)        |
| 35.41 | Смотрим фильм «Зелёная миля» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-green-mile)          |
| 35.42 | Смотрим фильм «Тёмный рыцарь» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-dark-knight)        |
| 35.43 | Смотрим фильм «Пираты Карибского моря: Проклятие Чёрной жемчужины» | [WatchEnglish.tv](https://watchenglish.tv/movies/pirates-of-the-caribbean-the-curse-of-the-black-pearl)        |
| 35.44 | Смотрим фильм «Властелин колец: Братство кольца» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-lord-of-the-rings-the-fellowship-of-the-ring)          |
| 35.45 | Смотрим фильм «Властелин колец: Две крепости» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-lord-of-the-rings-the-two-towers)          |
| 35.46 | Смотрим фильм «Властелин колец: Возвращение короля» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-lord-of-the-rings-the-return-of-the-king)          |
| 35.47 | Смотрим фильм «Социальная сеть» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-social-network)          |
| 35.48 | Смотрим фильм «Одержимость» | [WatchEnglish.tv](https://watchenglish.tv/movies/whiplash)          |
| 35.49 | Смотрим фильм «Оппенгеймер» | [WatchEnglish.tv](https://watchenglish.tv/movies/oppenheimer)          |
| 35.50 | Смотрим фильм «Отель "Гранд Будапешт"» | [WatchEnglish.tv](https://watchenglish.tv/movies/the-grand-budapest-hotel)          |
| 35.51 | Смотрим фильм «Нефть» | [WatchEnglish.tv](https://watchenglish.tv/movies/there-will-be-blood)          |
| 35.52 | Смотрим фильм «Старикам тут не место» | [WatchEnglish.tv](https://watchenglish.tv/movies/no-country-for-old-men)          |
| 35.53 | Смотрим фильм «Большой куш» | [WatchEnglish.tv](https://watchenglish.tv/movies/snatch)          |

#### Дополнительная литература

- Stuart Redman — «English Vocabulary in Use: Pre-Intermediate and Intermediate» → Систематическое расширение словарного запаса для уровней A2–B1. Книга охватывает повседневную лексику, фразовые глаголы и устойчивые выражения, которые необходимы для уверенного общения на бытовые темы. Подходит для самостоятельного изучения и закрепления базовой лексики перед переходом на более сложные уровни.
- Liz and John Soars — «Headway» (серия) → Комплексный курс английского языка с четко выстроенной методикой, охватывающий уровни от Beginner до Advanced. Серия развивает все четыре навыка (говорение, аудирование, чтение, письмо) сбалансированно, с акцентом на практическое использование языка в реальных ситуациях. Подходит для системного изучения языка с любого уровня.
- Ann Baker — «Ship or Sheep? An Intermediate Pronunciation Course» → Классическое пособие для отработки произношения на уровне Intermediate. Основной фокус — различение похожих звуков (минимальные пары), что помогает сделать речь более понятной для носителей языка. Подходит для тех, кто уже владеет основами, но хочет улучшить произношение.
- Jean Yates — «Practice Makes Perfect: English Conversation» → Практическое пособие для развития разговорных навыков. Содержит диалоги на повседневные темы, упражнения на построение предложений и аудиозаписи для отработки произношения. Подходит для уровней Intermediate и выше, помогает быстрее заговорить и поддерживать беседу.
- Е. Ю. Бутенко — «Английский язык для ИТ-направлений (B1–B2). IT-English» → Учебное пособие, специально разработанное для специалистов в области информационных технологий. Охватывает профессиональную лексику, связанную с разработкой ПО, сетевыми технологиями, базами данных и IT-коммуникацией. Подходит для уровней B1–B2 и помогает быстрее адаптироваться к работе с технической документацией и общению с коллегами на английском.

### 36. Методологии разработки: Agile, Scrum, Kanban

**Цель**: сформировать целостное представление о гибких подходах к командной разработке ПО — Agile, Scrum и Kanban: понять ценности и принципы Agile, разобрать роли, события и артефакты Scrum, освоить принципы работы Kanban-доски и WIP-лимитов, а также научиться различать Scrum и Kanban.

**Agile (гибкая разработка)** — это набор ценностей и принципов (не конкретная методология) о том, как эффективнее разрабатывать продукт в условиях изменений и неопределённости.

Идеи и принципы Agile применяются в различных фреймворках, методах, практиках и инструментах разработки. 

```text
AGILE
│
│ Ценности и принципы
│ Что это: философия разработки, определяющая ценности,
│ принципы и приоритеты работы команды
│
├── ФРЕЙМВОРКИ
│   │ Что это: структуры организации работы команды,
│   │ задающие роли, события, правила и артефакты
│   │
│   ├── Scrum
│   ├── XP
│   └── Crystal
│
├── МЕТОДЫ / ПОДХОДЫ (Agile-совместимые)
│   │ Что это: способы организации и управления
│   │ рабочим процессом и потоком задач
│   │ Могут использоваться и вне Agile
│   │
│   ├── Kanban
│   └── Scrumban
│
└── ПРАКТИКИ
    │ Что это: конкретные приёмы и техники,
    │ которые команда использует в работе
    │
    ├── Planning Poker
    ├── Story Points
    ├── Definition of Ready
    └── Burndown / Burnup Chart

РЯДОМ (не внутри Agile):
│
├── ИНСТРУМЕНТЫ
│   │ Что это: средства технической поддержки,
│   │ не являются частью Agile
│   └── Jira, Trello, Miro
│
├── МАСШТАБИРОВАНИЕ AGILE / SCRUM
│   │ Что это: фреймворки для нескольких команд
│   └── SAFe, LeSS, Nexus, Scrum@Scale
│
├── ПЕРЕСЕКАЮЩИЕСЯ ПОДХОДЫ
│   └── Lean
│
└── ТРАДИЦИОННЫЕ МОДЕЛИ
    └── Waterfall
```

В современной IT-разработке среди наиболее распространённых подходов, связанных с Agile, можно выделить **фреймворк Scrum и метод Kanban**. С ними можно подробно ознакомиться в видеоматериалах, представленных ниже.

| #    | Ресурс                                                                                                 | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 36.1 | Олег Малышев. Методологии и модели разработки ПО. Scrum, Kanban, Agile, Водопадная модель, V-model                             | [YouTube](https://www.youtube.com/watch?v=QAj8X7FwQF8) |
| 36.2 | DocSourcing. Agile, Scrum, Kanban: гибкие методологии разработки продукта                             | [YouTube](https://www.youtube.com/watch?v=q6ewfO8B0CQ) |
| 36.3 | Андрей Кулагин. Рабочие процессы в IT: как все работает на самом деле?                          | [YouTube](https://www.youtube.com/watch?v=Jx-WAc-6iPY) |
| 36.4 | Одноглазый Змей. Всё о процессах в IT. Agile, Scrum, Kanban и прочая дичь                           | [YouTube](https://www.youtube.com/watch?v=IuqoiRAPn0A) |
| 36.5 | Социократия в России. Кратко: что такое Scrum за 5 минут                            | [YouTube](https://www.youtube.com/watch?v=bVWBiL8yv88) |
| 36.6 | Объясняшки. Что такое Канбан метод? И как пользоваться канбан доской                            | [YouTube](https://www.youtube.com/watch?v=qE9DDBbjqiw) |

#### Что такое Scrum?

**Scrum** — это фреймворк для разработки, поставки и поддержки сложных продуктов, основанный на итеративной и инкрементальной работе команды в рамках коротких циклов — спринтов (Sprint).

В Scrum-команде выделяют три основные области ответственности:
- **Владелец продукта (Product Owner)**: отвечает за максимизацию ценности продукта и эффективное управление его **Product Backlog** — упорядоченным списком задач, идей и требований, которые необходимо реализовать для создания и развития продукта. Он отвечает за упорядочивание элементов бэклога, а также формирует и поддерживает цели продукта.
- **Scrum-мастер (Scrum Master)**: отвечает за эффективное применение Scrum в соответствии с его официальным руководством. Он помогает команде и организации понимать принципы Scrum, устраняет препятствия и способствует повышению эффективности работы скрам-команды.
- **Разработчики (Developers)**: специалисты, создающие готовый **Increment** — рабочая часть продукта, формируемая за один спринт. Они самостоятельно планируют задачи на каждый спринт, гибко адаптируют план в процессе и отвечают за создание **Increment**, соответствующего **Definition of Done** — установленным критериям готовности продукта.

```text
Scrum Team
├── Product Owner
├── Scrum Master
└── Developers
    ├── Backend Developer
    ├── Frontend Developer
    ├── QA / Test Engineer
    ├── Business Analyst
    ├── System Analyst
    ├── UX/UI Designer
    └── другие специалисты
```

Scrum не выделяет аналитика, тестировщика, дизайнера и других специалистов в отдельные области ответственности. Если такие специалисты входят в скрам-команду и участвуют в создании продукта, они относятся к разработчикам в терминологии Scrum.

Scrum-команда обязуется достигать своих целей и поддерживать друг друга. В официальном руководстве Scrum формально выделяют три основные обязательства внутри команды:

- **Цель продукта (Product Goal)**: долгосрочная цель, описывающая будущее состояние продукта. Она задает вектор для создания и развития бэклога продукта (Product Backlog).

- **Цель спринта (Sprint Goal)**: главная цель, которую команда хочет достичь за время одного спринта (обычно за 1–4 недели). 

- **Определение готовности (Definition of Done, DoD)**: чек-лист качества, по которому проверяется любая выполненная задача. Если задача не соответствует DoD, её нельзя считать завершённой и показывать пользователям.

В течение спринта создаётся один или несколько **Increment** — конкретных, пригодных к использованию результатов, каждый из которых должен соответствовать **Definition of Done**.

Созданный **Increment** показывается **стейкхолдерам (Stakeholders)** — лицам, заинтересованным в его развитии. Они изучают результат, делятся обратной связью и обсуждают, как улучшить продукт.

После получения **обратной связи (Feedback)** владелец продукта адаптирует и корректирует бэклог продукта: меняет приоритеты задач, удаляет неактуальное или добавляет новые элементы под открывшиеся возможности.

По мере получения новой информации **Product Backlog** уточняется и изменяется. На планировании следующего Sprint команда выбирает из него элементы для дальнейшей работы.

#### Шпаргалка по Scrum: подробный цикл работы

```text
                       ЦЕЛЬ ПРОДУКТА (Product Goal)
                      Чего хотим достичь в продукте?
                                  │
                                  ▼
                     БЭКЛОГ ПРОДУКТА (Product Backlog)
                     Что нужно сделать для создания
                           и развития продукта?
                                  │
                                  ▼
                           УТОЧНЕНИЕ БЭКЛОГА
                      (Product Backlog Refinement)
                 Уточняем требования, разбиваем элементы,
                 выявляем зависимости и при необходимости
                         оцениваем объём работы
                                  │
                         ┌────────┴────────┐
                         │                 │
                         ▼                 ▼
                  STORY POINTS        PLANNING POKER
                  Относительная       Командная техника
                  оценка размера      оценки Story Points
                  работы. Обычно           │
                  с учётом:                │
                  • объёма работы          │
                  • сложности              │
                  • неопределённости       │
                  • рисков                 │
                         │                 │
                         │                 ▼
                         │            Каждый участник
                         │            самостоятельно
                         │            выбирает оценку
                         │                 │
                         │                 ▼
                         │            Сравниваем оценки
                         │            и обсуждаем различия
                         │                 │
                         │                 ▼
                         │            Повторно оцениваем
                         │            после обсуждения
                         │                 │
                         └────────┬────────┘
                                  ▼
                ПЛАНИРОВАНИЕ СПРИНТА (Sprint Planning)
                    Определяем цель и план работы
                        на предстоящий Sprint
                                  │
                       ┌──────────┴──────────┐
                       │                     │
                       ▼                     ▼
                ЦЕЛЬ СПРИНТА           БЭКЛОГ СПРИНТА
                (Sprint Goal)          (Sprint Backlog)
                Чего хотим достичь     Цель спринта, выбранные
                за Sprint?             элементы бэклога продукта
                       │               и план их реализации    
                       │                     │
                       └──────────┬──────────┘
                                  ▼
                            СПРИНТ (Sprint)
                          Создаём Increment и
                         адаптируем план работы
                                  │
                  ┌───────────────┼───────────────┐
                  │               │               │
                  ▼               ▼               ▼
          DAILY SCRUM        РАЗРАБОТКА       АДАПТАЦИЯ
          (Daily Scrum)      (Development)    (Adaptation)
          Проверяем          Реализуем        Адаптируем
          прогресс к         задачи,          план и
          Sprint Goal        тестируем        работу
                             и интегрируем
                  │               │               │
                  └───────────────┼───────────────┘
                                  ▼
                     ИНКРЕМЕНТ ПРОДУКТА (Increment)
                 Конкретный, пригодный к использованию   
                    результат, который соответствует 
                          Definition of Done
                                  │
                                  ▼
                      ОБЗОР СПРИНТА (Sprint Review)
                       Проверяем результат Sprint,
                      обсуждаем его со Stakeholders
                       и демонстрируем Increment
                                  │
                       ┌──────────┴──────────┐
                       │                     │
                       ▼                     ▼
                  ДЕМО (Demo)          ОБРАТНАЯ СВЯЗЬ
                  Демонстрация         (Feedback)
                  Increment для        Получаем отзывы
                  Stakeholders         и новую информацию
                       │                     │
                       └──────────┬──────────┘
                                  ▼
                           PRODUCT BACKLOG
                    Адаптируем содержание и порядок
                      элементов с учётом новой
                             информации
                                  │
                                  ▼
                        РЕТРОСПЕКТИВА СПРИНТА
                        (Sprint Retrospective)
                      Анализируем процесс работы:
                     люди, взаимодействие, процесс,
                    инструменты и Definition of Done
                                  │
                                  ▼
                         УЛУЧШЕНИЕ ПРОЦЕССА
                    Определяем улучшения, которые
                    можно применить в дальнейшем
                                  │
                                  ▼
                          СЛЕДУЮЩИЙ SPRINT
                           Повторяем цикл
```

#### Что такое Kanban?

**Kanban** — это метод управления потоком работы, который помогает визуализировать задачи, ограничивать количество одновременно выполняемой работы (WIP, Work in Progress) и непрерывно улучшать процесс разработки.

В отличие от Scrum, Kanban **не требует фиксированных спринтов, ролей или обязательного набора событий**. Работа поступает в систему непрерывным потоком: когда команда освобождает ресурсы, следующая задача берётся в работу.

Основные принципы Kanban:
- **Визуализация работы (Visualize Work)** — все задачи отображаются на Kanban-доске.
- **Ограничение незавершённой работы (WIP Limits)** — ограничивается количество задач, одновременно находящихся в работе.
- **Управление потоком (Manage Flow)** — команда следит за тем, чтобы задачи проходили через процесс равномерно и без длительных задержек.
- **Явные правила процесса (Explicit Policies)** — команда заранее определяет правила перехода задач между этапами.
- **Циклы обратной связи (Feedback Loops)** — команда регулярно анализирует процесс и результаты работы.
- **Непрерывное улучшение (Continuous Improvement)** — процесс постепенно изменяется на основе полученных данных и наблюдений.

#### Kanban-доска

**Канбан-доска** — это визуальный инструмент управления проектами и задачами, который помогает наглядно показывать рабочий процесс и двигать задачи по мере их выполнения.

В доске задача последовательно перемещается между этапами. Простейшая Kanban-доска может выглядеть так:

```text
┌──────────────┬────────────────┬────────────────┬──────────────┐
│    TO DO     │   IN PROGRESS  │     REVIEW     │     DONE     │
│              │                │                │              │
│ TASK-105     │ TASK-101       │ TASK-098       │ TASK-095     │
│ TASK-106     │ TASK-103       │                │ TASK-096     │
│ TASK-107     │                │                │              │
│              │                │                │              │
└──────────────┴────────────────┴────────────────┴──────────────┘
```

Конкретные колонки определяются самой командой: Kanban не требует какого-либо конкретного набора колонок. 

К примеру, вместо представленного выше примера мы могли бы создать  Kanban-доску с последовательностью Backlog → Analysis → Development → Code Review → Testing → Done.

```text
┌────────────┬────────────┬───────────────┬──────────────┬────────────┬──────────┐
│  BACKLOG   │  ANALYSIS  │  DEVELOPMENT  │ CODE REVIEW  │  TESTING   │   DONE   │
├────────────┼────────────┼───────────────┼──────────────┼────────────┼──────────┤
│ TASK-108   │ TASK-105   │ TASK-101      │ TASK-099     │ TASK-096   │ TASK-092 │
│ TASK-109   │ TASK-106   │ TASK-103      │ TASK-100     │            │ TASK-093 │
│ BUG-024    │            │ TASK-104      │              │            │ TASK-094 │
│ FEATURE-12 │            │               │              │            │          │
│            │            │               │              │            │          │
│            │            │               │              │            │          │
└────────────┴────────────┴───────────────┴──────────────┴────────────┴──────────┘
                   ↑               ↑              ↑
                 WIP: 2         WIP: 3         WIP: 2

WIP Limits: Analysis = 2, Development = 3, Code Review = 2
```

**WIP (Work in Progress)** — незавершённая работа, которая уже была взята в процесс, но ещё не закончена.

**WIP Limit** — максимальное количество задач, которое одновременно может находиться на определённом этапе.

В текущем примере все этапы с WIP-лимитами заполнены до предела: в Analysis — 2 из 2, в Development — 3 из 3, в Code Review — 2 из 2. Поэтому новые задачи из Backlog не могут быть взяты в работу, пока хотя бы одна задача не продвинется дальше по потоку. 
 
Команда вынуждена не начинать новую работу, а завершать уже начатую, чтобы освободить место в перегруженных колонках и продвинуть задачи по потоку. В этом и состоит одна из ключевых идей Kanban: **не брать в работу всё больше новых задач, а стремиться доводить уже начатую работу до конца.**

#### Отличия Scrum от Kanban

| Критерий | Scrum | Kanban |
| --- | --- | --- |
| **Тип** | Фреймворк | Метод управления потоком работы |
| **Философия** | Итеративная и инкрементальная разработка короткими циклами | Непрерывный поток задач без фиксированных итераций |
| **Ритм работы** | Фиксированные спринты (обычно 1–4 недели) | Непрерывный поток: задачи берутся по мере освобождения ресурсов |
| **Роли** | Обязательные: Product Owner, Scrum Master, Developers | Обязательных ролей нет; роли определяются командой |
| **События** | Обязательные: Sprint, Sprint Planning, Daily Scrum, Sprint Review, Sprint Retrospective | Обязательных событий нет; команда сама выбирает регулярные встречи |
| **Артефакты** | Product Backlog, Sprint Backlog, Increment | Kanban-доска; формальных артефактов нет |
| **Оценка работы** | Story Points, Planning Poker (популярные практики) | Оценка не обязательна; важнее размер задачи и время прохождения |
| **Ограничение работы** | Через Sprint Backlog — объём работы на спринт | Через WIP-лимиты — ограничение задач на каждом этапе |
| **Изменения в процессе** | Изменения внутри спринта не приветствуются; план фиксируется на Sprint | Изменения возможны в любой момент; процесс эволюционирует постепенно |
| **Ключевая метрика** | Velocity, Burndown / Burnup Chart | Cycle Time, Lead Time, Throughput, Cumulative Flow Diagram |
| **Цель спринта / итерации** | Обязательна: Sprint Goal | Не используется |
| **Definition of Done** | Обязательна для Increment | Может использоваться, но не обязательна |
| **Кому подходит** | Командам, работающим над продуктом с регулярными релизами | Командам с потоком разнородных задач: поддержка, эксплуатация, багфикс |
| **Стиль изменений** | Революционный: внедряется целиком по Scrum Guide | Эволюционный: изменения вводятся постепенно |
| **Совместимость с Agile** | Фреймворк внутри Agile | Agile-совместимый метод, может применяться и вне Agile |
| **Пример доски** | Sprint Backlog: To Do → In Progress → Done | Kanban-доска: Backlog → Analysis → Development → Review → Testing → Done |

#### Словарь терминов: Scrum и Kanban

| #    | Ресурс                                                                                                 | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 36.7 | Scrumtrek. Словарь терминов Scrum | [Scrumtrek.ru](https://scrumtrek.ru/blog/agile-scrum/scrum-glossary/) |
| 36.8 | Scrumtrek. Словарь терминов Kanban | [Scrumtrek.ru](https://scrumtrek.ru/blog/kanban/kanban-glossary/) |

#### Дополнительная литература

- Jeff Sutherland — «Scrum: The Art of Doing Twice the Work in Half the Time» → Основополагающая книга по Scrum от одного из его создателей. Подробно описывает роли, события, артефакты, спринты, планирование и ретроспективы. Использовать как основной источник для глубокого понимания Scrum и его практического применения.
- David J. Anderson — «Kanban: Successful Evolutionary Change for Your Technology Business» → Практическое руководство по внедрению Kanban: визуализация работы, WIP-лимиты, управление потоком, явные правила и эволюционные изменения. Использовать для изучения Kanban и сравнения его со Scrum.
- Henrik Kniberg — «Scrum and XP from the Trenches» → Краткое и практичное описание Scrum и Extreme Programming, их сочетания и ключевых практик. Включает примеры спринтов, бэклогов и оценок. Использовать как дополнительный источник для быстрого погружения в гибкие методологии.
- Mike Cohn — «Agile Estimating and Planning» → Книга о гибком планировании, оценке в story points, planning poker и итеративном планировании. Использовать для углубления в практики Agile-планирования и организации работы команды.
- Ken Schwaber, Jeff Sutherland — «The Scrum Guide» → Официальный и обязательный к прочтению документ, определяющий Scrum. Регулярно обновляется, содержит актуальные правила, роли и терминологию. Использовать как основной источник правил и стандартов Scrum.

### 37. Резюме, портфолио и собеседования

**Цель:** подготовиться к поиску работы разработчиком: составить резюме и портфолио, подготовиться к HR, техническим, алгоритмическим и System Design-собеседованиям и научиться уверенно презентовать свой опыт и проекты.

#### Полноценные гайды

| #    | Ресурс                                                                                                                                                                         | Ссылка                                        |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| 37.1 | Одноглазый Змей. Кому HR пишут первыми?                                                                                                                | [YouTube](https://www.youtube.com/watch?v=VwoD3FsJoWo) |
| 37.2 | Владимир Балун. Как точно пройти собеседование программисту. Собеседование программиста от А до Я | [YouTube](https://www.youtube.com/watch?v=wfeyDt20Zpw) |
| 37.3 | Александр Ильин. Как пройти собеседование на программиста. Ультимативный гайд                                     | [YouTube](https://www.youtube.com/watch?v=tzSdiYZ52kI) |

#### Как пройти ATS-фильтры?

| #    | Ресурс                                                                                                                                 | Ссылка                                                     |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| 37.4 | sergbe. Как улучшить резюме ИТ-специалиста на HH.RU, чтобы пройти фильтры ATS-систем | [Хабр](https://habr.com/ru/companies/ssp-soft/articles/897146/) |
| 37.5 | lena05k. Как обойти фильтры на hh.ru и сделать ваше резюме магнитом для рекрутеров  | [Хабр](https://habr.com/ru/articles/841744/)                    |
| 37.6 | nossao. Как сделать резюме, которое дойдёт до работодателя. Фильтры ATS в 2025 году   | [Хабр](https://habr.com/ru/articles/868344/)                    |
| 37.7 | katyafindmework. Страшные ATS-фильтры и как их пройти: мифы и реальность                           | [Хабр](https://habr.com/ru/articles/945766/)                    |

#### Как сделать резюме привлекательным для HR?

| #     | Ресурс                                                                          | Ссылка                                        |
| ----- | ------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 37.8  | theSeniorDev. Why your developer resume is NOT getting interviews (and how to fix it) | [YouTube](https://www.youtube.com/watch?v=S-0DD9uhLOE) |
| 37.9  | IGotAnOffer: Engineering. Engineering resume review (with top ex-Google recruiter)    | [YouTube](https://www.youtube.com/watch?v=-deIW2au-9Y) |
| 37.10 | Headless Headhunter. Why Software Engineer Gets ZERO Interviews                       | [YouTube](https://www.youtube.com/watch?v=YMDuVH1TtPU) |
| 37.11 | Headless Headhunter. How to Get a Software Engineer Job                               | [YouTube](https://www.youtube.com/watch?v=eC2ucWComX4) |

#### Как составить резюме?

| #     | Ресурс                                                                                                                                                     | Ссылка                                                            |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| 37.12 | Егор Малькевич. 80% специалистов не пройдут отбор. Как составить резюме и продать себя      | [YouTube](https://www.youtube.com/watch?v=5wz7ifeDaYY)                     |
| 37.13 | Владилен Минин.  Полный гайд на Резюме в IT. Как Правильно составить резюме программисту? | [YouTube](https://www.youtube.com/watch?v=mU-MghntMxg)                     |
| 37.14 | dmytrostriletskyi. Идеальное резюме для разработчика                                                                               | [Хабр](https://habr.com/ru/articles/542372/)                           |
| 37.15 | schnitzer. Идеальное резюме разработчика                                                                                              | [Хабр](https://habr.com/ru/companies/hh/articles/502802/)              |
| 37.16 | Morlena106. Идеальное резюме, разговор с IT-рекрутером                                                                         | [Хабр](https://habr.com/ru/articles/804687/)                           |
| 37.17 | igor-sheludko. Идеальное резюме, которому будут рады рекрутер и работодатель                                | [Хабр](https://habr.com/ru/articles/445168/)                           |
| 37.18 | Headless Headhunter. Resume Guide                                                                                                                                | [Headless Headhunter](https://www.headlessheadhunter.org/how-to-get-a-job) |

#### Как составить сопроводительное письмо?

| #     | Ресурс                                                                                                                                                                                           | Ссылка                                                                                 |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- |
| 37.19 | MyResume. Сопроводительное письмо к резюме: как написать, чтобы получить работу                                                             | [YouTube](https://www.youtube.com/watch?v=1UnYNGgqLzM)                                          |
| 37.20 | Никита Кабардин. Как составить Cover Letter. Сопроводительное письмо программиста                                                          | [YouTube](https://www.youtube.com/watch?v=JT0EmXBZBTU)                                          |
| 37.21 | Антон Ларичев. Сопроводительное письмо: шаблоны для разработчиков                                                                             | [PurpleSchool](https://purpleschool.ru/blog/soprovoditelnoe-pismo-shablony-dlya-razrabotchikov) |
| 37.22 | Александра Гонтарева. Как написать сопроводительное письмо, которое прочитают: шаблоны для ИТ-специалистов | [Cloud.ru](https://cloud.ru/blog/kak-napisat-soprovoditelnoye-pismo)                            |
| 37.23 | Denis_Potrubeiko. Как написать хорошее сопроводительное письмо                                                                                                 | [Хабр](https://habr.com/ru/posts/787220/)                                                   |
| 37.24 | konstantin_matyunin. Сопроводительное письмо: пережиток времени или шанс на оффер?                                                                 | [Хабр](https://habr.com/ru/articles/934688/)                                                |

#### Как определить свой технологический стек для резюме?

**Стек (технологический стек, tech stack)**  — то набор технологий и инструментов, которые применяются при разработке проектов, сайтов, приложений и информационных систем.

Короткая схема определения технологического стека: 
1. Заходим на HH.ru / LinkedIn
2. Ищем 20–30 релевантных вакансий по интересующей специальности. При желании можно проанализировать больше вакансий для получения более объективной картины
3. Выписываем все найденные технологии в единый список.
4. Подсчитываем частоту упоминания технологий в вакансиях и определяем, какие из них встречаются наиболее часто.
5. Выделяем наиболее востребованные технологии и типовые сочетания технологий, которые чаще всего встречаются в вакансиях.
6. Группируем найденные технологии по категориям, например: язык программирования, фреймворки, базы данных, тестирование, сборка, контейнеризация, CI/CD и т.д. Для группировки можно использовать ИИ.
7. Понимаем назначение каждой технологии: отвечаем на вопрос «Зачем это нужно?» и определяем, какую задачу она решает в проекте.
8. Не вникаем глубоко на этом этапе. Наша задача — получить общее представление о стеке и понимать назначение каждой технологии. Глубокое изучение выполняется позже, в соответствии с приоритетами roadmap.

Источник: [Одноглазый Змей](https://www.youtube.com/watch?v=dycMYvCKN0w&t=250s)

#### Полноценные проекты для резюме

Достаточно выбрать 1–3 проекта и довести до production-like состояния

| #  | Проект                                           | Что реализовать                                                                                                                                                                                                     | Ключевые компетенции                                                                           |
| -- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| 1  | **Task Management / Jira-like System**           | Проекты, задачи, роли, права, комментарии, статусы, приоритеты, поиск, фильтрация, сортировка, пагинация, уведомления              | Spring Boot, Security, RBAC, PostgreSQL, React/Next.js, WebSocket/SSE, OpenAPI, Docker, CI/CD                     |
| 2  | **E-commerce Platform**                          | Каталог, товары, категории, корзина, заказы, оплаты (mock), промокоды, остатки, роли Customer/Admin, история заказов                                   | Spring Boot, JPA, PostgreSQL, транзакции, optimistic locking, Security, Redis, React, Docker            |
| 3  | **Booking / Reservation System**                 | Поиск объектов, доступность, бронирование, отмена, временные слоты, предотвращение double booking, история операций                          | Spring Boot, PostgreSQL, транзакции, locking, concurrency, REST, React, Redis, тестирование |
| 4  | **Food Delivery Platform**                       | Клиенты, рестораны, меню, корзина, заказ, статусы доставки, курьеры, назначение заказов, realtime-обновления                                     | Spring Boot, Security, WebSocket/SSE, PostgreSQL, Redis, Kafka/RabbitMQ, React, Docker                            |
| 5  | **Banking / FinTech System**                     | Счета, переводы, платежи, история операций, лимиты, роли, идемпотентность, audit log, обработка ошибок                                                 | Java, Spring, transactions, isolation levels, locking, Security, PostgreSQL, Kafka, Testcontainers                |
| 6  | **Learning Management System (LMS)**             | Курсы, уроки, тесты, задания, прогресс, роли Student/Teacher/Admin, оценки, уведомления                                                                                        | Spring Boot, Security, RBAC, PostgreSQL, React/Next.js, file storage, WebSocket/SSE, Docker                       |
| 7  | **HR / Recruitment Platform**                    | Вакансии, кандидаты, отклики, этапы hiring pipeline, интервью, комментарии, роли Recruiter/Manager/Candidate                                                                  | Spring Boot, Security, RBAC, PostgreSQL, search/filtering, React, OpenAPI, notifications, CI/CD                   |
| 8  | **Help Desk / IT Service Management**            | Тикеты, категории, SLA, приоритеты, исполнители, статусы, комментарии, вложения, уведомления, история изменений                          | Spring Boot, PostgreSQL, Security, RBAC, WebSocket/SSE, audit log, React, Docker                                  |
| 9  | **Project Management / CRM System**              | Клиенты, компании, сделки, контакты, задачи, pipeline, activity history, роли, dashboard и аналитика                                                                             | Spring Boot, PostgreSQL, JPA, Security, REST/OpenAPI, React, charts, Redis, Docker                                |
| 10 | **Marketplace Platform**                         | Продавцы, товары, каталог, поиск, корзина, заказы, отзывы, рейтинги, остатки, роли Buyer/Seller/Admin                                                             | Spring Boot, PostgreSQL, Redis, Security, Kafka/RabbitMQ, React/Next.js, WebSocket, Docker, CI/CD                 |
| 11 | **Messenger / Chat Platform**                    | Личные и групповые чаты, сообщения, replies, reactions, read receipts, typing indicators, online status, вложения, поиск, история сообщений, offline/reconnect          | Spring Boot, WebSocket, Security, PostgreSQL, Redis, Kafka/RabbitMQ, React/Next.js, object storage, Docker, CI/CD |
| 12 | **Event Management Platform**                    | Создание мероприятий, билеты, места, регистрация, оплаты (mock), QR-коды, check-in, роли Organizer/Participant/Admin, уведомления                               | Spring Boot, Security, PostgreSQL, transactions, Redis, React, WebSocket/SSE, QR, Docker, CI/CD                   |
| 13 | **Logistics / Delivery Management System**       | Заказы на доставку, маршруты, курьеры, статусы, распределение заказов, геолокация, realtime tracking, история доставки                         | Spring Boot, Security, PostgreSQL, Redis, Kafka/RabbitMQ, WebSocket, React/Next.js, Docker, CI/CD                 |
| 14 | **Collaborative Workspace / Notion-like System** | Документы, страницы, папки, совместное редактирование, права доступа, комментарии, version history, поиск, realtime collaboration                       | Spring Boot, Security, PostgreSQL, Redis, WebSocket, React/Next.js, optimistic locking, Docker, CI/CD             |
| 15 | **Job Board / Career Platform**                  | Вакансии, компании, резюме, отклики, поиск, фильтры, рекомендации, статусы кандидатов, роли Recruiter/Employer/Candidate, чат Recruiter ↔ Candidate | Spring Boot, Security, RBAC, PostgreSQL, Redis, React/Next.js, WebSocket, OpenAPI, Docker, CI/CD                  |

#### HR / Behavioral-собеседование

Цель этапа — понять, как вы думаете, работаете в команде и ведёте себя в нестандартных ситуациях.

| #     | Ресурс                                                                                                                                                                                                       | Ссылка                                                     |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------- |
| 37.25 | Виктория Бородина.  Техника грамотных ответов на собеседовании. Как программисту пройти собеседование. Техника STAR | [YouTube](https://www.youtube.com/watch?v=KIlf0zPz6NA)              |
| 37.26 | AlexIsaev.  Софт-скилы: типовые вопросы, которые ждут на интервью, и шаблоны ответов для IT-инженеров                                       | [Хабр](https://habr.com/ru/companies/getmatch/articles/675972/) |
| 37.27 | Heads404Hearts. Как проходить HR-интервью и отвечать на странные вопросы HR?                                                                                         | [Хабр](https://habr.com/ru/articles/716838/)                    |
| 37.28 | eugene_october. Темная лошадка собеседований. Поведенческое (aka Behavioral interview)                                                                                      | [Хабр](https://habr.com/ru/articles/1004274/)                   |

Вопросы, к которым готовимся:

- Расскажите о себе
- Расскажите о последнем проекте
- Какую самую сложную техническую задачу вы решали?
- Расскажите о конфликте в команде
- Расскажите об ошибке или неудаче
- Как вы принимаете технические решения?
- Почему хотите сменить работу?
- Почему хотите работать у нас?
- Какие ваши сильные и слабые стороны?
- Какие у вас карьерные цели?
- Какие вопросы есть к нам?

Под каждую тему из списка выше стоит иметь 2–3 заготовленные истории в формате **STAR (Situation → Task → Action → Result)**.

| Этап  | Что раскрываем                                                                                                  |
| --------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Situation | Контекст: где, когда, в каком проекте, какая была команда                       |
| Task      | Ваша задача или проблема, которую нужно было решить                               |
| Action    | Что именно вы сделали (не «мы», а «я»), какие решения приняли и почему |
| Result    | Измеримый результат: метрики, сроки, эффект для команды и бизнеса      |

Пример: «В прошлом проекте (S) сервис падал под нагрузкой (T). Я профилировал запросы, добавил кэш и индексы, вынес тяжёлые операции в фон (A). Время ответа снизилось с 800 до 120 мс, ошибки 5xx ушли в ноль (R)».

Формулы для «опасных» вопросов:

- Слабые стороны → называем реальную слабость + что делаете, чтобы её компенсировать. Не «у меня нет слабых сторон» и не «я трудоголик».
- Причина ухода → через рост, а не через побег. Плохо: «надоели тупые задачи и плохой менеджер». Хорошо: «хочу работать с высоконагруженными системами, в текущей роли таких задач нет».
- Ошибка или неудача → показываем зрелость: что пошло не так, как заметили, что изменили в процессе, чтобы не повторилось.
- Конфликт в команде → фокус на решении, а не на людях. Не обесценивать коллег и не выставлять себя единственно правым.
- Почему хотим работать у нас → конкретика: продукт, стек, инженерная культура, задачи. Общие слова вида «вы большая и стабильная компания» не работают.
- Зарплатные ожидания → вилку и нижнюю границу определить заранее; по возможности сначала уточнить диапазон у компании.

Вопросы кандидату к работодателю:

- Как устроен [процесс разработки](#36-методологии-разработки-agile-scrum-kanban): спринты, код-ревью, CI/CD?
- Как принимаются технические решения?
- Какие ожидания от первых 3–6 месяцев?
- Почему открыта позиция: рост команды или замена?

Красные флаги в ответах:

- Негатив о прошлом работодателе или коллегах.
- «Хочу больше денег» как единственная причина смены работы.
- «У меня нет слабых сторон» — выглядит как отсутствие рефлексии.
- Слишком длинные ответы (норма — 1,5–2 минуты).
- Противоречия в фактах — заметны при перекрёстных вопросах.

Как репетировать:

- Проговорить ответы вслух или записать на видео.
- Провести mock-интервью с ИИ: попросить модель выступить в роли HR или Hiring Manager.
- Подготовить 2–3 истории под каждый блок: конфликт, ошибка, успех, сложная задача.

#### Техническое собеседование

##### Java

| #     | Ресурс                                                                                                                       | Ссылка                                                                        |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| 37.29 | Максим Добрынин. Техническое собеседование Middle Java Developer                             | [YouTube](https://www.youtube.com/watch?v=Yd4a77dz1GA)                                 |
| 37.30 | Митрофанов. Всё про Java-собеседования в 2026                                                        | [YouTube](https://www.youtube.com/watch?v=X7Nc1hdcHB8)                                 |
| 37.31 | Павел Сорокин. На этих вопросах сыпятся джуны - разбор Java собеседования | [YouTube](https://www.youtube.com/watch?v=_Eb3QiThx30)                                 |
| 37.32 | Павел Сорокин. Реальное Java Junior собеседование                                                 | [YouTube](https://www.youtube.com/watch?v=ThHSgWSwAbk)                                 |
| 37.33 | ШОРТКАТ. Как проходят Java Interview в 2026 году                                                            | [YouTube](https://www.youtube.com/watch?v=kBSCDBWsJo0)                                 |
| 37.34 | ШОРТКАТ. Java собеседование вживую                                                                       | [YouTube](https://www.youtube.com/watch?v=qCdFAQ0tk-A)                                 |
| 37.35 | ViacheslavChernyshov. Java Interview Questions and Answers                                                                         | [GitHub](https://github.com/ViacheslavChernyshov/java-interview-questions-and-answers) |

##### Алгоритмическая секция

| #     | Ресурс                                                                                                                                                                                        | Ссылка                                                                                |
| ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 37.36 | Владимир Балун. Как пройти алгоритмическое собеседование. Подготовка к алгоритмическим собеседованиям     | [YouTube](https://www.youtube.com/watch?v=R-4JkmAdARo)                                         |
| 37.37 | Антон Назаров. Подготовься к алгоритмическому собеседованию в Яндекс за 1.5 часа. Полный курс по алгоритмам | [YouTube](https://www.youtube.com/watch?v=STpA9rxN26I)                                         |
| 37.38 | Зраев Артем. Проходим алгоритмическое интервью                                                                                                             | [YouTube](https://www.youtube.com/watch?v=QbgkC_9_Ri4&list=PL0UhPLiDBaRmLpzk1I1fNiox3fKLJaG-G) |
| 37.39 | Sean Prashad. LeetCode Patterns                                                                                                                                                                     | [Seanprashad.com](https://seanprashad.com/leetcode-patterns/)                                  |
| 37.40 | LeetCode                                                                                                                                                                                            | [LeetCode](https://leetcode.com/)                                                              |

##### SQL

| #     | Ресурс                                                                                   | Ссылка                                                                                |
| ----- | ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 37.41 | Database Programmer. Вопросы по SQL на собеседовании                   | [YouTube](https://www.youtube.com/watch?v=RZhTi9TXeRo&list=PLJXRI1dijmWC_TsUe1Tr9bMyjtyvG-F6X) |
| 37.42 | Prog Blog. Топ вопросы на собеседовании по SQL                      | [YouTube](https://www.youtube.com/playlist?list=PLwHvxJae2LawmHmDpWMvimvB_SmUEcH2t)            |
| 37.43 | Stanislav Orlovskiy. Лучшие вопросы с собеседований по PostgreSQL | [YouTube](https://www.youtube.com/watch?v=dbBHgI5Sg1A)                                         |
| 37.44 | DevWizardHQ. Full-Stack Senior Engineer Interview Preparation. Databases                       | [GitHub](https://github.com/DevWizardHQ/software-engineering-interview-preparation#databases)  |
| 37.45 | kansiris. SQL Interview Questions & Answers                                                    | [GitHub](https://github.com/kansiris/SQL-interview-questions)                                  |

##### System Design

| #     | Ресурс                                                                                                                        | Ссылка                                                             |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| 37.46 | rexer. Как подготовиться и пройти System Design Interview                                                    | [Хабр](https://habr.com/ru/companies/spring_aio/articles/903542/)       |
| 37.47 | db-exp. Собеседование по System Design: как запроектировать и не потеряться           | [Хабр](https://habr.com/ru/companies/yandex_praktikum/articles/834230/) |
| 37.48 | MangoOffice. System Design интервью: как его проходить и что проверяют работодатели | [Хабр](https://habr.com/ru/companies/mango_telecom/articles/950578/)    |
| 37.49 | ШОРТКАТ. System Design интервью с разработчиком из adjoe, ex-Uzum                                    | [YouTube](https://www.youtube.com/watch?v=cUZHrKlocqQ)                      |
| 37.50 | Design Gurus. Grokking System Design                                                                                                | [GitHub](https://github.com/design-gurus/grokking-system-design)            |

##### Frontend

| #     | Ресурс                                                                                                                                      | Ссылка                                                     |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| 37.51 | Владилен Минин. Полный гайд по JavaScript-собеседованию                                                     | [YouTube](https://www.youtube.com/watch?v=M_pclb-58ZY)              |
| 37.52 | Владилен Минин.  Собеседование на FRONTEND Разработчика уровня Senior (Middle +)                    | [YouTube](https://www.youtube.com/watch?v=TOw2ME7Bvvw)              |
| 37.53 | Автоматизируем софт. Собеседование Middle Frontend-разработчика                                        | [RuTube](https://rutube.ru/video/25fb751257fe41ca9ae5e2629f0964d8/) |
| 37.54 | Result University. Собеседование на Frontend-разработчика. Вопросы по React, JavaScript, TypeScript, Frontend | [YouTube](https://www.youtube.com/watch?v=u0lkEidbKvE)              |
| 37.55 | Reactify. Frontend-собеседование с разбором. Групповой мок-формат                                         | [YouTube](https://www.youtube.com/watch?v=_A8PJ-X0_fA)              |
| 37.56 | Ulbi TV. Прохожу собеседование на Senior (Middle +) Frontend-разработчика                                       | [YouTube](https://www.youtube.com/watch?v=nqwJDi-z738)              |
| 37.57 | Yauhen Kavalchuk. Front-end. Вопросы на собеседовании                                                                       | [GitHub](https://github.com/YauhenKavalchuk/interview-questions)    |

#### Лайфхаки для поиска работы и прохождения собеседований

#### Лайфхак № 1. Использование ИИ для автоматического поиска работы

- Ключевые термины:
  
  - **n8n** — платформа для автоматизации рабочих процессов (workflow automation), которая позволяет соединять различные сервисы, приложения и API в единые автоматизированные сценарии.

- Полный гайд по использованию n8n можно найти здесь: [Владимир Карпухин. Полный гайд на n8n. ИИ агенты и автоматизации](https://www.youtube.com/watch?v=tUufFo-JTZQ)

**HH.ru**

| #     | Ресурс                                                                                                                                                                                                                                                                                                                                                                                                                       | Ссылка                                                                                                                     |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 37.58 | Рустам Камалов. Ищи работу правильно! AI анализ вакансий c n8n | [YouTube](https://www.youtube.com/watch?v=dCYI-7PweDw) |

**LinkedIn**

| #     | Ресурс                                                                                                                                                                                                                                                                                                                                                                                                                       | Ссылка                                                                                                                     |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 37.59 | Макс Нечаев.  Создал ИИ-АГЕНТА, который САМ ищет мне работу + [n8n шаблон]  | [YouTube](https://www.youtube.com/watch?v=So9RLx9qdig) |
| 37.60 | Jono Catliff.  Automate Your Job Search Using AI (Indeed, LinkedIn, ZipRecruiter) | [YouTube](https://www.youtube.com/watch?v=LIzZRgfW4ok) |

#### Лайфхак № 2. Автоотклики на платформах для поиска работы

- Ключевые термины:
  - **Автоотклик** — автоматическая отправка откликов на подходящие вакансии без необходимости вручную отправлять каждый отклик.

Обычно система самостоятельно:
- находит вакансии по заданным критериям
- отбирает подходящие вакансии
- отправляет на них отклики
- при необходимости прикрепляет резюме и сопроводительное письмо

**HH.ru**

| #     | Ресурс                                                                                                                                                                                                                                                                                                                                                                                                                       | Ссылка                                                                                                                     |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 37.61 | MrAnalitik. Автоотклик на hh | [YouTube](https://www.youtube.com/watch?v=bBzlRfQIGyE) |
| 37.62 | Александр Стародубцев. Как я сделал бота для автооткликов на HH.ru (n8n + Python + AI) | [YouTube](https://www.youtube.com/watch?v=EakL7eoSL9U) |
| 37.63 | ivandev. Как сделать 200 ОТКЛИКОВ на hh.ru за 1 МИНУТУ при помощи n8n | [YouTube](https://www.youtube.com/watch?v=kwdXGQO1_RE) |
| 37.64 | Nikon_Bruh. Поиск работы в IT: настраиваем автоотклики на HH.ru | [YouTube](https://www.youtube.com/watch?v=8oBGYa8lhBA) |

**LinkedIn**

| #     | Ресурс                                                                                                                                                                                                                                                                                                                                                                                                                       | Ссылка                                                                                                                     |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 37.65 | Michele Torti. I Built an AI System That Automates My Job Applications (n8n tutorial) | [YouTube](https://www.youtube.com/watch?v=lq8OaM-SeJo) |
| 37.66 | Eric Tech.  How I Automated My LinkedIn Job Hunt with BrowserUse + AI | [YouTube](https://www.youtube.com/watch?v=dmMMsq8Sp8s) |
| 37.67 | Padho with Pratyush. How I Automated My Entire Job Search | [YouTube](https://www.youtube.com/watch?v=hSDo59FppOU) |
| 37.68 | BuildWithPrashant.  How to Auto Apply to 100+ Jobs on LinkedIn with AI (Step by Step) | [YouTube](https://www.youtube.com/watch?v=yypO9tsjSSQ) |

#### Лайфхак № 3. Нетворкинг 

> «Кто-то сейчас в чате пишет, что в IT можно попасть по знакомству. Так вот вам эти знакомства: заходите по QR-коду и разговаривайте с людьми в формате нетворкинга. Пишите друг другу, знакомьтесь, заводите связи и обменивайтесь IT-опытом».
>
> — **Владимир Балун**, ex-Team Lead в Яндексе. 
> *Цитата с конференции «#РАЗНЕСИ_СОБЕС», 26.09.2026*

- Ключевые термины:  
  - **Нетворкинг (networking)** — это установление, развитие и поддержание профессиональных связей с другими людьми.

- Мероприятия:
  - IT-митапы и конференции → профессиональные знакомства и обмен опытом
  - Карьерные мероприятия / job fairs → работодатели, рекрутеры, вакансии

- Советы по подготовке резюме для митапов и конференций:
  - заранее изучите **список компаний и вакансий** участников мероприятия
  - адаптируйте резюме под интересующие **позиции и требования**
  - старайтесь уместить резюме в **1–2 страницы**
  - указывайте **целевую позицию и ключевой стек**
  - выделяйте **релевантные проекты и достижения**
  - добавляйте ссылки на **GitHub, портфолио и профессиональные профили**
  - подготовьте **электронную версию резюме** в форматах PDF и DOCX и QR-код со ссылкой на неё
  - для карьерных мероприятий возьмите **5–10 распечатанных экземпляров**, если планируете общаться с несколькими работодателями.


**IT-митапы и конференции**

| #     | Ресурс                                                                                                                                                                                                                                                                                                                                                                                                                       | Ссылка                                                                                                                     |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 37.69 | Timepad. Все события по теме ИТ и интернет в Москве | [Timepad](https://afisha.timepad.ru/moscow/categories/it-i-internet) |
| 37.70 | ЗДЕСЬ events. Все события по теме ИТ и интернет в Москве | [ЗДЕСЬ events](https://zdes.events/blog/moscow/meetups) |
| 37.71 | Networkly. IT-мероприятия в Москве | [Networkly](https://networkly.app/event/moscow) |
| 37.72 | All-events.ru. Мероприятия по IT-Информационным технологиям по Нетворкингу в Москве | [All-events.ru](https://all-events.ru/events/calendar/city-is-moskva/theme-is-informatsionnye_tekhnologii/tags-is-networking/) |
| 37.73 | Freeitevent . IT мероприятия в Москве 2026 | [Freeitevent](https://freeitevent.ru/events/moscow/) |
| 37.74 | ICT2GO.ru. IT мероприятия в Москве | [ICT2GO.ru](https://ict2go.ru/events/) |

**Карьерные мероприятия**

| #     | Ресурс                                                                                                                                                                                                                                                                                                                                                                                                                       | Ссылка                                                                                                                     |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 37.75 | FutureToday. Дни карьеры FutureToday | [Careerday.fut.ru](https://careerday.fut.ru/events-msk) |
| 37.76 | Fresh Business. Карьерный форум, ярмарка вакансий в Москве | [Careerforums.ru](https://careerforums.ru/fresh-business) |
| 37.77 | AIESEC. Карьерный форум, ярмарка вакансий в Москве | [Aiesecrussia.ru](https://aiesecrussia.ru/events) |
| 37.78 | Changellenge. Карьерный форум, ярмарка вакансий в Москве | [Changellenge.com](https://changellenge.com/event) |
| 37.79 | Трудкрут.рф. Твой форум. Твоя карьера | [Трудкрут.рф](https://трудкрут.рф/forum.html) |
| 37.80 | Яндекс. Гуглим в Яндексе: "карьерные IT форумы" и т.п. | [ya.ru](https://ya.ru/search/?text=%D0%BA%D0%B0%D1%80%D1%8C%D0%B5%D1%80%D0%BD%D1%8B%D0%B5+IT+%D1%84%D0%BE%D1%80%D1%83%D0%BC%D1%8B&lr=213) |

#### Лайфхак №4. Использование ИИ для подготовки к собеседованиям

- Готовимся с ИИ к интервью в формате Mock-собеседований: можно попросить их выступить в роли HR, Java Backend Interviewer или Senior Java Developer и провести полноценное пробное собеседование

| #     | Ресурс                                                                                                                                                                                                                                                                                                                                                                                                                       | Ссылка                                                                                                                     |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 37.81 | ChatGPT | [ChatGPT](https://chatgpt.com) |
| 37.82 | DeepSeek | [DeepSeek](https://www.deepseek.com) |
| 37.83 | Gemini | [Gemini](https://gemini.google.com) |
| 37.84 | Claude | [Claude](https://claude.ai) |
| 37.85 | Нейрокот. Telegram-бот для получения ответов от ChatGPT. Можно использовать для мобильной подготовки перед собеседованием в формате Mock-интервью  | [Telegram](https://t.me/zero_neuro_cat_bot) |
| 37.86 | Мэтч. Telegram-бот для проведения бесплатных mock-собеседований | [Telegram](https://it-interview.io/free-mock-interview?utm_source=meetup&utm_medium=cpc&utm_campaign=rnd) |

#### Как остаться незаменимым? (подходит только опытным сотрудникам)

| #     | Ресурс                                                                                                                                          | Ссылка                                        |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 37.87 | Сергей про Карьеру. Уволили всех, кроме меня. Что я делал иначе?                                    | [YouTube](https://www.youtube.com/watch?v=uY6cjQF7wP8) |
| 37.88 | Сергей про Карьеру. Тебя заменят, даже если ты лучший. Вот что решает на самом деле | [YouTube](https://www.youtube.com/watch?v=GEonVaFfvqU) |

#### Дополнительная литература

- Gayle Laakmann McDowell — «Cracking the Coding Interview» → Практическое руководство по техническим собеседованиям: алгоритмы, структуры данных, типовые задачи, вопросы и стратегии их решения. Использовать как основной дополнительный источник для подготовки к алгоритмической и технической части интервью.
- Alex Xu — «System Design Interview» → Практическое руководство по System Design-интервью: требования, API, базы данных, кэширование, масштабирование, очереди, балансировка нагрузки и отказоустойчивость. Использовать выборочно при подготовке к System Design после освоения базовой backend-архитектуры и распределённых систем.
- Martin Kleppmann — «Designing Data-Intensive Applications» → Фундаментальная книга по системам, работающим с большими объёмами данных: storage, репликация, партиционирование, транзакции, consistency, распределённые системы, batch/stream processing и messaging. Не является книгой исключительно для собеседований; использовать как углубление после изучения SQL, PostgreSQL, Redis, Kafka/RabbitMQ и микросервисов.
- John Sonmez — «The Complete Software Developer's Career Guide» → Практическое руководство по карьере разработчика: поиск работы, резюме, собеседования, переговоры, профессиональное развитие и построение долгосрочной карьеры. Использовать выборочно как дополнительный источник по карьерным вопросам.
- Gayle Laakmann McDowell — «The Google Resume» → Практическое руководство по составлению резюме, сопроводительных писем, поиску работы и подготовке к техническим интервью. Использовать как дополнительный источник при подготовке резюме и откликов; не является обязательным для прохождения roadmap.

## Лицензия

Этот проект распространяется под лицензией MIT. 

См. файл [LICENSE](LICENSE) для подробностей.