# Bandit5

## Level goal
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Logic
You need to check the file type and this can be achieved using the ```file``` command

Note: Simply trying to ```cat``` all the files doesn't really help because you get it all together and so it might be difficult to determine where exactly the readable file begins

## Commands
Lets do an ```ls -la``` to find all files in the current directory. There is a directory inhere. Lets go to this directory.  
```ls -la```  
```cd inhere```

Now let us list all the files in this directory.  
```ls -la```

So there are different files in this directory, all starting with the name -file0 and then 1 to 9.   
```file ./-*```  

From the command, we now know that the file07 contains ASCII text. It is mostly readable text. So, let’s read it using ```cat``` command  
```cat ./-file07```

**OR**  

The more tedious method would be to ```cat``` these files we need to write the whole path because there is a symbol in the filename.  
```cat /home/bandit4/inhere/-file00```

After printing *all* the files (this is why it's tedious) we found the password. Because the output is not readable you can reset the terminal with the command ```reset``` or just by pressing ```ctrl+c```

## Password
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
