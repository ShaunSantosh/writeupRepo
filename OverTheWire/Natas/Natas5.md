# Natas5

## Logic
The website says that access to the website is not allowed, and that *authorized users* should only be coming from http://natas5.natas.labs.overthewire.org/. So our task is to make it seem like the request has come from http://natas5.natas.labs.overthewire.org/.

What this challenge requires us to work with is called the “*HTTP Referer*”. One way to go about spoofing this is using a proxy which will allow us to edit our request before it is sent. I have used Burp Suite's proxy intercept for this task but this can be done using similar proxy tools.   
Once Burp is running, reload the website and go back to Burp. To see the *intercepted packet* in Burp, go to Proxy > Intercept.
The packet’s Referer is set to: “http://natas4.natas.labs.overthewire.org/index.php” so change that to “http://natas5.natas.labs.overthewire.org/”. Once done, click *Forward*, and we get the password.

Note: I would suggest familiarizing yourself with a proxy of your choice and maybe look into HTTP Referer and other such HTTP header fields.

## Password
Z0NsrtIkJoKALBCLi5eqFfcRN82Au2oD 
