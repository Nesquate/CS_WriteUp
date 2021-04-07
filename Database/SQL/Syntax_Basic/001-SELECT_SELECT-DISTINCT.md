## SELECT 與 SELECT DISTINCT
_用於選擇想要顯示的 column_
### 基本語法
```sql=
SELECT column1, column2, ...
FROM tablename;
```
這樣就可以顯示特定欄位的所有值

至於 `SELECT DISTINCT` 則是選取**不重複資料**

### 利用 SELECT DISTINCT 數個數
```sql
-- MS Access 不支援
SELECT COUNT(DISTINCT columnname) FROM tablename;
-- MS Access 的語法
SELECT COUNT(*) AS DistinctCount 
FROM (SELECT columnname FROM tablename);
```