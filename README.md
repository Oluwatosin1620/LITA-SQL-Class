# LITA-SQL-Class

## SQL (STRUCTURED QUERY LANGUAGE)
It stores and manages data in a Relational Database Management System (RDBMS). It is a standard language for Relational Database Systems. It enables a user to relate databases and tables. All the RDBMS, like MySQL, PostgreSQL, Oracle, MS Access, and SQL servers, use SQL as the standard database language. 
SQL is used for storing, retrieving, and managing data. It is a standard language for querying, retrieving and deleting data. SQL is not case sensitive i.e. it can be written in either upper case or lower case. It depends on tuple relational calculus and relational algebra i.e. mathematical or statistical calculations can be done. SQL is a great tool for analysing multiple data at once and it allows to analyse more complex questions than dashboard tools.

**Database**: It is an organized collection of data stored, and managed in a structured way to allow for easy access, retrieval and manipulation. 
**Database stores data** in a structured format using tables which are composed of rows and columns. Each table represents a specific type of data, and the row is called RECORD while the column is referred to as FIELD.

**Data in Database** is stored in tables that can be thought of just like Excel spreadsheets. All data in the same column must match in terms of data type.
**A table** is an organised data composed of rows and columns.


### SQL Command
They are instructions used to communicate with the database. It is also used to perform specific tasks, functions, and queries of data. It performs various tasks like CREATE a table, ADD data to the table, DROP the table, MODIFY the table, and set permission for users.

#### Types of SQL Command
1.  **DDL (Data Definition Language)**: for defining database schemas. **Schema** is the overall layout of the database. The command changes the structure of the table and is auto committed i.e. it permanently saves all the changes in the database. they are:
  * CREATE: to create a table
  * ALTER: to modify the characteristics of an existing attribute or add a new one
  * TRUNCATE: to delete all rows from the table
  * DROP: to delete the changes in the database i.e. to delete an entire table

2. **DML (Data Manipulation Language)**: for inserting, updating and deleting data from a database. It is responsible for all forms of changes in the database. It cannot permanently save all changes in the database. they are:
  * INSERT: to insert data in a row
  * UPDATE: to update values of a column in a row
  * DELETE: to delete records

3. **DCL (Data Control Language)**: for controlling access to the data in the database, user and permission management. It is used to GRANT and TAKEBACK authority from any database user. they are:
  * GRANT: to give user access privileges to a database.
  * REVOKE: to take back permission from the user.

4. **DQL ( Data Query Language)**: to query the database for information already stored there. Used to fetch data from the database and has only one command;
  * SELECT: to retrieve data from a database. To select an attribute based on the condition described by the WHERE clause

5. **TCL (Transaction Control Language)**: to manage transactions in a database. It allows statements to be grouped into logical transactions. they are:
  * COMMIT: to save transactions in a database and it permanently performs its tasks
  * ROLLBACK: to undo transactions that have not been saved
  * SAVEPOINT: to roll back transactions to a certain point without rolling back whenever necessary


### Data Type
It is used to define the value column can contain. Each column is required to have a name and data type in a database table.
  * Binary Datatype- YES/NO, TRUE/FALSE
  * Numeric Datatype- bit, tinybit, smallint, int, bigint, decimal, money, float, real, etc
  * String Datatype- char, varchar, nchar, varbinary, mvarchar. Allows a group of characters to be stored that is enclosed in a single quote of table which could either be numbers, letters, symbols, etc.
  * Data Datebase: to store values in date. date, datetime, timestamp.

### keys
It helps to create relationships between tables, maintain uniqueness and ensure data is consistent and valid. they are:
  * Foreign Key         * Primary Key         * Candidate Key          * Composite Key         
  * Database Key        * Super Key           * Surrogate Key          * Alternate Key
* **Primary Key**: it uniquely identifies each record in a table
* **Foreign Key**: a field in one table that uniquely identifies a row of another table creating a relationship between two tables.


### Database Management System (DBMS)
A special software program that helps users create and maintain a database, handles security backups, importing/exporting data, and makes it easy to interact with software applications.
**Types of Database
  **Relational Database**: organize data into one or more tables and each table has a unique key identifying each row
  **Non-Relational Database (No SQL)**: organize data in anything but a traditional table. Anything that is not relational.


  ### Writing Queries ( Using SQL server)

![Creat table](https://github.com/user-attachments/assets/c474ef87-79b7-442a-8930-c986e54e3fde)

* Not Null- means no empty space
* varchar- means numbers and letters
* (Number)- means the number of characters it should contain and not exceed
* Difference between Date & Datetime- datetime comes with the hours and seconds

![2024-11-06 (1)](https://github.com/user-attachments/assets/b95b2b94-f57b-4b2a-b572-73cace00a3af)

To insert more records in a table, INSERT function is used.

To view the table created, SELECT function is used;
~~~SQL
SELECT * from Employee
~~~


![Salary Table(2)](https://github.com/user-attachments/assets/41c0c41a-c597-4c19-8473-9100ca56596b)


To perform the following functions:
.....SUM, COUNT, MAX, MIN, AVERAGE.........

~~~SQL
SELECT SUM(salary) as TOTALSALARY from salary
~~~

~~~SQL
SELECT AVG(salary) as AVERAGESALARY from salary
~~~

~~~SQL
SELECT COUNT(staffid) as EmployeeCount from employee
~~~


**Update function**: to update the features of a table
![2024-11-06 (3)](https://github.com/user-attachments/assets/3a377093-4042-4728-bf61-7bd5344e1140)
To make an auto-increment- (1,1) means from 1 and increase by 1


To create an additional field (column)
~~~SQL
ALTER TABLE EMPLOYEE
add state_of_origin varchar (50)
~~~


### SQL Clauses
![2024-11-06 (4)](https://github.com/user-attachments/assets/560adf54-3a5b-4e2b-9f0e-999bd4e8e055)

GROUP BY: it follows the WHERE clause in a SELECT statement and precedes the ORDER BY clause

HAVING: used to specify a search condition for a group or an aggregate
ORDER BY: sorts the result in ascending or descending order. DESC(descending)







