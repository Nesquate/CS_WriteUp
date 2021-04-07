## `COUNT()` , `AVG()` 與 `SUM()`
_`COUNT()` = > 數特定 column 有多少 row_  
_`AVG()` => 特定 column 所有值的平均_  
_`SUM()` => 特定 column 所有值得總和_  

### 語法
```sql
SELECT COUNT(columnname) | AVG(columnname) | SUM(columnname)
FROM tablename
WHERE condition;
```

- 可在 `SELECT` 後加上 `AS`
    - 不加的話會自動產生一個暫時的 column 名稱叫做 `Expr1000`
- 可用 [WHERE](../../Syntax_Basic/002-WHERE-AND-OR-NOT.md) 進行條件篩選