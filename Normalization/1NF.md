> [!NOTE] Rules
> - Each column contains atomic (indivisible) values
> - Each column contains values of the same type
> - Each column has a unique name
> - Order of rows and columns doesn't matter

---

**Before 1NF:**

| Employee_ID | Name | Phone_Numbers      |
| ----------- | ---- | ------------------ |
| 1           | John | 555-1234, 555-5678 |


**After 1NF:**

| Employee_ID | Name | Phone_Numbers |
| ----------- | ---- | ------------- |
| 1           | John | 555-1234      |
| 1           | John | 555-5678      |
