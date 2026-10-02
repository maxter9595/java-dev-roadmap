# План подготовки: Java Backend Developer (Middle)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](../../../LICENSE)

## Цель

Подготовиться к Java Backend-вакансиям уровня Middle и сформировать техническую базу, соответствующую требованиям рынка.

<img src="../../../assets/images/backend-dev-pepe.png" alt="It's coding time" width="100%">

## Параметры

| Параметр | Значение |
|---|---|
| Длительность | 78 недель (~18 месяцев), календарь — ориентир |
| Норма | 15–17 качественных часов в неделю |
| Максимум | 19–21 час в неделю |
| Java | Java 21 |
| Сборка | Maven + Gradle (базово) |
| Принцип | Календарь — ориентир. Лучше 78 недель с усвоением, чем 70 с пробелами |

**Структура:**
- Часть 1 (недели 1–33): Junior+ база
- Часть 2 (недели 34–78): Middle Extension

**Важно:** Техническая подготовка — необходимое, но недостаточное условие для Middle. Реальный Middle требует 2–3 лет коммерческого опыта, участия в архитектурных решениях и работы с production. Этот план даёт техническую базу, но опыт приходит только с работой.

**Стратегия:**
1. Пройти Часть 1 (33 недели).
2. Начать подаваться на Junior/Junior+ вакансии.
3. Получить оффер и работать.
4. Параллельно проходить Часть 2 (45 недель).
5. Через 1.5–2 года работы — подаваться на Middle.

---

## Что такое Task Management System?

Task Management System — сквозной пет-проект, разрабатывается с недели 12 по 78. Часть 1 — монолит. Часть 2 — эволюция в микросервисную систему.

Аналог Jira / Trello / Asana.

### Эволюция проекта

| Часть | Недели | Что происходит |
|---|---|---|
| Часть 1 | 12–33 | Backend Monolith: Spring Boot + PostgreSQL + JPA + Security + Redis + Docker + SQL deep |
| Часть 2 | 34–78 | Микросервисы: Clean + DDD + Kafka + RabbitMQ + K8s + Cloud + Observability |

### Итоговая архитектура

**Функциональность:**
- Пользователи, регистрация, логин (JWT + OAuth2/OIDC)
- Проекты, задачи (CRUD), статусы, приоритеты, дедлайны
- Комментарии, роли (USER, ADMIN)
- Поиск, фильтрация, сортировка, пагинация
- REST API + OpenAPI/Swagger + GraphQL (опционально)
- Realtime-уведомления через WebSocket
- Event-Driven: Kafka + RabbitMQ
- Микросервисы: User Service, Task Service, Notification Service
- Cloud: AWS (EC2/ECS, RDS, ElastiCache, S3, CloudFront)

**Технический стек:**
- Backend: Java 21 + Spring Boot + Spring Data JPA + Spring Security + Spring Cloud
- БД: PostgreSQL + Flyway + Redis
- Messaging: Kafka + RabbitMQ
- Resilience: Resilience4j
- Observability: Micrometer, Prometheus, Grafana, OpenTelemetry
- Reactive: WebFlux (для отдельных сервисов)
- gRPC: для межсервисного взаимодействия
- Infrastructure: Docker + Compose + Kubernetes (Helm) + Nginx
- CI/CD: GitHub Actions
- Cloud: AWS
- Сборка: Maven + Gradle (базово)
- Тестирование: JUnit 5 + Mockito + Testcontainers + WireMock + Pact + PIT
- Static Analysis: SonarQube
- Load Testing: k6

---

## Реальность рынка Middle

**Технические требования Middle Java Backend (типичные):**
- Java Core глубоко: Collections, Concurrency, JVM, GC
- Spring Boot, JPA, Spring Security уверенно + Spring Internals
- SQL: сложные запросы, EXPLAIN, оптимизация, транзакции, window functions
- Kafka и RabbitMQ
- Микросервисы (или модульный монолит)
- Docker, CI/CD уверенно
- System Design базовый
- Testing на хорошем уровне + contract testing
- Observability (логи, метрики, трассировка)
- Kubernetes — часто требуется, с Helm
- Cloud (AWS/GCP/Azure) — базово
- Load Testing — базово

