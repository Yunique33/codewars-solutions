# [Check same case](https://www.codewars.com/kata/5dd462a573ee6d0014ce715b)

# Description
Write a function that will check if two given characters are the same case.

* If either of the characters is not a letter, return <code>-1</code>
* If both characters are the same case, return <code>1</code>
* If both characters are letters, but not the same case, return <code>0</code>

## Examples
<code>'a'</code> and <code>'g'</code> returns <code>1</code>\
<code>'A'</code> and <code>'C'</code> returns <code>1</code>\
<code>'b'</code> and <code>'G'</code> returns <code>0</code>\
<code>'B'</code> and <code>'g'</code> returns <code>0</code>\
<code>'0'</code> and <code>'?'</code> returns <code>-1</code>



# My Solution
```ruby
def same_case(a, b)
  if [a,b].all?(/[[:alpha:]]/)
    a.match?(/[A-Z]/) == b.match?(/[A-Z]/) ? 1 : 0
  else
    -1
  end
end
```
