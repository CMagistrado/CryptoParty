# CryptoParty
## How to install GPG
Providing additional details from my talks on cryptography.

# Windows Installation
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/j7WzLw-UKQ0/0.jpg)](https://www.youtube.com/watch?v=j7WzLw-UKQ0)

1. Download gpg4win - https://www.gpg4win.org/

2. 

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

# Mac OS X / Linux Usage 

1. Create gpg keys
```
gpg --gen-key
```

2. Print your public key
```
gpg --export --armour username
```

3. Print your PRIVATE KEY
```
gpg --export-secret-key --armour username
```

4. Import Key
```
gpg --import-key filename.pub
```

5. Print keyring (Keys your have)
```
gpg --list-keys
```

6. Encrypt file
```
gpg --encrypt --armour filename
```
7. Decrypt file
```
gpg --decrypt filename
```
