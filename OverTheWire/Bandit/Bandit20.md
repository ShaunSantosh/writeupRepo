# Bandit20

## Level goal
To gain access to the next level, you should use the *setuid binary* in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

## Logic
A quick ```ls -la``` gives us our prime suspect *bandit20-do*. Also notice that the owner of the file is apparently bandit20 and not bandit19 as one would expect. Execute it and use it to get the password for bandit20.   
Note: I would suggest looking into setuid binaries to get a better idea even though the understanding isn't required for this level.

## Commands
```ls -la```   
```file bandit20-do ```   
```./bandit20-do```   
```./bandit20-do cat /etc/bandit_pass/bandit20```   

## Password
VxCazJaVykI6W36BkBU0mJTCM8rR95XT
