# План подготовки: Java Fullstack Developer (Middle)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](../../../LICENSE)

## Цель

Подготовиться к Java Fullstack-вакансиям уровня Middle и сформировать техническую базу, соответствующую требованиям рынка.

<img src="../../../assets/images/fullstack-dev-pepe.png" alt="It's coding time" width="100%">

## Параметры

| Параметр | Значение |
|---|---|
| Длительность | 103 недели (~24 месяца), календарь — ориентир |
| Норма | 15–17 качественных часов в неделю |
| Максимум | 19–21 час в неделю |
| Java | Java 21 |
| Node.js | Node.js 22 LTS |
| Frontend-стек | React 19 + TypeScript + Next.js 15 + Zustand + TanStack Query + Redux Toolkit |
| Сборка | Maven + Gradle (базово) + pnpm |
| Принцип | Календарь — ориентир. Лучше 103 недели с усвоением, чем 90 с пробелами |

**Структура:**
- Часть 1 (недели 1–33): Backend Junior+ база
- Часть 2 (недели 34–68): Frontend Junior+ база + Fullstack Integration + Cloud
- Часть 3 (недели 69–103): Middle Extension

**Важно:** Техническая подготовка — необходимое, но недостаточное условие для Middle. Реальный Middle требует 2–3 лет коммерческого опыта, участия в архитектурных решениях и работы с production. Этот план даёт техническую базу, но опыт приходит только с работой.

**Стратегия:**
1. Пройти Часть 1 (33 недели).
2. Начать подаваться на Backend Junior/Junior+ вакансии.
3. Получить оффер и работать.
4. Параллельно проходить Часть 2 (35 недель) и Часть 3 (35 недель).
5. Через 1.5–2 года работы — подаваться на Middle Fullstack.

---

## Что такое Task Management System?

Task Management System — сквозной fullstack пет-проект, разрабатывается с недели 12 по 103. Аналог Jira / Trello / Asana.

### Эволюция проекта

| Часть | Недели | Что происходит |
|---|---|---|
| Часть 1 | 12–33 | Backend Monolith: Spring Boot + PostgreSQL + JPA + Security + Redis + Docker + SQL Deep |
| Часть 2 | 34–68 | Frontend: HTML/CSS → JS → TS → React → Next.js → интеграция → Cloud |
| Часть 3 | 69–103 | Микросервисы: Clean + DDD + Kafka + RabbitMQ + K8s + Cloud + Observability |

### Итоговая архитектура

**Функциональность:**
- Пользователи, регистрация, логин (JWT + OAuth2/OIDC)
- Проекты, задачи (CRUD), статусы, приоритеты, дедлайны
- Комментарии, роли (USER, ADMIN)
- Поиск, фильтрация, сортировка, пагинация
- REST API + OpenAPI/Swagger + GraphQL (опционально)
- Realtime-уведомления (WebSocket / SSE)
- Event-Driven: Kafka + RabbitMQ
- Микросервисы: User Service, Task Service, Notification Service
- Frontend: React + Next.js + TypeScript
- Deployed: frontend на Vercel, backend на AWS, БД managed

**Технический стек:**
- Backend: Java 21 + Spring Boot + Spring Data JPA + Spring Security + Spring Cloud
- БД: PostgreSQL + Flyway + Redis
- Messaging: Kafka + RabbitMQ
- Resilience: Resilience4j
- Observability: Micrometer, Prometheus, Grafana, OpenTelemetry, Sentry
- Frontend: React 19 + TypeScript + Next.js 15
- State: Zustand + TanStack Query + React Hook Form + Zod + Redux Toolkit
- Styling: Tailwind CSS + CSS Modules + design tokens
- UI: Storybook + Radix UI / shadcn
- Tests: Vitest + RTL + MSW + Playwright + Storybook + visual + a11y + Pact + PIT
- Contract: OpenAPI + generated TS client
- Static Analysis: SonarQube
- Infra: Docker + Compose + Kubernetes (Helm) + Nginx
- CI/CD: GitHub Actions
- Cloud: Vercel + AWS (VPC, EC2, ECS/EKS, RDS, ElastiCache, S3, CloudFront, IAM, Secrets Manager)
- Сборка: Maven + Gradle (базово) + pnpm
- Monorepo: Nx / Turborepo
- Load Testing: k6

---

## Реальность рынка Middle Fullstack

**Технические требования:**
- Backend: Java Core глубоко, Spring Boot, JPA, Security + Spring Internals
- Backend: SQL: сложные запросы, EXPLAIN, оптимизация, транзакции, window functions
- Backend: Kafka и RabbitMQ
- Backend: Микросервисы (или модульный монолит)
- Backend: Docker, CI/CD уверенно
- Backend: Observability — базово
- Frontend: React + TypeScript глубоко
- Frontend: Next.js / SSR / CSR / ISR
- Frontend: State management
- Frontend: Performance optimization
- Frontend: Testing (unit + component + E2E + contract)
- Frontend: CSS-архитектура, design systems
- Frontend: System Design (архитектура SPA, data fetching, code splitting)
- Fullstack: OpenAPI contract, auth flow, deployment
- Cloud: Vercel + AWS
- System Design базовый
- Kubernetes — часто требуется, с Helm
- Load Testing — базово

**Не технические требования:**
- 2–3 года коммерческого опыта
- Code review, архитектурные решения, production, менторство, бизнес-контекст

**План покрывает технические требования.** Остальное приходит с работой.

---

## Контрольные точки по месяцам

### После месяца 1 (Java Fundamentals)
- Java-приложение без подсказок
- Collections, Generics, Streams — уверенно
- Git: branch, merge, rebase
- Maven + Gradle: собрать JAR
- 5–10 задач LeetCode (Easy)

### После месяца 2 (JVM + Concurrency + Algorithms)
- JVM memory model — базово
- Concurrency: race condition, deadlock, ExecutorService
- Virtual Threads (Java 21) — концептуально
- 25–30 задач LeetCode

### После месяца 4 (JPA + Security + Testing)
- @Transactional: propagation, isolation
- N+1 — воспроизвести и исправить
- Spring Security: JWT, roles
- Unit + Controller + Integration tests
- Testcontainers + Flyway + WireMock

### После месяца 6 (Docker + Patterns + Architecture)
- Docker + Compose (Spring Boot + PostgreSQL)
- SOLID + 5 паттернов
- Архитектура: слои, dependency direction
- Redis: cache-aside, TTL, invalidation
- Nginx: reverse proxy

### После месяца 8 (SQL Deep + Junior+ база завершена)
- Window functions, рекурсивные CTE, EXPLAIN ANALYZE
- Оптимизация сложных запросов
- CI/CD: GitHub Actions
- Работающий монолитный Backend Task Manager
- 50–60 задач LeetCode
- **Действие: начать подаваться на Backend Junior+**

### После месяца 13 (Frontend Core + Integration)
- HTML/CSS — адаптивная вёрстка, CSS architecture
- JavaScript — глубоко (event loop, closures, prototypes)
- TypeScript — строгая типизация без any
- React — компоненты, hooks, router, state
- Storybook + design system
- OpenAPI-клиент сгенерирован в TypeScript
- Auth flow, security
- Frontend Testing: unit + component + E2E

### После месяца 15 (Fullstack + Cloud + Next.js)
- Next.js: App Router, Server Components, Server Actions
- SSR / CSR / ISR trade-offs
- Frontend Performance: Core Web Vitals
- Frontend System Design
- Fullstack Docker Compose
- Cloud: Vercel + AWS
- Deployed URL (HTTPS)

### После месяца 18 (Clean + DDD + Messaging + Microservices)
- Clean / Hexagonal Architecture
- DDD: Aggregates, Bounded Contexts
- Kafka: producer, consumer, consumer groups, DLT
- RabbitMQ: exchange, queue, DLQ
- Микросервисы с Database per Service
- Spring Cloud: Config, Gateway, Discovery

### После месяца 21 (K8s + Observability + Cloud Advanced)
- Kubernetes: Pod, Deployment, Service, Ingress, HPA
- Helm, StatefulSet, RBAC, Network Policies
- Observability: metrics, logs, traces, alerting
- AWS: VPC, RDS, ElastiCache, S3, CloudFront, ECS/EKS
- Monorepo: Nx / Turborepo

### После месяца 24 (Load Testing + System Design + Финал)
- Load Testing: k6
- System Design HLD: URL Shortener, Chat, Feed
- Distributed systems: CAP, consensus, consistency
- CQRS + Event Sourcing
- Contract Testing (Pact), Mutation Testing (PIT), SonarQube
- Резюме + mock-интервью для Middle

