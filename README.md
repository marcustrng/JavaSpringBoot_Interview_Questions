# Databases & Persistence

### Table of Contents

<details open>
<summary>Show/Hide Table of Contents</summary>

| No.  | Section & Topics                                                                                     |
| ---- |-----------------------------------------------------------------------------------------------------|
|      | **Database Fundamentals**                                                                             |
| 1    | [Relational Databases (RDBMS)](#relational-databases-rdbms)                                          |
| 1.1  | [Concepts](#concepts)                                                                                 |
| 1.2  | [ACID Properties](#acid-properties)                                                                   |
| 1.3  | [Normalization](#normalization)                                                                       |
| 2    | [NoSQL Databases](#nosql-databases)                                                                   |
| 2.1  | [Types of NoSQL Databases](#types-of-nosql-databases)                                                 |
| 2.2  | [CAP Theorem](#cap-theorem)                                                                           |
| 2.3  | [Use Cases & Polyglot Persistence](#use-cases-polyglot-persistence)                                   |
|      | **SQL Mastery**                                                                                       |
| 3    | [Advanced SQL Queries](#advanced-sql-queries)                                                         |
| 3.1  | [Joins & Subqueries](#joins-subqueries)                                                               |
| 3.2  | [Window Functions & Aggregations](#window-functions-aggregations)                                     |
| 3.3  | [Stored Procedures, Functions, Triggers](#stored-procedures-functions-triggers)                       |
| 4    | [Query Optimization](#query-optimization)                                                             |
| 4.1  | [Execution Plans & Index Usage](#execution-plans-index-usage)                                         |
| 4.2  | [Avoiding N+1 Problems](#avoiding-nplus1-problems)                                                    |
| 4.3  | [Analyzing Slow Queries](#analyzing-slow-queries)                                                     |
|      | **Database Design & Modeling**                                                                        |
| 5    | [Entity-Relationship Modeling](#entity-relationship-modeling)                                         |
| 6    | [Schema Design](#schema-design)                                                                       |
| 7    | [Indexing Strategies](#indexing-strategies)                                                           |
| 8    | [Partitioning & Sharding](#partitioning-sharding)                                                     |
|      | **Persistence Frameworks & ORM**                                                                      |
| 9    | [JPA / Hibernate](#jpa-hibernate)                                                                     |
| 9.1  | [Entity Mapping & Relationships](#entity-mapping-relationships)                                       |
| 9.2  | [Fetch Types](#fetch-types)                                                                            |
| 9.3  | [Lifecycle Callbacks & Entity States](#lifecycle-callbacks-entity-states)                             |
| 9.4  | [JPQL & Criteria API](#jpql-criteria-api)                                                             |
| 9.5  | [Caching Strategies](#caching-strategies)                                                             |
| 10   | [Alternatives & Extensions](#alternatives-extensions)                                                 |
|      | **Transactions & Concurrency Control**                                                                |
| 11   | [Transaction Isolation Levels](#transaction-isolation-levels)                                         |
| 11.1 | [Isolation Phenomena](#isolation-phenomena)                                                           |
| 12   | [Optimistic vs Pessimistic Locking](#optimistic-pessimistic-locking)                                 |
| 13   | [Distributed Transactions](#distributed-transactions)                                                 |
| 14   | [Deadlocks & Concurrency Issues](#deadlocks-concurrency-issues)                                       |
|      | **Database Migration & Versioning**                                                                   |
| 15   | [Schema Migration Tools](#schema-migration-tools)                                                     |
| 16   | [Version Control for Database](#version-control-for-database)                                         |
| 17   | [Rolling Back & Forward](#rolling-back-forward)                                                       |
| 18   | [CI/CD Integration for Migrations](#cicd-integration-for-migrations)                                 |
|      | **Performance & Scalability**                                                                          |
| 19   | [Connection Pooling](#connection-pooling)                                                             |
| 20   | [Caching Strategies](#caching-strategies-performance)                                                 |
| 21   | [Read Replicas & Load Balancing](#read-replicas-load-balancing)                                       |
| 22   | [Data Archival & Purging](#data-archival-purging)                                                     |
|      | **Backup, Recovery & Security**                                                                        |
| 23   | [Backup Strategies](#backup-strategies)                                                               |
| 24   | [Disaster Recovery Planning](#disaster-recovery-planning)                                             |
| 25   | [Database Security](#database-security)                                                               |
| 25.1 | [Authentication & Authorization](#authentication-authorization)                                       |
| 25.2 | [Encryption](#encryption)                                                                             |
| 25.3 | [Auditing & Compliance](#auditing-compliance)                                                        |
|      | **NoSQL & NewSQL Specifics**                                                                           |
| 26   | [Document Stores (MongoDB)](#document-stores-mongodb)                                                 |
| 27   | [Key-Value Stores (Redis)](#key-value-stores-redis)                                                  |
| 28   | [Column Stores (Cassandra)](#column-stores-cassandra)                                                |
| 29   | [Graph Databases (Neo4j)](#graph-databases-neo4j)                                                   |
| 30   | [NewSQL Databases](#newsql-databases)                                                                |
|      | **Tools & Utilities**                                                                                  |
| 31   | [Database Clients](#database-clients)                                                                |
| 32   | [Profiling & Monitoring](#profiling-monitoring)                                                      |
| 33   | [Data Import/Export](#data-import-export)                                                            |
| 34   | [Cloud Database Services](#cloud-database-services)                                                  |

</details>

---

## Detailed Sections

<a name="relational-databases-rdbms"></a>
### 1. **Relational Databases (RDBMS)**

<a name="concepts"></a>
#### 1.1 **Concepts**

* Tables  
* Rows  
* Columns  
* Schemas  
* Primary Keys  
* Foreign Keys  
* Indexes  

<a name="acid-properties"></a>
#### 1.2 **ACID Properties**

* Atomicity  
* Consistency  
* Isolation  
* Durability  

<a name="normalization"></a>
#### 1.3 **Normalization**

* Forms: 1NF, 2NF, 3NF, BCNF  
* Denormalization trade-offs  

<a name="nosql-databases"></a>
### 2. **NoSQL Databases**

<a name="types-of-nosql-databases"></a>
#### 2.1 **Types of NoSQL Databases**

* Document (MongoDB)  
* Key-Value (Redis)  
* Column-Family (Cassandra)  
* Graph (Neo4j)  

<a name="cap-theorem"></a>
#### 2.2 **CAP Theorem**

* Consistency  
* Availability  
* Partition tolerance trade-offs  

<a name="use-cases-polyglot-persistence"></a>
#### 2.3 **Use Cases & Polyglot Persistence**

* Use case examples for each NoSQL type  
* Polyglot persistence approach  

<a name="advanced-sql-queries"></a>
### 3. **Advanced SQL Queries**

<a name="joins-subqueries"></a>
#### 3.1 **Joins & Subqueries**

* INNER, LEFT, RIGHT, FULL Joins  
* Subqueries  
* Common Table Expressions (CTEs)  

<a name="window-functions-aggregations"></a>
#### 3.2 **Window Functions & Aggregations**

* Window functions  
* Aggregations  
* Grouping Sets  

<a name="stored-procedures-functions-triggers"></a>
#### 3.3 **Stored Procedures, Functions, Triggers**

* Stored procedures  
* Functions  
* Triggers  

<a name="query-optimization"></a>
### 4. **Query Optimization**

<a name="execution-plans-index-usage"></a>
#### 4.1 **Execution Plans & Index Usage**

<a name="avoiding-nplus1-problems"></a>
#### 4.2 **Avoiding N+1 Problems**

<a name="analyzing-slow-queries"></a>
#### 4.3 **Analyzing Slow Queries**

<a name="entity-relationship-modeling"></a>
### 5. **Entity-Relationship Modeling**

<a name="schema-design"></a>
### 6. **Schema Design**

<a name="indexing-strategies"></a>
### 7. **Indexing Strategies**

<a name="partitioning-sharding"></a>
### 8. **Partitioning & Sharding**

<a name="jpa-hibernate"></a>
### 9. **JPA / Hibernate**

<a name="entity-mapping-relationships"></a>
#### 9.1 **Entity Mapping & Relationships**

<a name="fetch-types"></a>
#### 9.2 **Fetch Types**

<a name="lifecycle-callbacks-entity-states"></a>
#### 9.3 **Lifecycle Callbacks & Entity States**

<a name="jpql-criteria-api"></a>
#### 9.4 **JPQL & Criteria API**

<a name="caching-strategies"></a>
#### 9.5 **Caching Strategies**

<a name="alternatives-extensions"></a>
### 10. **Alternatives & Extensions**

<a name="transaction-isolation-levels"></a>
### 11. **Transaction Isolation Levels**

<a name="isolation-phenomena"></a>
#### 11.1 **Isolation Phenomena**

<a name="optimistic-pessimistic-locking"></a>
### 12. **Optimistic vs Pessimistic Locking**

<a name="distributed-transactions"></a>
### 13. **Distributed Transactions**

<a name="deadlocks-concurrency-issues"></a>
### 14. **Deadlocks & Concurrency Issues**

<a name="schema-migration-tools"></a>
### 15. **Schema Migration Tools**

<a name="version-control-for-database"></a>
### 16. **Version Control for Database**

<a name="rolling-back-forward"></a>
### 17. **Rolling Back & Forward**

<a name="cicd-integration-for-migrations"></a>
### 18. **CI/CD Integration for Migrations**

<a name="connection-pooling"></a>
### 19. **Connection Pooling**

<a name="caching-strategies-performance"></a>
### 20. **Caching Strategies**

<a name="read-replicas-load-balancing"></a>
### 21. **Read Replicas & Load Balancing**

<a name="data-archival-purging"></a>
### 22. **Data Archival & Purging**

<a name="backup-strategies"></a>
### 23. **Backup Strategies**

<a name="disaster-recovery-planning"></a>
### 24. **Disaster Recovery Planning**

<a name="database-security"></a>
### 25. **Database Security**

<a name="authentication-authorization"></a>
#### 25.1 **Authentication & Authorization**

<a name="encryption"></a>
#### 25.2 **Encryption**

<a name="auditing-compliance"></a>
#### 25.3 **Auditing & Compliance**

<a name="document-stores-mongodb"></a>
### 26. **Document Stores (MongoDB)**

<a name="key-value-stores-redis"></a>
### 27. **Key-Value Stores (Redis)**

<a name="column-stores-cassandra"></a>
### 28. **Column Stores (Cassandra)**

<a name="graph-databases-neo4j"></a>
### 29. **Graph Databases (Neo4j)**

<a name="newsql-databases"></a>
### 30. **NewSQL Databases**

<a name="database-clients"></a>
### 31. **Database Clients**

<a name="profiling-monitoring"></a>
### 32. **Profiling & Monitoring**

<a name="data-import-export"></a>
### 33. **Data Import/Export**

<a name="cloud-database-services"></a>
### 34. **Cloud Database Services**

**[⬆ Back to Top](#databases--persistence)**
