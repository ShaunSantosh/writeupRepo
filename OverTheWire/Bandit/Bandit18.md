# Bandit18

## Level goal
There are 2 files in the homedirectory: *passwords.old* and *passwords.new*. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

## Logic
Use the ```diff``` command to get the lines that differ between the two files. From the output, pick the line from passwords.new (the output gives the lines in the same order the files were given to ```diff``` i.e. if passwords.new is the second argument then pick the second line)

## Commands
```diff passwords.old passwords.new```

## Password
hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
