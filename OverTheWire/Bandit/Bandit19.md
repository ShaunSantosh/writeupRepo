# Bandit19

## Level goal
The password for the next level is stored in a file *readme* in the homedirectory. Unfortunately, someone has modified *.bashrc* to log you out when you log in with SSH.

## Logic
When a command is appended to the end of the ```ssh``` command, it will be executed on the remote host instead of the login shell. So we use this to get the password before we are inevitably logged out.

## Commands
```ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme```

## Password
awhqfNnAbc1naukrpqDYcF95h7HoMTrC
