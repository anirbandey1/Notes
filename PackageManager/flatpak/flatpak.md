# Flatpak on arch linux

Install flatpak
```
sudo pacman -S flatpak
```

The installation of flatpak will, by default, add the official Flathub repository as a system-wide installation. To add the official repo with a per-user configuration:

Add flathub remote repo link for per-user installation (Recommended)
```
flatpak remote-add --if-not-exists --user flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

Add flathub remote repo link for system-wide installation (Not Recommended)
Dangerous
It will ask for password everytime you try to install something
```
# system-wide installation
# flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

To delete a remote flatpak repository do:

```
flatpak remote-delete name
```

where name is the name of the remote repository to be deleted.
List repositories

To list all the added repositories do:
```
flatpak remotes
```

Search
```
flatpak search <whatever you want to search>
```

Install gnome-extensions-manager
```
flatpak install flathub com.mattjakeman.ExtensionManager
```

Flatpak packages are stored in
```
/var/lib/flatpak/repo
```
