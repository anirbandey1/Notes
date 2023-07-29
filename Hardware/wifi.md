# Wifi Adapter 


TP Link T2U Archer A600

[Youtube Link](https://youtu.be/JAoj5tOFJZc)



On Debian based distros

```sh

# Install dependencies
sudo apt install dkms git
sudo apt install build-essential libelf-dev 
sudo apt install linux-headers-$(uname -r)


git clone https://github.com/aircrack-ng/rtl8812au.git

cd rtl8812au

# Install the Driver
sudo make dkms_install

# Check the wireless interface Is Connected
lsusb


```
