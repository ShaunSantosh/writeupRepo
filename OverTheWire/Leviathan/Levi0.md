# Leviathan0

### Level
Find the file *bookmarks.html* in the hidden directory *.backup* and search for a password in the file.     
p.s: I somehow missed *.backup* the first few times I had a crack at this :/

### Logic
SSH into the system, then look around and keep an eye out for any *hidden* files/directories.       
Once you find *.backup* `cd` in and `ls` again to find *bookmarks.html*. `cat` to find that it's got a bunch of info inside, so `grep` for a *keyword*(in this case leviathan). 

### Commands
```ssh leviathan0@levithan.labs.overthewire.org -p 2223```
(password is leviathan0)
```ls -la```
```cd .backup/```
```ls -la```
```cat bookmarks.html | grep leviathan```

### Password
rioGegei8m