# [Nordlayer](https://nordlayer.com) VPN package for Linux (esp [ArchLinux](https://archlinux.org/)) 
[![AUR version](https://img.shields.io/aur/version/nordlayer)](https://aur.archlinux.org/packages/nordlayer) [![Nordlayer version](https://img.shields.io/badge/nordlayer-3.1.0-green)](https://nordlayer.com/download/linux/)

### Important
* Original [repository](https://github.com/mearaj/nordlayer) was archived by [mearaj](https://github.com/mearaj).

If you run into any errors feel free to leave a comment [in AUR](https://aur.archlinux.org/packages/nordlayer)

To check latest official [nordlayer](https://nordlayer.com) version:
```sh
curl https://downloads.nordlayer.com/linux/latest/version -w "\n"
```
---
### Installing Nordlayer from AUR:
```sh
yay -S nordlayer
```

### Building the package manually:
```sh
git clone https://github.com/Sidicer/nordlayer.git
cd nordlayer
makepkg -si
# If 'makepkg -si' fails to install automatically:
sudo pacman -U nordlayer-3.0.0-0-x86_64.pkg.tar.zst
```
