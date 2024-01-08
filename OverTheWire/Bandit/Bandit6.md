# Bandit6

## Level goal
The password for the next level is stored in a file somewhere under the *'inhere'* directory and has all of the following properties:
* human-readable
* 1033 bytes in size
* not executable

## Logic
We look into *'inhere'* and find a bunch of folders....but we're also given multiple properties of the file which contains the password. Now we just need to find a file that has these properties

## Commands
```ls```  
```cd inhere/```  
```ls```  
```find . -size 1033c```  
```cat ./maybehere07/.file2```  

## Password
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
