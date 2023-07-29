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




If you want to list all the files currently being tracked under the branch master, you could use this command:
```
git ls-tree -r master --name-only
```
If you want a list of files that ever existed (i.e. including deleted files):
```
git log --pretty=format: --name-only --diff-filter=A | sort - | sed '/^$/d'
```

