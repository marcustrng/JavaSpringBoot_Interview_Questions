# Java Spring Boot Interview Questions and Answers

### Table of Contents

<details open>
<summary>
Hide/Show table of contents
</summary>

| No. | Questions                                                                                                                                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|     | **Java Core (Java 8+)**                                                                                                                                       |
| 1   | [JVM memory model: heap, stack, metaspace, GC types (G1, ZGC, CMS)](#jvm-memory-model-heap-stack-metaspace-gc-types)                                         |
| 2   | [Performance tuning: GC tuning, escape analysis, JIT optimizations](#performance-tuning-gc-tuning-escape-analysis-jit-optimizations)                        |
| 3   | [Concurrency: Thread pools, ExecutorService, ForkJoinPool, CompletableFuture](#concurrency-thread-pools-executorservice-forkjoinpool-completablefuture)     |
| 4   | [Thread-safety: synchronization, volatile, atomic classes, immutability](#thread-safety-synchronization-volatile-atomic-immutability)                        |
| 5   | [Java 8 features: Streams, Lambdas, Functional interfaces, Optionals](#java-8-features-streams-lambdas-functional-interfaces-optionals)                      |
|     | **Spring Ecosystem**                                                                                                                                          |
| 6   | [Spring Boot: AutoConfiguration, Actuator, Profiles, Starters](#spring-boot-autoconfiguration-actuator-profiles-starters)                                    |
| 7   | [Spring MVC: Request lifecycle, Controllers, Filters, Interceptors](#spring-mvc-request-lifecycle-controllers-filters-interceptors)                          |
| 8   | [Spring Security: JWT, OAuth2, method-level security, CSRF](#spring-security-jwt-oauth2-method-level-security-csrf)                                          |
| 9   | [Spring Data JPA: Lazy vs Eager, Entity lifecycle, Criteria API](#spring-data-jpa-lazy-vs-eager-entity-lifecycle-criteria-api)                               |
| 10  | [Spring Transaction Management: @Transactional, isolation, propagation](#spring-transaction-management-transactional-isolation-propagation)                 |
|     | **Microservices & API Design**                                                                                                                                |
| 11  | [REST API principles: HTTP verbs, status codes, pagination, HATEOAS](#rest-api-principles-http-verbs-status-codes-pagination-hateoas)                        |
| 12  | [API versioning strategies and backward compatibility](#api-versioning-strategies-and-backward-compatibility)                                                |
| 13  | [Service-to-service communication: REST, Feign, Kafka, SQS](#service-to-service-communication-rest-feign-kafka-sqs)                                          |
| 14  | [Resilience patterns: circuit breaker, retry, bulkhead (Resilience4j)](#resilience-patterns-circuit-breaker-retry-bulkhead-resilience4j)                    |
|     | **Cloud & DevOps**                                                                                                                                            |
| 15  | [AWS services: Lambda, API Gateway, SQS, SNS, DynamoDB, S3](#aws-services-lambda-api-gateway-sqs-sns-dynamodb-s3)                                             |
| 16  | [Serverless architecture: cold start, event-driven design, limits](#serverless-architecture-cold-start-event-driven-design-limits)                           |
| 17  | [Containers: Dockerfile best practices, ECS, Kubernetes basics](#containers-dockerfile-best-practices-ecs-kubernetes-basics)                                 |
| 18  | [Infrastructure as Code (IaC): CloudFormation, Terraform, CDK basics](#infrastructure-as-code-cloudformation-terraform-cdk-basics)                           |
| 19  | [CI/CD pipelines: Jenkins, GitHub Actions, GitLab CI, Gradle, Maven](#ci-cd-pipelines-jenkins-github-actions-gitlab-ci-gradle-maven)                         |
| 20  | [DevOps culture: shift-left testing, blue-green deployments](#devops-culture-shift-left-testing-blue-green-deployments)                                      |
|     | **Testing & Quality Assurance**                                                                                                                               |
| 21  | [Unit testing: JUnit 5, parameterized tests, test lifecycle](#unit-testing-junit-5-parameterized-tests-test-lifecycle)                                       |
| 22  | [Mocking: Mockito best practices, spies vs mocks](#mocking-mockito-best-practices-spies-vs-mocks)                                                            |
| 23  | [Integration testing: Testcontainers, @SpringBootTest, @DataJpaTest](#integration-testing-testcontainers-springboottest-datajpatest)                         |
| 24  | [Contract testing: consumer-driven contracts with Pact](#contract-testing-consumer-driven-contracts-with-pact)                                                |
|     | **Architecture & System Design**                                                                                                                              |
| 25  | [Domain-driven design (DDD): aggregates, value objects, repositories](#domain-driven-design-ddd-aggregates-value-objects-repositories)                       |
| 26  | [System design principles: scalability, availability, CAP theorem](#system-design-principles-scalability-availability-cap-theorem)                           |
| 27  | [Event-driven architecture: pub/sub, eventual consistency](#event-driven-architecture-pubsub-eventual-consistency)                                           |
| 28  | [Monitoring & Observability: Prometheus, Grafana, Actuator, CloudWatch](#monitoring-observability-prometheus-grafana-actuator-cloudwatch)                    |
|     | **Clean Code & Patterns**                                                                                                                                     |
| 29  | [SOLID principles, Clean Architecture, YAGNI, DRY, KISS](#solid-principles-clean-architecture-yagni-dry-kiss)                                                 |
| 30  | [Design patterns: Builder, Strategy, Factory, Template, Adapter](#design-patterns-builder-strategy-factory-template-adapter)                                 |
|     | **Agile & Collaboration**                                                                                                                                     |
| 31  | [Working in Agile teams: ceremonies, story pointing, retrospectives](#working-in-agile-teams-ceremonies-story-pointing-retrospectives)                       |
| 32  | [Code reviews and mentoring best practices](#code-reviews-and-mentoring-best-practices)                                                                      |
| 33  | [Effective technical documentation and communication](#effective-technical-documentation-and-communication)                                                  |

</details>


Good luck with your interview 😊
