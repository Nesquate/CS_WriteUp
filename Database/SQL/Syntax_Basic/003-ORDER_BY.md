## ORDER BY
_資料排序_
### 基本語法
```sql
SELECT column1, column2, ...
FROM tablename
ORDER BY columnname1, columnname2, ... ASC|DESC
```

- `columnname1` , `columnname2` 的順序會影響排序  
ex: `columnname1` 先排完，如果 `columnname1` 有重複，再根據 `columnname2` 做排序
- 預設是由低到高 (ascending), 也就是 `ASC`  
如果要由高到低 (descending) 排序，要在欄位名稱後面打上 `DESC`