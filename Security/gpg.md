List keys:
----------
gpg --list-secret-keys
gpg --list-keys

Generate keys:
-------------
gpg --full-generate-key
OR
gpg --gen-key

Export/Import keys:
-------------------
gpg --export -a Melvin > melvin_public.key
gpg --import melvin_public.key
gpg --export-secret-keys Melvin > melvin-private-key.key
gpg --import melvin-private-key.key

Encrypt & Decrypt
-----------------
gpg -e -r "Melvin" users.csv
gpg --always-trust -e -r "Melvin" users.csv

gpg -d users.csv.gpg
gpg --batch --passphrase demo users.csv.gpg
