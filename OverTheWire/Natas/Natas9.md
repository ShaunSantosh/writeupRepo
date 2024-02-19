# Natas9

## Logic
Upon viewing the source code, we come across a *PHP script* which is encoding a secret. *Reverse* the order of operations to get the secret and submit the secret to recieve the password.
Note: you can go about doing this however you wish. You can use a language of your choice like Python or PHP. You can use command line utilities or can also use tools like cyberchef.

## Commands
(using PHP)      
```php -a```     
```echo base64_decode(strrev(hex2bin('3d3d516343746d4d6d6c315669563362')));```

(using python)      
```import binascii```      
```import base64```

```print(base64.b64decode(binascii.unhexlify(my_str).decode('utf-8')[::-1]).decode('utf-8'))```

## Password
Sda6t0vkOPkM8YeOZkAGVhFoaplvlJFd 
