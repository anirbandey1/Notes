# Gpu Passthrough 

Edit

/etc/default/grub
/etc/modprobe.d/vfio.conf


To build image
```
sudo mkinitcpi  linux linux-zen
```

Update grub
```
sudo grub-mkconfig -o /boot/grub/grub.cfg
```


Check 

```
# Get device ids
lspci -nn | grep NVIDIA

# For kernel modules
lspci -k 

```

