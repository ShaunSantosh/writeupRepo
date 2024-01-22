# Bandit13

## Level goal
The password for the next level is stored in the file *data.txt*, which is a hexdump of a file that has been *repeatedly compressed*. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Logic
Basically decompress and check the file over and over again (I'm not a big fan of this level) until we get the right format. If required use ```mv``` to rename the file with the appropriate extension

## Commands
```ls```
```cat data.txt```
```mkdir /tmp/bumbum```
```cp data.txt /tmp/bumbum```
```cd /tmp/bumbum```
```ls```
```file data.txt```
```xxd -r data.txt data1```
```file data1```
```mv data1 data2.gz```
```gzip -d data2.gz```
```file data2```
```mv data2 data3.bz2```
```bzip2 -d data3.bz2```
```file data3```
```mv data3 data4.gz```
```gzip -d data4.gz```
```file data4```
```tar -xvf data4```
```file data5.bin```
```tar -xvf data5.bin```
```file data6.bin```
```mv data6.bin data7.bz2```
```bzip2 -d data7.bz2```
```file data7```
```tar -xvf data7```
```file data8.bin```
```mv data8.bin data9.gz```
```gzip -d data9.gz```
```file data9```
```cat data9```

## Password
wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
