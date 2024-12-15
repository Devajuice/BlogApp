+++
date = '2024-12-15T18:00:19+05:30'
draft = false
title = 'Database Concepts'
description = "Database Concepts: A Foundation for Data Management"
image = "/images/I.P/DC.webp"
imageBig = "/images/I.P/DC2.webp"
categories = ["Notes", "I.P"]
author = ["Devajuice"]
avatar = "/images/avatar.webp"
+++
# Limitations of Manual Record-Keeping

1. Repetition of Data
2. Inconstancy
3. Loss of Data

# File System

- A file can be understood as a container to store data in a computer. Files can be stored on the storage device of a computer system.
- Files stored on a computer can be accessed directly and searched for desired data.

# Limitation of a File System

- File system becomes difficult to handle when the number of files increases, and the volume of data also grows.

## (A) Difficulty in Access

- Files themselves do not provide any mechanism to retrieve data.

## (B) Data Redundancy

- Redundancy means the same data are duplicated in different places (files).

## (C) Data Inconsistency

- Data inconsistency occurs when the same data maintained in different places does not match.

## (D) Data Isolation

- Data mapping is not supported in the file system.
- It is difficult to write new application programs to retrieve data from different files maintained at multiple places, as one has to understand the underlying structure of each file.

## (E) Data Dependence

- Data are stored in a specific format or structure in a file. If the structure or format itself is changed, all the existing application programs accessing that file also need to be changed.

## (F) Controlled Data Sharing

- There can be different categories of users like teachers, office staff and parents.
- This means these users should be given limited access.

# Database Management System

- Limitations faced in file systems can be overcome by storing the data in a database where data are logically related.
- A database management system (DBMS), or database system, in short, is software that can be used to create and manage databases.
- DBMS lets users create a database and store, manage, update/modify and retrieve data from that database by users or application programs.
- DBMS include MySQL, Oracle, PostgreSQL, SQL Server, Microsoft Access, and MongoDB.
- The DBMS serves as an interface between the database and end users or application programs.
- Retrieving data from a database through a special type of command is called querying the database.

  ### Difference between DBMS and RDBMS

  - DBMS stands for Database Management System, and RDBMS is the acronym for the Relational Database Management system. In DBMS, the data is stored as a file, whereas in RDBMS, data is stored in the form of tables. To know what is the difference between RDBMS and DBMS, check out the table below.

| No  |                                     RDBMS                                     |                      DBMS                      |
| :-: | :---------------------------------------------------------------------------: | :--------------------------------------------: |
| 1)  |                        Data stored is in table format                         |       Data stored is in the file format        |
| 2)  |                Multiple data elements are accessible together                 |       Individual access of data elements       |
| 3)  |                Data in the form of a table are linked together                |           No connection between data           |
| 4)  |                        Normalisation is not achievable                        |             There is normalisation             |
| 5)  |                         Support distributed database                          |      No support for distributed database       |
| 6)  |                       Data is stored in a large amount                        |        Data stored is a small quantity         |
| 7)  | Here, redundancy of data is reduced with the help of key and indexes in RDBMS |           Data redundancy is common            |
| 8)  |                         RDBMS supports multiple users                         |          DBMS supports a single user           |
| 9)  |          It features multiple layers of security while handling data          | There is only low security while handling data |
| 10) |               The software and hardware requirements are higher               | The software and hardware requirements are low |
| 11) |                            EG: Oracle, SQL Server.                            |           EG: XML, Microsoft Access.           |

# Key Concepts in DBMS

## (A) Database Schema

- Database Schema is the design of a database. It is the skeleton of the database that represents the structure (table names and their fields/columns), the type of data each column can hold, constraints on the data to be stored (if any), and the relationships among the tables.
- Database schema is also called the visual or logical architecture.

## (B) Data Constraint

- Certain restrictions or limitations on the type of data that can be inserted in one or more columns of a table.

## (C) Meta-data or Data Dictionary

- The database schema along with various constraints on the data is stored by DBMS in a database catalog or dictionary, called meta-data. A meta-data is data about the data.

## (D) Database Instance

- The state or snapshot of the database at any given time is the database instance.

## (E) Query

- A query is a request to a database for obtaining information in a desired way.

## (F) Data Manipulation

- Modification of database consists of three operations viz. Insertion, Deletion or Update. This is called Update operation on the database.

## (G) Database Engine

- Database engine is the underlying component or set of programs used by a DBMS to create database and handle various queries for data retrieval and manipulation.

# Relational Data Model

## ATTRIBUTE

- The columns of a relation are the attributes which are also referred as fields.

## TUPLE

- Each row of data in a relation (table) is called a tuple.

## DOMAIN

- It is a set of values from which an attribute can take a value in each row.

## DEGREE

- The number of attributes in a relation is called the Degree of the relation.

## CARDINALITY

- The number of tuples in a relation is called the Cardinality of the relation.

# Keys in a Relational Database

## Candidate Key

- ***Attributes*** can be used to uniquely identify the ***tuples*** in the relation. Such attributes are called ***candidate keys*** as each of them are candidates for the ***primary key***.

## Primary Key

- Out of one or more candidate keys, the attribute chosen by the database designer to uniquely identify the tuples in a relation is called the primary key of that relation.

## Composite Primary Key

- If no single attribute in a relation is able to uniquely distinguish the tuples, then more than one attribute are taken together as primary key. Such primary key consisting of more than one attribute is called Composite Primary key.

## Foreign Key

- A foreign key is used to represent the relationship between two relations. A foreign key is an attribute whose value is derived from the primary key of another relation.
