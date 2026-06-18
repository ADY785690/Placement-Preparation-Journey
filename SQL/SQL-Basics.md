# SQL Basics

## What is SQL?

SQL (Structured Query Language) is used to communicate with relational databases.

Examples:
- MySQL
- PostgreSQL
- Oracle
- SQL Server

---

## Important Commands

### SELECT

Used to retrieve data.

```sql
SELECT * FROM Employees;
```

---

### WHERE

Used for filtering.

```sql
SELECT *
FROM Employees
WHERE Salary > 50000;
```

---

### ORDER BY

Used for sorting.

```sql
SELECT *
FROM Employees
ORDER BY Salary DESC;
```

---

### DISTINCT

Returns unique values.

```sql
SELECT DISTINCT Department
FROM Employees;
```

---

### LIMIT

Returns limited records.

```sql
SELECT *
FROM Employees
LIMIT 5;
```

---

## Aggregate Functions

### COUNT()

```sql
SELECT COUNT(*)
FROM Employees;
```

### SUM()

```sql
SELECT SUM(Salary)
FROM Employees;
```

### AVG()

```sql
SELECT AVG(Salary)
FROM Employees;
```

### MAX()

```sql
SELECT MAX(Salary)
FROM Employees;
```

### MIN()

```sql
SELECT MIN(Salary)
FROM Employees;
```

---

## Operators

### AND

```sql
SELECT *
FROM Employees
WHERE Salary > 50000
AND Department='IT';
```

### OR

```sql
SELECT *
FROM Employees
WHERE Department='IT'
OR Department='HR';
```

---

## SQL Execution Order

1. FROM
2. WHERE
3. GROUP BY
4. HAVING
5. SELECT
6. ORDER BY

---

## Common Interview Questions

Q1. Difference between WHERE and HAVING?

WHERE:
Filters rows before grouping.

HAVING:
Filters groups after grouping.

---

Q2. Difference between DELETE and TRUNCATE?

DELETE:
- Removes selected rows
- Can use WHERE

TRUNCATE:
- Removes all rows
- Faster

---

## Frequently Asked Placement Questions

1. Second Highest Salary
2. Employee Count by Department
3. Duplicate Records
4. Top N Records
5. Joins

---

## Revision Notes

SELECT = Retrieve Data

WHERE = Filter Rows

ORDER BY = Sort Data

GROUP BY = Group Data

HAVING = Filter Groups
