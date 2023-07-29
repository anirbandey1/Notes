# Flatpak on arch linux

install flatpak
```
sudo pacman -S flatpak
```

add flathub remote repo link
```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

search
```
flatpak search <whatever you want to search>
```

install gnome-extensions-manager
```
flatpak install flathub com.mattjakeman.ExtensionManager
```

Flatpak packages are stored in
```
/var/lib/flatpak/repo
```