**Не технические требования Middle:**
- 2–3 года коммерческого опыта
- Опыт code review
- Участие в принятии архитектурных решений
- Работа с production-инцидентами
- Менторство Junior-разработчиков
- Понимание бизнес-контекста

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
- Concurrency: race condition, deadlock, ExecutorService, synchronized, volatile
- Virtual Threads (Java 21) — концептуально
- 25–30 задач LeetCode

### После месяца 3 (HTTP + Spring + Spring Internals)
- HTTP → Controller → DTO → Service → Repository → PostgreSQL
- Validation + Exception Handling
- OpenAPI/Swagger
- Spring Internals: BeanPostProcessor, AOP, proxies
- Spring Boot REST API с CRUD

### После месяца 5 (JPA + Security + Testing)
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

### После месяца 8 (SQL deep + Junior+ база завершена)
- Window functions, рекурсивные CTE, EXPLAIN ANALYZE
- Оптимизация сложных запросов
- CI/CD: GitHub Actions
- Работающий монолитный Task Manager
- 50–60 задач LeetCode
- **Действие: начать подаваться на Junior+**

### После месяца 10 (Clean + DDD + Messaging)
- Clean / Hexagonal Architecture
- DDD: Aggregates, Bounded Contexts, Domain Events
- Kafka: producer, consumer, consumer groups, DLT
- RabbitMQ: exchange, queue, DLQ

### После месяца 12 (Microservices + Resilience + Observability)
- Микросервисы с Database per Service
- Spring Cloud: Config, Gateway, Discovery
- Resilience4j: Circuit Breaker, Retry
- Saga + Outbox
- Observability: метрики, логи, трейсинг
- Redis: distributed lock, cache stampede

### После месяца 14 (K8s + Cloud + gRPC + Reactive)
- K8s: Pod, Deployment, Service, Ingress, probes, HPA
- Helm, StatefulSet, RBAC, Network Policies
- AWS: VPC, RDS, ElastiCache, S3, CloudFront, ECS/EKS
- gRPC + Protobuf
- WebFlux + Reactor

### После месяца 16 (Performance + Advanced SQL + Linux + Load Testing)
- JFR, JMC, profiling
- Partitioning, replication, MVCC
- Linux для production
- k6: p95/p99, bottleneck

### После месяца 18 (System Design + CQRS + Финал)
- System Design HLD: URL Shortener, Chat, Feed
- Distributed systems: CAP, consensus, consistency
- CQRS + Event Sourcing
- GraphQL / API Versioning
- Contract Testing (Pact), Mutation Testing (PIT), SonarQube
- Резюме + mock-интервью для Middle

---

# ЧАСТЬ 1 (недели 1–33): JUNIOR+ БАЗА

Backend — фундамент Middle. Без этой части переход к Middle невозможен.

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

**Мини-проект CLI Task Manager:** пользователи (в памяти), задачи (CRUD), статусы, приоритеты, поиск, фильтрация, Collections + Stream API + Optional, Maven/Gradle + Git.

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

**Результат Части 1:** работающий монолитный Task Manager:
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

**Действие:** начать подаваться на Junior/Junior+ вакансии.

---

# ЧАСТЬ 2 (недели 34–78): MIDDLE EXTENSION

45 недель на темы, отличающие Middle от Junior+.

---

## Месяц 7 (недели 34–38): Clean Architecture + DDD

### Неделя 34: Clean / Hexagonal Architecture (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Clean Architecture, Dependency Rule | Понять принцип |
| Ср | Ports & Adapters (Hexagonal) | Схема |
| Пт | Domain / Application / Infrastructure / Presentation | Разделение слоёв |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: рефакторинг под Clean | Первые шаги |

**Ресурс:** Robert C. Martin «Clean Architecture» (гл. 1–10).

### Неделя 35: Clean / Hexagonal Architecture (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Use Cases / Interactors | Реализовать |
| Ср | Repository как абстракция, Adapters | Разделить JPA и domain |
| Пт | Dependency Inversion в коде | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: завершить рефакторинг Clean | Проверить |

**Критерий:** domain не зависит от Spring/JPA.

### Неделя 36: DDD (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Ubiquitous Language | Словарь Task Manager |
| Ср | Entity, Value Object | Реализовать |
| Пт | Aggregate, Aggregate Root | Спроектировать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: применить DDD | Рефакторинг |

**Ресурс:** Eric Evans «Domain-Driven Design» (гл. 1–7).

### Неделя 37: DDD (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Bounded Context, Context Map | Границы контекстов |
| Ср | Domain Service, Application Service | Разделить |
| Пт | Domain Events | Реализовать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: DDD завершено | Проверить |

