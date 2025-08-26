# pixels

## Challenge description

### For some reason, it seems as though this folder of pixels are not what they seem. Can you find out what is going on?

For this challenge, we are given a zip file

However, unzipping the file reveals 


Through the **strings** commands, we get some idea that flag.txt is in the file somewhere.

![Alt text](images/strings.png)


Binwalk reveals that the flag in the form of gzip compressed data

![Alt text](images/binwalk.png)


We extract the flag using the command **binwalk -e** and it creates a folder **_stick.img.extracted**


Navigating into the folder created by binwalk and listing the directory, we get our flag

![Alt text](images/ls.png)


![Alt text](images/flag.png)

## Flag
```
scriptCTF{1_l0v3_m461c_7r1ck5}
```