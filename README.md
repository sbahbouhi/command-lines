# command-lines

## Encription

### GPG

`gpg --armor --symmetric --cipher-algo CIPHER message.txt`

`gpg --output original_message.txt --decrypt message.gpg`

### OpenSSL

`openssl aes-256-cbc -e -in message.txt -out encrypted_message`

`openssl aes-256-cbc -d -in encrypted_message -out original_message.txt`

`openssl aes-256-cbc -pbkdf2 -iter 10000 -e -in message.txt -out encrypted_message`

`openssl aes-256-cbc -pbkdf2 -iter 10000 -d -in encrypted_message -out original_message.txt`

### RSA 

`openssl genrsa -out private-key.pem 2048`

`openssl rsa -in private-key.pem -pubout -out public-key.pem`

`openssl rsa -in private-key.pem -text -noout`

`openssl pkeyutl -encrypt -in plaintext.txt -out ciphertext -inkey public-key.pem -pubin`

`openssl pkeyutl -decrypt -in ciphertext -inkey private-key.pem -out decrypted.txt`

### Deffie Hellman

`openssl dhparam -out dhparams.pem 2048`

`openssl dhparam -in dhparams.pem -text -noout`

### Certificate signing

`openssl req -new -nodes -newkey rsa:4096 -keyout key.pem -out cert.csr`

## Gobuster

gobuster dir -w /usr/share/wordlists/rockyou.txt -u "http://localhost:8000/"

## nmap


## Git

`git remote set-url origin git@github.com:sbahbouhi/command-lines.git`

`git init`

`git commit -m "xxxx"`

`git branch -M main`

`git remote add origin git@github.com:sbahbouhi/xxxx.git`

`git push -u origin main`


