# [Welcome to the City](https://www.codewars.com/kata/5302d846be2a9189af0001e4)

# Description
Create a method that takes as input a name, city, and state to welcome a person. Note that `name` will be an array 
consisting of one or more values that should be joined together with one space between each, and the length of the 
`name` array in test cases will vary.

Example:

```
['John', 'Smith'], 'Phoenix', 'Arizona'
```

This example will return the string `Hello, John Smith! Welcome to Phoenix, Arizona!`

# My Solution
```ruby
def say_hello(name, city, state)
  "Hello, #{name.join(' ')}! Welcome to #{city}, #{state}!"
end
```
