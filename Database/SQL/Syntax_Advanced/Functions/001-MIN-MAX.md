## `MIN()` 與 `MAX()`
_取出資料特定 column 當中的最大值與最小值_

### 語法
```sql
SELECT MIN(columnname) | MAX(columnname)
FROM tablename
WHERE condition;
```

### 注意
- 可在 `SELECT` 後加上 `AS`
    - 不加的話會自動產生一個暫時的 column 名稱叫做 `Expr1000`
- 可用 [WHERE](../../Syntax_Basic/002-WHERE-AND-OR-NOT.md) 進行條件篩選