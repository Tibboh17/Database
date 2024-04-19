# WHERE
- Used to extract only those records that fulfill a specified condition.
```SQL
SELECT * FROM Customers
WHERE CustomerID = 1;
```

# ORDER BY
- Used to sort the result-set in ascending or descending order.
- ASC (ascending order), DESC (descending order).
```SQL
SELECT * FROM Products
ORDER BY Price ASC;
```

# GROUP BY
- Groups rows that have the same values into summary rows, like "find the number of customers in each country".
- Often used with aggregate functions to group the result-set by one or more columns.
```SQL
SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country;
```

# HAVING
- Used to filter the result set based on aggregate functions.
- Added to SQL because **WHERE** cannot be used with aggregate functions.
```SQL
SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country
HAVING COUNT(CustomerID) > 5
ORDER BY COUNT(CustomerID) DESC;
```

# LIMIT
- Used to to select a limited number of records.
- Useful on large tables with thousands of records.
```SQL
SELECT * FROM Customers
LIMIT 3;
```

# DISTINCT
- Used to return only distinct (different) values.
```SQL
SELECT DISTINCT Country FROM Customers;
```

# LIKE
- Used in **WHERE** to search for a specified pattern in a column.
- The percent sign (%) represents zero, one, or multiple characters.
- The underscore sign (_) represents one, single character
```SQL
SELECT * FROM Customers
WHERE CustomerName LIKE 'a%';
```

# AS
- Alias.
- Used to give a table, or a column in a table, a temporary name.
- An alias only exists for the duration of that query.
```SQL
SELECT CustomerID AS ID
FROM Customers;
```

# AND
- Used to filter records based on more than one condition.
```SQL
SELECT *
FROM Customers
WHERE Country = 'Spain' AND CustomerName LIKE 'G%';
```

# OR
- Used to filter records based on more than one condition.
```SQL
SELECT *
FROM Customers
WHERE Country = 'Germany' OR Country = 'Spain';
```

# NOT
-  used in combination with other operators to give the opposite result.
```SQL
SELECT * FROM Customers
WHERE NOT Country = 'Spain';
```
