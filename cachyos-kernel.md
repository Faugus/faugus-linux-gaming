# Arch Linux

Install the CachyOS keyring
```
sudo pacman-key --recv-keys F3B607488DB35A47 --keyserver keyserver.ubuntu.com
sudo pacman-key --lsign-key F3B607488DB35A47
```

Install required packages:
```
sudo pacman -U 'https://mirror.cachyos.org/repo/x86_64/cachyos/cachyos-keyring-20240331-1-any.pkg.tar.zst' \
               'https://mirror.cachyos.org/repo/x86_64/cachyos/cachyos-mirrorlist-18-1-any.pkg.tar.zst'
```

Add CachyOS repository
```
sudo nano /etc/pacman.conf
```
```
[cachyos]
Include = /etc/pacman.d/cachyos-mirrorlist
```

Update repositories
```
sudo pacman -Sy
```
Install CachyOS kernel
```
sudo pacman -S linux-cachyos
```

# Fedora

Add CachyOS repository
```
sudo dnf -y copr enable bieszczaders/kernel-cachyos
```

Install CachyOS kernel
```
sudo dnf -y install kernel-cachyos
```