---

# ЧАСТЬ 1 (недели 1–33): BACKEND JUNIOR+ БАЗА

Backend — фундамент Fullstack. Без этой части переход к Fullstack невозможен.

---

## Месяц 1 (недели 1–5): Java Fundamentals + Git + Maven + Gradle + SQL

### Неделя 1: Java Fundamentals + Git + Maven + Gradle

| День | Тема | Что делать |
|---|---|---|
| Пн | Синтаксис, primitive/reference types, operators, if/switch/loops | 10 мини-программ |
| Ср | Методы, массивы, классы, объекты, конструкторы | Класс Student |
| Пт | static, final, access modifiers, packages | Разобрать на примерах |
| Сб | Git: branch, merge, конфликты | Репозиторий, коммиты |
| Вс | Maven: создать проект, собрать JAR | Maven-проект |

**Ресурс:** Хорстманн (том 1, гл. 1–5), Pro Git (гл. 2–3).

### Неделя 2: OOP + Git + Maven + Gradle

| День | Тема | Что делать |
|---|---|---|
| Пн | Наследование, полиморфизм, абстракция | Shape → Circle/Rectangle |
| Ср | Интерфейсы, composition vs inheritance | Через композицию |
| Пт | Object, equals/hashCode, String, String Pool | Примеры |
| Сб | Git: rebase, cherry-pick, reset vs revert | Практика |
| Вс | Maven: dependency:tree, profiles + Gradle basics: build.gradle, tasks | Оба сборщика |

**Ресурс:** «Effective Java» Блоха (гл. 1–4).

### Неделя 3: Java Essentials + Collections

| День | Тема | Что делать |
|---|---|---|
| Пн | enums, records, modern switch | Высокий приоритет |
| Ср | pattern matching, Date/Time API, var | Высокий приоритет |
| Пт | Exceptions: checked/unchecked, try-with-resources | Программа с обработкой |
| Сб | Collections: List, ArrayList vs LinkedList | Сложность операций |
| Вс | SQL: JOIN, GROUP BY | 10 задач |

### Неделя 4: Collections + Generics + Streams

| День | Тема | Что делать |
|---|---|---|
| Пн | Set, HashSet, TreeSet, LinkedHashSet | Когда что использовать |
| Ср | Map, HashMap (внутреннее устройство), TreeMap | hash, bucket, resize |
| Пт | Queue, Deque, ArrayDeque + Generics | FIFO/LIFO |
| Сб | Wildcards, PECS, type erasure | ? extends T, ? super T |
| Вс | Stream API + Optional | Переписать на Stream API |

**Критерий:** могу выбрать коллекцию и объяснить сложность.

### Неделя 5: Review / Buffer + CLI Task Manager

| День | Тема | Что делать |
|---|---|---|
| Пн | Повторение Collections + Generics | 15 вопросов |
| Ср | Повторение Stream API + Optional | 10 задач на Stream |
| Пт | Повторение Git + Maven + Gradle | Пробелы |
| Сб | Мини-проект: CLI Task Manager | Применить всё |
| Вс | Итог месяца 1 | Контрольная точка |

---

## Месяц 2 (недели 6–11): JVM + Concurrency + Algorithms

### Неделя 6: JVM + память + GC

| День | Тема | Что делать |
|---|---|---|
| Пн | JVM: Heap, Stack, Metaspace, Class Loading | Схема памяти |
| Ср | GC: G1, ZGC, Stop-the-World | Как работает GC |
| Пт | Утечки памяти | 3 примера |
| Сб | LeetCode: Two Sum, Valid Parentheses, Merge Two Sorted Lists | 3 Easy |
| Вс | SQL: подзапросы, CTE + EXPLAIN | 5 задач |

### Неделя 7: Concurrency (базово)

| День | Тема | Что делать |
|---|---|---|
| Пн | Thread, Runnable, Callable | Примеры |
| Ср | synchronized, volatile, race condition | Race condition + fix |
| Пт | ExecutorService, Thread Pool | Пример |
| Сб | LeetCode: Best Time to Buy and Sell Stock, Contains Duplicate | 3 Easy |
| Вс | SQL: индексы + EXPLAIN | Практика |

**Ресурс:** «Java Concurrency in Practice» (гл. 1–3).

### Неделя 8: Concurrency (продолжение) + Virtual Threads

| День | Тема | Что делать |
|---|---|---|
| Пн | Atomic, CAS, ConcurrentHashMap | AtomicInteger + ConcurrentHashMap |
| Ср | Virtual Threads (Java 21) | Концептуально |
| Пт | JMM: happens-before, deadlock | Пример deadlock |
| Сб | LeetCode: Valid Palindrome, Merge Intervals | 3 Easy/Medium |
| Вс | Повторение concurrency | 15 вопросов |

### Неделя 9: Concurrency (глубоко)

| День | Тема | Что делать |
|---|---|---|
| Пн | ReentrantLock, ReentrantReadWriteLock, StampedLock | Примеры |
| Ср | CompletableFuture, ForkJoinPool | Практика |
| Пт | Semaphore, CountDownLatch, CyclicBarrier, Phaser | Примеры |
| Сб | LeetCode: Group Anagrams, Kth Largest Element | 3 Medium |
| Вс | Повторение concurrency | 20 вопросов |

**Критерий:** могу объяснить happens-before, выбрать примитив синхронизации, найти deadlock.

### Неделя 10: Алгоритмы + структуры данных

| День | Тема | Что делать |
|---|---|---|
| Пн | Стек, очередь, deque | Реализовать |
| Ср | Heap, PriorityQueue | Kth Largest Element |
| Пт | Деревья: BST, обходы | Реализовать BST |
| Сб | LeetCode: Number of Islands, Course Schedule | 3 Medium |
| Вс | Повторение Java | 20 вопросов |

### Неделя 11: Review / Buffer + Producer-Consumer

| День | Тема | Что делать |
|---|---|---|
| Пн | Повторение JVM | 15 вопросов |
| Ср | Повторение concurrency | 20 вопросов |
| Пт | Повторение алгоритмов | 5 задач |
| Сб | Мини-проект: Producer-Consumer | Многопоточная программа |
| Вс | Итог месяца 2 | 25–30 задач LeetCode |

---

## Месяц 3 (недели 12–16): HTTP + Spring + Spring Internals + JPA

### Неделя 12: HTTP + REST + Spring Core

| День | Тема | Что делать |
|---|---|---|
| Пн | HTTP: request/response, methods, status codes, headers | curl |
| Ср | JSON, idempotency, caching, CORS | Примеры |
| Пт | REST: resource, URI, CRUD, DTO, pagination | Спроектировать API Task Manager |
| Сб | Spring Core: DI/IoC, beans, scopes, lifecycle | Примеры |
| Вс | SQL: транзакции, ACID, isolation levels | Практика |

### Неделя 13: Spring Boot + MVC + старт backend-проекта

| День | Тема | Что делать |
|---|---|---|
| Пн | @SpringBootApplication, profiles, application.yml | Создать проект |
| Ср | @RestController, @GetMapping, @PostMapping | Первый контроллер |
| Пт | DTO, validation (@Valid, @NotNull) | DTO + валидация |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Глава 1 Алекса Сюя |
| Вс | Пет-проект backend: Spring Boot + PostgreSQL CRUD | Task Manager |

### Неделя 14: Spring Internals

| День | Тема | Что делать |
|---|---|---|
| Пн | BeanPostProcessor, BeanFactoryPostProcessor | Примеры |
| Ср | AOP: aspects, pointcuts, advice | Реализовать aspect |
| Пт | Proxies: JDK dynamic vs CGLIB | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Глава 2 |
| Вс | Пет-проект: применить AOP (логирование) | Реализовать |

**Критерий:** понимаю, как Spring создаёт бины, как работает AOP, чем отличаются прокси.

### Неделя 15: Spring Data JPA (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | JpaRepository, derived queries | Repository |
| Ср | @Query, JPQL | Собственные запросы |
| Пт | SQL: EXPLAIN + оптимизация | 3 запроса |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Глава 3 |
| Вс | Пет-проект: repository + derived queries | Обновление |

### Неделя 16: Spring Data JPA (часть 2) + OpenAPI

| День | Тема | Что делать |
|---|---|---|
| Пн | Pagination, sorting | Пагинация |
| Ср | OpenAPI / Swagger: спецификация + UI | Добавить в Task Manager |
| Пт | Testing: Mockito basics (@Mock, @InjectMocks, verify) | Unit-тесты |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Глава 4 |
| Вс | Пет-проект: OpenAPI + Testing | Swagger + unit-тесты |

