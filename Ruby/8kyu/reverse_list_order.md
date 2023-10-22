# [Reverse List Order](https://www.codewars.com/kata/53da6d8d112bd1a0dc00008b)

# Description

In this kata you will create a function that takes in a list and returns a list with the reverse order.

## Examples (Input -> Output)

```
* [1, 2, 3, 4]  -> [4, 3, 2, 1]
* [9, 2, 0, 7]  -> [7, 0, 2, 9]
```

# My Solution
```ruby
def reverse_list(list)
  reversed_list = []
  index = list.size - 1
  while index >= 0
    reversed_list << list[index]
    index -= 1
  end
  reversed_list
end
```

# Better/Alternative solution from Codewars
```ruby
def reverse_list list
  list.reverse
end
```
