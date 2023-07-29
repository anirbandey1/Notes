# Touchpad

It works on Arch Linux KDE Xorg
with two extra packages **xf86-input-libinput** and **xf86-input-synaptics**

In my case, xf86-input-libinput was already installed

My touchpad's tap to click action was not working, but the pointer on screen was moving

I just had to install **xf86-input-synaptics** from standard Arch Repository and it started working

```
pacman -sS xf86-input-libinput
sudo pacman -S xf86-input-libinput
```

```
pacman -sS xf86-input-synaptics
sudo pacman -S xf86-input-synaptics
```

You can tweak touch pad options in KDE using **System Settings** 




