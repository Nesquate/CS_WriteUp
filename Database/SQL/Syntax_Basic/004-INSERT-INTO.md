## INSERT INTO
_插入一筆資料_
### 基本語法
```sql=
INSERT INTO tablename (column1, column2, ...)
VALUES (value1, value2, ...);
```
### 注意
1. 在已知要填入的欄位的順序下，可以簡化成：
```sql
INSERT INTO tablename
VALUES (value1, value2, ...);
```
2. 可以只填入特定欄位，但記得要填寫欲被填入的格子  
未填入的 attribute，value 會變成 `null`
3. 字串字元一定要加上引號，而數字可不加
    - 個人覺得還是加一下好了...怕資料填不進去