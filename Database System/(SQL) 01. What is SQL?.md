# SQL
- Structured Query Language.
- A programming language storing and processing datas in RDB.
- Used to maintain, manage, and optimize the database performance.

# Concepts of SQL
- **SQL Table**
    - Basic element of a relational database.
    - Consists of row and column.
- **SQL Statements**
    - SQL statements or SQL Queries are valid commands that RDBMS understands.
    - Written by using various SQL language elements.
- **Stored Procedures**
    - A collection of SQL statements stores in RDB.
    - Used to improve efficiency and performance.
 
# How does SQL works?
- **Parser**
  - The parser starts by tokenizing, or replacing, some of the words in the SQL statements wuth special symbols.
  - It checks the statement for **correctness** and **Authorization**.
- **Relational Engine**
  - The relational engine, or query processor, creates a plan for retrieving, writing, or updating the corresponding data in the most effective manner.
  - It writes the plan in an intermediate-level representation of the SQL statement called byte code.
- **Storage Engine**
  - The storage engine, or database engine, is the software component that processes the byte code and runs the intended SQL statement.
  - It reads and stores the data in the database files on physical disk storage.
  
# SQL commands
<div align="center">
  <img src="https://scaler.com/topics/images/different-sql-command.webp", width="70%">
</div>

- **Data Definition Language (DDL)**
    - Used to design the database structure.
    - Used to create and modify the database object according to requirements.
- **Data Query Language (DQL)**
    - Configure commands to retrieve data stored in RDB.
- **Data Manipulation Language (DML)**
    - Use to write new information or modify existing records in an RDB.
- **Data Control Language (DCL)**
    - Used to manage or grant access to databases.
- **Transaction Control Language (TCL)**
    - Help users manage and control a database’s transactions (changes) to maintain consistency.
