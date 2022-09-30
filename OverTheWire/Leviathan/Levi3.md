# Leviathan3

## Level
Analyzing a setuid binary

## Logic
This level was quite similar to Levi1.md   
```ls -la```     
We find *level3*    
```file ./level3```     
We can see that it is a setuid binary owned by *leviathan4*.           
Let's try running the executable   
```./level3```    
This one also expects a password, so we try what worked previously   
```ltrace ./level3```   
Notice that the string we input is compared against *snlprintf*, so let's give that a try   
```./level3```   
(input password "snlprintf")
You will be rewarded with a shell!   
(as leviathan4)       
```whoami```     
```cat /etc/leviathan_pass/leviathan4```    

## Password
AgvropI4OA