## SELECT TOP
_指定特定數字可以控制回傳資料的數量_

### 語法
MS SQL Server / Access :
```sql
SELECT TOP number | PERCENT columnname(s)
FROM table_name
WHERE condition;
```

MySQL 沒有 `SELECT TOP`，但有 `LIMIT` :
```sql
SELECT columnname(s)
FROM tablename
WHERE condition
LIMIT number;
```

Oracle 則要用 `FETCH` (12 以後) :
```sql
SELECT columnname(s)
FROM tablename
ORDER BY columnname(s)
FETCH FIRST number ROWS ONLY;
```

與 [WHERE](../Syntax_Basic/002-WHERE-AND-OR-NOT.md) 搭配可以達到**篩選特定條件的前幾項**的效果

使用 `PERCENT` 可以顯示整體資料的前百分之幾的資料