# -SQL-vs-No-SQL-
Comparision of Mysql vs MongoDB


## Abstract

As technology continues to evolve, the methods for storing data have also advanced. Initially, relational databases dominated the field, but ongoing research and development have introduced various storage technologies, including non-relational databases. This survey aims to provide a comprehensive understanding of the differences between relational and non-relational databases, offering a quantitative and qualitative analysis to highlight those distinctions.

## 1. Introduction

The primary objective of this project is to compare MySQL, a relational database, with No-SQL databases like Cassandra and MongoDB. This comparison is crucial for making informed decisions when selecting a database for an application.

### 1.1 SQL Databases

SQL (Structured Query Language) databases are based on tuple calculus and relational algebra. They use tables and columns to store data and ensure properties like atomicity, consistency, isolation, and durability.

- **Atomicity**: Ensures that transactions must be completed effectively or rolled back entirely.
- **Consistency**: The database should be consistent before and after a transaction.
- **Isolation**: Each transaction is treated as a distinct entity with no overlap between two transactions.
- **Durability**: All transaction modifications are permanent.

### 1.2 No-SQL Databases

No-SQL databases do not follow the relational model and are schema-less. They encompass various models, including document stores, graph databases, wide columns, and key-value stores. These databases adhere to the CAP theorem (Consistency, Availability, Partition Tolerance).

### 1.3 CAP Theorem

The CAP theorem states that a distributed store cannot provide more than two of the three desirable features (Consistency, Availability, Partition Tolerance). It introduces trade-offs in distributed systems.

- **Consistency**: All clients see the same data at the same time, regardless of the connected node.
- **Availability**: The system is always available, even if some nodes are offline.
- **Partition Tolerance**: The system continues to function despite network partitions.

## 2. Advantages of SQL Database

Some advantages of SQL databases include:

- Interactivity with multiple data views
- Minimal coding skills required
- A standardized language
- Fast query processing
- Portability
  
## 3. Advantages of No-SQL

Advantages of No-SQL databases include:

- Storage of unstructured, semi-structured, and structured data
- High scalability and availability
- High flexibility
- Open source

## 4. Graph Database

Graph databases are used for navigating relationships, storing entities in nodes and relations on edges. They find applications in social media, recommendation engines, and fraud detection.

## 5. Key-Value Store

A key-value store is a type of non-relational database that stores data using a simple key-value method. Each key is associated with a unique value, allowing efficient data retrieval.

## 6. Comparison of Databases

### 6.1 My-SQL

MySQL is an open-source relational database management system known for its ease of use with Java and broad adoption.

#### 6.1.1 Architecture of MySQL

MySQL architecture consists of several essential components, including connectors, clients, query cache, parser, optimizer, storage engine, and file system-level storage. These components work together to manage data storage and retrieval efficiently.

#### 6.1.2 Backup and Recovery in MySQL

MySQL offers various backup and recovery options, including physical and logical backups. It provides methods for choosing what data to backup and using tools like mysqldump for backups. Point-in-time recovery is also supported.

#### 6.1.3 Security in MySQL

Security in MySQL involves handling passwords securely, detecting unauthorized requests, preventing SQL injections, and managing access controls. Encrypted connections are used to protect data during transmission.

#### 6.1.4 Advantages of MySQL

MySQL offers several advantages, including support for multiple platforms, ease of administration, open-source nature, ACID compliance, and support for high availability techniques.

#### 6.1.5 Disadvantages of MySQL

MySQL has some limitations, such as fewer features in the open-source version, limited efficiency in text searches for large datasets, and challenges with complex queries on extensive data.

#### 6.1.6 CRUD Operations in MySQL

MySQL supports CRUD (Create, Read, Update, Delete) operations for managing data. These operations are performed using SQL queries.

### 6.2 Apache Cassandra

Apache Cassandra is a wide-column store non-relational distributed database known for its scalability and fault tolerance.

#### 6.2.1 Cassandra Architecture

Cassandra's architecture includes clusters, nodes, and keyspaces. Keyspaces contain column families, and nodes can be distributed across different physical locations while maintaining data consistency.

#### 6.2.2 Keyspace

Keyspaces in Cassandra are comparable to databases in relational databases. They define attributes like replication factor and replication placement strategy. Column families and primary keys are created within keyspaces.

#### 6.2.3 Wide-Column Store

Cassandra uses a wide-column store data model, allowing variable columns in each row. Rows are grouped by a partition key, and this schema flexibility supports efficient storage and retrieval of complex data.

#### 6.2.4 Peer-to-Peer Distribution

Cassandra employs a peer-to-peer distribution model, enabling horizontal scalability and eliminating single points of failure. Nodes communicate using the gossip protocol to detect failures and maintain data consistency.

#### 6.2.5 Gossip Protocol

The gossip protocol facilitates failure detection in Cassandra by enabling nodes to exchange information about their status. If a node fails to respond, it triggers hinted handoff for data synchronization.

#### 6.2.6 Anti Entropy Read-Repair

Anti entropy read-repair is a manual mechanism for data synchronization in Cassandra. Nodes compare their Merkle trees to identify and repair data inconsistencies, ensuring data availability and consistency.

#### 6.2.7 CRUD Operations in Cassandra

Cassandra supports CRUD operations, including Create, Read, Update, and Delete, using the Cassandra Query Language (CQL).

### 6.3 MongoDB

MongoDB is an open-source, high-performance, No-SQL database known for its flexibility and document-based data model.

#### 6.3.1 Data Model

MongoDB operates with databases, collections, and documents. It is schema-free, and documents can have dynamic structures.

#### 6.3.2 Terminologies Comparison

MongoDB terminology differs from traditional RDBMS, with databases, collections, documents, and fields playing analogous roles.

#### 6.3.3 CRUD Operations in MongoDB

MongoDB supports CRUD operations using a document-based approach, including Create, Read, Update, and Delete.

#### 6.3.4 Advantages of MongoDB

MongoDB offers advantages such as scalability, availability, document-based query language, and the ability to handle unstructured and semi-structured data efficiently.

## 7 Conclusion

When choosing between SQL and No-SQL databases, consider factors such as data structure, query requirements, and scalability needs. Both SQL and No-SQL databases have their strengths and weaknesses, and the choice depends on the specific application and use case.

