# [Is it a palindrome?](https://www.codewars.com/kata/57a1fd2ce298a731b20006a4)

# Description
Write a function that checks if a given string (case insensitive) is a 
[palindrome](https://en.wikipedia.org/wiki/Palindrome). A palindrome is a word, number, phrase, or other sequence of 
symbols that reads the same backwards as forwards, such as madam or racecar, the date and time 12/21/33 12:21, and the 
sentence: "A man, a plan, a canal – Panama"

# My Solution
```ruby
def is_palindrome(str)
  str.downcase!
  str == str.reverse
end
```
# Better/Alternative solution from Codewars
```ruby
def is_palindrome str
  str.casecmp?(str.reverse)
end
```