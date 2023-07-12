# [Multiplication table for number](https://www.codewars.com/kata/5a2fd38b55519ed98f0000ce)

# Description
Your goal is to return multiplication table for <code>number</code> that is always an integer from 1 to 10.

For example, a multiplication table (string) for <code>number == 5</code> looks like below:

>1 * 5 = 5\
2 * 5 = 10\
3 * 5 = 15\
4 * 5 = 20\
5 * 5 = 25\
6 * 5 = 30\
7 * 5 = 35\
8 * 5 = 40\
9 * 5 = 45\
10 * 5 = 50

P. S. You can use <code>\n</code> in string to jump to the next line.

Note: newlines should be added between rows, but there should be no trailing newline at the end. If you're unsure about 
the format, look at the sample tests.

```ruby
def multiTable(number)
  (1..10).to_a.map { |el| "#{el} * #{number} = #{ el * number }" }.join("\n")
end
```
