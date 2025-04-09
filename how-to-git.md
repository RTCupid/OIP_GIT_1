# How to add SSH to GitHub

## Creating SSH key
To create SSH key you need do some simple actions:

```
ssh-keygen -t ed25519 -C "your_email@example.com"

> Generating public/private ed25519 key pair.

> Enter a file in which to save the key (/Users/you/.ssh/id_ed25519): [Press enter]

> Enter passphrase (empty for no passphrase): [Press enter]
> Enter same passphrase again: [Press enter]

eval "$(ssh-agent -s)"
> Agent pid 59566

$ ssh-add ~/.ssh/id_ed25519
```
##  Add SSH key to GitHub
- Open Settings - SSH and GPG keys

- Press "add SSH key"

- Put name of key and paste key to field.

- Then press "add SSH key"

## Clone repository

To clone repository enter:
``` 
git clone "SSH link to repository from GitHub"

```