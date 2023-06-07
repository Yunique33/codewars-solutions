# [Counting sheep...](https://www.codewars.com/kata/54edbc7200b811e956000556)

# Description
Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).

For example,

>[true,  true,  true,  false,\
true,  true,  true,  true ,\
true,  false, true,  false,\
true,  false, false, true ,\
true,  true,  true,  true ,\
false, false, true,  true]

The correct answer would be <code>17</code>.

Hint: Don't forget to check for bad values like <code>null</code>/<code>undefined</code>

# My Solution
```ruby
def countSheeps(array)
  array.count(true)
end
```
