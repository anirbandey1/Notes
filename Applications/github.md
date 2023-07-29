```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Just add Github fingerprint to known hosts this way:
```
mkdir -p ~/.ssh
ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts

```

To make changes in .gitignore take effect
```
git rm -rf --cached .
```
and then add and commit changes


To set nvim as the editor to write commit messages for git
```
git config --global core.editor nvim
```
