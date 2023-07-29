# Andoid sdk

#### Java version
Install older version of java
```
sudo pacman -S jre8-openjdk
```

Set that as default
```
sudo archlinux-java set java-8-openjdk/jre
```

## Install

Do not use AUR Android sdk 
Install Android Sdk using Android Studio


#### AUR android-sdk (Not Recommended)

To use sdk manager

Stuck at .android/repositories.cfg could not be loaded
```
mkdir -p ~/.android && touch ~/.android/repositories.cfg
```

Use sdkmanager
```
/opt/android-sdk/tools/bin/sdkmanager
```
