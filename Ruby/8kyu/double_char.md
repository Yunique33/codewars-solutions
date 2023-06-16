# [Double Char](https://www.codewars.com/kata/56b1f01c247c01db92000076)

# Description
Given a string, you have to return a string in which each character (case-sensitive) is repeated once.

### Examples (Input -> Output):
<pre>
* "String"      -> "SSttrriinngg"
* "Hello World" -> "HHeelllloo  WWoorrlldd"
* "1234!_ "     -> "11223344!!__  "
</pre>

Good Luck!

# My Solution
```ruby
def double_char(str)
  str.chars.map { |ch| ch*2 }.join
end
```
# Better/Alternative solution from Codewars
```ruby
def double_char(str)
  str.gsub /(.)/, '\1\1'
end
```
