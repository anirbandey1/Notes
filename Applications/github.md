```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Just add Github fingerprint to known hosts this way:
```
mkdir -p ~/.ssh
ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts

```
