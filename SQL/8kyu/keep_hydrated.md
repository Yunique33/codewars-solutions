# [Keep Hydrated!](https://www.codewars.com/kata/582cb0224e56e068d800003c)

# Description
Nathan loves cycling.

Because Nathan knows it is important to stay hydrated, he drinks 0.5 litres of water per hour of cycling.

You get given the time in hours and you need to return the number of litres Nathan will drink, rounded to the smallest 
value.

For example:

>hours = 3 ----> liters = 1
>
>hours = 6.7---> liters = 3
>
>hours = 11.8--> liters = 5

Input data is available from the table <code>cycling</code>, which has 2 columns: <code>id</code> 
and <code>hours</code>. For each row, you have to return 3 columns: <code>id</code>, <code>hours</code> and
<code>liters</code>(not litres, it's a difference from the kata description)

# My Solution
```SQL
SELECT id,
       hours,
       FLOOR(hours * 0.5) AS liters
FROM cycling;
```
# Better/Alternative solution from Codewars
```sql
SELECT *, floor(hours / 2) as liters FROM cycling
```