---

## Месяц 4 (недели 17–22): JPA + Security + Testing

### Неделя 17: Review / Buffer (HTTP + Spring + JPA)

| День | Тема | Что делать |
|---|---|---|
| Пн | Повторение Spring Core + Internals | 20 вопросов |
| Ср | Повторение Spring Data JPA | 15 вопросов |
| Пт | Повторение HTTP + REST | 15 вопросов |
| Сб | Пет-проект: закрыть пробелы | Рефакторинг |
| Вс | Итог месяца 3 | Контрольная точка |

### Неделя 18: @Transactional + JPA performance

| День | Тема | Что делать |
|---|---|---|
| Пн | @Transactional: propagation, rollback, isolation | Propagation types |
| Ср | Hibernate — LAZY/EAGER, N+1 | Разобрать N+1, JOIN FETCH |
| Пт | SQL: EXPLAIN ANALYZE — читать план | 3 запроса |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Глава 5 |
| Вс | Пет-проект: @Transactional + исправление N+1 | Обновление |

### Неделя 19: Testing Controller + @ExceptionHandler

| День | Тема | Что делать |
|---|---|---|
| Пн | Testing: @WebMvcTest, MockMvc | Тесты Controller |
| Ср | Testing: тесты для @ControllerAdvice | 400/404/500 |
| Пт | Пет-проект: @ExceptionHandler, @ControllerAdvice | Единый формат ошибок |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Глава 6 |
| Вс | Пет-проект: тесты для Controller | Покрытие |

### Неделя 20: Spring Security

| День | Тема | Что делать |
|---|---|---|
| Пн | SecurityFilterChain + AuthN vs AuthZ | Разница |
| Ср | JWT: header/payload/signature + 401 vs 403 | Практика |
| Пт | Testing: Spring Security Test + тесты на 401/403 | Тесты |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект: Spring Security + JWT | Защитить API |

**Ресурс:** Laurentiu Spilca «Spring Security in Action».

### Неделя 21: Integration Testing

| День | Тема | Что делать |
|---|---|---|
| Пн | @SpringBootTest, @DataJpaTest | Интеграционные тесты |
| Ср | Test Slices, @ActiveProfiles | Настройка |
| Пт | SQL: повторение EXPLAIN + оптимизация | 3 запроса |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект: интеграционные тесты | Controller → Service → Repository |

### Неделя 22: Testcontainers + Flyway + WireMock

| День | Тема | Что делать |
|---|---|---|
| Пн | Testcontainers: @Testcontainers, @Container | Настройка |
| Ср | Testcontainers + Spring Boot | Тесты с реальной БД |
| Пт | WireMock: мокирование внешних HTTP-сервисов | Реализовать |
| Сб | Flyway: миграции | Настроить Flyway |
| Вс | Пет-проект: интеграционные тесты с Flyway + WireMock | Проверить |

**Критерий:** умею мокать внешние API через WireMock, тестировать с реальной БД через Testcontainers.

---

## Месяц 5 (недели 23–28): Docker + Patterns + Architecture + Redis + Nginx

### Неделя 23: Docker + Compose

| День | Тема | Что делать |
|---|---|---|
| Пн | Docker: Dockerfile, multi-stage build | Dockerfile для Spring Boot |
| Ср | Docker Compose: services, networks, volumes | Compose backend + PostgreSQL |
| Пт | SQL: повторение EXPLAIN + оптимизация | 3 запроса |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Схема Task Manager |
| Вс | Пет-проект: Docker Compose | Запустить |

### Неделя 24: Design Principles & Patterns

| День | Тема | Что делать |
|---|---|---|
| Пн | SOLID, composition over inheritance | Примеры в JDK |
| Ср | GoF: Singleton, Factory, Builder | 3 паттерна |
| Пт | GoF: Strategy, Observer | Ещё 2 паттерна |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Rate Limiter |
| Вс | Пет-проект: применить 3–4 паттерна | Рефакторинг |

### Неделя 25: Application Architecture

| День | Тема | Что делать |
|---|---|---|
| Пн | Layered architecture, dependency direction | Слои проекта |
| Ср | package-by-layer vs package-by-feature | Примеры |
| Пт | Dependency Inversion в коде | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | URL Shortener |
| Вс | Пет-проект: рефакторинг под слои | Аудит |

### Неделя 26: Redis + System Design fundamentals

| День | Тема | Что делать |
|---|---|---|
| Пн | Requirements: functional vs non-functional | Task Manager |
| Ср | Capacity planning: RPS, storage | Оценка |
| Пт | Caching: cache-aside, TTL, invalidation | Redis в Task Manager |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Notification Service |
| Вс | Пет-проект backend: добавить Redis | Интеграция |

### Неделя 27: Nginx + System Design practice

| День | Тема | Что делать |
|---|---|---|
| Пн | Load balancing: L4 vs L7, round-robin | Nginx как LB |
| Ср | Scaling: vertical vs horizontal, stateless | Масштабирование |
| Пт | Nginx: reverse proxy, upstream, headers | Настроить Nginx |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Rate Limiter |
| Вс | Пет-проект: Nginx как reverse proxy | Nginx → Spring Boot |

### Неделя 28: Review / Buffer (Docker + Architecture + Redis + Nginx)

| День | Тема | Что делать |
|---|---|---|
| Пн | Повторение Docker + Compose | 15 вопросов |
| Ср | Повторение SOLID + паттернов | 15 вопросов |
| Пт | Повторение Architecture | 10 вопросов |
| Сб | Пет-проект: закрыть пробелы | Рефакторинг |
| Вс | Итог месяца 5 | Работающий backend |

---

## Месяц 6 (недели 29–33): SQL Deep + CI/CD + Интервью-подготовка

### Неделя 29: SQL Deep (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Window functions: ROW_NUMBER, RANK, LAG/LEAD | 10 задач |
| Ср | CTE, рекурсивные CTE | 10 задач |
| Пт | EXPLAIN ANALYZE: чтение планов, cost, rows | 5 запросов |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: сложные аналитические запросы | Реализовать |

### Неделя 30: SQL Deep (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Индексы: составные, частичные, covering | Практика |
| Ср | Оптимизация: переписать медленный запрос | 5 запросов |
| Пт | Транзакции: isolation levels, deadlocks | Примеры |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: оптимизация запросов | Сравнить до/после |

### Неделя 31: SQL Deep (часть 3) + MVCC

| День | Тема | Что делать |
|---|---|---|
| Пн | MVCC internals, WAL, vacuum | Разобрать |
| Ср | Блокировки: row-level, table-level, advisory | Примеры |
| Пт | Партиционирование: range, list, hash | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: партиционировать таблицу | Реализовать |

**Критерий:** могу найти причину медленного запроса, переписать его, объяснить план.

### Неделя 32: CI/CD

| День | Тема | Что делать |
|---|---|---|
| Пн | GitHub Actions: workflow, jobs, steps | CI: build + test |
| Ср | Docker build + push в registry | GHCR или Docker Hub |
| Пт | Deployment pipeline: staging → production | Базовая настройка |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Task Manager: полный цикл |
| Вс | Пет-проект: CI/CD pipeline | Работает |

### Неделя 33: Финальная подготовка Части 1 + Interview Prep

| День | Тема | Что делать |
|---|---|---|
| Пн | Резюме: ключевые слова | Написать резюме |
| Ср | STAR-истории: 5 историй | Конфликт, ошибка, успех, сложная задача, лидерство |
| Пт | LinkedIn, портфолио, GitHub profile | Оформить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Полный mock |
| Вс | Mock-интервью: Java + Spring + SQL | 2 интервью с ИИ |

**Результат Части 1:** работающий монолитный Backend Task Manager:
- Spring Boot + PostgreSQL + JPA + Flyway
- Spring Security + JWT
- Spring Internals: AOP, BeanPostProcessor
- Redis кэширование
- Docker Compose
- Nginx reverse proxy
- CI/CD GitHub Actions
- OpenAPI/Swagger
- Unit + Integration tests + Testcontainers + WireMock
- SQL: window functions, CTE, EXPLAIN, оптимизация
- 50–60 задач LeetCode

**Действие:** начать подаваться на Backend Junior/Junior+ вакансии.

---

# ЧАСТЬ 2 (недели 34–68): FRONTEND JUNIOR+ БАЗА + FULLSTACK + CLOUD

Frontend — вторая половина Fullstack. 35 недель.

---

