```sql
-- String functions
SELECT UPPER(name), LENGTH(name), SUBSTRING(name, 1, 3) FROM employees;

-- Date functions
SELECT name, hire_date, 
    DATEDIFF(CURRENT_DATE, hire_date) as days_employed
FROM employees;

-- CASE statements
SELECT name, salary,
    CASE 
        WHEN salary > 80000 THEN 'High'
        WHEN salary > 50000 THEN 'Medium'
        ELSE 'Low'
    END as salary_category
FROM employees;
```