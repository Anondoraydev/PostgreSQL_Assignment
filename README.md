# 📘 PostgreSQL Basic Concepts

This document includes basic concepts of PostgreSQL in question-answer format for quick understanding.

---

### ❓ What is PostgreSQL?

**Answer:**  
Postgre is an open-source object-relational database. Because it is relational, data can be easily stored and retrieved. Due to its performance and flexibility, it is used in large projects.

---

### ❓ Explain the Primary Key and Foreign Key concepts in PostgreSQL?

**Answer:**

- **Primary key:** It is used to uniquely identify the rows of a table. It cannot be NULL.
- **Foreign key:** When a primary key goes to another table and creates a relationship with that table, then the primary key in one table becomes a foreign key in another. It is used to create a relationship between two tables.

---

### ❓ Explain the purpose of the WHERE clause in a SELECT statement?

**Answer:**  
When we want to view data based on a specific condition, the WHERE clause is used. It can be used in SELECT, UPDATE, DELETE — these three types of SQL statements.

**Example:**
sql
SELECT * FROM students WHERE age > 18;

---
 
❓ What are the LIMIT and OFFSET clauses used for?

**Answer:**  
- LIMIT and OFFSET are commonly used for pagination.

- LIMIT specifies how many output rows will be shown.

- OFFSET specifies how many rows to skip before starting to show the results.

**Example:**
sql
SELECT * FROM student OFFSET 10 LIMIT 5;

---

❓ What is the significance of the JOIN operation, and how does it work in PostgreSQL?

**Answer:**  
JOIN is used to combine data from two tables based on a related column between them.
Joining multiple tables helps reduce data duplication and allows retrieving related information efficiently.
For JOIN to work, both tables must have a linking field (a common column).
There are several types of JOINs, such as:
INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, CROSSJOIN.
