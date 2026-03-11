# MySQL
MySQL is a database management system used to store and manage data in tables using SQL queries.

## Key Features of MySQL
- Open-source and free to use
- Fast and reliable database system
- Supports large databases
- Uses SQL for database operations
- Works on many platforms (Windows, Linux, etc.)

## Example of MySQL Query
### 1️⃣ CREATE (Create Table)
Used to create a new table in the database.

#### Syntax
    CREATE TABLE table_name (
        column1 datatype,
        column2 datatype,
        column3 datatype
    );

#### Example
    CREATE TABLE Students (
        ID INT,
        Name VARCHAR(50),
        Age INT
    );
This creates a table Students with three columns.

_____________________________________________________________________________________________________________________________________________

### 2️⃣ INSERT (Insert Data)
Used to add records into a table.

#### Syntax
    INSERT INTO table_name (column1, column2, column3)
    VALUES (value1, value2, value3);

#### Example
    INSERT INTO Students (ID, Name, Age)
    VALUES (1, 'Kimi', 20);

_____________________________________________________________________________________________________________________________________________

### 3️⃣ ALTER (Modify Table)
Used to add, delete, or modify columns in a table.

#### Add Column
    ALTER TABLE Students
    ADD Email VARCHAR(100);

#### Modify Column
    ALTER TABLE Students
    MODIFY Age INT;

#### Delete Column
    ALTER TABLE Students
    DROP COLUMN Email;

_____________________________________________________________________________________________________________________________________________

### 4️⃣ CONSTRAINT (Rules for Table Data)
Constraints are used to limit the type of data that can be inserted.

#### Common Constraints
- NOT NULL
- UNIQUE
- PRIMARY KEY
- FOREIGN KEY
- CHECK
- DEFAULT

#### Example
    CREATE TABLE Students (
        ID INT PRIMARY KEY,
        Name VARCHAR(50) NOT NULL,
        Age INT CHECK (Age >= 18)
    );

Explanation:
- PRIMARY KEY → unique identifier
- NOT NULL → value cannot be empty
- CHECK → condition for data

_____________________________________________________________________________________________________________________________________________

### 5️⃣ BACKUP DATABASE
Used to create a backup of a database.

#### Syntax (SQL Server)
    BACKUP DATABASE database_name
    TO DISK = 'C:\backup\database_name.bak';

#### Example
    BACKUP DATABASE SchoolDB
    TO DISK = 'C:\backup\SchoolDB.bak';

_____________________________________________________________________________________________________________________________________________

### 6️⃣ CHECK Constraint
Used to limit the values that can be inserted into a column.

#### Syntax
    CREATE TABLE Students (
        ID INT,
        Age INT CHECK (Age >= 18)
    );

#### Example
    INSERT INTO Students VALUES (1, 20);

If age is less than 18, the database will reject the value.

_____________________________________________________________________________________________________________________________________________

### 7️⃣ NOT NULL Constraint
Ensures that a column cannot have NULL (empty) values.

#### Syntax
    CREATE TABLE Students (
        ID INT,
        Name VARCHAR(50) NOT NULL
    );

#### Example
    INSERT INTO Students (ID, Name)
    VALUES (1, 'Kimi');

_____________________________________________________________________________________________________________________________________________

### 8️⃣ UNIQUE Constraint
Ensures that all values in a column are different.

#### Syntax
    CREATE TABLE Students (
        Email VARCHAR(100) UNIQUE
    );

#### Example
    INSERT INTO Students (Email)
    VALUES ('kimi@gmail.com');

Two rows cannot have the same email.

_____________________________________________________________________________________________________________________________________________

### 9️⃣ PRIMARY KEY
A primary key uniquely identifies each record in a table.

#### Syntax
    CREATE TABLE Students (
        ID INT PRIMARY KEY,
        Name VARCHAR(50)
    );

#### Example
    INSERT INTO Students VALUES (1, 'Kimi');

Primary key:
- Must be unique
- Cannot be NULL

_____________________________________________________________________________________________________________________________________________

### 🔟 FOREIGN KEY
A foreign key links two tables together.

#### Syntax
    CREATE TABLE Orders (
        OrderID INT,
        StudentID INT,
        FOREIGN KEY (StudentID) REFERENCES Students(ID)
    );
This connects Orders table to Students table.

_____________________________________________________________________________________________________________________________________________

### 1️⃣1️⃣ DEFAULT Constraint
Sets a default value for a column if no value is provided.

#### Syntax
    CREATE TABLE Students (
        ID INT,
        Country VARCHAR(50) DEFAULT 'India'
    );

#### Example
    INSERT INTO Students (ID)
    VALUES (1);
Output:

ID | Country
1  | India

_____________________________________________________________________________________________________________________________________________

### 1️⃣2️⃣ INDEX
An index improves the speed of data retrieval.

#### Syntax
    CREATE INDEX idx_name
    ON Students (Name);
This makes searching faster.

_____________________________________________________________________________________________________________________________________________

### 1️⃣3️⃣ AUTO_INCREMENT
Automatically generates unique numbers for new rows.

#### Syntax
    CREATE TABLE Students (
        ID INT AUTO_INCREMENT PRIMARY KEY,
        Name VARCHAR(50)
    );

#### Example
    INSERT INTO Students (Name)
    VALUES ('Kimi');
The ID will automatically become 1, 2, 3...

_____________________________________________________________________________________________________________________________________________

### 1️⃣4️⃣ DATES
SQL supports date and time data types.

#### Syntax
    CREATE TABLE Events (
        EventDate DATE
    );

#### Example
    INSERT INTO Events VALUES ('2026-03-11');
Date format:

    YYYY-MM-DD

_____________________________________________________________________________________________________________________________________________

### 1️⃣5️⃣ VIEWS
A view is a virtual table based on a SQL query.

#### Syntax
    CREATE VIEW StudentView AS
    SELECT Name, Age
    FROM Students;

Example
SELECT * FROM StudentView;
