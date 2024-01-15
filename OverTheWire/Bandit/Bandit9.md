# Bandit9

## Level goal
The password for the next level is stored in the file *data.txt* and is the *only line of text that occurs only once*

## Logic
It is hinted that the password is the only line of text that occurs only once.  
Use ```sort``` command to sort the text inside the *data.txt* file.  
The file contains a lot of *repeating statements* so use the ```uniq``` command to print the non-repeating statement.
Use multiple pipes here to get a filtered result.
Note: We sort the text before piping because ```uniq``` works on adjacent matching lines and so requires a sorted input to give the result we want.

## Commands
```cat data.txt | sort | uniq -u```

## Password
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
