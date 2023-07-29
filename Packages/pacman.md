# Pacman 

[link](https://itsfoss.com/pacman-command/)

To list installed packages which are not present in the official repository
AUR packages or other third party repositories
```
pacman -Qm 
```

To see where packaes are installed
```
pacman -Ql
```


### Cache - Space problem

[link](https://discovery.endeavouros.com/articles/root-partition-full-dont-panic-clear-pacmans-cache-first/2020/03/)

When you install a package with Pacman, it stores all downloaded packages in
```
/var/cache/pacman/pkg/ 
```
folder. The package manager doesn’t remove old and uninstalled packages 
automatically by default and after a while, the cache size can consume a 
substantial amount of real estate on your HDD or SDD.

