# [Register for the Party (SQL for Beginners #3)](https://www.codewars.com/kata/590cc86f7557c0494000007e)

# Description
You received an invitation to an amazing party. Now you need to write an insert statement to add yourself to the table of participants.

participants table schema

* name (string)
* age (integer)
* attending (boolean)

NOTES:

* Since alcohol will be served, you can only attend if you are 21 or older
* You can't attend if the attending column returns anything but true

# My Solution
```sql
INSERT INTO participants (name, age, attending)
VALUES ("Participant", 33, 'TRUE');
SELECT * FROM participants;
```
