# [Convert boolean values to strings 'Yes' or 'No'.](https://www.codewars.com/kata/53369039d7ab3ac506000467)

# Description
Complete the method that takes a boolean value and return a <code>"Yes"</code> string for <code>true</code>, or a
<code>"No"</code> string for <code>false</code>.

# My Solution
```ruby
def bool_to_word(bool)
  bool ? 'Yes' : 'No'
end
```
