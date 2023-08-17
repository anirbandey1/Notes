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

To see user.name and user.email
```
git config --global user.name
git config --global user.email
```

To set user.name and user.email
```
git config --global user.name "yourUserName"
git config --global user.email "you@example.com"
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


## Rebase 

[StacKOverflow](https://stackoverflow.com/questions/750172/how-do-i-change-the-author-and-committer-name-email-for-multiple-commits#1320317)
Rebase entire project

```sh
git rebase -r --root --exec "git commit --amend --no-edit --reset-author"
```

## Tags

List tags
```
git tag
```

Details of Specific tag
```
git show v1.0.0
```

Create 
```
git tag v1.0.1
```

Delete tag
```
git tag -d v1.0.1
```

Pushing to remote
```
git push origin v1.0.2
```

Delete remote tag
```
git push origin -d v1.0.2
```



