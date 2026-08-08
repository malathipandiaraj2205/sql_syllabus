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

The SELECT command in SQL is used to retrieve data from one or more tables in a database. It allows you to select specific columns or all columns and can be combined with clauses like WHERE, ORDER BY, and GROUP BY to filter, sort, and organize the retrieved data.

Syntax

<img width="272" height="79" alt="{5EA0A7D0-B0BE-4174-8301-2846EFC33B34}" src="https://github.com/user-attachments/assets/a3c01138-41d5-4587-8837-3e524de41393" />

Examples

1. ## Select all columns

syntex

<img width="218" height="20" alt="{B338133A-8EF0-41FA-8384-0F589B3F38CD}" src="https://github.com/user-attachments/assets/05a4d123-3a88-4653-9819-cd42f790e3b9" />


Example:

<img width="501" height="252" alt="{85FC4226-62B8-439D-85CD-D37352E984EC}" src="https://github.com/user-attachments/assets/b1630e3a-75f6-4606-94a5-b22288e97ed4" />

2. ## Select specific columns


syntex

<img width="281" height="51" alt="{E669160D-CB70-4D63-AC08-2254C0F0B808}" src="https://github.com/user-attachments/assets/f53b8892-f2f9-4064-83c5-137315b33e41" />

Example:

<img width="276" height="263" alt="{2F2F814D-3265-4548-AE28-F1AAECDA17E4}" src="https://github.com/user-attachments/assets/349cfda7-4c63-49a2-940d-42203ed57a47" />

2.## FROM

The FROM clause is used to specify the table from which data is retrieved.

Syntax

<img width="173" height="63" alt="{9FB42D0E-640F-4D24-86FF-82B9FA81585E}" src="https://github.com/user-attachments/assets/7aac4727-cf68-4fa7-80eb-a64e6b661d45" />

Example

<img width="202" height="36" alt="{977AD601-BBBA-4FD9-980A-CA7544FC0069}" src="https://github.com/user-attachments/assets/bcafd030-dd8a-4238-9414-e4b28a4eebaf" />

3.## WHERE Clause

The WHERE clause is used to filter records and retrieve only the rows that satisfy a specified condition.

Syntax

<img width="205" height="65" alt="{5D2AB00F-BBAB-40E4-8B03-C5F496259EBC}" src="https://github.com/user-attachments/assets/3e303848-4386-46b8-a8b8-d137a34e2683" />


Example:

<img width="208" height="213" alt="{545C6E76-69FF-4FFB-80E7-0C8530291D60}" src="https://github.com/user-attachments/assets/521a8e0a-e324-4731-9f8c-ecf043ed4bc5" />

4.## GROUP BY:

The GROUP BY clause is used to group rows that have the same values in specified columns. It is often used with aggregate functions such as COUNT(), SUM(), AVG(), MAX(), and MIN().


Syntex:

<img width="361" height="76" alt="{F13DFDD3-F23F-4CFA-868F-22A4112109E2}" src="https://github.com/user-attachments/assets/9490c20f-e5a0-4c75-a54a-7e54198a7605" />

Example:

<img width="280" height="220" alt="{524BB390-0063-42A1-BFA2-E22C6E69D85B}" src="https://github.com/user-attachments/assets/1e1f620d-2abe-4440-b24b-11f2d1649bb6" />

5.## HAVING:

The HAVING clause is used to filter groups created by the GROUP BY clause. It is similar to WHERE, but WHERE filters rows, while HAVING filters grouped data.

Syntex:

<img width="340" height="94" alt="{1AAB8CD4-D4A7-4B03-B81E-6B0BAC52D13A}" src="https://github.com/user-attachments/assets/a87c9e33-dcf0-420a-a1f1-313ec7429b43" />

Example:

<img width="270" height="227" alt="{59FF5478-45BC-4A99-862C-51FD61E8E746}" src="https://github.com/user-attachments/assets/fe71214c-31f4-49e6-99fa-9994bd191f03" />

