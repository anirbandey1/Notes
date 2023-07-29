# GRUB

Change grub configuration
```
sudo vim /etc/default/grub
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

```
GRUB_SAVEDEFAULT=true
GRUB_DEFAULT=saved
```

To detect other bootable partitions
```
GRUB_DISABLE_OS_PROBER=false
```

On Ubuntu
```
sudo update-grub
```
