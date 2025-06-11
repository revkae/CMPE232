```sql
-- ROW_NUMBER, RANK, DENSE_RANK
SELECT name, salary, 
    ROW_NUMBER() OVER (ORDER BY salary DESC) as row_num,
    RANK() OVER (ORDER BY salary DESC) as rank_pos
FROM employees;

-- Partition by department
SELECT name, department, salary,
    AVG(salary) OVER (PARTITION BY department) as dept_avg
FROM employees;
```