6.## ORDER BY :

The ORDER BY clause is used to sort the result set in ascending (ASC) or descending (DESC) order.

Syntax

<img width="327" height="72" alt="{1C5F2CF3-6C1A-4CBE-B85B-F0D469EA2B93}" src="https://github.com/user-attachments/assets/14cd7b92-662e-40fb-80a9-c4dee3e12183" />

Example:

<img width="356" height="223" alt="{3A9C94E9-5A38-43CF-8B54-EC088F608E7E}" src="https://github.com/user-attachments/assets/b7b0f8f1-3853-4734-9eba-e6f0a3e60f11" />

7.## LIMIT:

The LIMIT clause is used to restrict the number of rows returned by a query.

Syntax

<img width="293" height="96" alt="{CCD21F52-3444-4E64-A733-388257BD676B}" src="https://github.com/user-attachments/assets/03b1bc0c-82c9-4c5f-9e88-4ca906aacb9c" />

Example:

<img width="285" height="84" alt="{563191C0-82A2-476F-8758-E4252DAB8D97}" src="https://github.com/user-attachments/assets/7ac87344-32e4-4add-88a4-aaf9f9325c34" />

## Aggregate Functions:

Aggregate functions perform calculations on a set of values and return a single result.

## Common Aggregate Functions:

1.     COUNT()          Counts the number of rows
2.     SUM()	           Returns the total sum
3.     AVG()	           Returns the average value
4.     MAX()	           Returns the highest value
5.     MIN()	           Returns the lowest value
 
## AVG():

AVG() is an aggregate function used to calculate the average value of a numeric column.


Syntex:

<img width="329" height="50" alt="{A3C4A472-0DA7-4A98-9635-6EEF95EDE964}" src="https://github.com/user-attachments/assets/8f2844d9-2652-427e-8f19-7e17bd5f5b54" />


Example:

<img width="191" height="58" alt="{1B2916B6-CD0E-46FC-B1A2-3CFF6F0613B3}" src="https://github.com/user-attachments/assets/9c80bb98-5fac-45ef-9094-2570a5f98fa8" />


## LOGICAL OPERATOR:

Logical Operators in SQL are used to combine multiple conditions in a query.

Operator	Meaning:
   1.                 AND	        All conditions must be true
   2.                 OR	         Any one condition can be true
   3.                 NOT	        Reverses the condition

1.## AND Operator

Returns records only if all conditions are TRUE.

Syntex:

<img width="367" height="75" alt="{8E8B50AE-A185-4D0F-9AF4-7AFF8ED674CA}" src="https://github.com/user-attachments/assets/8bdbae0f-b7f1-4b13-a395-fb1e74b1b0de" />

example:

<img width="472" height="229" alt="{90C9AED8-CFE6-4A41-B7E4-A65B1BC992D2}" src="https://github.com/user-attachments/assets/d88a484d-c90f-4fa0-ba5c-343d0a86593e" />

2.## OR OPERATOR:

Returns records if at least one condition is TRUE.

Syntex:

<img width="363" height="68" alt="{1787A1AE-F6BB-4F50-A635-788D89DD8EBB}" src="https://github.com/user-attachments/assets/3e8938a3-281c-44e0-9684-627ba215ebee" />

Example:

<img width="466" height="221" alt="{EFCA824B-FD52-4BC2-AC11-14BC00129171}" src="https://github.com/user-attachments/assets/beaef650-c278-4b8a-a8ea-9780950e1668" />

3.## NOT OPERATOR:

Returns records where the condition is NOT TRUE.

Syntex:

<img width="258" height="70" alt="{A6A8787D-C728-4B17-81CE-C2DC6FB06AF9}" src="https://github.com/user-attachments/assets/b36c54fd-40fb-46d7-b333-8dc997388d59" />

Example:

