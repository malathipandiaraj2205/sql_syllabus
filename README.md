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

## DDL (Data Definition Language): 

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


**DML (Data Manipulation Language)**

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

<img width="152" height="65" alt="{DE14ED53-9427-4989-8A48-0026B56CE307}" src="https://github.com/user-attachments/assets/33b70bfd-6ea8-4fcd-8f8d-dcb1844147a6" />

## DELETE:
DELETE FROM Employee

<img width="206" height="54" alt="{B0D4BDFC-F174-4497-81B9-DB6306D06AE2}" src="https://github.com/user-attachments/assets/c9d93c33-7c5e-4e03-8d8a-5bdef19d2013" />


## DCL (Data Control Language) :

DCL commands are used to control user access and permissions in a database.

        Command	                           Purpose
          GRANT	                   Gives privileges to a user
          REVOKE           	       Removes privileges from a user

 ## GRANT:

The GRANT command is used to give permissions (privileges) to a user on database objects such as tables.

<img width="139" height="75" alt="{32F91343-3F05-47C3-9421-DCCAEE91FE58}" src="https://github.com/user-attachments/assets/365a0a04-91a9-4f75-98f8-5ec3b2d5fc2f" />


## REVOKE:

The REVOKE command is used to remove permissions (privileges) that were previously granted to a user.

<img width="140" height="82" alt="{847DB36A-C51C-4980-BCFD-8EAF1807D593}" src="https://github.com/user-attachments/assets/9e5c6fdc-56eb-4a42-9361-abe1a00e677a" />

TCL (Transaction Control Language) Command:

TCL commands are used to manage transactions in a database.

TCL Commands
                    Command	                               Purpose
                   COMMIT	                   Saves all changes permanently
                   ROLLBACK	                 Undoes changes since the last COMMIT
                   SAVEPOINT	                Creates a point within a transaction to roll back to

<img width="455" height="155" alt="{B1B0706F-934E-42C0-A75C-67724E06874C}" src="https://github.com/user-attachments/assets/07df132c-613e-4650-a049-42817d1124de" />

## COMMIT:

Saves all changes permanently.

<img width="332" height="89" alt="{714F2E65-37AE-4CAE-B166-A4171EE6E50F}" src="https://github.com/user-attachments/assets/1f572e3b-4874-4457-af01-9528cb06e458" />

## ROLLBACK:

Undoes changes that have not been committed

<img width="184" height="112" alt="{34A16BBD-06AD-4870-A507-02ED5A0D7DE6}" src="https://github.com/user-attachments/assets/7d5ed722-dad5-4103-a59c-c00d3beaccd4" />

## SAVEPOINT:

Creates a savepoint within a transaction.

<img width="390" height="64" alt="{0529A867-1869-411F-A98B-5F7F230844FC}" src="https://github.com/user-attachments/assets/44a82aa2-7040-4635-863f-c1a862bf28f8" />






