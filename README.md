# Spring Ecosystem

### Table of Contents

<details open>
<summary>Show/Hide Table of Contents</summary>

| No. | Section & Topics                                                                                     |
| ----|-----------------------------------------------------------------------------------------------------|
|      | **Spring Framework Core**                                                                           |
| 1    | [Dependency Injection (DI) & Inversion of Control (IoC)](#dependency-injection-di--inversion-of-control-ioc) |
| 2    | [Spring Container & Bean Factory](#spring-container--bean-factory)                                 |
| 3    | [Spring Expression Language (SpEL)](#spring-expression-language-spel)                               |
| 4    | [Resource Loading & Environment Abstraction](#resource-loading--environment-abstraction)           |
|      | **Spring Boot**                                                                                     |
| 5    | [Auto-Configuration](#auto-configuration)                                                           |
| 6    | [Opinionated Defaults](#opinionated-defaults)                                                       |
| 7    | [Spring Boot CLI & Initializr](#spring-boot-cli--initializr)                                       |
| 8    | [Externalized Configuration](#externalized-configuration)                                          |
| 9    | [Actuator](#actuator)                                                                               |
|      | **Spring MVC & Web Development**                                                                    |
| 10   | [RESTful Web Services](#restful-web-services)                                                       |
| 11   | [Request & Response Handling](#request--response-handling)                                         |
| 12   | [Multipart File Uploads & Streaming Responses](#multipart-file-uploads--streaming-responses)       |
| 13   | [WebFlux (Reactive Web)](#webflux-reactive-web)                                                    |
|      | **Spring Data & Persistence**                                                                       |
| 14   | [Spring Data JPA](#spring-data-jpa)                                                                 |
| 15   | [Spring Transaction Management](#spring-transaction-management)                                     |
| 16   | [Other Spring Data Modules](#other-spring-data-modules)                                            |
| 17   | [Hibernate Integration](#hibernate-integration)                                                     |
|      | **Spring Security**                                                                                 |
| 18   | [Authentication & Authorization](#authentication--authorization)                                   |
| 19   | [OAuth2 & OpenID Connect](#oauth2--openid-connect)                                                  |
| 20   | [Web Security](#web-security)                                                                       |
| 21   | [Security Testing](#security-testing)                                                               |
|      | **Spring Cloud & Microservices**                                                                    |
| 22   | [Service Discovery](#service-discovery)                                                             |
| 23   | [API Gateway](#api-gateway)                                                                         |
| 24   | [Circuit Breaker & Resilience](#circuit-breaker--resilience)                                       |
| 25   | [Distributed Configuration](#distributed-configuration)                                            |
| 26   | [Load Balancing](#load-balancing)                                                                   |
| 27   | [Messaging & Event-Driven Architectures](#messaging--event-driven-architectures)                   |
| 28   | [Tracing & Monitoring](#tracing--monitoring)                                                        |
|      | **Spring Batch & Integration**                                                                      |
| 29   | [Spring Batch](#spring-batch)                                                                       |
| 30   | [Spring Integration](#spring-integration)                                                           |
| 31   | [Scheduling & Asynchronous Processing](#scheduling--asynchronous-processing)                        |
|      | **Testing in Spring**                                                                               |
| 32   | [Spring Testing Support](#spring-testing-support)                                                   |
| 33   | [Mocking & Stubbing](#mocking--stubbing)                                                            |
| 34   | [Integration Testing](#integration-testing)                                                         |
| 35   | [Test Automation & Continuous Testing](#test-automation--continuous-testing)                        |
|      | **Reactive Programming with Spring**                                                                |
| 36   | [Project Reactor Basics](#project-reactor-basics)                                                   |
| 37   | [Spring WebFlux](#spring-webflux)                                                                   |
| 38   | [Reactive Data Access](#reactive-data-access)                                                       |
|      | **Best Practices & Patterns**                                                                       |
| 39   | [Layered Architecture](#layered-architecture)                                                       |
| 40   | [DTOs and Mapping](#dtos-and-mapping)                                                               |
| 41   | [Exception Handling](#exception-handling)                                                           |
| 42   | [Configuration Management](#configuration-management)                                               |
| 43   | [Performance Considerations](#performance-considerations)                                           |
| 44   | [Security by Design](#security-by-design)                                                           |

</details>
