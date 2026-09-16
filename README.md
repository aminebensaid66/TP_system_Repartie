# Distributed Systems Labs

Java coursework exploring message-oriented middleware and relational-database access.

## Contents

### TP1 — RabbitMQ messaging

Examples of point-to-point queues and direct-exchange routing using the RabbitMQ Java client:

- Basic producer and consumer
- Queue declaration and message publishing
- Direct exchange with routing keys
- Multiple log consumers

### TP2 — JDBC and MySQL

Examples of database retrieval and parameterized SQL statements using MySQL Connector/J.

## Requirements

- Java 17+
- RabbitMQ running locally for TP1
- MySQL and an appropriate local schema for TP2

The required client JARs are currently stored under each lab's `lib/` directory.

## Run

Compile from the relevant lab directory with its dependencies on the classpath. Start consumers before producers when testing RabbitMQ messaging.

These exercises use local default connections and may require host, database, and credential changes for your environment. Do not commit real database credentials.

## Learning goals

- Understand asynchronous producer/consumer communication
- Compare queues with exchange-based routing
- Work with AMQP connections and channels
- Use JDBC safely with prepared statements
- Separate infrastructure configuration from application logic

## Status

Educational repository. Compiled `.class` files and dependency JARs are retained from the original lab environment; a future cleanup should replace them with a Maven or Gradle build and ignore generated artifacts.
