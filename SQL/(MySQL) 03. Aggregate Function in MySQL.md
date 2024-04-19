# Aggregate Function
- A function that performs a calculation on a set of values, and returns a single value.
- Often used with **GROUP BY** of **SELECT**.

# MIN
- Returns the smallest value within the selected column.
```SQL
SELECT MIN(Price)
FROM Products;
```

# MAX
- Returns the largest value within the selected column.
```SQL
SELECT MAX(Price)
FROM Products;
```

# COUNT
- Returns the number of rows in a set.
```SQL
SELECT COUNT(*)
FROM Products;
```

# SUM
- Returns the total sum of a numerical column.
```SQL
SELECT SUM(Quantity)
FROM OrderDetails;
```

# AVG
- Returns the average value of a numerical column.
```SQL
SELECT AVG(Price)
FROM Products;
```
