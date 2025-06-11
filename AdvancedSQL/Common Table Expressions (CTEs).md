```sql
WITH high_earners AS (
    SELECT * FROM employees WHERE salary > 70000
)
SELECT department, COUNT(*) as high_earner_count
FROM high_earners
GROUP BY department;
```