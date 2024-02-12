# Natas6

## Logic
Says we don’t have access to the webpage because we are *not logged in*. Open up Burp Suite, intercept the packet and go through the request body. Notice that the packet header stores *cookie information*. Let’s change *loggedin=0* to *loggedin=1* (with the assumption that 0 would mean '*false*' and 1 would mean '*true*'), and forward that packet.

## Password
fOIvE0MDtPTgRhqmmvvAOt2EfXR6uQgR
