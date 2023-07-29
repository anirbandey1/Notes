# ssh 


```
ssh-keygen  -t rsa -b 4096 -C "comment" -N "" -f ~/.ssh/raspberrypi_rsa
ssh-copy-id -i ~/.ssh/raspberrypi_rsa.pub pi@raspberrypi
```


Then make changes to ~/.ssh/config file
