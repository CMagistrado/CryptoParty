# CryptoParty
## How to install GPG
Providing additional details from my talks on cryptography.

# Windows Installation
<iframe width="560" height="315" src="https://www.youtube.com/embed/j7WzLw-UKQ0" frameborder="0" gesture="media" allowfullscreen></iframe>

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/j7WzLw-UKQ0/0.jpg)](https://www.youtube.com/watch?v=j7WzLw-UKQ0)

# Mac OS X Installation

<a href="https://asciinema.org/a/eo3Vs5hzKAeRwoTZ2qXxMBlpc" target="_blank"><img src="https://asciinema.org/a/eo3Vs5hzKAeRwoTZ2qXxMBlpc.png" width=589 height=411 /></a>


1. Install Brew: https://brew.sh/
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

2. Install gpg
```
brew install gpg
```

3. Create gpg keys
```
gpg --gen-key
```

4. Print your public key
```
gpg --export --armour username
```

5. Print your PRIVATE KEY
```
gpg --export-secret-key --armour username
```

6. Import Key
```
gpg --import-key filename.pub
```

7. Print keyring (Keys your have)
```
gpg --list-keys
```

8. Encrypt file
```
gpg --encrypt --armour filename
```
9. Decrypt file
```
gpg --decrypt filename
```
