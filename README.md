# Java Core & JVM Internals

### Table of Contents

<details open>
<summary>Show/Hide Table of Contents</summary>

| No. | Section & Topics                                                                                     |
| ----|-----------------------------------------------------------------------------------------------------|
|      | **Java Language Fundamentals & Advanced Features**                                                  |
| 1    | [Core Syntax and Constructs](#core-syntax-and-constructs)                                           |
| 2    | [Generics](#generics)                                                                               |
| 3    | [Annotations](#annotations)                                                                         |
| 4    | [Enums](#enums)                                                                                     |
| 5    | [Records & Sealed Classes (Java 14+)](#records--sealed-classes-java-14)                             |
| 6    | [Functional Programming](#functional-programming)                                                   |
| 7    | [Modules (Java 9+)](#modules-java-9)                                                                 |
|      | **Concurrency & Multithreading**                                                                    |
| 8    | [Thread Basics](#thread-basics)                                                                     |
| 9    | [Synchronization](#synchronization)                                                                 |
| 10   | [Java Memory Model](#java-memory-model)                                                             |
| 11   | [Executors Framework](#executors-framework)                                                         |
| 12   | [Advanced Concurrency Utilities](#advanced-concurrency-utilities)                                   |
| 13   | [CompletableFuture & Reactive Programming](#completablefuture--reactive-programming)               |
|      | **Collections Framework & Data Structures**                                                         |
| 14   | [Core Interfaces](#core-interfaces)                                                                 |
| 15   | [Implementations](#implementations)                                                                 |
| 16   | [Performance Characteristics](#performance-characteristics)                                         |
| 17   | [Custom Collections](#custom-collections)                                                           |
| 18   | [Collections Utilities](#collections-utilities)                                                     |
|      | **Exception Handling & Best Practices**                                                             |
| 19   | [Checked vs Unchecked Exceptions](#checked-vs-unchecked-exceptions)                                 |
| 20   | [Creating Custom Exceptions](#creating-custom-exceptions)                                           |
| 21   | [Try-with-resources](#try-with-resources)                                                           |
| 22   | [Exception Propagation and Handling Strategies](#exception-propagation-and-handling-strategies)     |
|      | **JVM Architecture & Execution Model**                                                              |
| 23   | [JVM Components](#jvm-components)                                                                   |
| 24   | [Bytecode Execution](#bytecode-execution)                                                           |
| 25   | [Class Loading Mechanics](#class-loading-mechanics)                                                 |
|      | **Memory Management & Garbage Collection (GC)**                                                     |
| 26   | [Heap Structure](#heap-structure)                                                                   |
| 27   | [GC Algorithms](#gc-algorithms)                                                                     |
| 28   | [Tuning & Monitoring](#tuning--monitoring)                                                          |
| 29   | [Memory Leaks & Profiling](#memory-leaks--profiling)                                                |
|      | **Performance Optimization & Profiling**                                                            |
| 30   | [JIT Compilation](#jit-compilation)                                                                 |
| 31   | [Escape Analysis](#escape-analysis)                                                                 |
| 32   | [Inlining, Loop Unrolling, Dead Code Elimination](#inlining-loop-unrolling-dead-code-elimination)   |
| 33   | [Benchmarking](#benchmarking)                                                                       |
| 34   | [Profiling Tools](#profiling-tools)                                                                 |
| 35   | [Heap Dumps and Thread Dumps](#heap-dumps-and-thread-dumps)                                         |
|      | **Class Loading & Reflection**                                                                      |
| 36   | [ClassLoaders](#classloaders)                                                                       |
| 37   | [Reflection API](#reflection-api)                                                                   |
| 38   | [Use Cases & Performance Implications](#use-cases--performance-implications)                        |
| 39   | [Method Handles & InvokeDynamic](#method-handles--invokedynamic)                                    |
|      | **Serialization & Deserialization**                                                                 |
| 40   | [Java Serialization](#java-serialization)                                                           |
| 41   | [Custom Serialization](#custom-serialization)                                                       |
| 42   | [Alternatives](#alternatives)                                                                       |
| 43   | [Security Concerns](#security-concerns)                                                             |
|      | **Modules & Packaging (Java 9+)**                                                                   |
| 44   | [Java Platform Module System (JPMS)](#java-platform-module-system-jpms)                             |
| 45   | [Modularity Benefits](#modularity-benefits)                                                         |
| 46   | [Migrating Legacy Apps to Modules](#migrating-legacy-apps-to-modules)                               |

</details>
