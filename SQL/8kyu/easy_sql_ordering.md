# [Easy SQL - Ordering](https://www.codewars.com/kata/593ed37c93350098d600001d)

# Description
Your task is to sort the information in the provided table 'companies' by number of employees (high to low). Returned 
table should be in the same format as provided:

**companies table schema**

* id
* ceo
* motto
* employees

Solution should use pure SQL.

# My Solution
```SQL
SELECT * FROM companies
ORDER BY employees DESC;
```
