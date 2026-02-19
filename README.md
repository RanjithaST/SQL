SQL – Structured Query Language
SQL (Structured Query Language) is used to communicate with relational databases.
It helps us create, read, update, and delete data stored in tables.

SQL Statements
DDL – Data Definition Language
Used to define or change the structure of database objects.

CREATE – Create tables or databases
ALTER – Modify table structure
RENAME – Rename database objects
TRUNCATE – Remove all records from a table
DROP – Delete tables or databases

DML – Data Manipulation Language
Used to work with data inside tables.

INSERT – Add new records
UPDATE – Modify existing records
DELETE – Remove records

TCL – Transaction Control Language
Used to manage transactions.
COMMIT – Save changes permanently
ROLLBACK – Undo changes

DCL – Data Control Language
Used to control access to the database.
GRANT – Give permissions
REVOKE – Remove permissions

DQL – Data Query Language
Used to fetch data from the database.
SELECT – Retrieve data from tables

SQL Constraints
Constraints are rules applied to columns to ensure data accuracy and integrity.

PRIMARY KEY - Uniquely identifies each row in a table
FOREIGN KEY - Used to maintain relationships between tables
UNIQUE - Cannot contain Duplicate values
NOT NULL - Cannot contain NULL values
DEFAULT
CHECK

Example
CREATE TABLE Department (
    dept_id INT PRIMARY KEY,
    dept_name VARCHAR(50)
);

CREATE TABLE Employee (
    emp_id INT PRIMARY KEY,
    emp_name VARCHAR(50),
    dept_id INT,
    FOREIGN KEY (dept_id) REFERENCES Department(dept_id)
);
