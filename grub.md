Change grub configuration
```
sudo vim /etc/default/grub
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

```
GRUB_SAVEDEFAULT=true
GRUB_DEFAULT=saved
```

```
sudo update-grub
```
