# [Nordlayer](https://nordlayer.com) VPN package for Linux (esp [ArchLinux](https://archlinux.org/)) 
![AUR version](https://img.shields.io/aur/version/nordlayer)
### Important
Original repository was archived by mearaj as they are longer a nordlayer user ([mearaj/nordlayer](https://github.com/mearaj/nordlayer)) <br>
I will be maintaining this fork from now on.

To check latest official [nordlayer](https://nordlayer.com) version:
```sh
curl https://downloads.nordlayer.com/linux/latest/version -w "\n"
```
For any issues, please create an issue or leave a comment [in AUR](https://aur.archlinux.org/packages/nordlayer)

Installing from AUR:
```sh
yay -S nordlayer
```

Building the package manually:
```sh
git clone https://github.com/Sidicer/nordlayer.git
cd nordlayer
makepkg -si
# If 'makepkg -si' fails to install automatically:
sudo pacman -U nordlayer-2.6.2-0-x86_64.pkg.tar.zst
```
