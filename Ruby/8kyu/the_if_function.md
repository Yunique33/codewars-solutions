# [The 'if' function](https://www.codewars.com/kata/54147087d5c2ebe4f1000805)

# Description
Create a function called _`if` which takes 3 arguments: a value `bool` and 2 functions (which do not take any 
parameters): `func1` and `func2`

When `bool` is truthy, `func1` should be called, otherwise call the `func2`.

## Example:
```ruby
_if(true, proc{puts "True"}, proc{puts "False"})
# Logs 'True' to the console.
```

# My Solution
```ruby
def _if(bool, ifTrue, ifFalse)
  bool ? ifTrue.call : ifFalse.call
end
```
