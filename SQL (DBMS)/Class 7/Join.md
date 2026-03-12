# JOIN
In SQL, JOIN is used to combine rows from two or more tables based on a related column between them.

##### For example, imagine two tables:

##### Table 1: Students

student_id |	name
-----------|---------
1	|Kimi
2	|Rahul
3	|Anjali

##### Table 2: Marks

student_id	| marks
------------|----------
1	|85
2	|90
4	|75

We can join these tables using student_id.

--------------------------------------------------------------------------------------------------------------------------------------------
# Type of JOIN

## 1. INNER JOIN
Returns only the rows that have matching values in both tables.

### Syntax
    SELECT column_names
    FROM table1
    INNER JOIN table2
    ON table1.column = table2.column;

### Example
    SELECT Students.name, Marks.marks
    FROM Students
    INNER JOIN Marks
    ON Students.student_id = Marks.student_id;

### Result
  name	|marks
  ------|-------
  Kimi	|85
  Rahul	|90

Explanation: Only matching student_id (1,2) appear.



## 2. LEFT JOIN (LEFT OUTER JOIN)
Returns all rows from the left table and matching rows from the right table. If no match, it shows NULL.

### Syntax
    SELECT column_names
    FROM table1
    LEFT JOIN table2
    ON table1.column = table2.column;

### Example
    SELECT Students.name, Marks.marks
    FROM Students
    LEFT JOIN Marks
    ON Students.student_id = Marks.student_id;

### Result
  name	|markss
  ------|-------
  Kimi	|85
  Rahul	|90
  Anjali	|NULL
  
Explanation: Anjali has no marks, so SQL shows NULL.



## 3. RIGHT JOIN (RIGHT OUTER JOIN)
Returns all rows from the right table and matching rows from the left table.

### Syntax
    SELECT column_names
    FROM table1
    RIGHT JOIN table2
    ON table1.column = table2.column;

### Example
    SELECT Students.name, Marks.marks
    FROM Students
    RIGHT JOIN Marks
    ON Students.student_id = Marks.student_id;

### Result
  name	|markss
  ------|-------
  Kimi	|85
  Rahul	|90
  NULL	|75
  
Explanation: student_id 4 exists in Marks but not in Students, so name is NULL.



## 4. FULL JOIN (FULL OUTER JOIN)
Returns all rows from both tables. If there is no match, NULL is used.

### Syntax
    SELECT column_names
    FROM table1
    FULL JOIN table2
    ON table1.column = table2.column;

### Result
name	|marks
------|---------
Kimi	|85
Rahul	|90
Anjali	|NULL
NULL	|75
