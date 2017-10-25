# How to install GPG

# Windows Installation + Usage
## gpg4win
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/j7WzLw-UKQ0/0.jpg)](https://www.youtube.com/watch?v=j7WzLw-UKQ0)

1. Download gpg4win and following instructions - https://www.gpg4win.org/
Documentation - https://files.gpg4win.org/doc/gpg4win-compendium-en.pdf

2. Click "Create New Key Pair"
3. Provide Name and Email
4. Click "Advanced Settings"
5. Change 2048 bits to 4096 bits.
6. Check the "Valid till" box and set your expiration date of your new keys.
7. Click Create.
8. Enter a secure password twice. (Best practice would be to save this in an offline password manager, on a device that cannot connect to any network.
9. 


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
