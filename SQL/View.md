# View
- A kind of a virtual table.
- Has rows and columns like a table, but doesn't store data on the disk.
- Defines a customized query that retrieves data from one or more tables, and represents the data as if it was coming from a single source.

# Uses of View
- Restrict data access.
- Simplify commands.
- Store complex queries.
- Remove data dependency.

# Types of View
- **System Defined View**
    - Information Schema View
    - Catalog View
    - Dynamic Management View
- **User Defined View**
    - Simple View
    - Complex View
    - Materalized View

# Syntax
- Creating a view from a single table.
```SQL
CREATE VIEW DetailsView AS
SELECT NAME, ADDRESS
FROM StudentDetails
WHERE S_ID < 5
ORDER BY NAME;
```
- Creating a view from multiple tables.
```SQL
CREATE VIEW MarksView AS
SELECT StudentDetails.NAME, StudentDetails.ADDRESS, StudentMarks.MARKS
FROM StudentDetails, StudentMarks
WHERE StudentDetails.NAME = StudentMarks.NAME;
```
- Deleting a view.
```SQL
DROP VIEW MarksView;
```
- Updating a view.
    - The view should be created from a single table.
    - The view should not be created using nested queries or complex queries.
    - The SELECT statement which is used to create the view should not include GROUP BY clause or ORDER BY clause.
    - The SELECT statement should not have the DISTINCT keyword.
```SQL
UPDATE MarksView
SET MARKS = 95
WHERE NAME = "Harsh";
```
```SQL
CREATE OR REPLACE VIEW MarksView AS
SELECT StudentDetails.NAME, StudentDetails.ADDRESS, StudentMarks.MARKS, StudentMarks.AGE
FROM StudentDetails, StudentMarks
WHERE StudentDetails.NAME = StudentMarks.NAME;
```
```SQL
INSERT INTO DetailsView(NAME, ADDRESS)
VALUES("Suresh","Gurgaon");
```
```SQL
DELETE FROM DetailsView
WHERE NAME="Suresh";
```
