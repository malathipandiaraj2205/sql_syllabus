# sql_syllabus

Module 1: Database Fundamentals
What is SQL?
SQL (Structured Query Language) is used to create, manage, and query relational databases. A complete learning path typically covers database fundamentals, SQL command categories, querying, joins, functions, transactions, optimization, and advanced analytical features.


##RDMS##
RDBMS (Relational Database Management System) is software used to store, organize, and manage data in the form of tables that are related to each other.

##Features of RDBMS##
Data is stored in rows and columns.
Tables can be connected using Primary Keys and Foreign Keys.
Reduces data duplication.
Supports SQL for data operations.
Maintains data integrity and security.


DBMS (Database Management System) is software that helps users create, store, manage, and retrieve data efficiently.

##Functions of DBMS##
Store data in databases
Add new data
Update existing data
Delete data
Retrieve data quickly
Provide security and backup



SQL commands are mainly divided into 5 categories:

Category	Full Form	Purpose	Examples
DDL -	Data Definition Language	-	CREATE, ALTER, DROP, TRUNCATE
DML - 	Data Manipulation Language	-	INSERT, UPDATE, DELETE
DQL -	Data Query Language - SELECT, FROM, WHERE, GROUPBY, HAVING, ORDER BY, LIMIT
DCL- Data Control Language	-	GRANT, REVOKE
TCL - Transaction Control Language	COMMIT, ROLLBACK, SAVEPOINT

1. CREATE TABLE

Creates a new table.

CREATE TABLE Student (
    StudentID INT PRIMARY KEY,
    Name VARCHAR(50),
    Age INT
);






