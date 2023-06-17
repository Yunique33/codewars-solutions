# [Correct the mistakes of the character recognition software](https://www.codewars.com/kata/577bd026df78c19bca0002c0)

# Description
Character recognition software is widely used to digitise printed texts. Thus the texts can be edited, searched and 
stored on a computer.

When documents (especially pretty old ones written with a typewriter), are digitised character recognition softwares 
often make mistakes.

Your task is correct the errors in the digitised text. You only have to handle the following mistakes:

* <code>S</code> is misinterpreted as <code>5</code>
* <code>O</code> is misinterpreted as <code>0</code>
* <code>I</code> is misinterpreted as <code>1</code>

The test cases contain numbers only by mistake.

### Examples

>count_by(1,10) #should return [1,2,3,4,5,6,7,8,9,10]\
count_by(2,5) #should return [2,4,6,8,10]

# My Solution
```ruby
def correct(string)
  string.tr('501', 'SOI')
end
```
