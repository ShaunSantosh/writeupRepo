# Bandit4

## Level goal
The password for the next level is stored in a hidden file in the *inhere* directory.

## Logic
The file is hidden and so a simple ls won't do, we need to use the -a option which shows all the files

## Commands
```cd inhere```

Now we should do another ‘ls -la’ to see all the files in this directory.(-l is optional)
```ls -la```

There is a file called ‘.hidden’, lets see the contents of this file.
```cat .hidden```

## Password
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
