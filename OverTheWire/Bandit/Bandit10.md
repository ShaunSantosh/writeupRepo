# Bandit10

## Level goal
The password for the next level is stored in the file *'data.txt'* in one of the few *human-readable strings*, preceded by several **‘=’** characters.

## Logic
If we use the ```cat``` command our screen would be filled with *garbage data*.
Use ```strings``` command which prints character sequences that are at least 4 characters long.
To get to the exact location of the password, we are going to use ```grep```.

**OR**

Another solution is to remove the garbage (mentioned example uses ```tr``` to delete the garbage, check out the man page if you don't get it) and then use ```grep```.  
Note: ```strings``` is definitely the better solution. The other attempts were just for the sake of it :>  

## Commands
```strings data.txt | grep '=='```

**OR**

```cat data.txt|tr -cd '[:graph:]'|grep ==``` / ```cat data.txt|tr -c '[:graph:]' '.'|grep ==```

## Password
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