## Месяц 7 (недели 34–38): Frontend Fundamentals

### Неделя 34: HTML5 + Semantic + Accessibility

| День | Тема | Что делать |
|---|---|---|
| Пн | HTML5: структура документа, semantic tags | Свёрстать страницу |
| Ср | Формы, input types, validation, labels | Форма логина |
| Пт | Accessibility: ARIA, focus, keyboard navigation | Проверить в axe DevTools |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: semantic layout | Первый экран |

**Критерий:** могу объяснить, почему semantic HTML важен для a11y и SEO.

### Неделя 35: CSS3 — базовая вёрстка

| День | Тема | Что делать |
|---|---|---|
| Пн | Box model, positioning, display, overflow | 5 мини-макетов |
| Ср | Flexbox: оси, выравнивание, wrapping | Navbar + карточки |
| Пт | Grid: template, areas, auto-fit/minmax | Dashboard layout |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: адаптивная вёрстка | Мобильный + десктоп |

### Неделя 36: CSS Architecture + Design System

| День | Тема | Что делать |
|---|---|---|
| Пн | CSS methodology: BEM, CSS Modules | Рефакторинг вёрстки |
| Ср | Tailwind CSS: utility-first, config, variants | Перевести проект на Tailwind |
| Пт | Design tokens: цвета, типографика, spacing | Токены проекта |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: design system | Базовые компоненты |

**Критерий:** могу выбрать подход к CSS и обосновать trade-offs.

### Неделя 37: JavaScript — основы

| День | Тема | Что делать |
|---|---|---|
| Пн | Типы, операторы, функции, scope | 10 задач |
| Ср | DOM: выбор, изменение, события, delegation | Интерактивный список |
| Пт | Fetch API, async/await, обработка ошибок | Загрузка данных |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: интерактивность | Vanilla JS прототип |

### Неделя 38: JavaScript — глубоко

| День | Тема | Что делать |
|---|---|---|
| Пн | Closures, scope chain, IIFE | 10 задач |
| Ср | Prototypes, this, call/apply/bind | Разобрать на примерах |
| Пт | Event loop, microtasks/macrotasks, Promises | Схема + примеры |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Повторение JS | 20 вопросов |

**Критерий:** могу объяснить event loop, closures, prototype chain.

---

## Месяц 8 (недели 39–43): JavaScript Advanced + TypeScript

### Неделя 39: JavaScript — Advanced + DevTools

| День | Тема | Что делать |
|---|---|---|
| Пн | ES Modules, import/export, bundlers (Vite) | Настроить Vite |
| Ср | Memory management, leaks, garbage collection | Найти leak в DevTools |
| Пт | DevTools: Performance, Network, Memory | Профилировать |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Повторение JS | 15 вопросов |

### Неделя 40: TypeScript — основы

| День | Тема | Что делать |
|---|---|---|
| Пн | Типы, interfaces, type aliases, unions | Типизировать JS-код |
| Ср | Generics, constraints | Утилиты |
| Пт | Enums, tuples, readonly, keyof | Примеры |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: миграция на TS | Без any |

### Неделя 41: TypeScript — продвинутое

| День | Тема | Что делать |
|---|---|---|
| Пн | Utility types: Partial, Pick, Omit, Record | Практика |
| Ср | Conditional types, mapped types, infer | Примеры |
| Пт | Type guards, discriminated unions, satisfies | Рефакторинг |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: строгая типизация | Strict mode |

### Неделя 42: TypeScript — практика + Runtime validation

| День | Тема | Что делать |
|---|---|---|
| Пн | Zod: схемы, inference, parse/safeParse | Валидация API |
| Ср | React Hook Form + Zod | Формы |
| Пт | Типизация API-клиента (generated) | OpenAPI → TS |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: форма + валидация | Работает |

**Критерий:** типизация без any, runtime validation, strict mode.

### Неделя 43: Review / Buffer (HTML/CSS/JS/TS)

| День | Тема | Что делать |
|---|---|---|
| Пн | Повторение CSS + Tailwind | 15 вопросов |
| Ср | Повторение JavaScript | 20 вопросов |
| Пт | Повторение TypeScript | 15 вопросов |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Итог: статичный прототип Task Manager | Semantic + CSS + TS |

---

## Месяц 9 (недели 44–48): React

### Неделя 44: React Fundamentals

| День | Тема | Что делать |
|---|---|---|
| Пн | JSX, компоненты, props, children | 5 компонентов |
| Ср | State, useState, events, controlled inputs | Форма |
| Пт | Lists, keys, conditional rendering | Список задач |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: первые компоненты | Task Manager |

### Неделя 45: React Hooks + Context

| День | Тема | Что делать |
|---|---|---|
| Пн | useEffect, cleanup, dependencies | Загрузка данных |
| Ср | useRef, useMemo, useCallback | Оптимизация |
| Пт | Context API, useContext | Тема + auth |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: hooks + context | Работает |

### Неделя 46: React Router + Forms

| День | Тема | Что делать |
|---|---|---|
| Пн | React Router: nested, dynamic, protected | Настроить роутинг |
| Ср | React Hook Form + Zod | Формы проекта |
| Пт | Обработка ошибок, loading states | UX |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: роутинг + формы | Работает |

### Неделя 47: State Management — Zustand + TanStack Query

| День | Тема | Что делать |
|---|---|---|
| Пн | Zustand: store, actions, selectors | Client state |
| Ср | TanStack Query: queries, mutations, cache | Server state |
| Пт | Инвалидация, оптимистичные обновления | Практика |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: state management | Работает |

### Неделя 48: React Advanced

| День | Тема | Что делать |
|---|---|---|
| Пн | Reconciliation, memo, key, virtual DOM | Разобрать |
| Ср | Error Boundaries, Suspense, lazy | Практика |
| Пт | Accessibility, focus management | a11y |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: advanced React | Работает |

**Критерий:** понимаю reconciliation, могу оптимизировать ререндеры.

---

## Месяц 10 (недели 49–53): React Patterns + Design System + Integration

### Неделя 49: React Patterns

| День | Тема | Что делать |
|---|---|---|
| Пн | Compound components, render props, HOC | Примеры |
| Ср | Custom hooks: паттерны, тестируемость | 5 хуков |
| Пт | Feature-based архитектура | Рефакторинг |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: рефакторинг | Feature-based |

### Неделя 50: Storybook + Design System

| День | Тема | Что делать |
|---|---|---|
| Пн | Storybook: setup, stories, args | Настроить |
| Ср | Компоненты в изоляции, документация | Stories для UI |
| Пт | Radix UI / shadcn: доступные примитивы | Интеграция |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: design system | Stories готовы |

**Критерий:** UI-компоненты документированы и переиспользуемы.

### Неделя 51: OpenAPI Integration (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | OpenAPI schema: paths, schemas, components | Разобрать |
| Ср | openapi-typescript / orval: генерация клиента | Сгенерировать |
| Пт | Типизированные запросы, обработка ошибок | Интеграция |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: подключение к backend | Реальный API |

### Неделя 52: OpenAPI Integration (часть 2) + Realtime

| День | Тема | Что делать |
|---|---|---|
| Пн | Централизованная обработка HTTP-ошибок | Interceptors |
| Ср | WebSocket / SSE: подключение, reconnect | Realtime-уведомления |
| Пт | Realtime state sync с TanStack Query | Инвалидация |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: realtime | Работает |

### Неделя 53: Auth Flow + Security

| День | Тема | Что делать |
|---|---|---|
| Пн | JWT: cookies vs localStorage, refresh | Реализовать |
| Ср | Protected routes, role-based UI | Практика |
| Пт | XSS, CSRF, CORS, CSP basics | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: auth flow | Работает |

**Критерий:** auth flow безопасен, токены обрабатываются корректно.

---

## Месяц 11 (недели 54–58): Testing + Fullstack + Cloud

### Неделя 54: Frontend Testing (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Vitest: setup, unit-тесты | Настроить |
| Ср | React Testing Library: рендер, события, queries | Тесты компонентов |
| Пт | Тестирование хуков, async | Практика |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: unit + component тесты | Покрытие |

### Неделя 55: Frontend Testing (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | MSW: мокирование API | Настроить |
| Ср | Playwright: E2E, fixtures, POM | E2E-тесты |
| Пт | CI: запуск тестов в GitHub Actions | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: полный test pyramid | Работает |

**Критерий:** unit + component + E2E тесты проходят в CI.

### Неделя 56: Fullstack Docker Compose + Nginx

