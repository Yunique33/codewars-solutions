# [Expressions Matter](https://www.codewars.com/kata/5ae62fcf252e66d44d00008e)

## Description
### Task
* _**Given** three integers `a`, `b`, `c`, **return** the **largest number** obtained after inserting the following 
operators and brackets: `+`, `*`, `()`
* In other words , _**try every combination of a,b,c with [*+()] , and return the Maximum Obtained**_ 
<span style="color:red">(Read the notes for more detail about it)<span>

### Example
_**With the numbers are 1, 2 and 3**, here are some ways of placing signs and brackets:_

* `1 * (2 + 3) = 5`
* `1 * 2 * 3 = 6`
* `1 + 2 * 3 = 7`
* `(1 + 2) * 3 = 9`

So _**the maximum value**_ that you can obtain is **_9_**.

### Notes
* _**The numbers** are always **positive**._
* _**The numbers** are in the range **(1 ≤ a,b,c ≤ 10)**._
* _You can use the same operation **more than once**._
* **It's not necessary** _to place all the signs and brackets._
* _**Repetition** in numbers may occur._
* You _**cannot swap the operands**_. For instance, in the given example **_you cannot get expression_** 
`(1 + 3) * 2 = 8`.

### Input >> Output Examples:
> expressionsMatter(1,2,3)  ==>  return 9

### _Explanation:_
_After placing signs and brackets, the **Maximum value** obtained from the expression_ `(1+2) * 3 = 9`.

---

> expressionsMatter(1,1,1)  ==>  return 3

### _Explanation:_
_After placing signs, the **Maximum value** obtained from the expression is_ `1 + 1 + 1 = 3`.

---

> expressionsMatter(9,1,1)  ==>  return 18

### _Explanation:_
_After placing signs and brackets, the **Maximum value** obtained from the expression is_ `9 * (1+1) = 18`.

---

### Task
* _**Given** three integers_ `a`, `b`, `c` _**return** the **largest number** obtained after inserting the following 
operators and brackets:_ `+`, `*`, `()`
* In other words , _**try every combination of a,b,c with [*+()] , and return the Maximum Obtained**_

### Example
_**With the numbers are 1, 2 and 3**, here are some ways of placing signs and brackets:_

* `1 * (2 + 3) = 5`
* `1 * 2 * 3 = 6`
* `1 + 2 * 3 = 7`
* `(1 + 2) * 3 = 9`

So _**the maximum value**_ that you can obtain is **_9_**.

### Notes
* _**The numbers** are always **positive**._
* _**The numbers** are in the range **(1 ≤ a,b,c ≤ 10)**._
* _You can use the same operation **more than once**._
* **It's not necessary** _to place all the signs and brackets._
* _**Repetition** in numbers may occur._
* You _**cannot swap the operands**_. For instance, in the given example **_you cannot get expression_**
`(1 + 3) * 2 = 8`.

---

### Input >> Output Examples:
> expressionsMatter(1,2,3)  ==>  return 9

### _Explanation:_
_After placing signs and brackets, the **Maximum value** obtained from the expression is_ `(1+2) * 3 = 9`.

---

``` 
expressionsMatter(1,1,1)  ==>  return 3
```
---

### My Solution
```ruby
def expression_matter(a,b,c)
  [(a + b) * c, a * (b + c), a * b * c, a + b + c].max
end
```
