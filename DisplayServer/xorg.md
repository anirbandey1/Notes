# Xorg


If nvidia-xconfig messes up your /etc/X11/xorg.conf

First backup
```
sudo cp /etc/X11/xorg.conf /etc/X11/xorg.conf.bak
```

Regenerate using

```sh
# display :2 was used because there was no active display server there
sudo Xorg :2 -configure
sudo cp /root/xorg.conf.new /etc/X11/xorg.cong

```
