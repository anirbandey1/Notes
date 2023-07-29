user must be added to the audio group
```
sudo usermod -aG audio NameOfUser
```
check
```
cat /proc/asound/cards
ls -l /dev/snd/
sudo dmesg | grep -E 'snd|sof'
```

firmware and alsa
```
sudo pacman -S sof-firmware
sudo pacman alsa-ucm-conf
sudo pacman -S alsa-firmware
sudo pacman -S alsa-utils
sudo pacman -S pulseaudio
```


unmute
```
amixer sset Master unmute
amixer sset Speaker unmute
amixer sset Headphone unmute
```

optional
```
amixer -D pulse sset Master 100%
```

using alsamixer
```
alsamixer
```


history
```
  386  cat /proc/asound/cards
  387  ls -l /dev/snd/
  388  sudo dmesg ] grep -E 'snd|sof'
  389  sudo pacman -S sof-firmware
  390  sudo dmesg | grep -E 'snd|sof'
  391  sudo dmesg ] grep -E 'snd|sof'
  392  sudo dmesg | grep -E 'snd|sof'
  393  sudo pacman alsa-ucm-conf
  394  sudo pacman -S alsa-ucm-conf
  395  sudo dmesg | grep -E 'snd|sof'
  396  sudo pacman -S alsa-ucm-conf
  397  sudo dmesg | grep -E 'snd|sof'
  398  amixer sset Master unmute
  399   amixer sset Speaker unmute
  400   amixer sset Headphone unmute
  401  alsamixer
  402  speaker-test -c 2
  403  sudo pacman -S alsa-firmware
  404  sudo dmesg | grep -E 'snd|sof'
  405  alsamixer
  406  amixer sset Master unmute
  407  sudo pacman -S alsa-utils
  408  sudo dmesg | grep -E 'snd|sof'
  409  sudo pacman -S sof-bin
  410  amixer sset Master unmute
  411  reboot
  412  alsamixer
  413  alsamixer
  414  sudo pacman -S alsa-utils
  415  amixer sset Master unmute
  416  alsamixer
  417  clear
  418  amixer sset Master unmute
  419   amixer sset Speaker unmute
  420   amixer sset Headphone unmute
  421  amixer -D pulse sset Master 100%
  422   amixer sset Speaker unmute
  423  sudo pacman -S alsa-utils
  424   amixer sset Speaker unmute
  425   amixer sset Headphone unmute
  426  sudo pacman -S sof-bin
  427  sudo dmesg | grep -E 'snd|sof'
  428  sudo pacman alsa-ucm-conf
  429  sudo pacman -S alsa-firmware
  430  sudo pacman -S sof-firmware
  431  sudo dmesg | grep -E 'snd|sof'
  432  reboot
  433  sudo pacman -S pulseaudio
  434  sudo dmesg | grep -E 'snd|sof'
  435  alsamixer
  436  alsamixer
  437  alsamixer
  438  cat /etc/group
  439  cat /etc/group | grep audio
  440  usermod -aG audio darklord
  441  sudo usermod -aG audio darklord
  442  groups
  443  reboot
  444  ls
  445  cd Code/
  446  cd Notes/
  447  ls
  448  cd ..
  449  ls
  450  cd DSA/
  451  ls
  452  ls -a
  453  cp .gdbinit .vimrc ~
  454  ls
  455  cd ..
  456  cd ..
  457  l
  458  ls
  459  ls -a
  460  git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
  461  vim +PluginInstall +qall
  462  pacman -S astyle
  463  sudo pacman -S astyle
  464  vim
  465  clear
  466  ls
  467  cd Code/
  468  ls
  469  cd n
  470  cd Notes/
  471  ls
  472  cat github.md 
  473  mkdir Arch
  474  cd Arch/
  475  ld
  476  ls
  477  vim sound.md
  478  vim sound.md
  479  ls
  480  cat sound.md 
  481  history >> sound.md 
```
