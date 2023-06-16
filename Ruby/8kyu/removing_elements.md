# [Removing Elements](https://www.codewars.com/kata/5769b3802ae6f8e4890009d2)

# Description
Take an array and remove every second element from the array. Always keep the first element and start removing with the 
next element.

### Example:
<code>["Keep", "Remove", "Keep", "Remove", "Keep", ...]</code> --> <code>["Keep", "Keep", "Keep", ...]</code>

None of the arrays will be empty, so you don't have to worry about that!

# My Solution
```ruby
def remove_every_other(arr)
  arr.select.with_index { |_, i| i.even? }
end
```
# Better/Alternative solution from Codewars
```ruby
def remove_every_other(arr)
  arr.each_slice(2).map(&:first)
end
```
