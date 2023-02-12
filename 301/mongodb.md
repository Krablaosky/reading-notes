# MongoDB & Mongoose

## [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
Fill in the chart below with five differences between SQL and NoSQL databases:

| SQL  | NoSQL  |
|---|---|
| Relational Databases  | Non-Relational Database  |
| Table Based Data  | Document Base, Key-Value pairs  |
| Predefined Schema  | Dynamic Schema  |
| Vertically Scalable  | Horizontally Scalable  | 	 
 	  	 
1. What kind of data is a good fit for an SQL database?

complex queries are the best for SQL databases 

2. Give a real world example.

a good example of a type of data that would fit into an SQL database would be a retail store that has lots of different products and items that have a few categories that aren't going to change too frequently

3. What kind of data is a good fit a NoSQL database?

the best kind of data for a no SQL database would be a database with hierarchical data storage, as it follows key value pairs similar to JSON files

4. Give a real world example.

a nosql database would be really great for use in terms of data that matches customer ID's and order ID for an online website

5. Which type of database is best for hierarchical data storage?

nosql databases are preferred for large data sets that use key value pairs as a way to store similar data.

6. Which type of database is best for scalability?

It depends on the type of scalability you're going for, SQL databases are vertically scalable and you can manage increasing load by increasing hardware inside of the computer or the server.No SQL databases are horizontally scalable You can just add a few more servers in your database infrastructure to handle large traffic

## [SQL vs NoSQL Video](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

1. What does SQL stand for?

SQL stands for structured query language

2. What is a relational database?

A relational database is a type of database that stores data in a structured manner, using tables with rows and columns to represent data records and their relationships to one another. In a relational database, each table represents a separate entity (such as customers, orders, or products) and the relationships between entities are defined through the use of keys and foreign keys.

3. What type of structure does a relational database work with?

A relational database works with a tabular structure, where data is stored in tables made up of rows and columns. 

4. What is a ‘schema’?

A schema is a blueprint or structure that defines the organization of data in a relational database. A schema specifies the names, types, and constraints of columns in each table, as well as the relationships between tables.

5. What is a NoSQL database?

NoSQL databases are a type of database management system that do not use the traditional relational model to store data. 

6. How does it work?

Unlike relational databases, which use tables with rows and columns to represent data records and their relationships, NoSQL databases use a variety of data structures to store data, including key-value pairs, document-based, graph-based, and column-based.

7. What is inside of a MongoDB database?

A MongoDB database consists of a collection of documents. Each document is a unit of data that can be thought of as a row in a table of a relational database. Documents in MongoDB are stored in a binary representation called BSON (Binary JSON), which allows for the storage of rich, complex data types and structures.

8. Which is more flexible - SQL or MongoDB? and why.

MongoDB seems to be more flexible than SQL even though they each have their own strengths and weaknesses. Documents in MongoDB can have different structures, allowing for greater flexibility in the data model. This makes it easier to accommodate changes to the data structure over time, as well as to store complex, hierarchical data structures. However, this flexibility can also make it more difficult to enforce data integrity and consistency, as the schema is not defined up front and is more flexible.

9. What is the disadvantage of a NoSQL database?

NoSQL databases have several disadvantages, including:

Lack of standardization: Unlike SQL databases, which have a standardized language (SQL) for querying and manipulating data, NoSQL databases have a diverse set of query languages, making it more difficult to write and maintain database code.

Lack of transactions: Many NoSQL databases do not support transactions, which are a critical feature for ensuring data consistency and integrity in applications that require multiple database operations to be executed as a single, atomic unit.

Limited data relationships: NoSQL databases typically do not support complex relationships between data elements, making it more difficult to model and manage complex data structures.

Performance issues: NoSQL databases are optimized for fast read and write operations, but can suffer from performance degradation when querying and aggregating large amounts of data.

Learning curve: NoSQL databases have a different data model and set of query and management tools compared to SQL databases, and developers and administrators may need to invest time and effort in learning these new technologies.

