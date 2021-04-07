## UPDATE
### 語法
```sql
UPDATE tablename
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

### 注意
- 可以使用 [WHERE](./002-WHERE-AND-OR-NOT.md) 來達成多筆資料選擇
- **不打 WHERE 會導致 Table 內所有的資料通通更新**
    - 相關案例 : [台大平台成績全被改87分 原是資工系學生抓漏洞](https://news.ltn.com.tw/news/life/breakingnews/2971370)
        - 可能是少打 WHERE 導致 (?)
