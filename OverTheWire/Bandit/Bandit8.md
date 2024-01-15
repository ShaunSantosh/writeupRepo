# Bandit8

## Level goal
The password for the next level is stored in the file *'data.txt'* next to the word *millionth*

## Logic
If we find the word *'millionth'*, we find the password. We are going to use the ```grep``` command for finding millionth. Here we using the (|) *Unix pipe*.  
**The Pipe connects the standard output from the first command and feeds it as standard input to the second command.**  
In our case, first ```cat``` command reads the file and then the data inside the file is sent to grep command to work on.

## Commands
```ls```
```cat data.txt | grep millionth```

## Password
TESKZC0XvTetK0S9xNwm25STk5iWrBvP
