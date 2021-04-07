## WHERE
_篩選資料(filter)_
### 基本語法
```sql
SELECT column1, column2, ...
FROM tablename
WHERE condition(s)
```

> 不一定只有 `SELECT` 才能用 `WHERE`，其他語法也可以

### 相關操作
- 大於、小於、等於、不等於
    - 注意不等於有可能是 `<>` 或 `!=` (根據資料庫系統而定)
- `BETWEEN` : 特定區間 (與 [AND](#AND-OR-NOT) 搭配)
- `LIKE` : 字符篩選
- `IN` : 多重 conditions 篩選

### 注意
- 字串、字元要包起來 ( `''` 或 `""`)，數字不用
- 字串也可以用大於小於，[但似乎是根據字元集比較](https://stackoverflow.com/questions/26080187/sql-string-comparison-greater-than-and-less-than-operators)
    - 個人猜測是 ASCII code
    - 字串字元比較有**大小寫區分**

### AND, OR, NOT
`AND` 與 `OR` 用在 `WHERE` 上可以將多個 condition 聯合在一起比較  
而 `NOT` 則是 condition 的相反

語法大致上如下：  
```sql
WHERE condition1 AND condition2 AND ...;
-- 可以將 AND 換成 OR ，OR 的寫法跟 AND 差不多
-- NOT 則要擺在最前面
WHERE NOT condition;
-- 或是
WHERE NOT condition1 AND NOT condition2;
-- 之類的
```
如果要將他們結合在一起比較，你可能會需要括號