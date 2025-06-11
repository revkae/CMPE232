```sql
-- Basic SELECT
SELECT column1, column2 FROM table_name;
SELECT * FROM employees;  -- Select all columns

-- WHERE clause for filtering
SELECT * FROM employees WHERE salary > 50000;
SELECT * FROM employees WHERE department = 'IT' AND age > 25;

-- Sorting results
SELECT * FROM employees ORDER BY salary DESC;
SELECT * FROM employees ORDER BY department, salary ASC;
```