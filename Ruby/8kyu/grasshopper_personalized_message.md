# [Grasshopper - Personalized Message](https://www.codewars.com/kata/5772da22b89313a4d50012f7)

# Description
Create a function that gives a personalized greeting. This function takes two parameters: <code>name</code> and 
<code>owner</code>.

Use conditionals to return the proper message:


| case               | 	return   |
|--------------------|--------------|
| name equals owner | 'Hello boss'  |
| otherwise	   | 	'Hello guest' |

# My Solution
```ruby
def greet(name,owner)
  name == owner ? 'Hello boss' : 'Hello guest'
end
```
