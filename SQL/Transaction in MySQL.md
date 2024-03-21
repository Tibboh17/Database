# Isolation Level
- **READ UNCOMMITTED**
    - One transaction may read not yet committed changes made by other transactions.
- **READ COMMITED**
    - A transaction can only see changes made by other committed transactions. 
- **REPEATABLE READ**
    - A transaction will see the same data throughout its duration, even if other transactions commit changes to the data.
- **SERIALIZABLE**
    - All transactions must be executed sequentially.
 
<div align="center">
    <img src="https://github.com/TIBBOH17/Database/assets/121493257/9d53e4c6-b185-481a-8694-d7aa6b208822", width=70%>
</div>

# Syntax
- **BEGIN TRANSACTION**
    - Starts the transaction.
```SQL
BEGIN TRANSACTION;
```
- **COMMIT**
    - Saves all the transactions to the database.
```SQL
INSERT INTO Students VALUES ("Moon", "Seoul", "010-0000-0000");
COMMIT;
```
- **ROLLBACK**
    - Undos transactions.
```SQL
DELETE FROM Students WHERE NAME = "Moon";
ROLLBACK;
```
- **SAVEPOINT**
    - Creates points within the groups of transactions in which to ROLLBACK.
```SQL
SAVEPOINT SP1;
DELETE FROM Students WHERE NAME = "Moon";
SAVEPOINT SP2;
```
```SQL
ROLLBACK TO SP1;
```
- **RELEASE SAVEPOINT**
    - Removes a SAVEPOINT.
```SQL
RELEASE SAVEPOINT SP2;
```
