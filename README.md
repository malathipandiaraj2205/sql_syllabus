# sql_syllabus #

 SQL (Structured Query Language) is used to create, manage, and query relational databases. A complete learning path typically covers database fundamentals, SQL command categories, querying, joins, functions, transactions, optimization, and advanced analytical features.


**RDMS**
RDBMS (Relational Database Management System) is software used to store, organize, and manage data in the form of tables that are related to each other.

**Features of RDBMS**
Data is stored in rows and columns.
Tables can be connected using Primary Keys and Foreign Keys.
Reduces data duplication.
Supports SQL for data operations.
Maintains data integrity and security.


DBMS (Database Management System) is software that helps users create, store, manage, and retrieve data efficiently.

**Functions of DBMS**

Store data in databases
Add new data
Update existing data
Delete data
Retrieve data quickly
Provide security and backup



**SQL commands**

DDL -	Data Definition Language	-	CREATE, ALTER, DROP, TRUNCATE
DML - 	Data Manipulation Language	-	INSERT, UPDATE, DELETE
DQL -	Data Query Language - SELECT, FROM, WHERE, GROUPBY, HAVING, ORDER BY, LIMIT
DCL- Data Control Language	-	GRANT, REVOKE
TCL - Transaction Control Language	COMMIT, ROLLBACK, SAVEPOINT

**CREATE TABLE **
Creates a new table.


<img width="497" height="179" alt="{31EF9CA6-EEC2-4218-91C6-F6332A5B2D77}" src="https://github.com/user-attachments/assets/40677fc3-4484-4df3-bc37-3d535e08e07f" />

**2.ALTER**
Adds, modifies, or deletes columns.

<img width="248" height="63" alt="{C1CA06D8-7DB5-4828-A9E5-B188FC716CE9}" src="https://github.com/user-attachments/assets/6d34c6d5-0ba2-4d1d-bcd9-10d88a1490cf" />


**3. DROP**

Deletes the table permanently.


DROP TABLE Employee;

**4. TRUNCATE**

Removes all records but keeps the table structure.

TRUNCATE TABLE Employee;

**DML (Data Manipulation Language)**

DML commands are used to insert, update, delete, and retrieve data from tables.

1.INSERT	Adds new records
2.UPDATE	Modifies existing records
3.DELETE	Removes records


**1. INSERT**
<img width="339" height="44" alt="{E5E8FFA7-A543-4CC8-8C17-EE5B32668D53}" src="https://github.com/user-attachments/assets/59708a1d-6ca6-416d-a6e9-3391747ea446" />

**2. UPDATE**
<img width="152" height="65" alt="{DE14ED53-9427-4989-8A48-0026B56CE307}" src="https://github.com/user-attachments/assets/33b70bfd-6ea8-4fcd-8f8d-dcb1844147a6" />

**3. DELETE**
DELETE FROM Employee
<img width="206" height="54" alt="{B0D4BDFC-F174-4497-81B9-DB6306D06AE2}" src="https://github.com/user-attachments/assets/c9d93c33-7c5e-4e03-8d8a-5bdef19d2013" />


**DCL (Data Control Language) Commands in SQL**

DCL commands are used to control user access and permissions in a database.

Command	Purpose
GRANT	Gives privileges to a user
REVOKE	Removes privileges from a user

**1. GRANT**

The GRANT command is used to give permissions (privileges) to a user on database objects such as tables.

<img width="139" height="75" alt="{32F91343-3F05-47C3-9421-DCCAEE91FE58}" src="https://github.com/user-attachments/assets/365a0a04-91a9-4f75-98f8-5ec3b2d5fc2f" />


**2. REVOKE**

The REVOKE command is used to remove permissions (privileges) that were previously granted to a user.

<img width="140" height="82" alt="{847DB36A-C51C-4980-BCFD-8EAF1807D593}" src="https://github.com/user-attachments/assets/9e5c6fdc-56eb-4a42-9361-abe1a00e677a" />

TCL (Transaction Control Language) Commands in SQL

TCL commands are used to manage transactions in a database.

<img width="455" height="155" alt="{B1B0706F-934E-42C0-A75C-67724E06874C}" src="https://github.com/user-attachments/assets/07df132c-613e-4650-a049-42817d1124de" />

**1. COMMIT**

Saves all changes permanently.

<img width="332" height="89" alt="{714F2E65-37AE-4CAE-B166-A4171EE6E50F}" src="https://github.com/user-attachments/assets/1f572e3b-4874-4457-af01-9528cb06e458" />

**2.ROLLBACK**

Undoes changes that have not been committed

<img width="184" height="112" alt="{34A16BBD-06AD-4870-A507-02ED5A0D7DE6}" src="https://github.com/user-attachments/assets/7d5ed722-dad5-4103-a59c-c00d3beaccd4" />

**3.SAVEPOINT**

Creates a savepoint within a transaction.

<img width="390" height="64" alt="{0529A867-1869-411F-A98B-5F7F230844FC}" src="https://github.com/user-attachments/assets/44a82aa2-7040-4635-863f-c1a862bf28f8" />






