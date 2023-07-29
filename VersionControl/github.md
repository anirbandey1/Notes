# Github CLI (gh)

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Just add Github fingerprint to known hosts this way:
```
mkdir -p ~/.ssh
ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts

```


Change visibility to private, public, internal
```
gh repo edit --visibility <visibility-string>
```
Where visibility-string = private,public or internal

