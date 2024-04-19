# (INNER) JOIN
- Returns records that have matching values in both tables.
```SQL
SELECT ProductID, ProductName, CategoryName
FROM Products
INNER JOIN Categories ON Products.CategoryID = Categories.CategoryID;
```

# LEFT (OUTER) JOIN
- Returns all records from the left table, and the matched records from the right table.
```SQL
SELECT Customers.CustomerName, Orders.OrderID
FROM Customers
LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID
ORDER BY Customers.CustomerName;
```

# RIGHT (OUTER) JOIN
- Returns all records from the right table, and the matched records from the left table.
```SQL
SELECT Orders.OrderID, Employees.LastName, Employees.FirstName
FROM Orders
RIGHT JOIN Employees ON Orders.EmployeeID = Employees.EmployeeID
ORDER BY Orders.OrderID;
```


# FULL (OUTER) JOIN
- Returns all records when there is a match in either left or right table.
```SQL
SELECT Customers.CustomerName, Orders.OrderID
FROM Customers
FULL JOIN Orders ON Customers.CustomerID=Orders.CustomerID
ORDER BY Customers.CustomerName;
```
