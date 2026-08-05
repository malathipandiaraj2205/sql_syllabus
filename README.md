# sql_syllabus #

 SQL (Structured Query Language) is used to create, manage, and query relational databases. A complete learning path typically covers database fundamentals, SQL command categories, querying, joins, functions, transactions, optimization, and advanced analytical features.


## RDBMS (Relational Database Management System):

 RDMS is software used to store, organize, and manage data in the form of tables that are related to each other.

**Features of RDBMS:

    ● Tables can be connected using Primary Keys and Foreign Keys.

    ● Reduces data duplication.

    ● Supports SQL for data operations.

    ● Maintains data integrity and security.


##DBMS (Database Management System):

DBMS is software that helps users create, store, manage, and retrieve data efficiently.

##Functions of DBMS:

    ● Store data in databases
    ● Add new data
    ● Update existing data
    ● Delete data
    ● Retrieve data quickly
    ● Provide security and backup


## SQL commands:

    1     DDL 	       Data Definition Language	       	   CREATE, ALTER, DROP, TRUNCATE
    2     DML  	      Data Manipulation Language		        INSERT, UPDATE, DELETE
    3     DQL	        Data Query Language                 SELECT, FROM, WHERE, GROUPBY, HAVING, ORDER BY, LIMIT
    4     DCL         Data Control Language		             GRANT, REVOKE
    5     TCL         Transaction Control Language	       COMMIT, ROLLBACK, SAVEPOINT

1. ## DDL (Data Definition Language): 

DDL is a category of SQL commands used to define and modify the structure of database objects such as tables, views, and schemas.

DDL Commands
       Command                        	                 Purpose
       CREATE	                       Creates a new database object (table, view, etc.)
       ALTER                        	Modifies an existing database object
       DROP	                         Deletes a database object permanently
       TRUNCATE	                     Removes all records from a table
       RENAME	                       Changes the name of a database object

    
## CREATE: 

The CREATE command is used to create a new database object such as a table, database, view, or index.

Creates a new table.


<img width="497" height="179" alt="{31EF9CA6-EEC2-4218-91C6-F6332A5B2D77}" src="https://github.com/user-attachments/assets/40677fc3-4484-4df3-bc37-3d535e08e07f" />

## ALTER:

Adds, modifies, or deletes columns.

<img width="248" height="63" alt="{C1CA06D8-7DB5-4828-A9E5-B188FC716CE9}" src="https://github.com/user-attachments/assets/6d34c6d5-0ba2-4d1d-bcd9-10d88a1490cf" />


## DROP: 

Deletes the table permanently.

<img width="196" height="28" alt="{998CC7D2-E3D7-4D7B-B075-D2BE4312C8AF}" src="https://github.com/user-attachments/assets/6c3add11-0f19-407e-948c-47504154a415" />

## TRUNCATE:

Removes all records but keeps the table structure.

<img width="232" height="42" alt="{436486D4-8DD3-4274-8B8E-E28767E4EBEB}" src="https://github.com/user-attachments/assets/f39d5008-b9d3-4571-8352-eac46a1f6b60" />


2.## DML (Data Manipulation Language)

DML commands are used to insert, update, delete, and retrieve data from tables.

DML Commands
             Commands                    Purposes
             INSERT       	    Adds new records to a table
             UPDATE	           Modifies existing records
             DELETE       	    Removes records from a table
            	           

## INSERT:

Syntax:

INSERT INTO table_name (column1, column2, column3)
VALUES (value1, value2, value3);

Example:

<img width="444" height="61" alt="{D608C52A-8C06-4A93-94E2-A18BDD16E3FC}" src="https://github.com/user-attachments/assets/43096a9a-73dc-432a-a026-97874c84acfb" />


## UPDATE:

The UPDATE command is used to modify existing records in a table.

Syntax

UPDATE table_name
SET column1 = value1, column2 = value2
WHERE condition;

Example:

<img width="170" height="80" alt="{DBE0B2B7-4A44-437A-8ABD-72122BD58E29}" src="https://github.com/user-attachments/assets/d35abed5-e94f-41e4-a16e-0ccd6e29cf60" />

## DELETE:

The DELETE command is used to remove records (rows) from a table.

# Syntax

DELETE FROM Student
WHERE Student_ID = 101;

Example 1: Delete a Specific Employee

<img width="157" height="52" alt="{E4ED2EA7-C551-42D7-90F6-3A5290CCCAAE}" src="https://github.com/user-attachments/assets/961831bc-0885-4349-a513-0b2a643443b3" />

Example 2: Delete All Records from Employees Table

# Syntax

DELETE FROM employees;

Verify the Deletion:

SELECT * FROM employees;

3. ## DCL (Data Control Language) :

DCL commands are used to control user access and permissions in a database.

        Command	                           Purpose
          GRANT	                   Gives privileges to a user
          REVOKE           	       Removes privileges from a user

 ## GRANT:

The GRANT command is used to give permissions (privileges) to a user on database objects such as tables.

Syntax

GRANT privilege_name
ON table_name
TO user_name;

<img width="139" height="75" alt="{32F91343-3F05-47C3-9421-DCCAEE91FE58}" src="https://github.com/user-attachments/assets/365a0a04-91a9-4f75-98f8-5ec3b2d5fc2f" />


## REVOKE:

The REVOKE command is used to remove permissions (privileges) that were previously granted to a user.

Syntax

REVOKE privilege_name
ON table_name
FROM user_name;

<img width="140" height="82" alt="{847DB36A-C51C-4980-BCFD-8EAF1807D593}" src="https://github.com/user-attachments/assets/9e5c6fdc-56eb-4a42-9361-abe1a00e677a" />

4. ## TCL (Transaction Control Language) Command:

TCL commands are used to manage transactions in a database.

TCL Commands
                    Command	                               Purpose
                   COMMIT	                   Saves all changes permanently
                   ROLLBACK	                 Undoes changes since the last COMMIT
                   SAVEPOINT	                Creates a point within a transaction to roll back to

<img width="455" height="155" alt="{B1B0706F-934E-42C0-A75C-67724E06874C}" src="https://github.com/user-attachments/assets/07df132c-613e-4650-a049-42817d1124de" />

## COMMIT:

Saves all changes permanently.

Syntex

COMMIT;

<img width="332" height="89" alt="{714F2E65-37AE-4CAE-B166-A4171EE6E50F}" src="https://github.com/user-attachments/assets/1f572e3b-4874-4457-af01-9528cb06e458" />

## ROLLBACK:

The ROLLBACK command is a TCL (Transaction Control Language) command used to undo changes made during the current transaction before a COMMIT is issued.

Syntax

ROLLBACK;

<img width="182" height="90" alt="{BE03AFE0-A07D-4B82-B001-FF9EDBA01E07}" src="https://github.com/user-attachments/assets/b583c626-9dcb-4ba7-8a06-cb7a3cf00e1a" />


## SAVEPOINT:

The SAVEPOINT command is a TCL (Transaction Control Language) command used to create a point within a transaction. You can later roll back to that point without undoing the entire transaction.

Syntax

SAVEPOINT savepoint_name;

<img width="390" height="64" alt="{0529A867-1869-411F-A98B-5F7F230844FC}" src="https://github.com/user-attachments/assets/44a82aa2-7040-4635-863f-c1a862bf28f8" />

5. ## DQL (Data Query Language):

DQL is used to retrieve (fetch) data from a database.

SELECT

Syntax