**Ресурс:** Vaughn Vernon «Implementing Domain-Driven Design».

### Неделя 38: DDD (часть 3) — применение

| День | Тема | Что делать |
|---|---|---|
| Пн | Рефакторинг агрегатов: инварианты | Практика |
| Ср | Repository per aggregate | Разделить |
| Пт | Anti-corruption layer | Понять |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: финальный DDD-рефакторинг | Проверить |

**Критерий:** могу объяснить, где границы агрегатов и почему.

---

## Месяц 8 (недели 39–43): Kafka + RabbitMQ

### Неделя 39: Kafka (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Kafka: broker, topic, partition | Понять архитектуру |
| Ср | Producer, consumer, offset, consumer group | Практика |
| Пт | Delivery semantics: at-most-once, at-least-once, exactly-once | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: первый Kafka-топик | Events для задач |

**Ресурс:** «Kafka: The Definitive Guide».

### Неделя 40: Kafka (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Idempotent producer, transactions | Практика |
| Ср | Ordering, partitioning strategies | Разобрать |
| Пт | Kafka + Spring Boot: @KafkaListener | Интеграция |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Kafka consumer для событий | Интеграция |

### Неделя 41: Kafka (часть 3) — продвинутое

| День | Тема | Что делать |
|---|---|---|
| Пн | Retry, DLT (Dead Letter Topic) | Реализовать |
| Ср | Consumer lag, мониторинг | Настроить |
| Пт | Kafka Streams / KSQL — концептуально | Понимать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: DLT + retry | Работает |

**Критерий:** событие публикуется и обрабатывается, DLT работает.

### Неделя 42: RabbitMQ (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | RabbitMQ: exchange, queue, binding, routing key | Понять |
| Ср | Direct, Topic, Fanout | Практика |
| Пт | AMQP, message format | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: RabbitMQ для notification | Практика |

### Неделя 43: RabbitMQ (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Manual ACK / NACK | Практика |
| Ср | Prefetch, concurrency | Настроить |
| Пт | Retry, Dead Letter Exchange / Queue | Реализовать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: DLQ + retry | Проверить |

**Критерий:** понимаю разницу Kafka vs RabbitMQ, могу выбрать под задачу.

---

## Месяц 9 (недели 44–48): Микросервисы + Spring Cloud

### Неделя 44: Микросервисы (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Monolith vs Microservices: trade-offs | Понять |
| Ср | Границы сервисов (Bounded Context) | Определить |
| Пт | Database per Service | Спроектировать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: выделить User Service | Разделить монолит |

**Ресурс:** Sam Newman «Building Microservices» (гл. 1–4).

### Неделя 45: Микросервисы (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Синхронное (REST) vs асинхронное (Kafka) | Разобрать |
| Ср | API composition, BFF | Понять |
| Пт | Service discovery | Понять проблему |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: выделить Task Service | Разделить |

**Критерий:** 2–3 сервиса работают независимо, общаются через REST/Kafka.

### Неделя 46: Spring Cloud (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Spring Cloud Config | Centralized configuration |
| Ср | Eureka / Consul: service discovery | Реализовать |
| Пт | Spring Cloud Gateway | API Gateway |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Config + Gateway | Интеграция |

### Неделя 47: Spring Cloud (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Load balancing (Spring Cloud LoadBalancer) | Настроить |
| Ср | Distributed tracing (Micrometer Tracing) | Настроить |
| Пт | Spring Cloud Stream | Опционально |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Full Spring Cloud stack | Работает |

**Критерий:** 3 сервиса общаются через Gateway, Config централизован.

### Неделя 48: Review / Buffer (Messaging + Microservices)

| День | Тема | Что делать |
|---|---|---|
| Пн | Повторение Kafka | 15 вопросов |
| Ср | Повторение RabbitMQ | 15 вопросов |
| Пт | Повторение Spring Cloud | 10 вопросов |
| Сб | Пет-проект: закрыть пробелы | Рефакторинг |
| Вс | Итог: 3 сервиса работают | Контрольная точка |

---

## Месяц 10 (недели 49–53): Resilience + Saga + Caching + Observability

### Неделя 49: Resilience4j

