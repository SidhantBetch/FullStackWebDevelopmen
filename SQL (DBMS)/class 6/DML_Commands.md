# DML (Data Manipulation Language)
DML (Data Manipulation Language) commands are used to manipulate or manage the data stored in database tables.  
These commands allow users to insert, update, delete, and retrieve data.

## Main DML Commands
### 1️⃣ INSERT
Used to add new records into a table.

#### Syntax
    INSERT INTO table_name (column1, column2, column3)
    VALUES (value1, value2, value3);

#### Example
    INSERT INTO Students (ID, Name, Age)
    VALUES (1, 'Kimi', 20);

_________________________________________________________________________________________________________________________________________

### 2️⃣ SELECT
Used to retrieve data from a table.

#### Syntax
    SELECT column1, column2
    FROM table_name;

#### Example
    SELECT * FROM Students;

This displays all records from the Students table.

_________________________________________________________________________________________________________________________________________

### 3️⃣ UPDATE
Used to modify existing data in a table.

#### Syntax
    UPDATE table_name
    SET column1 = value1
    WHERE condition;

#### Example
    UPDATE Students
    SET Age = 21
    WHERE ID = 1;

_________________________________________________________________________________________________________________________________________

### 4️⃣ DELETE
Used to remove records from a table.

#### Syntax
    DELETE FROM table_name
    WHERE condition;

#### Example
    DELETE FROM Students
    WHERE ID = 1;
