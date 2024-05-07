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
