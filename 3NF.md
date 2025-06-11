## Rules
- Must be in 2NF
- No transitive dependencies (non-key attributes shouldn't depend on other non-key attributes)

---

**Before 3NF:**
```
| Employee_ID | Name | Department_ID | Department_Name | Department_Head |
|-------------|------|---------------|-----------------|-----------------|
| 1           | John | 10            | IT              | Sarah           |
```

**After 3NF:**
```
Employees Table:
| Employee_ID | Name | Department_ID |
|-------------|------|---------------|
| 1           | John | 10            |

Departments Table:
| Department_ID | Department_Name | Department_Head |
|---------------|-----------------|-----------------|
| 10            | IT              | Sarah           |
```