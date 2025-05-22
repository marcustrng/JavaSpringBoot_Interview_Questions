# REST APIs & Web Development

### Table of Contents

<details open>
<summary>Show/Hide Table of Contents</summary>

| No.  | Section & Topics                                                                                      |
| ---- | ---------------------------------------------------------------------------------------------------- |
|      | **REST Principles & Architecture**                                                                   |
| 1    | [REST Constraints](#rest-constraints)                                                                |
| 2    | [Resource Identification](#resource-identification)                                                  |
| 3    | [HTTP Methods](#http-methods)                                                                        |
| 4    | [Statelessness](#statelessness)                                                                      |
|      | **API Design & Best Practices**                                                                       |
| 5    | [Resource Modeling](#resource-modeling)                                                              |
| 6    | [URI Design](#uri-design)                                                                             |
| 7    | [Versioning](#versioning)                                                                             |
| 8    | [Hypermedia (HATEOAS)](#hypermedia-hateoas)                                                          |
| 9    | [Error Handling](#error-handling)                                                                    |
| 10   | [Pagination, Sorting, Filtering](#pagination-sorting-filtering)                                      |
|      | **HTTP Fundamentals**                                                                                 |
| 11   | [HTTP Status Codes](#http-status-codes)                                                              |
| 12   | [Headers](#headers)                                                                                   |
| 13   | [Content Negotiation](#content-negotiation)                                                          |
| 14   | [Caching](#caching)                                                                                   |
|      | **Data Formats & Serialization**                                                                      |
| 15   | [JSON](#json)                                                                                        |
| 16   | [XML](#xml)                                                                                          |
| 17   | [Protobuf/Avro](#protobufavro)                                                                       |
| 18   | [JSON API & GraphQL](#json-api-graphql)                                                              |
|      | **Security in REST APIs**                                                                             |
| 19   | [Authentication](#authentication)                                                                    |
| 20   | [Authorization](#authorization)                                                                      |
| 21   | [Transport Security](#transport-security)                                                            |
| 22   | [Preventing Common Attacks](#preventing-common-attacks)                                              |
|      | **API Documentation & Testing**                                                                       |
| 23   | [Documentation Tools](#documentation-tools)                                                          |
| 24   | [Interactive Documentation](#interactive-documentation)                                              |
| 25   | [Contract-Driven Development](#contract-driven-development)                                          |
| 26   | [Testing](#testing)                                                                                   |
| 27   | [Mocking & Stubbing](#mocking-stubbing)                                                              |
|      | **Web Frameworks & Tooling**                                                                          |
| 28   | [Spring MVC / Spring Boot](#spring-mvc-spring-boot)                                                  |
| 29   | [WebFlux (Reactive APIs)](#webflux-reactive-apis)                                                    |
| 30   | [Other Frameworks](#other-frameworks)                                                                |
| 31   | [Build & Dependency Management](#build-dependency-management)                                        |
|      | **Performance & Scalability**                                                                         |
| 32   | [Asynchronous Processing](#asynchronous-processing)                                                  |
| 33   | [Caching](#performance-caching)                                                                      |
| 34   | [Compression](#compression)                                                                           |
| 35   | [Rate Limiting](#rate-limiting)                                                                       |
| 36   | [Load Balancing & API Gateways](#load-balancing-api-gateways)                                        |
|      | **Cross-Origin Resource Sharing (CORS)**                                                             |
| 37   | [CORS Mechanism](#cors-mechanism)                                                                    |
| 38   | [Configuring CORS](#configuring-cors)                                                                |
|      | **WebSockets & Real-Time Communication**                                                             |
| 39   | [WebSocket Protocol](#websocket-protocol)                                                            |
| 40   | [Server-Sent Events (SSE)](#server-sent-events-sse)                                                  |
| 41   | [Use Cases & Trade-offs](#use-cases-trade-offs)                                                      |
|      | **Versioning & Backward Compatibility**                                                              |
| 42   | [Versioning Strategies](#versioning-strategies)                                                      |
| 43   | [Deprecation Policies](#deprecation-policies)                                                        |
| 44   | [Backward Compatibility](#backward-compatibility)                                                   |
|      | **Monitoring, Logging & Analytics**                                                                   |
| 45   | [API Usage Monitoring](#api-usage-monitoring)                                                        |
| 46   | [Logging](#logging)                                                                                   |
| 47   | [Distributed Tracing](#distributed-tracing)                                                          |

</details>

---

## Detailed Sections

<a name="rest-constraints"></a>
### 1. **REST Constraints:** Statelessness, Client-Server, Cacheability, Uniform Interface, Layered System, Code on Demand (optional)

* **Statelessness**
* **Client-Server**
* **Cacheability**
* **Uniform Interface**
* **Layered System**
* **Code on Demand (optional)**

---

<a name="resource-identification"></a>
### 2. **Resource Identification:** Using URIs to uniquely identify resources

---

<a name="http-methods"></a>
### 3. **HTTP Methods:** Understanding GET, POST, PUT, DELETE, PATCH and their idempotency and safety properties

---

<a name="statelessness"></a>
### 4. **Statelessness:** Ensuring that each request from client contains all necessary information

---

<a name="resource-modeling"></a>
### 5. **Resource Modeling:** Designing resource hierarchies and naming conventions (nouns, pluralization)

---

<a name="uri-design"></a>
### 6. **URI Design:** Clean, consistent, intuitive URIs following REST conventions

---

<a name="versioning"></a>
### 7. **Versioning:** Strategies (URI versioning, Header versioning, Content negotiation)

---

<a name="hypermedia-hateoas"></a>
### 8. **Hypermedia (HATEOAS):** Linking resources dynamically to guide clients

---

<a name="error-handling"></a>
### 9. **Error Handling:** Standardized error responses (HTTP status codes, error payload format)

---

<a name="pagination-sorting-filtering"></a>
### 10. **Pagination, Sorting, Filtering:** Techniques to manage large datasets and improve API usability

---

<a name="http-status-codes"></a>
### 11. **HTTP Status Codes:** 2xx (success), 3xx (redirection), 4xx (client errors), 5xx (server errors)

---

<a name="headers"></a>
### 12. **Headers:** Content-Type, Accept, Authorization, Cache-Control, CORS headers

---

<a name="content-negotiation"></a>
### 13. **Content Negotiation:** Supporting multiple media types (JSON, XML, YAML)

---

<a name="caching"></a>
### 14. **Caching:** Client-side and server-side caching mechanisms with proper cache headers

---

<a name="json"></a>
### 15. **JSON:** Most common data format, JSON Schema for validation

---

<a name="xml"></a>
### 16. **XML:** Legacy support, SOAP basics if applicable

---

<a name="protobufavro"></a>
### 17. **Protobuf/Avro:** Binary formats for high performance

---

<a name="json-api-graphql"></a>
### 18. **JSON API & GraphQL:** Alternative API paradigms and when to consider them

---

<a name="authentication"></a>
### 19. **Authentication:** Basic Auth, OAuth2, JWT, API keys

---

<a name="authorization"></a>
### 20. **Authorization:** Role-Based Access Control (RBAC), Attribute-Based Access Control (ABAC)

---

<a name="transport-security"></a>
### 21. **Transport Security:** HTTPS/TLS

---

<a name="preventing-common-attacks"></a>
### 22. **Preventing Common Attacks:** CSRF, XSS, Injection attacks, Rate limiting, Throttling

---

<a name="documentation-tools"></a>
### 23. **Documentation Tools:** OpenAPI (Swagger), RAML, API Blueprint

---

<a name="interactive-documentation"></a>
### 24. **Interactive Documentation:** Swagger UI, Redoc

---

<a name="contract-driven-development"></a>
### 25. **Contract-Driven Development:** Using API specs to drive client and server development

---

<a name="testing"></a>
### 26. **Testing:** Unit tests, Integration tests (REST-assured, Postman, SoapUI)

---

<a name="mocking-stubbing"></a>
### 27. **Mocking & Stubbing:** Using tools to simulate APIs during development

---

<a name="spring-mvc-spring-boot"></a>
### 28. **Spring MVC / Spring Boot:** Controllers, Request Mapping, Exception Handling

---

<a name="webflux-reactive-apis"></a>
### 29. **WebFlux (Reactive APIs):** Reactive programming model for non-blocking APIs

---

<a name="other-frameworks"></a>
### 30. **Other Frameworks:** JAX-RS, Micronaut, Quarkus basics

---

<a name="build-dependency-management"></a>
### 31. **Build & Dependency Management:** Maven, Gradle

---

<a name="asynchronous-processing"></a>
### 32. **Asynchronous Processing:** Deferred results, CompletableFuture, Reactive streams

---

<a name="performance-caching"></a>
### 33. **Caching:** HTTP cache headers, server-side caching (Redis, Ehcache)

---

<a name="compression"></a>
### 34. **Compression:** GZIP, Brotli for response payloads

---

<a name="rate-limiting"></a>
### 35. **Rate Limiting:** Protecting APIs from abuse with token buckets or leaky bucket algorithms

---

<a name="load-balancing-api-gateways"></a>
### 36. **Load Balancing & API Gateways:** NGINX, Kong, AWS API Gateway

---

<a name="cors-mechanism"></a>
### 37. **CORS Mechanism:** How browsers enforce cross-origin policies

---

<a name="configuring-cors"></a>
### 38. **Configuring CORS:** Server-side setup for allowed origins, methods, headers

---

<a name="websocket-protocol"></a>
### 39. **WebSocket Protocol:** Full-duplex communication over a single TCP connection

---

<a name="server-sent-events-sse"></a>
### 40. **Server-Sent Events (SSE):** Unidirectional streaming for real-time updates

---

<a name="use-cases-trade-offs"></a>
### 41. **Use Cases & Trade-offs:** When to use REST vs real-time communication

---

<a name="versioning-strategies"></a>
### 42. **Versioning Strategies:** URI, Header, Media Type versioning

---

<a name="deprecation-policies"></a>
### 43. **Deprecation Policies:** Gracefully phasing out old API versions

---

<a name="backward-compatibility"></a>
### 44. **Backward Compatibility:** Ensuring clients don’t break on API changes

---

<a name="api-usage-monitoring"></a>
### 45. **API Usage Monitoring:** Metrics collection (request rates, error rates, latencies)

---

<a name="logging"></a>
### 46. **Logging:** Structured logging of requests/responses, correlation IDs for tracing

---

<a name="distributed-tracing"></a>
### 47. **Distributed Tracing:** Integration with tools like Zipkin, Jaeger for request tracing across microservices

---

**[⬆ Back to Top](#rest-apis--web-development)**
