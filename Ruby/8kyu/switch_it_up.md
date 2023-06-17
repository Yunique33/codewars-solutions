# [Switch it Up!](https://www.codewars.com/kata/5808dcb8f0ed42ae34000031)

# Description
When provided with a number between 0-9, return it in words.

Input :: 1

Output :: "One".

If your language supports it, try using a [switch statement](https://en.wikipedia.org/wiki/Switch_statement).

# My Solution
```ruby
def switch_it_up(number)
  case number
  when 1 then 'One'
  when 2 then 'Two'
  when 3 then 'Three'
  when 4 then 'Four'
  when 5 then 'Five'
  when 6 then 'Six'
  when 7 then 'Seven'
  when 8 then 'Eight'
  when 9 then 'Nine'
  else
    'Zero'
  end
end
```
