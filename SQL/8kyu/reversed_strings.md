# [Reversed Strings](https://www.codewars.com/kata/5168bb5dfe9a00b126000018)

# Description
Complete the solution so that it reverses the string passed into it.

>'world'  =>  'dlrow'\
'word'   =>  'drow'

# Comment
>-- # write your SQL statement here: you are given a table 'solution' with column 'str', return a table with column 'str' and your result in a column named 'res'.

# My Solution
```SQL
SELECT str, REVERSE(str) AS res FROM solution;
```