📘 SQL Basics – Database & Table Commands (Soft Copy)
1️⃣ CREATE DATABASE
CREATE DATABASE DBNAME;

Explanation:
Creates a new database with the given name.

2️⃣ DROP DATABASE
DROP DATABASE DBNAME;

Explanation:
Deletes (removes) the database permanently along with all its tables and data.

⚠️ Warning: This action cannot be undone.

3️⃣ USE DATABASE
USE DBNAME;    


Explanation:
Selects the database so that all operations (tables, insert, select, etc.) are performed inside it.

4️⃣ CREATE DATABASE IF NOT EXISTS
CREATE DATABASE IF NOT EXISTS DBNAME;


Explanation:

Checks whether the database already exists

If it exists → shows a warning

If it does not exist → creates the database

5️⃣ DROP DATABASE IF EXISTS
DROP DATABASE IF EXISTS DBNAME;


Explanation:

Checks whether the database exists

If it exists → deletes the database

If it does not exist → no error occurs

6️⃣ SHOW DATABASES
SHOW DATABASES;


Explanation:
Displays the names of all databases available in the MySQL server.

7️⃣ SHOW TABLES
SHOW TABLES;


Explanation:
Displays all tables present in the currently selected database.

8️⃣ SELECT STATEMENT
SELECT * FROM TABLENAME;

Explanation:
Selects and displays all records (rows) and all fields (columns) from a table.

You must select from a table, not a database.

9️⃣ FIELDS (COLUMNS)

Explanation:
Fields are the columns in a table.
They represent attributes or properties.

Example:

id | name | age

🔟 RECORDS (ROWS)

Explanation:
Records are the rows in a table.
Each record represents one complete entry.

Example:

1 | Ramu | 21

1️⃣1️⃣ TABLE NAME

Explanation:
The table name is written above the table structure and is used in SQL queries to access data.

1️⃣2️⃣ PRIMARY KEY

Explanation:

A field that uniquely identifies each record in a table

Cannot contain NULL values

Cannot have duplicate values

Example:

id INT PRIMARY KEY

1️⃣3️⃣ FOREIGN KEY

Explanation:

A field in one table that refers to the primary key of another table

Used to create a relationship between tables

Example:

FOREIGN KEY (student_id) REFERENCES students(id)

1️⃣4️⃣ CREATE TABLE :

CREATE TABLE TBNAME (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    age INT,
    email VARCHAR(100)
);


Explanation:
Creates a table with:

id as primary key

name, age, and email as fields (columns)

Each field has a datatype

1️⃣5️⃣ INSERT INTO TABLE
INSERT INTO TBNAME VALUES (1, 'Ramu', 21, 'ramu@gmail.com');


Explanation:
Inserts data into the table in the same order as the fields.

✅ Better & safer method:

INSERT INTO TBNAME (id, name, age, email)
VALUES (2, 'Kumar', 22, 'kumar@gmail.com');

