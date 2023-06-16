# [Find the first non-consecutive number](https://www.codewars.com/kata/58f8a3a27a5c28d92e000144)

# Description
Your task is to find the first element of an array that is not consecutive.

By not consecutive we mean not exactly 1 larger than the previous element of the array.

E.g. If we have an array <code>[1,2,3,4,6,7,8]</code> then <code>1</code> then <code>2</code> then <code>3</code> then 
<code>4</code> are all consecutive but <code>6</code> is not, so that's the first non-consecutive number.

If the whole array is consecutive then return <code>null</code><sup>2</sup>.

The array will always have at least <code>2</code> elements<sup>1</sup> and all elements will be numbers. The numbers 
will also all be unique and in ascending order. The numbers could be positive or negative and the first non-consecutive 
could be either too!

If you like this Kata, maybe try this one next: https://www.codewars.com/kata/represent-array-of-numbers-as-ranges

<sup>1</sup> Can you write a solution that will return <code>null</code><sup>2</sup> for both <code>[]</code> and 
<code>[ x ]</code   > though? (This is an empty array and one with a single number and is not tested for, but you can 
write your own example test.)

<sup>2</sup>
Swift, Ruby and Crystal: <code>nil</code>\
Haskell: <code>Nothing</code>\
Python, Rust, Scala: <code>None</code>\
Julia: <code>nothing</code>\
Nim: <code>none(int)</code> (See [options](https://nim-lang.org/docs/options.html))

# My Solution
```ruby
def first_non_consecutive(arr)
  el = (arr.first..arr.last).to_a - arr
  arr[arr.index(el.first+1)] unless el.empty?
end
```
# Better/Alternative solution from Codewars
```ruby
def first_non_consecutive(arr)
  arr.each_index do |i|
    return arr[i + 1] if arr[i].next != arr[i + 1]
  end
end
```