| День | Тема | Что делать |
|---|---|---|
| Пн | Docker Compose: backend + frontend + БД + Redis | Собрать стек |
| Ср | Nginx: /api → backend, / → frontend | Настроить |
| Пт | Multi-stage build для frontend | Dockerfile |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект: полный стек в Docker | Работает |

### Неделя 57: Cloud Deployment (часть 1) — Vercel + CI/CD

| День | Тема | Что делать |
|---|---|---|
| Пн | Vercel: деплой Next.js, env vars, preview | Задеплоить frontend |
| Ср | GitHub Actions: build + deploy | Настроить |
| Пт | Домены, HTTPS, CDN | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект: frontend на Vercel | Deployed URL |

### Неделя 58: Cloud Deployment (часть 2) — AWS basics

| День | Тема | Что делать |
|---|---|---|
| Пн | AWS: EC2, S3, RDS, IAM basics | Разобрать |
| Ср | Backend на EC2 / ECS, RDS managed | Задеплоить |
| Пт | S3 для статики, CloudFront CDN | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект: backend на AWS | Deployed URL |

**Критерий:** frontend + backend задеплоены, HTTPS, CDN, БД managed.

---

## Месяц 12 (недели 59–63): Next.js + Frontend Performance + System Design

### Неделя 59: Next.js (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | App Router, pages, layouts, nested routes | Миграция с React |
| Ср | Server Components vs Client Components | Разделение |
| Пт | Data Fetching: server-side, caching, revalidation | Практика |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: миграция на Next.js | Task Manager |

### Неделя 60: Next.js (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Server Actions, Route Handlers | Практика |
| Ср | Metadata, images, fonts, env vars | Оптимизация |
| Пт | Middleware / Proxy, auth в Next.js | Практика |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: полный Next.js | Работает |

### Неделя 61: SSR / CSR / ISR + Caching

| День | Тема | Что делать |
|---|---|---|
| Пн | SSR / CSR / ISR / SSG: trade-offs | Разобрать |
| Ср | Next.js caching: use cache, PPR | Понять |
| Пт | revalidateTag / revalidatePath | Практика |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: осознанный rendering | Рефакторинг |

### Неделя 62: Frontend Performance

| День | Тема | Что делать |
|---|---|---|
| Пн | Bundle analysis: code splitting, tree shaking | Настроить |
| Ср | Core Web Vitals: LCP, INP, CLS | Оптимизировать |
| Пт | Lazy loading, prefetching, virtualization | Практика |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: Lighthouse audit | Оптимизировать |

**Критерий:** могу найти performance bottleneck и объяснить решение.

### Неделя 63: Frontend System Design (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Архитектура SPA: слои, модули, границы | Схема проекта |
| Ср | Data fetching стратегии, кэширование, invalidation | Разобрать |
| Пт | Code splitting, lazy routes, prefetch | Практика |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Mock Frontend System Design | С ИИ |

---

## Месяц 13 (недели 64–68): Advanced Frontend + Observability + Финалы

### Неделя 64: Advanced State — Redux Toolkit

| День | Тема | Что делать |
|---|---|---|
| Пн | Redux Toolkit: slices, createEntityAdapter | Практика |
| Ср | Normalisation, memoized selectors | Понять |
| Пт | Zustand vs Redux vs Jotai: trade-offs | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: сложный state | Реализовать |

### Неделя 65: Advanced Frontend Testing

| День | Тема | Что делать |
|---|---|---|
| Пн | Playwright advanced: fixtures, POM, sharding | Практика |
| Ср | Visual testing (Chromatic / Percy) | Разобрать |
| Пт | a11y testing (axe), contract testing (Pact) | Понять |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект: полный test pyramid | Работает |

### Неделя 66: i18n + Feature Flags + PWA

| День | Тема | Что делать |
|---|---|---|
| Пн | i18n: react-i18next, плюрализация, форматирование | Настроить |
| Ср | Feature flags: LaunchDarkly / Unleash | Понять |
| Пт | PWA: service worker, offline, manifest | Базово |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: i18n + flags | Работает |

### Неделя 67: Frontend Observability

| День | Тема | Что делать |
|---|---|---|
| Пн | Sentry: setup, error tracking, source maps | Настроить |
| Ср | Web Vitals: RUM, reporting | Настроить |
| Пт | Логирование на клиенте, session replay | Понять |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Пет-проект frontend: observability | Работает |

**Критерий:** могу найти frontend-ошибку по Sentry и метрикам.

### Неделя 68: Frontend System Design (часть 2) + Review

| День | Тема | Что делать |
|---|---|---|
| Пн | Проектирование большого SPA: state, data fetching | Разбор |
| Ср | Trade-offs: BFF vs прямые вызовы, offline-first | Разобрать |
| Пт | Повторение React + Next.js + TS | 30 вопросов |
| Сб | LeetCode: 2 задачи + System Design (1 ч) | Практика |
| Вс | Mock Frontend Interview | 2 интервью |

**Результат Части 2:** работающий Fullstack Task Manager:
- Backend: Spring Boot + PostgreSQL + JPA + Flyway + Redis + OpenAPI
- Frontend: React + TypeScript + Next.js + Zustand + TanStack Query
- Styling: Tailwind + design system + Storybook
- Integration: OpenAPI-generated client, Auth flow, CORS, Realtime
- Testing: unit + component + E2E + visual + a11y
- Docker + Compose + Nginx
- CI/CD GitHub Actions
- Cloud: Vercel (frontend) + AWS (backend)
- Frontend Observability: Sentry + Web Vitals
- Deployed URL (HTTPS)

**Действие:** продолжать работать, параллельно проходить Часть 3.

---

# ЧАСТЬ 3 (недели 69–103): MIDDLE EXTENSION

35 недель на темы, отличающие Middle от Junior+.

---

## Месяц 14 (недели 69–73): Clean Architecture + DDD

### Неделя 69: Clean / Hexagonal Architecture (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Clean Architecture, Dependency Rule | Понять принцип |
| Ср | Ports & Adapters (Hexagonal) | Схема |
| Пт | Domain / Application / Infrastructure / Presentation | Разделение слоёв |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: рефакторинг backend под Clean | Первые шаги |

**Ресурс:** Robert C. Martin «Clean Architecture» (гл. 1–10).

### Неделя 70: Clean / Hexagonal Architecture (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Use Cases / Interactors | Реализовать |
| Ср | Repository как абстракция, Adapters | Разделить JPA и domain |
| Пт | Frontend: Feature-based архитектура | Рефакторинг React |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Clean (backend + frontend) | Проверить |

**Критерий:** domain не зависит от Spring/JPA; frontend разделён на features.

### Неделя 71: DDD (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Ubiquitous Language | Словарь Task Manager |
| Ср | Entity, Value Object | Реализовать |
| Пт | Aggregate, Aggregate Root | Спроектировать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: применить DDD | Рефакторинг |

**Ресурс:** Eric Evans «Domain-Driven Design» (гл. 1–7).

### Неделя 72: DDD (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Bounded Context, Context Map | Границы контекстов |
| Ср | Domain Service, Application Service | Разделить |
| Пт | Domain Events | Реализовать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: DDD завершено | Проверить |

**Ресурс:** Vaughn Vernon «Implementing Domain-Driven Design».

### Неделя 73: DDD (часть 3) — применение

| День | Тема | Что делать |
|---|---|---|
| Пн | Рефакторинг агрегатов: инварианты | Практика |
| Ср | Repository per aggregate | Разделить |
| Пт | Anti-corruption layer | Понять |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: финальный DDD-рефакторинг | Проверить |

**Критерий:** могу объяснить, где границы агрегатов и почему.

---

## Месяц 15 (недели 74–78): Kafka + RabbitMQ

### Неделя 74: Kafka (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Kafka: broker, topic, partition | Понять архитектуру |
| Ср | Producer, consumer, offset, consumer group | Практика |
| Пт | Delivery semantics | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: первый Kafka-топик | Events для задач |

**Ресурс:** «Kafka: The Definitive Guide».

### Неделя 75: Kafka (часть 2) + Retry / DLT

| День | Тема | Что делать |
|---|---|---|
| Пн | Idempotent producer, transactions | Практика |
| Ср | Retry, DLT | Реализовать |
| Пт | Consumer lag, мониторинг | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Kafka consumer + DLT | Работает |

**Критерий:** событие публикуется и обрабатывается, DLT работает.

### Неделя 76: RabbitMQ (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | RabbitMQ: exchange, queue, binding, routing key | Понять |
| Ср | Direct, Topic, Fanout | Практика |
| Пт | AMQP, message format | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: RabbitMQ для notification | Практика |

