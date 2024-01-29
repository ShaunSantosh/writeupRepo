# Bandit16

## Level goal
The password for the next level can be retrieved by submitting the password of the current level to *port 30001* on localhost using *SSL encryption*.

Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…

## Logic
Use the *s_client* sub-command of *openssl* since (as far as my limited knowledge and numerous search engines results go) there isn't a straightforward way to get *netcat* or *telnet* to use *SSL encryption*. Note: use the *-quiet* option to make the output less verbose.

## Commands
```openssl s_client -connect localhost:30001 -quiet```   
\<Enter the password>

## Password
JQttfApK4SeyHwDlI9SXGR50qclOAil1