<img width="495" height="201" alt="{B2BC7743-67FC-4A10-99CF-4974BF140255}" src="https://github.com/user-attachments/assets/cd3795a4-440c-44d7-992f-fee011aba3e2" />

## COMPARISON OPERATOR:

Comparison operators are used to compare two values in a WHERE clause.

| Operator     | Meaning                  | Example              |
| ------------ | ------------------------ | -------------------- |
|   =          | Equal to                 |    salary = 50000    |
|   != or <>   | Not equal to             |    department <> HR  |
|   >          | Greater than             |    salary > 50000    |
|   <          | Less than                |    salary < 50000    |
|   >=         | Greater than or equal to |    salary >= 50000   |
|   <=         | Less than or equal to    |    salary <= 50000   |

Syntex:

<img width="212" height="52" alt="{0A7166FE-283A-4383-A2D6-5C920AC35A26}" src="https://github.com/user-attachments/assets/6b60944e-b7f2-46d9-b2b3-9dc1cad8ceed" />

Example:

<img width="514" height="241" alt="{2DD08276-A25F-411D-BE55-C8CD430A382E}" src="https://github.com/user-attachments/assets/d3540e0d-1fd2-4de2-bd14-b1a00b26b3e8" />


## ARITHMATIC OPERATORS:

Arithmetic operators are used to perform mathematical calculations on numeric values.

| Operator | Description         | Example         |
| -------- | ------------------- | --------------- |
|   +      | Addition            | salary + 1000   |
|   -      | Subtraction         | salary - 1000   |
|   *      | Multiplication      | salary * 2      |
|   /      | Division            | salary / 2      |
|   %      | Modulus (remainder) | salary % 1000   |


Syntex:

<img width="351" height="88" alt="{B8DB312E-BEA6-4D6E-AD5E-45A22FE72F7C}" src="https://github.com/user-attachments/assets/28f42d87-3036-4ed6-a4a6-05e7bd1343ce" />

Example:

<img width="327" height="215" alt="{8BB98BD7-A841-4AC0-BE8B-184A7B4DAB1C}" src="https://github.com/user-attachments/assets/8fac69f6-7f45-44d6-9343-db3533bf93bd" />

## LIKE OPERATOR:

The LIKE operator is used to search for a specified pattern in a column.

| Wildcard | Meaning                                  |
| -------- | ---------------------------------------- |
|    %     | Represents zero, one, or many characters |
|    _     | Represents exactly one character         |

| Pattern   | Meaning                       |
| --------- | ----------------------------- |
| R%        | Starts with R                 |
| %a        | Ends with a                   |
| %vi%      | Contains vi                   |
| R_        | R followed by one character   |
| R____     | R followed by four characters |

Syntex:

<img width="437" height="79" alt="{E946255D-8A6C-4E9D-8989-A67D9A160CF4}" src="https://github.com/user-attachments/assets/e2f6f044-4dda-452c-8df3-c02988b599c3" />

Exmple:

<img width="478" height="221" alt="{16E2040C-12EC-42A1-8E46-639911C37730}" src="https://github.com/user-attachments/assets/36198d05-d1b2-4cfc-a095-d42c475a9ff6" />

## CASE FUNCTION

The CASE function is used to apply conditions and return different values based on those conditions. It works like an IF-ELSE statement.

Syntex:

<img width="445" height="191" alt="{C8E934E7-070E-4243-AD04-2ECE48B8B91E}" src="https://github.com/user-attachments/assets/17aa7afd-547a-4465-9818-12bcf2bab35b" />

Example:

<img width="527" height="223" alt="{E364C04C-8445-4999-A0C2-3DFD41D5E040}" src="https://github.com/user-attachments/assets/9e6634df-30a8-4c74-95af-003074be4f3b" />

## JOINS:

JOIN is used to combine rows from two or more tables based on a related column.

Types of Joins
1.INNER JOIN
2.LEFT JOIN
3.RIGHT JOIN

1. ## INNER JOIN

