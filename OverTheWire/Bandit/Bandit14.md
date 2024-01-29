# Bandit14

## Level goal
The password for the next level is stored in */etc/bandit_pass/bandit14* and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

## Logic
Use the SSH key to login as bandit14 and read the password.

## Commands
```ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220```

(as bandit14)  
```cat /etc/bandit_pass/bandit14```

## Password
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq
