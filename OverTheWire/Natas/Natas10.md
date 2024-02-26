# Natas10

## Logic
From the way “key” is being used in the PHP script, it can probably take *arbitrary code* that is inserted as input. If we type in the word “password” then the passthru command in the PHP script will look like so: grep -i password dictionary.txt. Seeing the way that key is encapsulated in quotes, and there is *no input filtering*, we can assume that we are able to enter special characters.

We can use the ";" command separator, which will allow us to use 2 commands in one line. And we will also use the "#" comment command, which will comment out the rest of the text following the symbol.

So, in the input field we will type *; cat /etc/natas_webpass/natas10 #* which in turn will run the passthru command as below   
```grep -i ; cat /etc/natas_webpass/natas10 #```
effectively commenting out and removing dictionary.txt.

## Password
D44EcsFkLxPIkAAKLosx8z3hxX1Z4MCE
