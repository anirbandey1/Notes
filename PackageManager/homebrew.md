# Home Brew 

### On Linux


#### On Debian

Dependencies
```sh
sudo apt-get install build-essential procps curl file git
```

Install script
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Add the following to .bashrc or .zshrc
```sh
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```