| День | Тема | Что делать |
|---|---|---|
| Пн | Circuit Breaker: состояния, failure rate | Реализовать |
| Ср | Retry + exponential backoff | Настроить |
| Пт | Bulkhead, Rate Limiter, TimeLimiter | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Circuit Breaker на вызовах | Работает |

**Ресурс:** документация Resilience4j.

### Неделя 50: Saga + Transactional Outbox

| День | Тема | Что делать |
|---|---|---|
| Пн | Проблема distributed transaction | Понять |
| Ср | Saga: choreography vs orchestration | Разобрать |
| Пт | Transactional Outbox Pattern | Реализовать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: Saga для заказа задач | Практика |

**Критерий:** могу объяснить, почему distributed transaction — проблема и как её решает Saga.

### Неделя 51: Redis глубоко — Caching strategies

| День | Тема | Что делать |
|---|---|---|
| Пн | Cache stampede / thundering herd | Защита |
| Ср | Distributed lock на Redis | Реализовать (Redlock / SETNX) |
| Пт | Invalidation strategies: TTL vs explicit | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: distributed lock | Работает |

**Критерий:** могу спроектировать кэширование для high-load.

### Неделя 52: Observability (часть 1) — Metrics

| День | Тема | Что делать |
|---|---|---|
| Пн | Micrometer, метрики | Настроить |
| Ср | Prometheus: scrape, PromQL | Поднять |
| Пт | Grafana: dashboard | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: metrics + dashboard | Работает |

### Неделя 53: Observability (часть 2) — Logs + Traces

| День | Тема | Что делать |
|---|---|---|
| Пн | Structured logging (JSON) | Настроить |
| Ср | Centralized logging: Loki / ELK | Поднять |
| Пт | OpenTelemetry: traces, spans, context propagation | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: логи + трейсы | Работает |

**Критерий:** могу найти проблему по logs / metrics / traces.

---

## Месяц 11 (недели 54–58): Kubernetes + Cloud (AWS)

### Неделя 54: Kubernetes (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | K8s: cluster, node, control plane | Понять |
| Ср | Pod, ReplicaSet, Deployment | Практика |
| Пт | Service: ClusterIP, NodePort, LoadBalancer | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: 1 сервис в K8s | minikube / kind |

**Ресурс:** «Kubernetes: Up and Running».

### Неделя 55: Kubernetes (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | ConfigMap, Secret | Практика |
| Ср | Liveness / Readiness / Startup probes | Настроить |
| Пт | Ingress + Ingress Controller | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: часть сервисов в K8s | Работает |

### Неделя 56: Kubernetes (часть 3) — продвинутое

| День | Тема | Что делать |
|---|---|---|
| Пн | Helm: charts, values, templates | Настроить |
| Ср | StatefulSet, DaemonSet, Job/CronJob | Практика |
| Пт | RBAC, ServiceAccount, Network Policies | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: весь стек в K8s через Helm | Работает |

### Неделя 57: Kubernetes (часть 4) — диагностика + HPA

| День | Тема | Что делать |
|---|---|---|
| Пн | Resource requests/limits, QoS | Настроить |
| Ср | HorizontalPodAutoscaler (HPA) | Настроить |
| Пт | kubectl: get, describe, logs, exec, port-forward | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: HPA + диагностика | Работает |

**Критерий:** могу развернуть микросервисы в K8s с Helm, probes, RBAC, HPA.

### Неделя 58: Cloud (AWS) — часть 1

| День | Тема | Что делать |
|---|---|---|
| Пн | AWS: VPC, subnets, security groups, IAM | Понять |
| Ср | EC2, ECS, EKS basics | Разобрать |
| Пт | RDS: managed PostgreSQL | Задеплоить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: backend на AWS | Deployed |

---

## Месяц 12 (недели 59–63): Cloud + gRPC + Reactive + Performance

### Неделя 59: Cloud (AWS) — часть 2

| День | Тема | Что делать |
|---|---|---|
| Пн | S3: buckets, policies, lifecycle | Настроить |
| Ср | CloudFront: CDN, distributions | Настроить |
| Пт | ElastiCache: Redis managed | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: полный деплой в AWS | Работает |

### Неделя 60: Cloud (AWS) — часть 3 + Secrets

| День | Тема | Что делать |
|---|---|---|
| Пн | Vault / AWS Secrets Manager | Понять |
| Ср | Безопасность в AWS: security groups, IAM roles | Настроить |
| Пт | Cost optimization basics | Понять |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: secrets management | Реализовать |

