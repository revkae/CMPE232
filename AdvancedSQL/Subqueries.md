```sql
-- Subquery in WHERE clause
SELECT name FROM employees 
WHERE salary > (SELECT AVG(salary) FROM employees);

-- Correlated subquery
SELECT e1.name, e1.salary 
FROM employees e1 
WHERE e1.salary > (
    SELECT AVG(e2.salary) 
    FROM employees e2 
    WHERE e2.department = e1.department
);
```