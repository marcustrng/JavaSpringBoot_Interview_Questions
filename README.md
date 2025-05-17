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
<a name="java-core"></a>

1. ### **Java 8+ Features: Lambda, Streams, Optional, Records, Sealed Classes**  
<a name="java-features"></a>  
**[⬆ Back to Top](#table-of-contents)**

2. ### **Functional Interfaces and Method References**  
<a name="functional-interfaces"></a>  
**[⬆ Back to Top](#table-of-contents)**

3. ### **Stream API and Collector Operations**  
<a name="stream-api"></a>  
**[⬆ Back to Top](#table-of-contents)**

4. ### **Collections Framework and Concurrency Utilities**  
<a name="collections-framework"></a>  
**[⬆ Back to Top](#table-of-contents)**

5. ### **JVM Internals: Memory Model, Garbage Collection, Class Loading**  
<a name="jvm-internals"></a>  
**[⬆ Back to Top](#table-of-contents)**

6. ### **Generics, Annotations, and Reflection**  
<a name="generics-annotations-reflection"></a>  
**[⬆ Back to Top](#table-of-contents)**

7. ### **Exception Handling and Best Practices**  
<a name="exception-handling"></a>  
**[⬆ Back to Top](#table-of-contents)**

8. ### **Immutability and Performance Tuning**  
<a name="immutability-performance"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Object-Oriented Programming (OOP)**  
<a name="oop"></a>

9. ### **OOP Principles: Abstraction, Encapsulation, Inheritance, Polymorphism**  
<a name="oop-principles"></a>  
**[⬆ Back to Top](#table-of-contents)**

10. ### **SOLID Principles**  
<a name="solid-principles"></a>  
**[⬆ Back to Top](#table-of-contents)**

11. ### **Composition vs Inheritance**  
<a name="composition-vs-inheritance"></a>  
**[⬆ Back to Top](#table-of-contents)**

12. ### **Domain-Driven Design (DDD): Entities, Value Objects, Aggregates**  
<a name="ddd"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Spring JPA (Hibernate)**  
<a name="spring-jpa"></a>

13. ### **JPA Entity Mapping, Lifecycle, and Annotations**  
<a name="jpa-entity-mapping"></a>  
**[⬆ Back to Top](#table-of-contents)**

14. ### **Entity Relationships: OneToMany, ManyToOne, ManyToMany, OneToOne**  
<a name="entity-relationships"></a>  
**[⬆ Back to Top](#table-of-contents)**

15. ### **JPQL, Native Queries, and Criteria API**  
<a name="jpql-native-queries"></a>  
**[⬆ Back to Top](#table-of-contents)**

16. ### **Transaction Management and Propagation**  
<a name="transaction-management"></a>  
**[⬆ Back to Top](#table-of-contents)**

17. ### **Lazy vs Eager Loading, N+1 Problem, Fetch Joins**  
<a name="lazy-vs-eager"></a>  
**[⬆ Back to Top](#table-of-contents)**

18. ### **Auditing, Soft Deletes, Optimistic/Pessimistic Locking**  
<a name="auditing-soft-deletes"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Spring Security**  
<a name="spring-security"></a>

19. ### **Spring Security Architecture and Filter Chain**  
<a name="security-architecture"></a>  
**[⬆ Back to Top](#table-of-contents)**

20. ### **Authentication, Authorization, and Roles**  
<a name="authentication-authorization"></a>  
**[⬆ Back to Top](#table-of-contents)**

21. ### **JWT-Based Stateless Authentication**  
<a name="jwt-authentication"></a>  
**[⬆ Back to Top](#table-of-contents)**

22. ### **Method-Level Security, RBAC, and Custom Annotations**  
<a name="method-level-security"></a>  
**[⬆ Back to Top](#table-of-contents)**

23. ### **OAuth2 and OpenID Connect Integration**  
<a name="oauth2-openid"></a>  
**[⬆ Back to Top](#table-of-contents)**

24. ### **CSRF Protection, CORS, and Session Management**  
<a name="csrf-cors-session"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Spring Boot**  
<a name="spring-boot"></a>

25. ### **Auto-Configuration and Conditional Beans**  
<a name="auto-configuration"></a>  
**[⬆ Back to Top](#table-of-contents)**

26. ### **Application Configuration (YAML/Properties) and Profile Management**  
<a name="app-configuration"></a>  
**[⬆ Back to Top](#table-of-contents)**

27. ### **Spring Boot Actuator for Health Checks and Metrics**  
<a name="spring-boot-actuator"></a>  
**[⬆ Back to Top](#table-of-contents)**

28. ### **Externalized Configuration and Secret Management**  
<a name="externalized-configuration"></a>  
**[⬆ Back to Top](#table-of-contents)**

29. ### **Embedded Tomcat/Jetty/Undertow and Deployment Packaging**  
<a name="embedded-servers"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **SQL Database**  
<a name="sql-database"></a>

30. ### **SQL Syntax and Query Building Basics**  
<a name="sql-basics"></a>  
**[⬆ Back to Top](#table-of-contents)**

31. ### **Joins, Indexing, Query Planning and Optimization**  
<a name="joins-indexing"></a>  
**[⬆ Back to Top](#table-of-contents)**

32. ### **ACID Properties and Isolation Levels**  
<a name="acid-isolation"></a>  
**[⬆ Back to Top](#table-of-contents)**

33. ### **Database Migrations with Liquibase or Flyway**  
<a name="db-migrations"></a>  
**[⬆ Back to Top](#table-of-contents)**

34. ### **Data Modeling and Normalization**  
<a name="data-modeling"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **RESTful API Design**  
<a name="restful-api"></a>

35. ### **REST Principles and Resource Modeling**  
<a name="rest-principles"></a>  
**[⬆ Back to Top](#table-of-contents)**

36. ### **HTTP Methods, Status Codes, Headers, and Idempotency**  
<a name="http-methods-status-codes"></a>  
**[⬆ Back to Top](#table-of-contents)**

37. ### **Exception Handling and Validation**  
<a name="exception-handling-validation"></a>  
**[⬆ Back to Top](#table-of-contents)**

38. ### **API Versioning and HATEOAS**  
<a name="api-versioning-hateoas"></a>  
**[⬆ Back to Top](#table-of-contents)**

39. ### **Pagination, Sorting, and Filtering**  
<a name="pagination-sorting-filtering"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Microservices**  
<a name="microservices"></a>

40. ### **Microservice Architecture and Decomposition Strategies**  
<a name="microservice-architecture"></a>  
**[⬆ Back to Top](#table-of-contents)**

41. ### **Service Discovery and API Gateway**  
<a name="service-discovery"></a>  
**[⬆ Back to Top](#table-of-contents)**

42. ### **Synchronous (REST, gRPC) vs Asynchronous Communication**  
<a name="sync-async-communication"></a>  
**[⬆ Back to Top](#table-of-contents)**

43. ### **Event-Driven Architecture and Message Brokers**  
<a name="event-driven-architecture"></a>  
**[⬆ Back to Top](#table-of-contents)**

44. ### **Kafka Fundamentals: Producers, Consumers, Brokers, Partitions, Topics**  
<a name="kafka-fundamentals"></a>  
**[⬆ Back to Top](#table-of-contents)**

45. ### **Kafka Delivery Semantics and Stream Processing**  
<a name="kafka-delivery"></a>  
**[⬆ Back to Top](#table-of-contents)**

46. ### **Kafka Schema Registry, Avro, and Spring Integration**  
<a name="kafka-schema-avro"></a>  
**[⬆ Back to Top](#table-of-contents)**

47. ### **Circuit Breakers, Retries, and Rate Limiting (Resilience4j)**  
<a name="circuit-breakers"></a>  
**[⬆ Back to Top](#table-of-contents)**

48. ### **Spring Cloud Config, Centralized Logging**  
<a name="spring-cloud-config"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **CI/CD & Docker**  
<a name="cicd-docker"></a>

49. ### **CI/CD Pipelines: Jenkins, GitHub Actions, GitLab CI**  
<a name="cicd-pipelines"></a>  
**[⬆ Back to Top](#table-of-contents)**

50. ### **Docker Fundamentals: Images, Containers, Dockerfile**  
<a name="docker-fundamentals"></a>  
**[⬆ Back to Top](#table-of-contents)**

51. ### **Docker Compose and Multi-Container Apps**  
<a name="docker-compose"></a>  
**[⬆ Back to Top](#table-of-contents)**

52. ### **Deployment Strategies: Blue/Green, Rolling, Canary**  
<a name="deployment-strategies"></a>  
**[⬆ Back to Top](#table-of-contents)**

53. ### **Artifact Versioning and Environment Promotion**  
<a name="artifact-versioning"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Testing**  
<a name="testing"></a>

54. ### **Unit Testing with JUnit and Mockito**  
<a name="unit-testing"></a>  
**[⬆ Back to Top](#table-of-contents)**

55. ### **Integration Testing and Spring Boot Test**  
<a name="integration-testing"></a>  
**[⬆ Back to Top](#table-of-contents)**

56. ### **Contract Testing and Consumer-Driven Contracts**  
<a name="contract-testing"></a>  
**[⬆ Back to Top](#table-of-contents)**

57. ### **Performance Testing and Load Testing Tools**  
<a name="performance-testing"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Software Architecture**  
<a name="software-architecture"></a>

58. ### **Design Patterns: Creational, Structural, Behavioral**  
<a name="design-patterns"></a>  
**[⬆ Back to Top](#table-of-contents)**

59. ### **Event-Driven Architecture and CQRS**  
<a name="event-driven-cqrs"></a>  
**[⬆ Back to Top](#table-of-contents)**

60. ### **Domain-Driven Design (DDD) Tactical and Strategic Patterns**  
<a name="ddd-tactical-strategic"></a>  
**[⬆ Back to Top](#table-of-contents)**

61. ### **Scalability, Availability, and CAP Theorem**  
<a name="scalability-availability"></a>  
**[⬆ Back to Top](#table-of-contents)**

62. ### **API Gateway and Backend for Frontend (BFF)**  
<a name="api-gateway-bff"></a>  
**[⬆ Back to Top](#table-of-contents)**

63. ### **Monolith vs Microservices vs Serverless**  
<a name="monolith-vs-microservices"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Clean Code & Best Practices**  
<a name="clean-code"></a>

64. ### **Code Readability and Naming Conventions**  
<a name="code-readability"></a>  
**[⬆ Back to Top](#table-of-contents)**

65. ### **Refactoring Techniques and Code Smells**  
<a name="refactoring-code-smells"></a>  
**[⬆ Back to Top](#table-of-contents)**

66. ### **Unit Test Coverage and Test-Driven Development (TDD)**  
<a name="unit-test-tdd"></a>  
**[⬆ Back to Top](#table-of-contents)**

67. ### **Logging, Monitoring, and Observability**  
<a name="logging-monitoring"></a>  
**[⬆ Back to Top](#table-of-contents)**


## **Agile & Scrum**  
<a name="agile-scrum"></a>

68. ### **Agile Principles and Scrum Framework**  
<a name="agile-principles"></a>  
**[⬆ Back to Top](#table-of-contents)**

69. ### **Sprint Planning, Stand-ups, and Retrospectives**  
<a name="sprint-planning"></a>  
**[⬆ Back to Top](#table-of-contents)**

70. ### **User Stories, Epics, and Story Points Estimation**  
<a name="user-stories"></a>  
**[⬆ Back to Top](#table-of-contents)**

71. ### **Continuous Improvement and Team Collaboration**  
<a name="continuous-improvement"></a>  
**[⬆ Back to Top](#table-of-contents)**

