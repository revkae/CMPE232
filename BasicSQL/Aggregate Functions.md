```sql
-- COUNT, SUM, AVG, MIN, MAX
SELECT COUNT(*) FROM employees;
SELECT AVG(salary) FROM employees;
SELECT department, SUM(salary) FROM employees GROUP BY department;

-- GROUP BY with HAVING
SELECT department, AVG(salary) 
FROM employees 
GROUP BY department 
HAVING AVG(salary) > 55000;
```