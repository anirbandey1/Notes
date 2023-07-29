# Proxychains

Install 
```
sudo pacman -Syu proxychains-ng
```

To verify connection to tor

```
proxychains curl ifconfig.me

proxychains curl https://api.ipify.org

proxychains curl https://check.torproject.org
```


Config file  **/etc/proxychains.conf**

Use dynamic_chain not strict_chain
