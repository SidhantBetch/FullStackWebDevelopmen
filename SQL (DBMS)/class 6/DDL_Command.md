# DDL (Data Definition Language)
DDL (Data Definition Language) commands are used to define and manage the structure of database objects such as tables, schemas, and indexes. 🗄️
They change the structure of the database, not the data itself.

## Main DDL Commands
### 1️⃣ CREATE
Used to create a new table or database.

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

__________________________________________________________________________________________________________________________________________

### 2️⃣ ALTER
Used to modify the structure of an existing table.

#### Add Column
ALTER TABLE Students
ADD Email VARCHAR(100);

#### Modify Column
ALTER TABLE Students
MODIFY Age INT;

__________________________________________________________________________________________________________________________________________

### 3️⃣ DROP
Used to delete a table from the database.

#### Syntax
DROP TABLE table_name;

#### Example
DROP TABLE Students;

__________________________________________________________________________________________________________________________________________

### 4️⃣ TRUNCATE
Used to remove all records from a table but keep the table structure.

#### Syntax
TRUNCATE TABLE table_name;

#### Example
TRUNCATE TABLE Students;

__________________________________________________________________________________________________________________________________________

### 5️⃣ RENAME
Used to rename a table.

#### Syntax
RENAME TABLE old_table_name TO new_table_name;

Example
RENAME TABLE Students TO StudentData;
