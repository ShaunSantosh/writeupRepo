# Bandit3

## Level goal
The password for the next level is stored in a file called *spaces in this filename* located in the home directory

## Logic
When we give *spaces in this filename* as the input as it is, cat takes it as multiple inputs i.e. *spaces*, *in*, *this* and *filename*
We can solve this in a few ways:
* Using single (') or double (") qoutes
* Using ``\<space>`` which is the escape character in most linux systems

## Commands
* ```cat "spaces in this filename"```
* ```cat spaces\ in\ this\ filename```

## Password
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
