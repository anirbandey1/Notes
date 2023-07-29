# Docker


```
sudo pacman -S docker
```

for unsquashfs

```
sudo pacman -S squashfs-tools
```


Create docker image from iso

[medium article](https://medium.com/@SofianeHamlaoui/convert-iso-images-to-docker-images-4e1b1b637d75)


```
mkdir rootfs unquashfs

sudo mount -o loop ubuntu-22.04.2-desktop-amd64.iso rootfs

find . -type f | grep filesystem.squashfs

sudo unsquashfs -f -d unsquashfs/ rootfs/casper/filesystem.squashfs

sudo tar -C unsquashfs -c . | docker import - sofiane/myimg

docker run -h ubuntu -i -t sofiane/myimg bash
```


Docker for kali
```
docker rm

docker tag sofiane/myimg ubuntu/lts22

docker commit 22a8176584ee my-kali-img1

docker volume create vol1

docker run -it --name kal1 -v vol1:/data my-kali-img1

docker start -i kal1
```
