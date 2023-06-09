# [Beginner Series #2 Clock](https://www.codewars.com/kata/55f9bca8ecaa9eac7100004a)

# Description
Clock shows <code>h</code> hours, <code>m</code> minutes and <code>s</code> seconds after midnight.

Your task is to write a function which returns the time since midnight in milliseconds.

### Example:
>h = 0\
m = 1\
s = 1
>
>result = 61000

Input constraints:

* <code>0 <= h <= 23</code>
* <code>0 <= m <= 59</code>
* <code>0 <= s <= 59</code>

# My Solution
```ruby
def past(h, m, s)
  1000*(3_600*h + 60*m + s)
end
```
