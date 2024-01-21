# [Logical calculator](https://www.codewars.com/kata/57096af70dad013aa200007b)

# Description
## Your Task
Given an array of Boolean values and a logical operator, return a Boolean result based on sequentially applying the 
operator to the values in the array.

## Examples
1. booleans = `[True, True, False]`, operator = `"AND"`
* `True` `AND` `True` -> `True`
* `True` `AND` `False` -> `False`
* return `False`

2. booleans = `[True, True, False]`, operator = `"OR"`
* `True` `OR` `True` -> `True`
* `True` `OR` `False` -> `True`
* return `True`

3. booleans = `[True, True, False]`, operator = `"XOR"`
* `True` `XOR` `True` -> `False`
* `False` `XOR` `False` -> `False`
* return `False`

## Input
1. an array of Boolean values `(1 <= array_length <= 50)`
2. a string specifying a logical operator: `"AND"`, `"OR"`, `"XOR"`

## Output
A Boolean value (`True` or `False`).

# My Solution
```ruby
def logical_calc(array, op)
   case op
   when "AND"
      array.all?
   when "OR"
      array.any?
   when "XOR"
      array.count(true) % 2 != 0
   end
end
```

# Better/Alternative solution from Codewars
```ruby
def logical_calc(arr, op)
  op=='AND' ? arr.reduce(:&) : op=='OR' ? arr.reduce(:|) : arr.reduce(:^)
end
```
