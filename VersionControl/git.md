# Git


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

Set upstream branch
```
$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master
```