### Неделя 77: RabbitMQ (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Manual ACK / NACK | Практика |
| Ср | Prefetch, concurrency | Настроить |
| Пт | Retry, Dead Letter Exchange / Queue | Реализовать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: DLQ + retry | Проверить |

**Критерий:** понимаю разницу Kafka vs RabbitMQ, могу выбрать под задачу.

### Неделя 78: Review / Buffer (Clean + DDD + Messaging)

| День | Тема | Что делать |
|---|---|---|
| Пн | Повторение Clean + DDD | 20 вопросов |
| Ср | Повторение Kafka | 15 вопросов |
| Пт | Повторение RabbitMQ | 15 вопросов |
| Сб | Пет-проект: закрыть пробелы | Рефакторинг |
| Вс | Итог: Clean + DDD + Kafka + RabbitMQ | Контрольная точка |

---

## Месяц 16 (недели 79–83): Микросервисы + Spring Cloud + Resilience + Saga

### Неделя 79: Микросервисы (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Monolith vs Microservices: trade-offs | Понять |
| Ср | Границы сервисов (Bounded Context) | Определить |
| Пт | Database per Service | Спроектировать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: выделить User Service | Разделить монолит |

**Ресурс:** Sam Newman «Building Microservices» (гл. 1–4).

### Неделя 80: Микросервисы (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Синхронное (REST) vs асинхронное (Kafka) | Разобрать |
| Ср | API composition, BFF | Понять |
| Пт | Service discovery | Понять проблему |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: выделить Task Service | Разделить |

**Критерий:** 2–3 сервиса работают независимо, общаются через REST/Kafka.

### Неделя 81: Spring Cloud (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Spring Cloud Config | Centralized configuration |
| Ср | Eureka / Consul: service discovery | Реализовать |
| Пт | Spring Cloud Gateway | API Gateway |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Config + Gateway | Интеграция |

### Неделя 82: Spring Cloud (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Load balancing (Spring Cloud LoadBalancer) | Настроить |
| Ср | Distributed tracing (Micrometer Tracing) | Настроить |
| Пт | Spring Cloud Stream | Опционально |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Full Spring Cloud stack | Работает |

**Критерий:** 3 сервиса общаются через Gateway, Config централизован.

### Неделя 83: Resilience4j + Saga + Outbox

| День | Тема | Что делать |
|---|---|---|
| Пн | Circuit Breaker, Retry, Bulkhead | Реализовать |
| Ср | Saga: choreography vs orchestration | Разобрать |
| Пт | Transactional Outbox Pattern | Реализовать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: CB + Saga + Outbox | Работает |

**Критерий:** могу объяснить, почему distributed transaction — проблема и как её решает Saga.

---

## Месяц 17 (недели 84–88): Caching + Observability + Kubernetes

### Неделя 84: Redis глубоко — Caching strategies

| День | Тема | Что делать |
|---|---|---|
| Пн | Cache stampede / thundering herd | Защита |
| Ср | Distributed lock на Redis | Реализовать (Redlock / SETNX) |
| Пт | Invalidation strategies: TTL vs explicit | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: distributed lock | Работает |

**Критерий:** могу спроектировать кэширование для high-load.

### Неделя 85: Observability — Metrics + Logs

| День | Тема | Что делать |
|---|---|---|
| Пн | Micrometer, метрики | Настроить |
| Ср | Prometheus, PromQL | Поднять |
| Пт | Grafana dashboards | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: metrics + dashboard | Работает |

### Неделя 86: Observability — Traces + Alerting

| День | Тема | Что делать |
|---|---|---|
| Пн | Structured logging (JSON) + Loki / ELK | Настроить |
| Ср | OpenTelemetry: traces, spans | Настроить |
| Пт | Alerting, SLI / SLO / SLA, error budget | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: логи + трейсы + alerting | Работает |

**Критерий:** могу найти проблему по logs / metrics / traces и сформулировать SLI/SLO.

### Неделя 87: Kubernetes (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | K8s: cluster, node, control plane | Понять |
| Ср | Pod, ReplicaSet, Deployment | Практика |
| Пт | Service: ClusterIP, NodePort, LoadBalancer | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: 1 сервис в K8s | minikube / kind |

**Ресурс:** «Kubernetes: Up and Running».

### Неделя 88: Kubernetes (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | ConfigMap, Secret | Практика |
| Ср | Liveness / Readiness / Startup probes | Настроить |
| Пт | Ingress + Ingress Controller, HPA | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: часть сервисов в K8s | Работает |

---

## Месяц 18 (недели 89–93): K8s Advanced + Cloud (AWS) + gRPC

### Неделя 89: Kubernetes (часть 3) — продвинутое

| День | Тема | Что делать |
|---|---|---|
| Пн | Helm: charts, values, templates | Настроить |
| Ср | StatefulSet, DaemonSet, Job/CronJob | Практика |
| Пт | RBAC, ServiceAccount, Network Policies | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: весь стек в K8s через Helm | Работает |

### Неделя 90: Kubernetes (часть 4) — диагностика

| День | Тема | Что делать |
|---|---|---|
| Пн | Resource requests/limits, QoS | Настроить |
| Ср | kubectl: get, describe, logs, exec, port-forward | Практика |
| Пт | Диагностика проблем в K8s | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: полный стек + диагностика | Работает |

**Критерий:** могу развернуть микросервисы в K8s с Helm, probes, RBAC, HPA.

### Неделя 91: Cloud (AWS) — часть 1

| День | Тема | Что делать |
|---|---|---|
| Пн | AWS: VPC, subnets, security groups, IAM | Понять |
| Ср | EC2, ECS, EKS basics | Разобрать |
| Пт | RDS: managed PostgreSQL | Задеплоить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: backend на AWS | Deployed |

### Неделя 92: Cloud (AWS) — часть 2

| День | Тема | Что делать |
|---|---|---|
| Пн | S3: buckets, policies, lifecycle | Настроить |
| Ср | CloudFront: CDN, distributions | Настроить |
| Пт | ElastiCache: Redis managed | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: полный деплой в AWS | Работает |

### Неделя 93: Cloud (AWS) — часть 3 + Secrets + gRPC

| День | Тема | Что делать |
|---|---|---|
| Пн | Vault / AWS Secrets Manager | Понять |
| Ср | Protobuf: schema, code generation + gRPC | Практика |
| Пт | gRPC vs REST: trade-offs | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: gRPC + secrets | Работает |

**Критерий:** могу задеплоить fullstack-приложение в AWS с managed-сервисами и secrets management.

---

## Месяц 19 (недели 94–98): Reactive + Performance + Linux + Load Testing

### Неделя 94: Spring WebFlux (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Reactive Streams, Publisher/Subscriber | Понять |
| Ср | Mono, Flux базово | Практика |
| Пт | WebFlux: контроллеры, роутеры | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: переписать 1 сервис на WebFlux | Реализовать |

### Неделя 95: Spring WebFlux (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | R2DBC: reactive database access | Практика |
| Ср | Backpressure | Понять |
| Пт | Когда WebFlux — плохой выбор | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: WebFlux сервис с R2DBC | Проверить |

**Критерий:** понимаю, когда WebFlux даёт выигрыш.

### Неделя 96: Performance Tuning

| День | Тема | Что делать |
|---|---|---|
| Пн | JVM tuning: heap, GC + JFR + JMC | Практика |
| Ср | Thread dumps, deadlock detection | Практика |
| Пт | Heap dumps, memory leaks + Async profiler | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: оптимизация + HikariCP tuning | Сравнить до/после |

**Критерий:** могу найти CPU/memory bottleneck, настроить connection pool.

### Неделя 97: Linux для production

| День | Тема | Что делать |
|---|---|---|
| Пн | systemd: units, service, enable | Практика |
| Ср | journalctl, logs | Практика |
| Пт | SSH, scp, rsync, права, сети | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: деплой на VPS без Docker | Реализовать |

**Критерий:** могу задеплоить Java-приложение на Linux.

### Неделя 98: Load Testing

| День | Тема | Что делать |
|---|---|---|
| Пн | latency, throughput, RPS, p95/p99 | Понять |
| Ср | k6: сценарии | Настроить |
| Пт | Bottleneck, saturation | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: нагрузочный тест | Найти bottleneck |

**Критерий:** могу провести нагрузочный тест и найти bottleneck.

---

## Месяц 20 (недели 99–103): Advanced Testing + CQRS + System Design + Финал

### Неделя 99: Advanced Testing

