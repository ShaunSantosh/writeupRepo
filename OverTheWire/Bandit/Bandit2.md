# Bandit2

## Level goal
The password for the next level is stored in a file named - located in the home directory

## Logic
Characters like "-","#", "!" etc. are treated like *special characters* so we've to *delimit* them   
We've got a few options
* Mention the whole filepath 
* Redirect into an i/o stream explicitly (seems to expect only a file as an input, so works)

## Commands
* ```cat /home/bandit2/-```  **OR** ```cat ./-```
* ```cat < -```

## Password
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
