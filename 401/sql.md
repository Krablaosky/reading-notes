# SQL Notes

SQL (Structured Query Language) is a programming language used to manage and manipulate data in a relational database. A relational database is a collection of related data tables that are organized according to specific rules and relationships.

In a relational database, each table contains rows and columns (also called fields). The rows represent individual instances of data, while the columns represent specific attributes of that data. The relationships between tables are defined by shared keys or common columns.

SQL is used to create, update, and retrieve data from these tables, and it provides a standardized way of interacting with relational databases across different platforms and systems. SQL commands can be used to perform various operations such as selecting specific data, sorting and grouping data, updating and deleting data, and creating and modifying database objects such as tables, views, and indexes.

Relational databases and SQL are widely used in a variety of industries and applications, including finance, healthcare, e-commerce, and more. They provide a powerful and flexible way to store and manage large amounts of data, and their standardization and ubiquity make them accessible to developers and organizations around the world.

## SQL Cheat Sheet

SELECT Statement:

Retrieve data from one or more tables
Syntax: SELECT column1, column2, ... FROM table_name;
WHERE Clause:

Filter data based on a condition
Syntax: SELECT column1, column2, ... FROM table_name WHERE condition;
ORDER BY Clause:

Sort data in ascending or descending order
Syntax: SELECT column1, column2, ... FROM table_name ORDER BY column_name ASC|DESC;
JOIN Clause:

Combine data from two or more tables based on a related column
Syntax: SELECT column1, column2, ... FROM table1 JOIN table2 ON table1.column_name = table2.column_name;
GROUP BY Clause:

Group data based on a column and perform aggregate functions (SUM, AVG, COUNT, etc.) on each group
Syntax: SELECT column1, aggregate_function(column2) FROM table_name GROUP BY column1;
HAVING Clause:

Filter data after grouping has been applied
Syntax: SELECT column1, aggregate_function(column2) FROM table_name GROUP BY column1 HAVING condition;
INSERT Statement:

Insert new data into a table
Syntax: INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...);
UPDATE Statement:

Modify existing data in a table
Syntax: UPDATE table_name SET column1 = value1, column2 = value2, ... WHERE condition;
DELETE Statement:

Remove data from a table
Syntax: DELETE FROM table_name WHERE condition;


## SQL examples


SELECT Statement:
Example: SELECT name, age FROM customers;

WHERE Clause:
Example: SELECT name, age FROM customers WHERE age > 30;

ORDER BY Clause:
Example: SELECT name, age FROM customers ORDER BY age DESC;

JOIN Clause:
Example: SELECT customers.name, orders.order_date FROM customers JOIN orders ON customers.id = orders.customer_id;

GROUP BY Clause:
Example: SELECT category, SUM(price) FROM products GROUP BY category;

HAVING Clause:
Example: SELECT category, SUM(price) FROM products GROUP BY category HAVING SUM(price) > 1000;

INSERT Statement:
Example: INSERT INTO customers (name, age) VALUES ('John Smith', 35);

UPDATE Statement:
Example: UPDATE customers SET age = 36 WHERE name = 'John Smith';

DELETE Statement:
Example: DELETE FROM customers WHERE name = 'John Smith';

## SQL Completion

1. ![SQL: 1](img/sql%201.png)
2. ![SQL: 2](img/sql%202.png)
3. ![SQL: 3](img/SQL%203.png)
4. ![SQL: 4](img/SQL%204.png)
5. ![SQL: 5](img/SQL%205.png)
6. ![SQL: 6](img/SQL%206.png)
13. ![SQL: 13](img/SQl%2013.png)
14. ![SQL: 14](img/SQL%2014.png)
15. ![SQL: 15](img/SQL%2015.png)
16. ![SQL: 16](img/SQL%2016.png)
17. ![SQL: 17](img/SQL%2017.png)
18. ![SQL: 18](img/SQL%2018.png)