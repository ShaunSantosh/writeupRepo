# Bandit15

## Level goal
The password for the next level can be retrieved by submitting the password of the current level to *port 30000* on localhost.

## Logic
After logging in as bandit14 using the ssh key, send the password we got to localhost using *netcat* or *telnet*.

## Commands
```nc localhost 30000```  
**OR**  
```telnet localhost 30000```

\<Enter the password>

## Password
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
