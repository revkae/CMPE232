```sql
-- INSERT new records
INSERT INTO employees (name, department, salary) 
VALUES ('John Doe', 'IT', 60000);

-- UPDATE existing records
UPDATE employees 
SET salary = 65000 
WHERE employee_id = 1;

-- DELETE records
DELETE FROM employees WHERE department = 'Marketing';
```