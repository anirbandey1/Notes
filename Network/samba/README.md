# Samba 

Daemon - **smbd.service**

Create backup
```
sudo cp /etc/samba/smb.conf /etc/samba/smb.conf.bak
```

Main commands
```
sudo mkdir -p /share/public_files
sudo mkdir -p /share/private_files
sudo groupadd --system smbgroup 
cat /etc/group | grep smbgroup
sudo useradd --system --no-create-home --group smbgroup -s /bin/false smbuser
cat /etc/passwd | grep smbuser
sudo chown -R smbuser:smbgroup /share
ls -l / 
sudo chmod -R g+w /share
ls -l /
sudo systemctl status smbd.service
sudo systemctl start smbd.service
sudo systemctl status smbd.service
```

For permissions 
```
sudo nvim /etc/apparmor.d/local/usr.sbin.smbd
```

Add to /etc/apparmor.d/local/usr.sbin.smbd
```
"/share/" rk,
"/share/**" lrwk,
```



Install 
- gvfs-smb
- dolphin

In dolphin, just type smb://pop-os


Reference
- [ArchWiki apparmor](https://wiki.archlinux.org/title/samba#Permission_issues_on_AppArmor)
- [Manjaro forum](https://forum.manjaro.org/t/cant-connect-to-samba-after-update-service-is-running-2022-08-13/119396/29?page=2)
- [LearnLinuxTV youtube video](https://www.youtube.com/watch?v=7Q0mnAT1MRg&pp=ygUUbGVhcm4gbGludXggdHYgc2FtYmE%3D)