**Критерий:** могу задеплоить fullstack-приложение в AWS с managed-сервисами.

### Неделя 61: gRPC + Protobuf

| День | Тема | Что делать |
|---|---|---|
| Пн | Protobuf: schema, code generation | Понять |
| Ср | gRPC: unary, streaming | Практика |
| Пт | gRPC vs REST: trade-offs | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: gRPC между двумя сервисами | Работает |

### Неделя 62: Spring WebFlux (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Reactive Streams, Publisher/Subscriber | Понять |
| Ср | Mono, Flux базово | Практика |
| Пт | WebFlux: контроллеры, роутеры | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: переписать 1 сервис на WebFlux | Реализовать |

### Неделя 63: Spring WebFlux (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | R2DBC: reactive database access | Практика |
| Ср | Backpressure | Понять |
| Пт | Когда WebFlux — плохой выбор | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: WebFlux сервис с R2DBC | Проверить |

**Критерий:** понимаю, когда WebFlux даёт выигрыш.

---

## Месяц 13 (недели 64–68): Advanced Security + Performance + Linux + Load Testing

### Неделя 64: Advanced Security (OAuth2 / OIDC)

| День | Тема | Что делать |
|---|---|---|
| Пн | OAuth2: роли, flows | Разобрать |
| Ср | OIDC: ID Token vs Access Token | Понять |
| Пт | Keycloak или Auth0: интеграция | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: OAuth2 вместо ручного JWT | Реализовать |

**Критерий:** понимаю разницу OAuth2 vs OIDC.

### Неделя 65: Performance Tuning (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | JVM tuning: heap, GC | Практика |
| Ср | JFR (Java Flight Recorder) | Запись событий |
| Пт | JMC (Java Mission Control) | Анализ |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: профилирование | Найти bottleneck |

**Ресурс:** Scott Oaks «Java Performance».

### Неделя 66: Performance Tuning (часть 2) + HikariCP

| День | Тема | Что делать |
|---|---|---|
| Пн | Thread dumps, deadlock detection | Практика |
| Ср | Heap dumps, memory leaks | Анализ |
| Пт | Async profiler / YourKit / VisualVM | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: оптимизация + HikariCP tuning | Сравнить до/после |

**Критерий:** могу найти CPU/memory bottleneck, настроить connection pool.

### Неделя 67: Linux для production

| День | Тема | Что делать |
|---|---|---|
| Пн | systemd: units, service, enable | Практика |
| Ср | journalctl, logs | Практика |
| Пт | SSH, scp, rsync, права, сети | Практика |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: деплой на VPS без Docker | Реализовать |

**Критерий:** могу задеплоить Java-приложение на Linux.

### Неделя 68: Load Testing

| День | Тема | Что делать |
|---|---|---|
| Пн | latency, throughput, RPS, p95/p99 | Понять |
| Ср | k6: сценарии | Настроить |
| Пт | Bottleneck, saturation | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: нагрузочный тест | Найти bottleneck |

**Критерий:** могу провести нагрузочный тест и найти bottleneck.

---

## Месяц 14 (недели 69–73): Advanced Testing + CQRS + API Design

### Неделя 69: Advanced Testing

| День | Тема | Что делать |
|---|---|---|
| Пн | Contract Testing: Pact | Реализовать |
| Ср | Mutation Testing: PIT | Настроить |
| Пт | Static Analysis: SonarQube | Настроить |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: contract + mutation тесты | Работает |

### Неделя 70: CQRS + Event Sourcing

| День | Тема | Что делать |
|---|---|---|
| Пн | CQRS: разделение read/write | Понять |
| Ср | Event Sourcing: event store, projections | Разобрать |
| Пт | Применение в Task Manager | Спроектировать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: CQRS для audit log | Реализовать |

**Критерий:** могу объяснить, когда CQRS/ES оправданы.

### Неделя 71: API Design — Versioning + GraphQL

| День | Тема | Что делать |
|---|---|---|
| Пн | REST API versioning: URI, header, media type | Разобрать |
| Ср | Idempotency в REST: Idempotency-Key | Реализовать |
| Пт | GraphQL: schema, resolvers, сравнение с REST | Понять |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: API versioning | Реализовать |

### Неделя 72: Feature Flags + Zero-downtime Deployment

