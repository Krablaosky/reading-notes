# Data Modeling

## [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

1. What type of database is the best fit for the complex query intensive environment?
In a complex query-intensive environment, where there is a need to perform advanced and intricate queries on large datasets, SQL databases are often a better fit. SQL (Structured Query Language) databases, also known as relational databases, excel in handling complex relationships between data and support powerful query languages. They are designed to efficiently process complex joins, aggregations, and data manipulations. SQL databases use tables with predefined schemas, ensuring data integrity and consistency. Examples of popular SQL databases include MySQL, PostgreSQL, and Oracle.

2. What type of database is the best fit for hierarchical data storage?
For hierarchical data storage, where data is organized in a tree-like structure or nested relationships, NoSQL databases are often the best fit. NoSQL (Not only SQL) databases offer flexible data models that can handle hierarchical data more efficiently than traditional SQL databases. They allow for the storage of unstructured or semi-structured data without strict schemas, which makes them well-suited for scenarios like storing JSON or XML documents. NoSQL databases provide various models like key-value, document, columnar, and graph databases, among which document databases like MongoDB and Couchbase are commonly used for hierarchical data storage.

3. Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

SQL databases scale vertically by adding more powerful hardware, like expanding a library's shelves. NoSQL databases scale horizontally by adding more servers, like adding modular libraries.

## [sql modeling techniques](https://www.essentialsql.com/get-ready-to-learn-sql-7-simplified-data-modeling/)

1.  Among data tables, what is a one-to-many relationship and how do we “relate” them?

A one-to-many relationship is a type of relationship between two tables in a relational database. It means that one record in the first table can be associated with multiple records in the second table, but each record in the second table is associated with only one record in the first table. To "relate" them, you establish a foreign key in the table representing the "many" side. The foreign key refers to the primary key of the table representing the "one" side, creating a connection between the two tables.

2. Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.

Prior to designing your relational database, it might be useful to create a diagram of the database tables and their relationships. This diagram, known as an entity-relationship diagram (ER diagram), visually represents the tables and their relationships, helping you understand the structure and dependencies of the database. It serves as a blueprint for designing the database and guides the creation of tables, fields, and their relationships.

3. Explain the difference between a primary and foreign key.

A primary key is a unique identifier for each record in a table. It helps identify and access specific records in the table.

A foreign key is a field in a table that links to the primary key of another table. It establishes a relationship between the tables and ensures data consistency.

## [sql vs nosql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

1. How do we treat keywords and parameters differently in SQL syntax?

In SQL syntax, we treat keywords and parameters differently. Keywords are predefined words in the SQL language that have specific meanings and functions, such as SELECT, INSERT, or WHERE. They are used to specify the type of operation we want to perform on the data. Parameters, on the other hand, are values that we pass into the SQL statement to provide specific information for the operation. Parameters are typically used for filtering data, defining conditions, or inserting values into the database. They allow us to make the SQL statement more dynamic and adaptable to different scenarios.

2. Define normalization within the context of schemas and data.

Normalization, within the context of schemas and data, refers to the process of organizing and structuring a relational database in such a way that minimizes redundancy and improves data integrity. It involves breaking down a database into multiple tables and establishing relationships between them. The goal of normalization is to eliminate data duplication and dependency issues, ensuring that each piece of data is stored in the most appropriate place and that updates or modifications to the data are done efficiently and consistently. Normalization follows a set of rules or normal forms to ensure the optimal design of the database schema.

3. Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

One-to-one relationship: Imagine a person and their passport. In a one-to-one relationship, one person can have only one passport, and one passport belongs to only one person. It's like a unique pairing between two entities.

One-to-many relationship: Think of a company and its employees. In a one-to-many relationship, one company can have many employees, but each employee belongs to only one company. It's like a hierarchical structure where one entity (company) has multiple related entities (employees).

Many-to-many relationship: Consider students and courses. In a many-to-many relationship, multiple students can enroll in multiple courses, and each course can have multiple students. It's like a flexible association where many entities on one side can be related to many entities on the other side.

These relationships help recruiters understand the nature of data associations and how different entities are connected in a database.

## [Back](../401readingNotes.md)