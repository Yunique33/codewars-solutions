# [Adults only (SQL for Beginners #1)](https://www.codewars.com/kata/590a95eede09f87472000213)

# Description
In your application, there is a section for adults only. You need to get a list of names and ages of users from the users table, who are 18 years old or older.

users table schema

* name
* age

# My Solution
```SQL
SELECT name, age FROM users
WHERE age >= 18;
```
