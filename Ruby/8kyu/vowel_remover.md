# [Vowel remover](https://www.codewars.com/kata/5547929140907378f9000039)

# Description
Create a function called <code>shortcut</code> to remove the **lowercase** vowels 
(<code>a</code>, <code>e</code>, <code>i</code>, <code>o</code>, <code>u</code>) in a given string.

## Examples
>"hello"     -->  "hll"\
"codewars"  -->  "cdwrs"\
"goodbye"   -->  "gdby"\
"HELLO"     -->  "HELLO"

* don't worry about uppercase vowels
* <code>y</code> is not considered a vowel for this kata

# My Solution
```ruby
def shortcut(s)
  s.delete('aeiou')
end
```
# Better/Alternative solution from Codewars
```ruby
def shortcut(s)
  s.gsub(/[aeiou]/, '')
end
```
