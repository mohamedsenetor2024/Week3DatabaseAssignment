# Week 3 Database Assignment – SQL Transactions and Data Manipulation

## 📌 Project Overview

This assignment focuses on practicing SQL database management using MySQL. It demonstrates how to create database tables, insert records, update existing data, and retrieve information using SQL statements.

The assignment is part of the Database module and builds practical skills in managing relational databases and manipulating records.

## 🎯 Learning Objectives

By completing this assignment, I practiced how to:

- Create database tables with appropriate data types.
- Define primary keys to uniquely identify records.
- Insert multiple records into a database table.
- Update existing records using SQL UPDATE statements.
- Retrieve and verify database records using SELECT queries.
- Understand basic SQL data manipulation operations.

## 🛠️ Technologies Used

- **Database Management System:** MySQL
- **Database Tool:** MySQL Workbench
- **Language:** Structured Query Language (SQL)

## 📝 Assignment Tasks and Solutions

### Question 1: Create a Student Table

Created a table named `student` with the following columns:

- `id` – Integer and Primary Key.
- `fullName` – VARCHAR(100), stores student names.
- `age` – Integer, stores student ages.

**SQL Statement:**

```sql
CREATE TABLE student (
    id INT PRIMARY KEY,
    fullName VARCHAR(100),
    age INT
);
```

### Question 2: Insert Student Records

Inserted three student records into the `student` table.

**SQL Statement:**

```sql
INSERT INTO student (id, fullName, age)
VALUES
    (1, 'Mohamed Ahmed', 25),
    (2, 'Abdi Hassan', 22),
    (3, 'Fatima Ali', 24);
```

**Verification Query:**

```sql
SELECT * FROM student;
```

**Result:** Three records were successfully inserted into the table.

### Question 3: Update Student Age

Updated the age of the student whose ID is 2 from 22 to 20.

**SQL Statement:**

```sql
UPDATE student
SET age = 20
WHERE id = 2;
```

**Verification Query:**

```sql
SELECT * FROM student
WHERE id = 2;
```

**Result:** The student's age was successfully updated from 22 to 20.

## 📊 Final Database Records

After completing all three tasks, the student table contains the following records:

| ID | Full Name | Age |
|---|---|---|
| 1 | Mohamed Ahmed | 25 |
| 2 | Abdi Hassan | 20 |
| 3 | Fatima Ali | 24 |

## 📚 Key Concepts Learned

| SQL Command | Purpose |
|---|---|
| CREATE TABLE | Creates a new database table. |
| INSERT INTO | Adds new records to a table. |
| UPDATE | Modifies existing records. |
| WHERE | Specifies which records to modify or retrieve. |
| SELECT | Retrieves data from a table. |
| PRIMARY KEY | Uniquely identifies each record. |

## 🚀 Conclusion

This assignment provided practical experience in SQL database creation and data manipulation using MySQL.

I successfully created a student table, inserted three records, and updated a student's age using SQL statements.

These exercises strengthened my understanding of relational database management and prepared me for more advanced SQL concepts, including aggregate functions and database transactions.

---

**Module:** Database Management  
**Week:** 3  
**Assignment:** SQL Transactions and Data Manipulation  
**Database System:** MySQL