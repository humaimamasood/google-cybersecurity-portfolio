# SQL - Filtering Queries

## Objective
Learn how to filter data from a database using SQL.

## Commands

### Select all records

```sql
SELECT * FROM employees;
```

### Filter by department

```sql
SELECT * FROM employees
WHERE department = 'IT';
```

### Filter by salary

```sql
SELECT * FROM employees
WHERE salary > 50000;
```

### Multiple conditions

```sql
SELECT * FROM employees
WHERE department = 'IT'
AND salary > 50000;
```

### OR condition

```sql
SELECT * FROM employees
WHERE department = 'IT'
OR department = 'HR';
```

### LIKE

```sql
SELECT * FROM employees
WHERE name LIKE 'A%';
```

### BETWEEN

```sql
SELECT * FROM employees
WHERE salary BETWEEN 30000 AND 60000;
```

### IN

```sql
SELECT * FROM employees
WHERE department IN ('IT', 'Finance');
```

## Skills Learned

- WHERE clause
- AND / OR
- LIKE
- BETWEEN
- IN
- Filtering records

## Result

Successfully filtered records using SQL queries.
