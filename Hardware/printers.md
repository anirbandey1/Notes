# Printers

For specific drivers
[ArchWiki CUPS/Printer-specific_problems](https://wiki.archlinux.org/title/CUPS/Printer-specific_problems)


#### CUPS
```
sudo pacman -S cups
sudo systemctl enable cups
sudo systemctl start cups
```

#### lp group
```
sudo usermod -a $USER -G lp
# newgrp lp
```

Cups web interface opens at  **[https://localhost:631](https://localhost:631)**
Login as root and provide root password

#### GUI for CUPS
```
sudo pacman -S system-config-printer
```
Can be launched with
```
system-config-printer
```

#### For our canon printer - Canon G3010 series

```
sudo pacman -S gutenprint foomatic-db-ppds
/usr/bin/cups-genppdupdate
sudo systemctl restart cups
sudo systemctl status cups

```

#### Ghostscript
Ghostscript is needed by the printer to parse info
```
sudo pacman -S ghostsript
```

(Not sure if its needed)
For avahi
```
sudo pacman -S avahi
```

Common dependencies
```
sudo pacman -S dbus
sudo pacman -S python-dbus pygtk
sudo pacman -S python-dbus
```

avahi-daemon
```
sudo avahi-daemon
```

avahi-discover
```
avahi-discover
```

#### Reference

- [Distrotube video](https://www.youtube.com/watch?v=jnmCbEWNV1w&pp=ygUScHJpbnRlciBhcmNoIGxpbnV4)
- [Lakur.tech article](https://lakur.tech/2021/09/16/adding-a-hp-printer-on-arch-linux/)

Notes 

Management of cups is done over the cups web interface, listening on port 631. Go to https://localhost:631, click on Administration located in the top menu bar, and select “Add Printer” in the Printers section. This will ask you for your credentials, which is your local root account. Enter root as user and your root password as password and proceed.

In the following list, you’ll see some printers that could be added now. Select the desired printer and continue.

# Command history

```
sudo pacman -S cups
sudo systemctl start cups
sudo systemctl enable cups
sudo systemctl service cups
sudo systemctl status cups
cupsenable
cups-browsed
sudo pacman -S avahi
avahi-discover
sudo pacman -S dbus
avahi-discover
sudo pacman -S python-dbus pygtk
sudo pacman -S python-dbus
avahi-discover
flatpak search printer
sudo systemctl start avahi
usbutils
pacman -sS usbutils
sudo pacman -S usbutils
usb-devices
avahi-daemon
sudo avahi-daemon
avahi-discover
sudo avahi-daemon
ip a
cups
sudo pacman -S sway
sudo pacman -S wayland
sway
lsmod | grep drm
sway
sudo modprobe drm
sway
pacman -Qi wayalnd
pacman -Qi wayland
sudo pacman -S  sway alacritty waybar wofi xorg-xwayland xorg-xlsclients qt5-wayland glfw-wayland
sway
xlsclients
cd ~/.config\nmkdir sway\ncd sway\ncp /etc/sway/config .
ls
nvim config
sway
nvim config
sway
sudo pacmna -S wayland
sudo pacan -S wayland
sudo pacman -S wayland
sudo pacman -S xorg
sudo pacman -S xorg-xwayland
nvim ~/.config/sway/config
sway
nvim ~/.config/sway/config
echo $XDG_SESSION_TYPE
l
WOFI
wofi
man wofi
wofi -show drun
wofi
man wofi
wofi --show
wofi --show=drun
wofi --show drun
wofi -G -show drun
wofi -G -show=drun
wofi -show=drun -theme
wofi --show=drun
wofi -G --show=drun
setxkbmap
nvim .bash_keymaps
nvim ~/.config/sway/config
dmenu_path
nvim ~/.config/sway/config
dmenu_run
rofi
setxkbmap -option
wofi -G --show drun
nvim ~/.config/sway/config
xev
alsamixer
nvim ~/.config/sway/config
df -h
sudo pacman -S waydroid
yay -sS waydroid
yay -S waydroid
sudo pacman -Syu
nvim ~/.config/sway/config
pacman -sS hyperland
pacman -sS hyper
pacman -Qi wl-root
pacman -Qi wlroot
wofi
wofi --show drun
h
h | grep wl
wlroots
pacman -sS hyprland
wlroots
cat /usr/share/X11/xkb/keycodes/README
cd ~/.config/qtile
gs
gd
sudo systemctl status cups
sudo usermod -a alice -G lp
cat /etc/group
cat /etc/group | grep lp
sudo usermod -a alice -G lp
groups
newgrp lp
groups
pacman -sS system-config-printers
pacman -sS system-config-printer
sudo pacman -S system-config-printer
system-config-printer
groups
sudo pacman -S gutenprint foomatic-db-ppds
/usr/bin/cups-genppdupdate
sudo systemctl restart cups
sudo systemctl status cups
cd Downloads
l
tar -xcf cnijfilter2-source-5.30-1.tar.gz
tar --help
man tar
tar -xf cnijfilter2-source-5.30-1.tar.gz
ls
cd cnijfilter2-source-5.30-1
l
nvim README
ls
nvim scripts
pacman -sS ghost
gs
ghostscript
gs
sudo pacman -S ghostscript
h
sudo usermod -a $USER -G lp
sudo echo "$USER"
sudo usermod -a "$USER" -G lp
groups
h
nvim ~/Code/Notes/Hardware/touchpad.md
nvim ~/Code/Notes/Hardware/printers.md
h
sudo systemctl start avahi
avahi-daemon
nvim ~/Code/Notes/Hardware/printers.md
c
```



