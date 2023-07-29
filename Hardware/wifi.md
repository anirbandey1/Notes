# Wifi Adapter 

## Dependencies

Debian

```sh

sudo apt install dkms git
sudo apt install build-essential libelf-dev 
sudo apt install linux-headers-$(uname -r)

```


## Install 

### TP Link T2U Archer A600 RTL8812au

[Youtube Link](https://youtu.be/JAoj5tOFJZc)

Github repo [https://github.com/aircrack-ng/rtl8812au.git](https://github.com/aircrack-ng/rtl8812au.git)


```sh

git clone https://github.com/aircrack-ng/rtl8812au.git

cd rtl8812au

# Install the Driver
sudo make dkms_install

# Check the wireless interface Is Connected
lsusb


```



### TP Link T2U Archer A1300 RTL8812au

Github repo [https://github.com/morrownr/88x2bu](https://github.com/morrownr/88x2bu)

```sh

git clone https://github.com/morrownr/88x2bu-20210702.git
cd 88x2bu-20210702
sudo ./install-driver.sh

```