| День | Тема | Что делать |
|---|---|---|
| Пн | Contract Testing: Pact | Реализовать |
| Ср | Mutation Testing: PIT | Настроить |
| Пт | Static Analysis: SonarQube | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: contract + mutation тесты | Работает |

### Неделя 100: CQRS + Event Sourcing

| День | Тема | Что делать |
|---|---|---|
| Пн | CQRS: разделение read/write | Понять |
| Ср | Event Sourcing: event store, projections | Разобрать |
| Пт | Применение в Task Manager | Спроектировать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: CQRS для audit log | Реализовать |

**Критерий:** могу объяснить, когда CQRS/ES оправданы.

### Неделя 101: API Design — Versioning + GraphQL + Feature Flags

| День | Тема | Что делать |
|---|---|---|
| Пн | REST API versioning: URI, header, media type | Разобрать |
| Ср | Idempotency в REST: Idempotency-Key | Реализовать |
| Пт | GraphQL: schema, resolvers + Feature Flags | Понять |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: API versioning + feature flags | Реализовать |

### Неделя 102: Distributed Systems + DDIA + System Design

| День | Тема | Что делать |
|---|---|---|
| Пн | CAP, PACELC, consistency models | Понять |
| Ср | Replication, partitioning, consensus | Разобрать |
| Пт | Distributed transactions, 2PC, Saga | Понять |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | DDIA: главы 5–9 | Прочитать |

**Ресурс:** Martin Kleppmann «Designing Data-Intensive Applications».

### Неделя 103: Финальная подготовка + буфер

| День | Тема | Что делать |
|---|---|---|
| Пн | Резюме под Middle Fullstack | Обновить |
| Ср | LinkedIn, GitHub, портфолио + STAR-истории (7–8) | Оформить |
| Пт | Повторение ключевых тем | 50 вопросов |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Mock-интервью Middle | 3 интервью |

**Результат Части 3:** техническая база Middle Fullstack:
- Clean Architecture + DDD (применение)
- Kafka + RabbitMQ
- Микросервисы + Spring Cloud
- Resilience4j + Saga + Outbox
- Advanced Caching (distributed lock, cache stampede)
- Observability (metrics, logs, traces, alerting)
- Kubernetes + Helm + RBAC + Network Policies
- Cloud (AWS): VPC, RDS, ElastiCache, S3, CloudFront, ECS/EKS, IAM, Secrets
- gRPC + Protobuf
- WebFlux + Reactive
- Performance tuning (JFR, JMC, HikariCP)
- Advanced SQL (window functions, CTE, EXPLAIN, оптимизация, MVCC)
- Linux для production
- Load Testing
- Contract Testing (Pact), Mutation Testing (PIT), SonarQube
- CQRS + Event Sourcing
- API Versioning + GraphQL + Feature Flags
- System Design (HLD) глубоко
- Frontend System Design
- Frontend Performance + Observability

---

# Шаблон недели

| День | Время | Что делаешь | Часы |
|---|---|---|---|
| Пн | 21:00–24:00 | Java Core / Backend / Middle-тема | 3 |
| Вт | — | Отдых | — |
| Ср | 21:00–24:00 | Spring / Frontend / Middle-тема | 3 |
| Чт | — | Отдых | — |
| Пт | 21:00–24:00 | Frontend / SQL / Docker / архитектура | 3 |
| Сб | 20:00–22:00 | Алгоритмы | 2 |
| Сб | 22:00–24:00 | System Design | 2 |
| Вс | 12:30–15:00 | Пет-проект | 2.5 |
| Вс | 16:00–19:00 | Пет-проект + тесты | 3 |
| Вс | 19:00–20:00 | System Design: практика | 1 |
| Вс | 21:00–22:30 | Конспекты + mock + повторение | 1.5 |
| Вс | 22:30–24:00 | Свободно | — |
| **Итого (максимум)** | | | **21 ч** |

**Целевая норма — 15–17 ч.** Остальное — резерв.

**Буферные недели** — можно вставить между блоками (например, после 33, 43, 53, 58, 68, 73, 78, 83, 88, 93, 98).

**SQL** — тонким слоем: 15–20 минут в конце занятия, плюс отдельный блок по пятницам. Плюс 3 недели выделенного SQL Deep.

**Git** — минимум 3 осмысленных коммита в Task Manager каждую неделю.

---

# Чек-лист: критерии «могу применить»

## Java Core (Middle)

- [ ] HashMap: устройство, trade-offs vs TreeMap
- [ ] Generics, PECS, type erasure
- [ ] Stream API — когда хуже циклов
- [ ] Concurrency: synchronized, volatile, Atomic, ConcurrentHashMap, JMM, happens-before, deadlock
- [ ] ReentrantLock, ReentrantReadWriteLock, StampedLock, CAS, CompletableFuture, Semaphore, Phaser
- [ ] Virtual Threads (Java 21) — концептуально
- [ ] JVM: heap/stack/metaspace, GC (G1, ZGC), Stop-the-World
- [ ] JFR, JMC, thread dumps, heap dumps

## Spring (Middle)

- [ ] REST API с DTO, validation, exception handling
- [ ] @Transactional: propagation, isolation, rollback
- [ ] N+1: воспроизвести и исправить
- [ ] Spring Security: authentication + authorization
- [ ] OAuth2 / OIDC — flows
- [ ] OpenAPI/Swagger
- [ ] Spring Cloud: Config, Gateway, Discovery
- [ ] Resilience4j: Circuit Breaker, Retry, Bulkhead
- [ ] Spring WebFlux
- [ ] Spring Internals: BeanPostProcessor, AOP, proxies

## SQL (Middle)

- [ ] JOIN, CTE, window functions, рекурсивные CTE
- [ ] EXPLAIN ANALYZE — найти причину
- [ ] Индексы: составные, частичные, covering
- [ ] Partitioning, replication, MVCC internals
- [ ] Транзакции, isolation levels, deadlocks

## Архитектура

- [ ] Clean / Hexagonal Architecture
- [ ] DDD: Entity, Value Object, Aggregate, Bounded Context, Domain Events
- [ ] Layered architecture, dependency direction
- [ ] Microservices vs Monolith — trade-offs
- [ ] Database per Service
- [ ] Saga, Transactional Outbox, idempotency
- [ ] CQRS + Event Sourcing

## Messaging

- [ ] Kafka: topic, partition, consumer group, offset, delivery semantics
- [ ] Kafka: retry, DLT, idempotent producer
- [ ] RabbitMQ: exchange, queue, binding, DLQ
- [ ] Разница между Kafka и RabbitMQ

## Caching

- [ ] cache-aside, TTL, invalidation
- [ ] cache stampede / thundering herd — защита
- [ ] distributed lock (Redis)
- [ ] trade-offs кэширования

## Observability

- [ ] Micrometer, Prometheus, Grafana
- [ ] Structured logging, centralized logging (Loki / ELK)
- [ ] OpenTelemetry: traces, spans, context propagation
- [ ] Alerting, SLI/SLO

## Kubernetes

- [ ] Pod, Deployment, Service, ConfigMap, Secret
- [ ] Probes: liveness, readiness, startup
- [ ] Ingress, HPA
- [ ] Helm, StatefulSet, DaemonSet, RBAC, Network Policies
- [ ] `kubectl get/describe/logs/exec`

## Cloud (AWS)

- [ ] VPC, subnets, security groups, IAM
- [ ] EC2, ECS, EKS basics
- [ ] RDS, ElastiCache
- [ ] S3, CloudFront
- [ ] Secrets Manager / Vault

## Load Testing

- [ ] k6 базово
- [ ] latency, throughput, p95/p99
- [ ] bottleneck analysis

## Advanced Testing

- [ ] Contract Testing (Pact)
- [ ] Mutation Testing (PIT)
- [ ] Static Analysis (SonarQube)

## API Design

- [ ] REST API versioning
- [ ] Idempotency в REST
- [ ] GraphQL basics
- [ ] Feature Flags

## Frontend — HTML/CSS

- [ ] Semantic HTML, accessibility
- [ ] Flexbox, Grid, media queries
- [ ] CSS Architecture: BEM / CSS Modules / Tailwind
- [ ] Design tokens, design system
- [ ] Адаптивная вёрстка по макету

## Frontend — JavaScript

- [ ] Типы, scope, closures
- [ ] Prototypes, this, call/apply/bind
- [ ] Event loop, microtasks/macrotasks, Promises
- [ ] DOM manipulation, events, delegation
- [ ] Fetch API, async/await
- [ ] ES Modules, Vite
- [ ] DevTools: Performance, Network, Memory

