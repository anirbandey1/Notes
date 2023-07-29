# gnome settings

get
```
gsettings get org.gnome.desktop.interface gtk-theme
```

set 
```
gsettings set org.gnome.desktop.interface gtk-theme Adwaita-dark
```

to check if you are running wayland or xorg
```
echo $XDG_SESSION_TYPE
```

A ridiculous but fun way to know if you are using Wayland on GNOME

Press Alt + F2, type 'r' and press enter
Normally, it restarts the Normally it restarts the GNOME shell.
But it won’t work in Wayland. It will display ‘restart is not available on Wayland’
