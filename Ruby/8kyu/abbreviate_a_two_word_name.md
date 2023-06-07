# [Abbreviate a Two Word Name](https://www.codewars.com/kata/57eadb7ecd143f4c9c0000a3)

# Description
Write a function to convert a name into initials. This kata strictly takes two words with one space in between them.

The output should be two capital letters with a dot separating them.

It should look like this:

<code>Sam Harris</code> => <code>S.H</code>

<code>patrick feeney</code> => <code>P.F</code>
# My Solution
```ruby
def abbrev_name(name)
  name.split(' ').map{|el| el[0].upcase}.join('.')
end
```
# Better/Alternative solution from Codewars
```ruby
def abbrev_name(name)
  name.split.map { |s| s[0]}.join('.').upcase
end
```

