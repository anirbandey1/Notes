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


## Submodule 

#### ref 
- [stackoverflow](https://stackoverflow.com/questions/1030169/pull-latest-changes-for-all-git-submodules#1032653)


If it's the first time you check-out a repo you need to use --init first:
```sh
git submodule update --init --recursive
```
For git 1.8.2 or above, the option --remote was added to support updating to latest tips of remote branches:
```sh
git submodule update --recursive --remote
```
This has the added benefit of respecting any "non default" branches specified in the .gitmodules or .git/config files (if you happen to have any, default is origin/master, in which case some of the other answers here would work as well).

For git 1.7.3 or above you can use (but the below gotchas around what update does still apply):
```sh
git submodule update --recursive
```
or:
```sh
git pull --recurse-submodules
```
if you want to pull your submodules to latest commits instead of the current commit the repo points to.