## Frontend — TypeScript

- [ ] Типизация без any
- [ ] Generics, utility types, conditional types
- [ ] Type guards, discriminated unions
- [ ] Strict mode
- [ ] Runtime validation (Zod)
- [ ] Типизация API-клиента

## Frontend — React

- [ ] Компоненты, hooks, Context
- [ ] Router (nested, dynamic, protected)
- [ ] Zustand (client state)
- [ ] TanStack Query (server state)
- [ ] React Hook Form + Zod
- [ ] Error Boundaries
- [ ] Suspense + lazy loading
- [ ] Reconciliation, memoization
- [ ] Accessibility
- [ ] React Patterns: compound, render props, HOC, custom hooks

## Frontend — Next.js

- [ ] App Router, Server Components, Client Components
- [ ] Data Fetching: server-side, caching, revalidation
- [ ] Server Actions, Route Handlers
- [ ] Metadata, images, fonts
- [ ] SSR / CSR / ISR trade-offs
- [ ] Middleware / Proxy

## Frontend — Performance

- [ ] Bundle analysis, code splitting, tree shaking
- [ ] Core Web Vitals: LCP, INP, CLS
- [ ] Lazy loading, prefetching, virtualization
- [ ] Lighthouse audit

## Frontend — State

- [ ] Redux Toolkit: slices, createEntityAdapter
- [ ] Normalisation, memoized selectors
- [ ] Zustand vs Redux vs Jotai: trade-offs

## Frontend Testing

- [ ] Vitest: unit
- [ ] React Testing Library: component
- [ ] MSW: мокирование API
- [ ] Playwright: E2E (fixtures, POM)
- [ ] Visual testing, a11y testing
- [ ] Contract testing (Pact)

## Frontend System Design

- [ ] Архитектура SPA: слои, модули, границы
- [ ] Data fetching стратегии, кэширование
- [ ] Code splitting, lazy routes, prefetch
- [ ] Trade-offs: SSR vs CSR vs ISR
- [ ] BFF vs прямые вызовы
- [ ] Offline-first, optimistic UI

## Frontend Observability

- [ ] Sentry: setup, error tracking, source maps
- [ ] Web Vitals: RUM, reporting
- [ ] Session replay

## Design System

- [ ] Storybook: setup, stories, args
- [ ] Radix UI / shadcn
- [ ] Design tokens

## Monorepo

- [ ] Monorepo vs Multirepo
- [ ] Nx / Turborepo: workspaces, shared packages
- [ ] Dependency graph, build caching

## Microfrontends (концептуально)

- [ ] Runtime vs build-time integration
- [ ] Module Federation
- [ ] Когда microfrontends оправданы

## Fullstack Integration

- [ ] OpenAPI-клиент сгенерирован в TypeScript
- [ ] Интеграция через generated client
- [ ] Auth flow: cookies vs localStorage, refresh
- [ ] Security: XSS, CSRF, CORS, CSP
- [ ] Централизованная обработка HTTP-ошибок
- [ ] Nginx: /api → backend, / → frontend
- [ ] WebSocket / SSE realtime

## Advanced Security

- [ ] OAuth2: flows
- [ ] OIDC: ID Token vs Access Token
- [ ] CSP, Trusted Types, security headers
- [ ] Clickjacking, CSRF, XSS

## System Design

- [ ] Requirements, capacity planning
- [ ] Load balancing, caching, CDN
- [ ] URL Shortener / Notification Service / Rate Limiter
- [ ] CAP, PACELC, consistency models
- [ ] Replication, partitioning, consensus
- [ ] Trade-offs: consistency vs availability, latency vs throughput

## Пет-проект (Task Manager Fullstack — Microservices)

- [ ] Monolith → Microservices evolution
- [ ] Clean / Hexagonal Architecture
- [ ] DDD: Aggregates, Bounded Contexts, Domain Events
- [ ] Kafka + RabbitMQ
- [ ] Spring Cloud: Config, Gateway, Discovery
- [ ] Resilience4j: Circuit Breaker, Retry
- [ ] Saga + Outbox
- [ ] Observability: metrics + logs + traces + alerting
- [ ] Kubernetes deployment (Helm)
- [ ] gRPC между сервисами
- [ ] Cloud: Vercel + AWS
- [ ] CI/CD с Docker + K8s
- [ ] Frontend: Next.js, Storybook, Sentry
- [ ] Contract Testing (Pact)
- [ ] Документация: архитектура, диаграммы, ADR

## Собеседования (Middle Fullstack)

- [ ] Резюме с Middle-позиционированием
- [ ] 7–8 STAR-историй
- [ ] 5+ mock-интервью Middle-уровня (Backend + Frontend + System Design)
- [ ] 110–130 задач LeetCode
- [ ] Готовность обсуждать архитектурные решения

---

# Что осталось за пределами плана

Даже после 103 недель для Middle **не хватает:**

1. 2–3 года коммерческого опыта на Java + Frontend.
2. Code review — чтение чужого кода, обратная связь.
3. Участие в архитектурных решениях — выбор технологий, trade-offs.
4. Работа с production — инциденты, on-call, incident response.
5. Менторство Junior — важно для Middle.
6. Понимание бизнес-контекста — приходит только с работой.
7. Коммуникация с заказчиком — опыт.

**Эти вещи нельзя выучить по плану.** Они приходят с работой.

---

# Как использовать этот план

## Стратегия A (рекомендуемая)

1. Пройти Часть 1 (недели 1–33).
2. Начать подаваться на Backend Junior/Junior+ вакансии — не ждать Middle.
3. Получить оффер и работать.
4. Параллельно проходить Часть 2 (недели 34–68) и Часть 3 (недели 69–103).
5. Через 1.5–2 года — подаваться на Middle Fullstack.

**Почему:** быстрее оффер, реальный опыт, Middle приходит с работой.

## Стратегия B

1. Пройти весь план (103 недели) без работы.
2. Подаваться на Middle Fullstack.

**Минусы:** 24 месяца без дохода, риск выгорания, рынок не берёт Middle без опыта.

## Стратегия C (гибрид)

1. Пройти Часть 1 (33 недели).
2. Пройти Часть 2 (35 недель).
3. Подаваться на Fullstack Junior+.
4. Часть 3 — параллельно с работой.

---

# Целевая планка

> Подготовиться к Java Fullstack-вакансиям уровня **Middle** и сформировать техническую базу, соответствующую требованиям рынка.
>
> **Реальный Middle приходит через 2–3 года коммерческого опыта.** План даёт техническую подготовку, но опыт приходит с работой.

---

# Главные правила

1. **Один вечер — одна тема.**
2. **15 минут в конце занятия** — конспект.
3. **Вс — день практики и повторения.**
4. **Пропустил день — не наверстывай в ущерб сну.**
5. **Тема не усвоена — переносится.**
6. **Критерий усвоения — «могу применить».**
7. **Календарь — ориентир, не догма.**
8. **Норма 15–17 ч**, а не 21.
9. **Воскресенье — не второй рабочий день.**
10. **Backend (1–33) → Frontend (34–68) → Middle Extension (69–103).** Не параллельно.
11. **Буферные недели — не «отставание», а часть плана.**
12. **Java/Spring/SQL/Testing → основа. System Design → дополнительный слой.**
13. **Целевая версия Java — 21. Virtual Threads — концептуально.**
14. **Минимум 3 осмысленных коммита в Task Manager каждую неделю.**
15. **Альтернативная стратегия:** после 33 недель (когда backend-часть готова) начать подаваться на Backend Junior+.
16. **Middle нельзя получить только по плану.** Нужен коммерческий опыт 2–3 года.
17. **Deployed URL обязателен.** Без живого приложения портфолио слабее.
18. **Не превращай roadmap в бесконечное редактирование.**

---

# Что делать на этой неделе

1. Составить список тем Java Fundamentals, которых не знаешь. Отметить 10 слабых.
2. Поставить Java 21.
3. Поставить Node.js 22 LTS + pnpm.
4. Поставить IntelliJ IDEA Community + VS Code.
5. Пн–Пт: по одному вечеру на Java Fundamentals + OOP.
6. Сб: Git — branch, merge, конфликты. Заккоммить свои программы.
7. Вс: Maven — создать проект, собрать JAR. SQL: 5 задач на JOIN.
8. Через неделю: проверить, сколько часов реально ушло. Скорректировать темп, а не план.

## Лицензия

Этот проект распространяется под лицензией MIT. 

См. файл [LICENSE](../../../LICENSE) для подробностей.