Returns only matching records from both tables.

Syntex:

<img width="476" height="68" alt="{CC900381-BC38-449D-AAD2-7B8E7A8EE3E3}" src="https://github.com/user-attachments/assets/987d4bf4-d40d-456a-966b-75adc15e2d3b" />

Example:

<img width="500" height="241" alt="{08DD842F-39AF-4262-BC9D-51330FC47EF6}" src="https://github.com/user-attachments/assets/e6675860-f970-4899-bb9b-e4966c7e91fc" />


2.## LEFT JOIN:

Returns all records from the left table and matching records from the right table.

Syntex:


<img width="513" height="74" alt="{B14A94D3-5E71-4EAC-93F4-3240EC74D0F2}" src="https://github.com/user-attachments/assets/abb2043a-9a2c-48e6-8b15-386707a863dd" />

Example:

<img width="510" height="222" alt="{8D9B4B5F-3A1F-4F5A-B8D1-A3AC18853727}" src="https://github.com/user-attachments/assets/db9c1d9d-af42-4d2e-b442-52ba19d5c6a2" />

3.## RIGHT JOIN

Returns all records from the right table and matching records from the left table.

Syntex:

<img width="461" height="62" alt="image" src="https://github.com/user-attachments/assets/eadf92d0-7098-470e-ac54-22fd264ffd66" />

Example:

<img width="667" height="236" alt="{533F7AB8-8280-4945-AA89-7E40EBA0CF08}" src="https://github.com/user-attachments/assets/963373a8-b361-4f0f-b98a-7ad20b86d7dd" />

## SUBQUERIES:

A Subquery is a query inside another SQL query. It is also called a nested query.

Syntex:

<img width="420" height="214" alt="{4EF91A19-42A8-4159-A1DC-D885E4FFE944}" src="https://github.com/user-attachments/assets/97880c57-a7bf-4c09-bff8-0aa72de9e749" />

## CTE (Common Table Expression):

A CTE (Common Table Expression) is a temporary result set that can be referenced within a SELECT, INSERT, UPDATE, or DELETE statement.

CTEs make complex queries easier to read and maintain.

## Advantages of CTE:

● Improves query readability.

● Breaks complex queries into simpler parts.

● Can be referenced multiple times in the same query.

● Useful for recursive queries.

## Difference Between Subquery and CTE:

| Subquery                    | CTE                              |
| --------------------------- | -------------------------------- |
| Written inside a query      | Defined using  WITH              |
| Harder to read when complex | Easier to read and maintain      |
| Used once                   | Can be referenced multiple times |

Syntex:

<img width="415" height="220" alt="{240A64AD-F662-4F3A-8122-3F048F79ED2C}" src="https://github.com/user-attachments/assets/ce10757b-da65-4048-958a-1dc4bc043294" />

Example:

<img width="474" height="252" alt="{60408734-3DD2-44D9-BC8B-61DC62337A3E}" src="https://github.com/user-attachments/assets/60b27137-9ab7-4291-a411-05552aff6d8e" />

## Window Function Definition :

A Window Function is a SQL function that performs calculations across a set of table rows related to the current row without grouping the rows into a single output row.

Examples:

● ROW_NUMBER ()

● RANK ()

● DENSE_RANK ()

● LAG ()

● LEAD ()

● SUM ()

● AVG ()

Syntex:

<img width="436" height="113" alt="{F7DC3A77-BF85-4063-8534-8B13827BA81E}" src="https://github.com/user-attachments/assets/588d7a88-9028-47b8-b96d-56f992d13bed" />

Example:

<img width="409" height="260" alt="{9541291A-2C2B-406B-84DE-5E0FB81F4393}" src="https://github.com/user-attachments/assets/e5498eda-daef-4cec-a142-dd9ad792439f" />

## Advantages of CTE:
1. Improves query readability.
2. Makes complex queries easier to understand.
3. Can be reused within the same query.
4. Supports recursive queries.
