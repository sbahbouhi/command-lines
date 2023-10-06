# command-lines

## Encription

`gpg --armor --symmetric --cipher-algo CIPHER message.txt`
`gpg --output original_message.txt --decrypt message.gpg`

`openssl aes-256-cbc -pbkdf2 -iter 10000 -e -in message.txt -out encrypted_message`
`openssl aes-256-cbc -pbkdf2 -iter 10000 -d -in encrypted_message -out original_message.txt`


## Gobuster

