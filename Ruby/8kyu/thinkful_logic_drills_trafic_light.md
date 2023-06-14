# [Thinkful - Logic Drills: Traffic light](https://www.codewars.com/kata/58649884a1659ed6cb000072)

# Description
You're writing code to control your town's traffic lights. You need a function to handle each change from 
<code>green</code>, to <code>yellow</code>, to <code>red</code>, and then to <code>green</code> again.

Complete the function that takes a string as an argument representing the current state of the light and returns a 
string representing the state the light should change to.

For example, when the input is <code>green</code>, output should be <code>yellow</code>.

# My Solution

```ruby
def update_light(current)
  {'green' => 'yellow',
   'yellow' => 'red',
   'red' => 'green'}[current]
end
```
