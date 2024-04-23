# [Is there a vowel in there?](https://www.codewars.com/kata/57cff961eca260b71900008f)

## Description
Given an array of numbers, check if any of the numbers are the character codes for lower case vowels (`a, e, i, o, u`).

If they are, change the array value to a string of that vowel.

Return the resulting array.

## My Solution
```ruby
def is_vow(a)
  vowels = %w(a e i o u)
  codes = {}
  vowels.each {|vowel| codes[vowel.ord] = vowel }
  a.map {|el| codes[el] || el}
end
```

## Better/Alternative solution from Codewars
```ruby
def is_vow(a)
  a.map { |l| l.chr =~ /[aeoui]/ ? l.chr : l }
end
```