| День | Тема | Что делать |
|---|---|---|
| Пн | Feature Flags: LaunchDarkly / Unleash | Понять |
| Ср | Blue-green deployment | Разобрать |
| Пт | Canary deployment | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: feature flags | Реализовать |

### Неделя 73: Distributed Systems + DDIA

| День | Тема | Что делать |
|---|---|---|
| Пн | CAP, PACELC, consistency models | Понять |
| Ср | Replication, partitioning, consensus | Разобрать |
| Пт | Distributed transactions, 2PC, Saga | Понять |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | DDIA: главы 5–9 | Прочитать |

**Ресурс:** Martin Kleppmann «Designing Data-Intensive Applications».

---

## Месяц 15 (недели 74–78): System Design + Финал

### Неделя 74: System Design (часть 1)

| День | Тема | Что делать |
|---|---|---|
| Пн | Requirements, capacity planning | URL Shortener |
| Ср | API design, data model | Практика |
| Пт | Cache, DB, LB | Разобрать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Пет-проект: схема микросервисов | Диаграмма |

**Ресурс:** Alex Xu Vol. 1, главы 1–7.

### Неделя 75: System Design (часть 2)

| День | Тема | Что делать |
|---|---|---|
| Пн | Notification Service: полный разбор | Разбор |
| Ср | Rate Limiter: полный разбор | Разбор |
| Пт | Chat / Feed: полный разбор | Разбор |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Mock System Design | С ИИ |

### Неделя 76: Interview Prep — Backend

| День | Тема | Что делать |
|---|---|---|
| Пн | Java Core: 50 вопросов | Повторение |
| Ср | Spring + JPA + Internals: 40 вопросов | Повторение |
| Пт | SQL + Kafka + RabbitMQ + Microservices | Повторение |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Mock Backend Interview | С ИИ |

### Неделя 77: Interview Prep — System Design + Behavioral

| День | Тема | Что делать |
|---|---|---|
| Пн | System Design: 3 задачи | Полный разбор |
| Ср | Distributed Systems: 20 вопросов | Повторение |
| Пт | Behavioral: 7–8 STAR-историй | Написать |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Mock System Design + Behavioral | 2 интервью |

### Неделя 78: Финальная подготовка + буфер

| День | Тема | Что делать |
|---|---|---|
| Пн | Резюме под Middle | Обновить |
| Ср | LinkedIn, GitHub, портфолио | Оформить |
| Пт | Повторение ключевых тем | 50 вопросов |
| Сб | LeetCode: 2 задачи + System Design (1.5 ч) | Практика |
| Вс | Mock-интервью Middle | 3 интервью |

**Результат Части 2:** техническая база Middle:
- Clean Architecture + DDD (применение)
- Kafka + RabbitMQ
- Микросервисы + Spring Cloud
- Resilience4j + Saga + Outbox
- Advanced Caching (distributed lock, cache stampede)
- Observability (metrics, logs, traces)
- Kubernetes + Helm + RBAC + Network Policies
- Cloud (AWS): VPC, RDS, ElastiCache, S3, CloudFront, ECS/EKS
- gRPC + Protobuf
- WebFlux + Reactive
- Performance tuning (JFR, JMC, HikariCP)
- Advanced SQL (window functions, CTE, EXPLAIN, оптимизация, MVCC)
- Linux для production
- Load Testing
- Contract Testing (Pact), Mutation Testing (PIT), SonarQube
- CQRS + Event Sourcing
- API Versioning + GraphQL basics
- Feature Flags + Zero-downtime deployment
- System Design (HLD) глубоко

---

# Шаблон недели

| День | Время | Что делаешь | Часы |
|---|---|---|---|
| Пн | 21:00–24:00 | Java Core / Spring / Middle-тема | 3 |
| Вт | — | Отдых | — |
| Ср | 21:00–24:00 | Spring / Middle-тема | 3 |
| Чт | — | Отдых | — |
| Пт | 21:00–24:00 | SQL / Docker / архитектура | 3 |
| Сб | 20:00–22:00 | Алгоритмы | 2 |
| Сб | 22:00–24:00 | System Design | 2 |
| Вс | 12:30–15:00 | Пет-проект | 2.5 |
| Вс | 16:00–19:00 | Пет-проект + тесты | 3 |
| Вс | 19:00–20:00 | System Design: практика | 1 |
| Вс | 21:00–22:30 | Конспекты + mock + повторение | 1.5 |
| Вс | 22:30–24:00 | Свободно | — |
| **Итого (максимум)** | | | **21 ч** |

