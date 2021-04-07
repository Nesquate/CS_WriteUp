# SQL 筆記
此處為資料庫 SQL 相關筆記。

一樣的，若有任何錯誤，歡迎提 Issue 跟我說。

資料參考：  
- [W3School](https://www.w3schools.com/sql/)

下面為基本簡介。

---

## SQL 簡介
### 簡單介紹
SQL (Structured Query Language) => 存取、操作資料庫的語言  
分別在 1986 (ANSI)、1987 (ISO) 成為國際標準

在 W3School 學到的應該是 ANSI 標準  
(其實標準應該大同小異)

必須要注意的是，儘管有標準，各家資料庫的語法 (如 MySQL 或 MSSQL) 仍有些不同

### RDBMS 
Relational Database Management System  
**基於 SQL 的**關聯式資料庫管理系統

Data 由 Table 儲存  
每個 Table 有 Attribute (資料的屬性，當作表個的 First row 也行)  
其他的 row 為 Table 的 records

反正有用過 Excel 應該不會太難理解

## SQL 語法
### 原則
- 指令**不分大小寫**，但建議統一寫法 (一下大寫一下小寫會造成維護者困擾)
- **不一定有分號**，這部份根據不同的資料庫系統而有不同的規定
    - W3School 有分號