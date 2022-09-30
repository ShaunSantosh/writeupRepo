# Leviathan1

## Level
setuid binary in homedirectory. If you aren't familiar with setuid binaries I'd suggest looking them up but for the purpose of this level, in short setuid binaries allow any user to execute certain commands with privileges of the owner of the binary (usually an elevated user).

## Logic
```ls -la```       
```file check```        
On inspection of the file we can see that it is a setuid binary owned by *leviathan2*.           
We can try to run the setuid *check* and see how it reacts.            
```./check```         
It seems to ask for a password and doesn't seem like an obvious one. Let's `cat` it to try and figure out what inside.            
```cat check```       
It's a bunch of unreadable characters so let's try out `strings`.        
```strings check```       
None of the words in here seem to be the password we need. However, we notice a few *library function calls*. Let's try `ltrace`.           
```ltrace ./check```         
The function seems to take the first 3 characters of the user and compare it to 'sex' :3          
```./check```     
(input password "sex")       
Now once we use the password sex the program spawns an instance of a shell. `whoami` tells us that we're now leviathan2. Simply `cat` the password for leviathan2.       
(as leviathan2)       
```whoami```     
```cat /etc/leviathan_pass/leviathan2```    

## Password
mEh5PNl10e