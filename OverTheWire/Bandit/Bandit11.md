# Bandit11

## Level goal
The password for the next level is stored in the file *data.txt*, which contains *base64 encoded data*

## Logic
Basically just decode. Two ways to go about it:
* ```cat``` the file and pipe the data into ```base64``` to decode

**OR**

* Directly give the file as input to ```base64``` and decode

## Commands
* ```cat data.txt | base64 --decode```

**OR**

* ```base64 -d data.txt```

## Password
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
