# MySQL
- Open-source RDBMS 

# DDL
- **CREATE**
```SQL
CREATE SCHEMA my_db;

CREATE TABLE my_table(
    id INT NOT NULL AUTO_INCREMENT,
    age TINY INT,
    name VARCHAR(10) NOT NULL,
    personal VARCHAR(10),
    PRIMARY KEY(id)
);
```
- **DROP**
```SQL
DROP TABLE IF EXISTS my_table;
```
- **ALTER**
```SQL
ALTER TABLE my_table ADD COLUMN phone VARCHAR(20);
ALTER TABLE my_table MODIFY COLUMN name VARCHAR(20) NOT NULL;
ALTER TABLE my_table CHANGE COLUMN personal personal_id VARCHAR(14) NOT NULL;
ALTER TABLE my_table DROP COLUMN age;
```

# DQL
- **SELECT**
```SQL

```

# DML
- **INSERT**
```SQL
INSERT INTO my_table (age, name, personal_id, phone)
VALUES (28, 'Moon', '111111-1111111', '000-0000-0000');
```
- **UPDATE**
```SQL
UPDATE my_table SET age = 27, phone = '111-1111-1111'
WHERE name = 'Moon';
```
- **DELETE**
```SQL
DELETE FROM my_table
WHERE name = 'Moon'
```
# DCL
```SQL
```
# TCL
```SQL
```
