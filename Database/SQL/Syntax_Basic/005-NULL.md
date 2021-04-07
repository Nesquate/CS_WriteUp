## NULL
**空** ，沒有內容，跟 0 不一樣，**0算有內容**

可以在 [WHERE](./002-WHERE-AND-OR-NOT.md) 用 `IS NULL` 或 `IS NOT NULL` 測試

```sql=
SELECT column1, column2, ...
FROM tablename
WHERE condition(s) IS|IS NOT NULL
```