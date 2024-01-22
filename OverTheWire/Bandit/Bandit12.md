# Bandit12

## Level goal
The password for the next level is stored in the file *data.txt*, where all lowercase (a-z) and uppercase (A-Z) letters have been *rotated by 13 positions*

## Logic
To convert the text, we can use the ```tr``` command. This command translates characters depending on the parameters provided. We used n-z and a-m because tr won’t continue to translate after the Z (It requires 26 characters for both the sets, original and the set to be rotated to).
Fun fact: this is what is called ROT13, a simple substitution cipher that is a variant of the Caesar cipher.

## Commands
```cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'```

## Password
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
