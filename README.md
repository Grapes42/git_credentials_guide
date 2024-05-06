# Git Credentials Guide

## Email and username
Configure your email and username with:
```
git config --global user.name "your username"
git config --global user.email your.email@address.com
```

## Curl
Check `curl` is installed with:
```
curl --version
```
If not, install curl with:

### For Debian/Ubuntu
```
sudo apt install curl
```

### For Fedora
```
sudo dnf install curl
```


## Setup script
Download and run the setup script with
```
curl -L https://aka.ms/gcm/linux-install-source.sh | sh
git-credential-manager configure
```

## Generate keys
Choose credential store with:
```
git config --global credential.credentialStore gpg
```

Generate a new key pair with
```
gpg --gen-key
```

## Initialize your keys
Check if `pass` is installed with:
```
pass --version
```
If not, install it with:

### For Debian/Ubuntu
```
sudo apt install pass
```
### For Fedora
```
sudo dnf install pass
```

Then, initialize your keys with:
```
pass init your.email@address.com
```

Done!






