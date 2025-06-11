```sql
-- INNER JOIN (only matching records)
SELECT e.name, d.department_name 
FROM employees e 
INNER JOIN departments d ON e.dept_id = d.dept_id;

-- LEFT JOIN (all records from left table)
SELECT e.name, d.department_name 
FROM employees e 
LEFT JOIN departments d ON e.dept_id = d.dept_id;

-- RIGHT JOIN (all records from right table)
SELECT e.name, d.department_name 
FROM employees e 
RIGHT JOIN departments d ON e.dept_id = d.dept_id;
```