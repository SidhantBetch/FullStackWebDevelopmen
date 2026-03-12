## ORDER BY (Descending Order)
Used to sort the data in ascending or descending order.

### Syntax
    SELECT column_name
    FROM table_name
    ORDER BY column_name DESC;

### Example
    SELECT name, marks
    FROM Students
    ORDER BY marks DESC;
DESC = Descending (Highest to Lowest)

### result:
name	| marks
-------|--------
Rahul	|90
Kimi	|85
Anjali	|70

------------------------------------------------------------------------------------------------------------------------------------------

## ORDER BY Ascending
### Syntax
    SELECT column_name
    FROM table_name
    ORDER BY column_name ASC;
ASC = Ascending (Lowest to Highest)

### Example:
    SELECT name, marks
    FROM Students
    ORDER BY marks ASC;

------------------------------------------------------------------------------------------------------------------------------------------

 ## WHERE (Finding specific data)
Used to find specific rows from a table.

### Syntax
    SELECT column_name
    FROM table_name
    WHERE condition;

### Example
    SELECT * 
    FROM Students
    WHERE name = 'Kimi';
This shows only the row where name = Kimi.

------------------------------------------------------------------------------------------------------------------------------------------

## LIKE (Search pattern)
Used to find data using patterns.

### Example
    SELECT * 
    FROM Students
    WHERE name LIKE 'K%';
This finds names starting with K.

results:
- Kimi
- Karan
- Kunal

------------------------------------------------------------------------------------------------------------------------------------------

## LIMIT (Show limited rows)
Used to show only a few records.

### Example
    SELECT * 
    FROM Students
    LIMIT 3;
Shows only 3 rows.

------------------------------------------------------------------------------------------------------------------------------------------
## SELECT
Used to retrieve data from a table.

### Syntax
    SELECT column_name
    FROM table_name;

### Example
    SELECT name FROM Students;

------------------------------------------------------------------------------------------------------------------------------------------
## SELECT *
Used to show all columns.

    SELECT * FROM Students;

------------------------------------------------------------------------------------------------------------------------------------------
## AND
Used to combine multiple conditions.

    SELECT *
    FROM Students
    WHERE marks > 70 AND city = 'Delhi';

------------------------------------------------------------------------------------------------------------------------------------------
  
  ## OR
Returns rows if any condition is true.

    SELECT *
    FROM Students
    WHERE city = 'Delhi' OR city = 'Mumbai';

------------------------------------------------------------------------------------------------------------------------------------------
## NOT
Returns rows that do not match the condition.

    SELECT *
    FROM Students
    WHERE NOT city = 'Delhi';

------------------------------------------------------------------------------------------------------------------------------------------
## IN
Used to match multiple values.

    SELECT *
    FROM Students
    WHERE city IN ('Delhi', 'Mumbai', 'Pune');

------------------------------------------------------------------------------------------------------------------------------------------
## LIKE
Used for pattern searching.

    SELECT *
    FROM Students
    WHERE name LIKE 'A%';
Names starting with A.

------------------------------------------------------------------------------------------------------------------------------------------
## ORDER BY
Sort data.

    SELECT *
    FROM Students
    ORDER BY marks DESC;

------------------------------------------------------------------------------------------------------------------------------------------
## GROUP BY
Used with aggregate functions.

    SELECT city, COUNT(*)
    FROM Students
    GROUP BY city;
Counts students in each city.

------------------------------------------------------------------------------------------------------------------------------------------
## HAVING
Used with GROUP BY to filter groups.

    SELECT city, COUNT(*)
    FROM Students
    GROUP BY city
    HAVING COUNT(*) > 2;

------------------------------------------------------------------------------------------------------------------------------------------
## COUNT()
Counts rows.

    SELECT COUNT(*)
    FROM Students;

------------------------------------------------------------------------------------------------------------------------------------------
## MAX()
Find maximum value.

    SELECT MAX(marks)
    FROM Students;

------------------------------------------------------------------------------------------------------------------------------------------
## MIN()
Find minimum value.

    SELECT MIN(marks)
    FROM Students;

------------------------------------------------------------------------------------------------------------------------------------------
## AVG()
Find average value.
    
    SELECT AVG(marks)
    FROM Students;
    
------------------------------------------------------------------------------------------------------------------------------------------
