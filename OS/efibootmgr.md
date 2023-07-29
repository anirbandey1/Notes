# efibootmgr

List entries
```
efibootmgr -v
```

Create entry 
```sh
# Not Verified
# efibootmgr -c  -d /dev/sda -p 1 -L LinuxMint -l /EFI/ubuntu/grubx64.efi


# Verified
# Recommended
sudo efibootmgr --create --disk=/dev/sda --part=4 --label="fedora_ssd" --loader='\EFI\fedora\shimx64.efi'
# 
# This also works
sudo efibootmgr --create --disk=/dev/sda --part=4 --label="fedora_ssd2" --loader='EFI\fedora\shimx64.efi'
# 
```

Both seem to work fine
'part' should specify the partition number of the EFI parition (FAT32) vfat filesystem

Delete entry
```
sudo efibootmgr --delete-bootnum --bootnum 0
```
 when passing the boot entry number we are not requested to include the padding 0s. If the bootnum is 000A just write A


Reference 
- [youtube](https://youtu.be/MN-Q5h2Iv8A)
- [linuxconfig.org](https://linuxconfig.org/how-to-manage-efi-boot-manager-entries-on-linux)