**Целевая норма — 15–17 ч.** Остальное — резерв.

**Буферные недели** — можно вставить между блоками (например, после 38, 43, 48, 53, 58, 63, 68, 73).

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
- [ ] Actuator, health checks, liveness/readiness

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
- [ ] Zero-downtime deployment

## System Design

- [ ] Requirements, capacity planning
- [ ] Load balancing, caching, CDN
- [ ] URL Shortener / Notification Service / Rate Limiter
- [ ] CAP, PACELC, consistency models
- [ ] Replication, partitioning, consensus
- [ ] Trade-offs: consistency vs availability, latency vs throughput

## Пет-проект (Task Manager — Microservices)

- [ ] Monolith → Microservices evolution
- [ ] Clean / Hexagonal Architecture
- [ ] DDD: Aggregates, Bounded Contexts, Domain Events
- [ ] Kafka + RabbitMQ
- [ ] Spring Cloud: Config, Gateway, Discovery
- [ ] Resilience4j: Circuit Breaker, Retry
- [ ] Saga + Outbox
- [ ] Observability: metrics + logs + traces
- [ ] Kubernetes deployment (Helm)
- [ ] gRPC между сервисами
- [ ] Cloud: AWS
- [ ] CI/CD с Docker + K8s
- [ ] Contract Testing (Pact)
- [ ] Документация: архитектура, диаграммы, ADR

## Собеседования (Middle)

- [ ] Резюме с Middle-позиционированием
- [ ] 7–8 STAR-историй
- [ ] 5+ mock-интервью Middle-уровня
- [ ] 100–120 задач LeetCode
- [ ] Готовность обсуждать архитектурные решения

---

# Что осталось за пределами плана

Даже после 78 недель для Middle **не хватает:**

1. 2–3 года коммерческого опыта на Java.
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
2. Начать подаваться на Junior/Junior+ вакансии — не ждать Middle.
3. Получить оффер и работать.
4. Параллельно проходить Часть 2 (недели 34–78).
5. Через 1.5–2 года — подаваться на Middle.

**Почему:** быстрее оффер, реальный опыт, Middle приходит с работой.

## Стратегия B

1. Пройти весь план (78 недель) без работы.
2. Подаваться на Middle.

**Минусы:** 18 месяцев без дохода, риск выгорания, рынок не берёт Middle без опыта.

## Стратегия C (гибрид)

1. Пройти Часть 1 (33 недели).
2. Пройти Часть 2 до недели 53 (Clean, DDD, Kafka, RabbitMQ, Microservices, Resilience, Saga, Redis глубоко, Observability).
3. Подаваться на Middle- / Junior+.
4. Остальное (K8s, Cloud, gRPC, WebFlux, Performance, SQL deep, Linux, Load Testing, DDIA, Advanced Testing, CQRS) — параллельно с работой.

---

# Целевая планка

> Подготовиться к Java Backend-вакансиям уровня **Middle** и сформировать техническую базу, соответствующую требованиям рынка.
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
10. **Часть 1 (1–33) → Junior+ оффер → Часть 2 (34–78).** Не ждать Middle для подачи.
11. **Буферные недели — не «отставание», а часть плана.**
12. **Java/Spring/SQL/Testing → основа. System Design → дополнительный слой.**
13. **Целевая версия Java — 21. Virtual Threads — концептуально.**
14. **Минимум 3 осмысленных коммита в Task Manager каждую неделю.**
15. **Middle нельзя получить только по плану.** Нужен коммерческий опыт 2–3 года.
16. **Не превращай roadmap в бесконечное редактирование.**

---

# Что делать на этой неделе

1. Составить список тем Java Fundamentals, которых не знаешь. Отметить 10 самых слабых.
2. Поставить Java 21.
3. Поставить IntelliJ IDEA Community или VS Code + Extension Pack for Java.
4. Пн–Пт: по одному вечеру на Java Fundamentals + OOP.
5. Сб: Git — branch, merge, конфликты. Закоммить свои программы.
6. Вс: Maven — создать проект, собрать JAR. SQL: 5 задач на JOIN.
7. Через неделю: проверить, сколько часов реально ушло. Скорректировать темп, а не план.

## Лицензия

Этот проект распространяется под лицензией MIT. 

См. файл [LICENSE](../../../LICENSE) для подробностей.