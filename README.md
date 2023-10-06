# command-lines

## Encription

`gpg --armor --symmetric --cipher-algo CIPHER message.txt`

`gpg --output original_message.txt --decrypt message.gpg`

`openssl aes-256-cbc -pbkdf2 -iter 10000 -e -in message.txt -out encrypted_message`

`openssl aes-256-cbc -pbkdf2 -iter 10000 -d -in encrypted_message -out original_message.txt`


## Gobuster


## nmap


## Git

`git remote set-url origin git@github.com:sbahbouhi/command-lines.git`

`git init`

`git commit -m "xxxx"`

`git branch -M main`

`git remote add origin git@github.com:sbahbouhi/xxxx.git`

`git push -u origin main`


