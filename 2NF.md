## Rules
- Must be in 1NF
- All non-key attributes must be fully functionally dependent on the primary key
- Eliminates partial dependencies

---

**Before 2NF:**
```
| Student_ID | Course_ID | Student_Name | Course_Name | Grade |
|------------|-----------|--------------|-------------|--------|
| 1          | 101       | Alice        | Math        | A      |
| 1          | 102       | Alice        | Science     | B      |
```

**After 2NF:**
```
Students Table:
| Student_ID | Student_Name |
|------------|--------------|
| 1          | Alice        |

Courses Table:
| Course_ID | Course_Name |
|-----------|-------------|
| 101       | Math        |
| 102       | Science     |

Enrollments Table:
| Student_ID | Course_ID | Grade |
|------------|-----------|-------|
| 1          | 101       | A     |
| 1          | 102       | B     |
```