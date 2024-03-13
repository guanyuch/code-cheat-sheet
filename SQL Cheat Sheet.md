# **SQL Cheat Sheet**

## **Basic Commands**

#### Create a new database
- `CREATE DATABASE database_name;`

#### Delete a database
- `DROP DATABASE database_name;`

#### Create a new table
- `CREATE TABLE table_name (column1 datatype, column2 datatype, ...);`

#### Delete a table
- `DROP TABLE table_name;`

#### Insert a single row into a table
- `INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...);`

#### Insert multiple rows into a table
- `INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...), (value3, value4, ...), ...;`

#### Select all columns from a table
- `SELECT * FROM table_name;`

#### Select specific columns from a table
- `SELECT column1, column2 FROM table_name;`

#### Update rows in a table
- `UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;`

#### Delete rows from a table
- `DELETE FROM table_name WHERE condition;`

## **Query Modifiers**

#### Filter results using a condition
- `SELECT * FROM table_name WHERE condition;`

#### Sort results by a column (ASCending or DESCending)
- `SELECT * FROM table_name ORDER BY column ASC|DESC;`

#### Limit the number of returned results
- `SELECT * FROM table_name LIMIT number;`

#### Count the number of rows that match a condition
- `SELECT COUNT(*) FROM table_name WHERE condition;`

#### Find the minimum/maximum value of a column
- `SELECT MIN(column) FROM table_name;`
- `SELECT MAX(column) FROM table_name;`

#### Calculate the sum of a column
- `SELECT SUM(column) FROM table_name;`

#### Calculate the average value of a column
- `SELECT AVG(column) FROM table_name;`

#### Group rows that have the same values in specified columns into summary rows
- `SELECT column, AGG_FUNC(column) FROM table_name GROUP BY column;`

#### Filter groups with HAVING
- `SELECT column, AGG_FUNC(column) FROM table_name GROUP BY column HAVING condition;`

## **Join Operations**

#### Inner join
- `SELECT columns FROM table1 INNER JOIN table2 ON table1.column = table2.column;`

#### Left (outer) join
- `SELECT columns FROM table1 LEFT JOIN table2 ON table1.column = table2.column;`

#### Right (outer) join
- `SELECT columns FROM table1 RIGHT JOIN table2 ON table1.column = table2.column;`

#### Full (outer) join
- `SELECT columns FROM table1 FULL OUTER JOIN table2 ON table1.column = table2.column;`

## **Advanced Operations**

#### Subquery
- `SELECT column FROM (SELECT column FROM table) AS subquery;`

#### UNION operation to combine results of two queries
- `SELECT column FROM table1 UNION SELECT column FROM table2;`

#### Create index on a column
- `CREATE INDEX index_name ON table_name (column);`

#### Drop index
- `DROP INDEX index_name;`
