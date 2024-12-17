+++
date = '2024-12-15T11:47:05+05:30'
draft = false
title = 'Introduction To MySQL'
description = "This is a comprehensive guide to MySQL, a popular relational database management system (RDBMS). It covers the basics of databases, SQL (Structured Query Language), data types, constraints, and data manipulation techniques."
image = "/images/I.P/MySQL.webp"
imageBig = "/images/I.P/MySQL2.webp"
categories = ["I.P"]
author = ["Devajuice"]
avatar = "/images/avatar.webp"
+++
# Introduction

- Many RDBMS exist, such as [MySQL](https://www.mysql.com/), [Microsoft SQL Server](https://www.microsoft.com/en-in/sql-server/sql-server-downloads), [PostgreSQL](https://www.postgresql.org/), [Oracle](https://www.oracle.com/), etc. These allow us to create a database of relations and link one or more relations for efficient querying to store, retrieve, and manipulate data on that database.

# Structured Query Language(SQL)

- The Structured Query Language(SQL) is the most popular query language used by major relational database management systems such as [MySQL](https://www.mysql.com/), [Oracle](https://www.oracle.com/),  [SQL Server](https://www.microsoft.com/en-in/sql-server/sql-server-downloads), etc.

# Data type of Attribute

- Data type indicates the type of data value that an attribute can have. The data type of an attribute decides the operations that can be performed on the data of that attribute.

## Commonly used data types in MySQL

### 1. CHAR

- `CHAR` is of fixed length, which means declaring `CHAR(10)` implies reserving spaces for ten characters.

### 2. VARCHAR

- `VARCHAR` is a variable-length data type. Declaring `VARCHAR(30)` means a maximum of 30 characters can be stored, but the actual allocated bytes will depend on the length of the entered string.

### 3. INT

- `INT` specifies an integer value. Each `INT` value occupies ***4 bytes*** of storage. The range of values allowed in integer type are ***-2147483648*** to ***2147483647***.

### 4. FLOAT

- Holds numbers with decimal points. Each `FLOAT` value occupies ***4 bytes***.

### 5. DATE

- The `DATE` type is used for dates in the '**YYYY-MM-DD**' format. It is the four-digit year, **MM** is the two-digit month, and **DD** is the two-digit date. The supported range is '**1000-01-01**' to '**9999-12-31'**.

# Constraints

- Constraints are certain types of restrictions on the data values that an attribute can have. They are used to ensure the accuracy and reliability of data.

# SQL for Data Definition

- SQL provides commands for *defining* the *relation schemas*, *modifying relation schemas* and *deleting relations*. These are called **Data Definition Language**(**DDL**), through which the set of relations are specified, including their schema, data type for each attribute, the constraints, as well as the security and access-related authorisations.

## Create Database

```sql
CREATE DATABASE databasename;
```

- A DBMS can manage multiple databases on one computer. Therefore, we need to select the database that we want to use. Once the database is selected, we can proceed with creating tables or querying data.

```sql
USE databasename;
```

## Create Table

- After creating a database, we need to define relations(create tables) in the database and specify attributes for each relation, along with data types for each attribute. This is done using the `CREATE TABLE`

```sql
CREATE TABLE tablename(
attributename1 datatype constraint,
attributename2 datatype constraint
);
```

- The attribute name specifies the name of the column in the table.
- Datatype specifies the type of data that an attribute can hold.
- Constraint indicates the restrictions imposed on the values of an attribute. By default, each attribute can take NULL values except for the primary key.

## Describe Table

- We can view the structure of an already created table using the describe statement.

```sql
DESC tablename;
```

## Alter Table

- After creating a table, we may realise that we need to add/remove an attribute, modify the datatype of an existing attribute, or add a constraint in the attribute. In all such cases, we need to change or alter the structure of the table by using the alter statement.

```sql
ALTER TABLE tablename ADD/Modify/DROP attribute1, attribute2,.....
```

### (A) Add Primary Key to a relation

```sql
ALTER TABLE tablename ADD PRIMARY KEY(GUID);
```

### (B) Add foreign key to a relation

```sql
ALTER TABLE tablename ADD FOREIGN KEY(GUID) REFERENCES referencedtablename(attributename);
```

- The referenced relation must be already created.
- The referenced attribute must be a part of the primary key of the referenced relation.
- Data types and sizes of referenced and referencing attributes must be the same.

### (C) Add constraint *UNIQUE* to an existing attribute

```sql
ALTER TABLE tablename ADD UNIQUE(attribute name);
```

### (D) Add an attribute to an existing table

```sql
ALTER TABLE tablename ADD attribute_name DATATYPE;
```

### (E) Modify the constraint of an attribute

```sql
ALTER TABLE table_name MODIFY attribute DATATYPE NOT NULL;
```

### (F) Modify datatype of an attribute

```sql
ALTER TABLE table_name MODIFY attribute DATATYPE;
```

### (G) Add a default value to an attribute

```sql
ALTER TABLE table_name MODIFY attribute DATATYPE DEFAULT default_value;
```

### (H) Remove an attribute

```sql
ALTER TABLE table_name DROP attribute;
```

### (I) Remove the primary key from the table

```sql
ALTER TABLE table_name DROP PRIMARY KEY;
```

# Drop Statement

- Sometimes, a table in a database or the database itself needs to be removed. We can use a `DROP` statement to remove a database or a table permanently from the system.

```sql
DROP TABLE table_name;
```

# Insertion of Records

- `INSERT INTO` statement is used to insert new records in a table.

```sql
INSERT INTO table_name VALUES(value1, value2,......);
```

# SQL for Data Query

## SELECT Statement

- The SQL statement `SELECT` is used to retrieve data from the tables in a database, and the output is also displayed in a tabular form.

```sql
SELECT attribute1, attribute2,... FROM table_name WHERE condition;
```

# Data Updation

- The `UPDATE` statement is used to make such modifications in the existing data.

```sql
UPDATE table_name SET attribute1 = value1, attribute2 = value2,..... WHERE condition;
```

# Data Deletion

- The `DELETE` statement is used to delete one or more record(s) from a table.

```sql
DELETE FROM table_name WHERE condition;
```
