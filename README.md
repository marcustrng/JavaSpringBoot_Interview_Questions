# Java Software Engineer Interview Topics

### Table of Contents

<details open>
<summary>Hide/Show Table of Contents</summary>

| No. | Section & Topics                                                                                          |
| ----|----------------------------------------------------------------------------------------------------------|
|      | **Java Core (Java 8+)**                                                                                   |
| 1    | [Java 8–17 features: Lambda, Streams, Optional, Records, Sealed Classes](#java-features)                  |
| 2    | [Functional Interfaces and Method References](#functional-interfaces)                                     |
| 3    | [Stream API and Collector Operations](#stream-api)                                                       |
| 4    | [Collections Framework and Concurrency Utilities](#collections-framework)                                 |
| 5    | [JVM Internals: Memory Model, Garbage Collection, Class Loading](#jvm-internals)                          |
| 6    | [Generics, Annotations, and Reflection](#generics-annotations-reflection)                                |
| 7    | [Exception Handling and Best Practices](#exception-handling)                                             |
| 8    | [Immutability and Performance Tuning](#immutability-performance)                                         |
|      | **Object-Oriented Programming (OOP)**                                                                     |
| 9    | [OOP Principles: Abstraction, Encapsulation, Inheritance, Polymorphism](#oop-principles)                  |
| 10   | [SOLID Principles](#solid-principles)                                                                     |
| 11   | [Composition vs Inheritance](#composition-vs-inheritance)                                                 |
| 12   | [Domain-Driven Design (DDD): Entities, Value Objects, Aggregates](#ddd)                                  |
|      | **Spring JPA (Hibernate)**                                                                                |
| 13   | [JPA Entity Mapping, Lifecycle, and Annotations](#jpa-entity-mapping)                                    |
| 14   | [Entity Relationships: OneToMany, ManyToOne, ManyToMany, OneToOne](#entity-relationships)                 |
| 15   | [JPQL, Native Queries, and Criteria API](#jpql-native-queries)                                           |
| 16   | [Transaction Management and Propagation](#transaction-management)                                        |
| 17   | [Lazy vs Eager Loading, N+1 Problem, Fetch Joins](#lazy-vs-eager)                                        |
| 18   | [Auditing, Soft Deletes, Optimistic/Pessimistic Locking](#auditing-soft-deletes)                          |
|      | **Spring Security**                                                                                        |
| 19   | [Spring Security Architecture and Filter Chain](#security-architecture)                                  |
| 20   | [Authentication, Authorization, and Roles](#auth-authorization)                                         |
| 21   | [JWT-Based Stateless Authentication](#jwt-authentication)                                               |
| 22   | [Method-Level Security, RBAC, and Custom Annotations](#method-security)                                  |
| 23   | [OAuth2 and OpenID Connect Integration](#oauth2-openid)                                                 |
| 24   | [CSRF Protection, CORS, and Session Management](#csrf-cors-session)                                     |
|      | **Spring Boot**                                                                                            |
| 25   | [Auto-Configuration and Conditional Beans](#auto-configuration)                                         |
| 26   | [Application Configuration (YAML/Properties) and Profile Management](#app-configuration)                 |
| 27   | [Spring Boot Actuator for Health Checks and Metrics](#actuator)                                         |
| 28   | [Externalized Configuration and Secret Management](#external-config)                                    |
| 29   | [Embedded Tomcat/Jetty/Undertow and Deployment Packaging](#embedded-containers)                          |
|      | **SQL Database**                                                                                           |
| 30   | [SQL Syntax and Query Building Basics](#sql-basics)                                                     |
| 31   | [Joins, Indexing, Query Planning, and Optimization](#joins-indexing)                                    |
| 32   | [ACID Properties and Isolation Levels](#acid-isolation)                                                |
| 33   | [Database Migrations with Liquibase or Flyway](#db-migrations)                                          |
| 34   | [Data Modeling and Normalization](#data-modeling)                                                      |
|      | **RESTful API Design**                                                                                     |
| 35   | [REST Principles and Resource Modeling](#rest-principles)                                              |
| 36   | [HTTP Methods, Status Codes, Headers, and Idempotency](#http-basics)                                    |
| 37   | [Exception Handling and Validation](#api-exception-handling)                                           |
| 38   | [API Versioning and HATEOAS](#api-versioning-hateoas)                                                  |
| 39   | [Pagination, Sorting, and Filtering](#pagination-sorting)                                              |
|      | **Microservices**                                                                                          |
| 40   | [Microservice Architecture and Decomposition Strategies](#microservice-architecture)                   |
| 41   | [Service Discovery and API Gateway](#service-discovery)                                                |
| 42   | [Synchronous (REST, gRPC) vs Asynchronous Communication](#sync-vs-async)                               |
| 43   | [Event-Driven Architecture and Message Brokers](#event-driven)                                        |
| 44   | [Kafka Fundamentals: Producers, Consumers, Brokers, Partitions, Topics](#kafka-fundamentals)           |
| 45   | [Kafka Delivery Semantics and Stream Processing](#kafka-delivery)                                     |
| 46   | [Kafka Schema Registry, Avro, and Spring Integration](#kafka-schema-avro)                              |
| 47   | [Circuit Breakers, Retries, and Rate Limiting (Resilience4j)](#resilience4j)                           |
| 48   | [Spring Cloud Config and Centralized Logging](#spring-cloud-config)                                   |
|      | **CI/CD & Docker**                                                                                         |
| 49   | [CI/CD Pipelines: Jenkins, GitHub Actions, GitLab CI](#ci-cd-pipelines)                               |
| 50   | [Docker Fundamentals: Images, Containers, Dockerfile](#docker-fundamentals)                            |
| 51   | [Docker Compose and Multi-Container Apps](#docker-compose)                                            |
| 52   | [Deployment Strategies: Blue/Green, Rolling, Canary](#deployment-strategies)                          |
| 53   | [Artifact Versioning and Environment Promotion](#artifact-versioning)                                 |
|      | **Testing & Quality Assurance**                                                                            |
| 54   | [Unit Testing with JUnit and Mockito](#unit-testing)                                                  |
| 55   | [Integration Testing with Spring Boot](#integration-testing)                                         |
| 56   | [Test Slicing and Testcontainers](#test-slicing)                                                     |
| 57   | [Contract Testing and CI Testing Strategies](#contract-testing)                                       |
| 58   | [Static Analysis: SonarQube, JaCoCo, SpotBugs](#static-analysis)                                      |
|      | **Architecture & System Design**                                                                           |
| 59   | [Scalability, Availability, Fault Tolerance](#scalability-availability)                              |
| 60   | [CAP Theorem and Consistency Models](#cap-theorem)                                                   |
| 61   | [Caching: In-Memory, Redis, Caffeine](#caching)                                                     |
| 62   | [Redis: Data Types, TTL, Pub/Sub, Locks, Rate Limiting](#redis)                                      |
| 63   | [Design Patterns: CQRS, Saga, Event Sourcing](#design-patterns)                                      |
| 64   | [Load Balancing, Partitioning, Replication](#load-balancing)                                        |
| 65   | [API Security and Token Management](#api-security)                                                  |
|      | **Clean Code & Design Patterns**                                                                            |
| 66   | [Clean Code Principles and Refactoring Techniques](#clean-code)                                     |
| 67   | [Creational Patterns: Singleton, Factory, Builder, Prototype](#creational-patterns)                  |
| 68   | [Structural Patterns: Adapter, Decorator, Proxy, Facade](#structural-patterns)                       |
| 69   | [Behavioral Patterns: Strategy, Observer, Chain of Responsibility](#behavioral-patterns)             |
| 70   | [Clean Architecture, Hexagonal, Onion](#clean-architecture)                                         |
|      | **Agile & Scrum**                                                                                           |
| 71   | [Agile Manifesto and Scrum Roles](#agile-manifesto)                                                 |
| 72   | [Scrum Ceremonies and User Stories](#scrum-ceremonies)                                              |
| 73   | [Story Points, Velocity, and Metrics](#story-points)                                                |
| 74   | [Agile Tools: Jira, Trello, ClickUp](#agile-tools)                                                  |

</details>

## **Java Core (Java 8+)**   

<a name="java-features"></a>  
### 1. **Java 8+ Features: Lambda, Streams, Optional, Records, Sealed Classes**  

**[⬆ Back to Top](#table-of-contents)**

<a name="functional-interfaces"></a>  
### 2. **Functional Interfaces and Method References**  

**[⬆ Back to Top](#table-of-contents)**

<a name="stream-api-collector-operations"></a>  
### 3. **Stream API and Collector Operations**  

**[⬆ Back to Top](#table-of-contents)**

<a name="collections-concurrency"></a>  
### 4. **Collections Framework and Concurrency Utilities**  

**[⬆ Back to Top](#table-of-contents)**

<a name="jvm-internals"></a>  
### 5. **JVM Internals: Memory Model, Garbage Collection, Class Loading**  

**[⬆ Back to Top](#table-of-contents)**

<a name="generics-annotations-reflection"></a>  
### 6. **Generics, Annotations, and Reflection**  

**[⬆ Back to Top](#table-of-contents)**

<a name="exception-handling"></a>  
### 7. **Exception Handling and Best Practices**  

**[⬆ Back to Top](#table-of-contents)**

<a name="immutability-performance-tuning"></a>  
### 8. **Immutability and Performance Tuning**  

**[⬆ Back to Top](#table-of-contents)**


## **Object-Oriented Programming (OOP)**  

<a name="oop-principles"></a>  
### 9. **OOP Principles: Abstraction, Encapsulation, Inheritance, Polymorphism**  

**[⬆ Back to Top](#table-of-contents)**

<a name="solid-principles"></a>  
### 10. **SOLID Principles**  

**[⬆ Back to Top](#table-of-contents)**

<a name="composition-vs-inheritance"></a>  
### 11. **Composition vs Inheritance**  

**[⬆ Back to Top](#table-of-contents)**

<a name="ddd-entities-value-objects-aggregates"></a>  
### 12. **Domain-Driven Design (DDD): Entities, Value Objects, Aggregates**  

**[⬆ Back to Top](#table-of-contents)**


## **Spring JPA (Hibernate)**  
<a name="jpa-entity-mapping"></a>  
<a name="jpa-entity-mapping"></a>  
### 13. **JPA Entity Mapping, Lifecycle, and Annotations**  

**[⬆ Back to Top](#table-of-contents)**

<a name="entity-relationships"></a>  
### 14. **Entity Relationships: OneToMany, ManyToOne, ManyToMany, OneToOne**  

**[⬆ Back to Top](#table-of-contents)**

<a name="jpql-native-criteria-api"></a>  
### 15. **JPQL, Native Queries, and Criteria API**  

**[⬆ Back to Top](#table-of-contents)**

<a name="transaction-management"></a>  
### 16. **Transaction Management and Propagation**  

**[⬆ Back to Top](#table-of-contents)**

<a name="lazy-eager-loading-nplus1"></a>  
### 17. **Lazy vs Eager Loading, N+1 Problem, Fetch Joins**  

**[⬆ Back to Top](#table-of-contents)**

<a name="auditing-soft-deletes-locking"></a>  
### 18. **Auditing, Soft Deletes, Optimistic/Pessimistic Locking**  

**[⬆ Back to Top](#table-of-contents)**


## **Spring Security**  

<a name="spring-security-architecture"></a>  
### 19. **Spring Security Architecture and Filter Chain**  

**[⬆ Back to Top](#table-of-contents)**

<a name="authentication-authorization-roles"></a>  
### 20. **Authentication, Authorization, and Roles**  

**[⬆ Back to Top](#table-of-contents)**

<a name="jwt-stateless-authentication"></a>  
### 21. **JWT-based Stateless Authentication**  

**[⬆ Back to Top](#table-of-contents)**

<a name="method-level-security-rbac"></a>  
### 22. **Method-level Security, RBAC, and Custom Annotations**  

**[⬆ Back to Top](#table-of-contents)**

<a name="oauth2-openid-connect"></a>  
### 23. **OAuth2 and OpenID Connect Integration**  

**[⬆ Back to Top](#table-of-contents)**

<a name="csrf-cors-session-management"></a>  
### 24. **CSRF Protection, CORS, and Session Management**  

**[⬆ Back to Top](#table-of-contents)**


## **Spring Boot**  
<a name="spring-boot-auto-configuration"></a>  
### 25. **Auto-configuration and Conditional Beans**  

**[⬆ Back to Top](#table-of-contents)**

<a name="application-configuration-profile-management"></a>  
### 26. **Application Configuration (YAML/Properties) and Profile Management**  

**[⬆ Back to Top](#table-of-contents)**

<a name="spring-boot-actuator"></a>  
### 27. **Spring Boot Actuator for Health Checks and Metrics**  

**[⬆ Back to Top](#table-of-contents)**

<a name="externalized-configuration-secret-management"></a>  
### 28. **Externalized Configuration and Secret Management**  

**[⬆ Back to Top](#table-of-contents)**

<a name="embedded-servers-deployment"></a>  
### 29. **Embedded Tomcat/Jetty/Undertow and Deployment Packaging**  


## **SQL Database**  

<a name="sql-syntax-query-basics"></a>  
### 30. **SQL Syntax and Query Building Basics**  

**[⬆ Back to Top](#table-of-contents)**

<a name="joins-indexing-query-optimization"></a>  
### 31. **Joins, Indexing, Query Planning and Optimization**  

**[⬆ Back to Top](#table-of-contents)**

<a name="acid-properties-isolation-levels"></a>  
### 32. **ACID Properties and Isolation Levels**  

**[⬆ Back to Top](#table-of-contents)**

<a name="database-migrations"></a>  
### 33. **Database Migrations with Liquibase or Flyway**  

**[⬆ Back to Top](#table-of-contents)**

<a name="data-modeling-normalization"></a>  
### 34. **Data Modeling and Normalization**  

**[⬆ Back to Top](#table-of-contents)**


## **RESTful API Design**  
<a name="rest-principles-resource-modeling"></a>  
### 35. **REST Principles and Resource Modeling**  

**[⬆ Back to Top](#table-of-contents)**

<a name="http-methods-status-codes-idempotency"></a>  
### 36. **HTTP Methods, Status Codes, Headers, and Idempotency**  

**[⬆ Back to Top](#table-of-contents)**

<a name="exception-handling-validation"></a>  
### 37. **Exception Handling and Validation**  

**[⬆ Back to Top](#table-of-contents)**

<a name="api-versioning-hateoas"></a>  
### 38. **API Versioning and HATEOAS**  

**[⬆ Back to Top](#table-of-contents)**

<a name="pagination-sorting-filtering"></a>  
### 39. **Pagination, Sorting, and Filtering**  

**[⬆ Back to Top](#table-of-contents)**


## **Microservices**  

<a name="microservices-architecture"></a>  
### 40. **Microservice Architecture and Decomposition Strategies**  

**[⬆ Back to Top](#table-of-contents)**

<a name="service-discovery-api-gateway"></a>  
### 41. **Service Discovery and API Gateway**  

**[⬆ Back to Top](#table-of-contents)**

<a name="sync-vs-async-communication"></a>  
### 42. **Synchronous (REST, gRPC) vs Asynchronous Communication**  

**[⬆ Back to Top](#table-of-contents)**

<a name="event-driven-architecture-message-brokers"></a>  
### 43. **Event-driven Architecture and Message Brokers**  

**[⬆ Back to Top](#table-of-contents)**

<a name="kafka-fundamentals"></a>  
### 44. **Kafka Fundamentals: Producers, Consumers, Brokers, Partitions, Topics**  

**[⬆ Back to Top](#table-of-contents)**

<a name="kafka-delivery-semantics-stream-processing"></a>  
### 45. **Kafka Delivery Semantics and Stream Processing**  

**[⬆ Back to Top](#table-of-contents)**

<a name="kafka-schema-registry-avro-spring"></a>  
### 46. **Kafka Schema Registry, Avro, and Spring Integration**  

**[⬆ Back to Top](#table-of-contents)**

<a name="circuit-breakers-retries-rate-limiting"></a>  
### 47. **Circuit Breakers, Retries, and Rate Limiting (Resilience4j)**  

**[⬆ Back to Top](#table-of-contents)**

<a name="spring-cloud-config-logging"></a>  
### 48. **Spring Cloud Config, Centralized Logging**  

**[⬆ Back to Top](#table-of-contents)**


## **CI/CD & Docker**  

<a name="ci-cd-pipelines"></a>  
### 49. **CI/CD Pipelines: Jenkins, GitHub Actions, GitLab CI**  

**[⬆ Back to Top](#table-of-contents)**

<a name="docker-fundamentals"></a>  
### 50. **Docker Fundamentals: Images, Containers, Dockerfile**  

**[⬆ Back to Top](#table-of-contents)**

<a name="docker-compose-multi-container"></a>  
### 51. **Docker Compose and Multi-container Apps**  

**[⬆ Back to Top](#table-of-contents)**

<a name="deployment-strategies"></a>  
### 52. **Deployment Strategies: Blue/Green, Rolling, Canary**  

**[⬆ Back to Top](#table-of-contents)**

<a name="artifact-versioning-environment-promotion"></a>  
### 53. **Artifact Versioning and Environment Promotion**  

**[⬆ Back to Top](#table-of-contents)**


## **Testing**  

<a name="unit-testing-junit-mockito"></a>  
### 54. **Unit Testing with JUnit, Mockito**  

**[⬆ Back to Top](#table-of-contents)**

<a name="integration-testing-spring-boot"></a>  
### 55. **Integration Testing with Spring Boot**  

**[⬆ Back to Top](#table-of-contents)**

<a name="test-slicing-testcontainers"></a>  
### 56. **Test Slicing and Testcontainers**  

**[⬆ Back to Top](#table-of-contents)**

<a name="contract-testing-ci-strategies"></a>  
### 57. **Contract Testing, CI Testing Strategies**  

**[⬆ Back to Top](#table-of-contents)**

<a name="static-analysis"></a>  
### 58. **Static Analysis: SonarQube, JaCoCo, SpotBugs**  

**[⬆ Back to Top](#table-of-contents)**


## **Software Architecture**  

<a name="scalability-availability-fault-tolerance"></a>  
### 59. **Scalability, Availability, Fault Tolerance**  

**[⬆ Back to Top](#table-of-contents)**

<a name="cap-theorem-consistency-models"></a>  
### 60. **CAP Theorem and Consistency Models**  

**[⬆ Back to Top](#table-of-contents)**

<a name="caching-in-memory-redis-caffeine"></a>  
### 61. **Caching: In-memory, Redis, Caffeine**  

**[⬆ Back to Top](#table-of-contents)**

<a name="redis-data-types-ttl-pubsub-locks-rate-limiting"></a>  
### 62. **Redis: Data Types, TTL, Pub/Sub, Locks, Rate Limiting**  

**[⬆ Back to Top](#table-of-contents)**

<a name="design-patterns-cqrs-saga-event-sourcing"></a>  
### 63. **Design Patterns: CQRS, Saga, Event Sourcing**  

**[⬆ Back to Top](#table-of-contents)**

<a name="load-balancing-partitioning-replication"></a>  
### 64. **Load Balancing, Partitioning, Replication**  

**[⬆ Back to Top](#table-of-contents)**

<a name="api-security-token-management"></a>  
### 65. **API Security and Token Management**  

**[⬆ Back to Top](#table-of-contents)**


## **Clean Code & Best Practices**  

<a name="clean-code-principles-refactoring"></a>  
### 66. **Clean Code Principles and Refactoring Techniques**  

**[⬆ Back to Top](#table-of-contents)**

<a name="creational-patterns-singleton-factory-builder-prototype"></a>  
### 67. **Creational Patterns: Singleton, Factory, Builder, Prototype**  

**[⬆ Back to Top](#table-of-contents)**

<a name="structural-patterns-adapter-decorator-proxy-facade"></a>  
### 68. **Structural Patterns: Adapter, Decorator, Proxy, Facade**  

**[⬆ Back to Top](#table-of-contents)**

<a name="behavioral-patterns-strategy-observer-chain-of-responsibility"></a>  
### 69. **Behavioral Patterns: Strategy, Observer, Chain of Responsibility**  

**[⬆ Back to Top](#table-of-contents)**

<a name="clean-architecture-hexagonal-onion"></a>  
### 70. **Clean Architecture, Hexagonal, Onion**  

**[⬆ Back to Top](#table-of-contents)**


## **Agile & Scrum**  
<a name="agile-manifesto-scrum-roles"></a>  
### 71. **Agile Manifesto and Scrum Roles**  

**[⬆ Back to Top](#table-of-contents)**

<a name="scrum-ceremonies-user-stories"></a>  
### 72. **Scrum Ceremonies and User Stories**  

**[⬆ Back to Top](#table-of-contents)**

<a name="story-points-velocity-metrics"></a>  
### 73. **Story Points, Velocity, and Metrics**  

**[⬆ Back to Top](#table-of-contents)**

<a name="agile-tools-jira-trello-clickup"></a>  
### 74. **Agile Tools: Jira, Trello, ClickUp**  

**[⬆ Back to Top](#table-of-contents)**
