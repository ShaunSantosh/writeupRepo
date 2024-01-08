# Bandit7

## Level goal
The password for the next level is stored *somewhere on the server* and has all of the following properties:
* owned by user bandit7
* owned by group bandit6
* 33 bytes in size

## Logic
After doing an ```ls``` you'll notice that there are no files in the home dir, so shift to root (/).
Do a ```find``` for a file with the given properties.
There will be a big list of files that match this file, with alot of error messages saying permission denied. If we add a redirect from errors to *dev/null* we should get a cleaner output.

## Commands
```find / -user bandit7 -group bandit6 -size 33c 2>/dev/null```  
```cat /var/lib/dpkg/info/bandit7.password```

## Password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
