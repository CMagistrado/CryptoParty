# CryptoParty
Providing additional details from my talks on cryptography.

<a href="https://asciinema.org/a/eo3Vs5hzKAeRwoTZ2qXxMBlpc" target="_blank"><img src="https://asciinema.org/a/eo3Vs5hzKAeRwoTZ2qXxMBlpc.png" /></a>

# Mac OS X Installation

[![asciicast](https://asciinema.org/a/eo3Vs5hzKAeRwoTZ2qXxMBlpc.png)](https://asciinema.org/a/eo3Vs5hzKAeRwoTZ2qXxMBlpc)

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
