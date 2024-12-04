<div align="center">
  
# Termux-Pentesting-Distro
| Kali Linux | BlackArch Linux | BackBox Linux | Parrot Sec Linux | Kali Debian |
for
Termux Proot-Distro & Chroot
</div>

# Kali Nethunter Full [chroot]
> - official tarball
> - support vnc service
> - login:`nethunter` or `nethunter -r`
> - login w/ vnc:`nethunter kex &` or `nethunter -r kex &`
> - uninstall:`cd && rm -rf chroot`
```
apt update && apt install proot wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-full | sh && nethunter -r
```

# Kali Nethunter Minimal [chroot]
> - official tarball
> - login:`nethunter` or `nethunter -r`
> - uninstall:`cd && rm -rf chroot`
```
apt update && apt install proot wget -y && wget -qO https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-minimal | sh && nethunter -r
```

# Kali Nethunter Full [proot-distro]
> - Official tarball
> - login:`pd sh kali-full`
> - uninstall:`pd rm kali-full`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-full | sh && pd sh kali-full
```

# Kali Nethunter Minimal [proot-distro]
> - Official tarball
> - login:`pd sh kali-minimal`
> - uninstall:`pd rm kali-minimal`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-minimal | sh && pd sh kali-minimal
```
- Setup .zshrc profile
```
wget -O /root/.zshrc https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/.zshrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Proot/kali-proot.png">
</div>

# BackBox Linux [proot-distro]
> Custom build tarball
> login:`pd sh backbox`
> uninstall:`pd rm backbox`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BackBox/install | sh && pd sh backbox
```

# BlackArch Linux [proot-distro]
> - Custom build tarball
> - login:`pd sh blackarch`
> - uninstall:`pd rm blackarch`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BlackArch/install | sh && pd sh blackarch
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BlackArch/blackarch.png">
</div>


# Kali in Debian [proot-distro]
> - debian convert to kali custom build tarball
> - login:`pd sh debkali`
> - uninstall:`pd rm debkali`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && pd sh debkali
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliDeb/debkali.png">
</div>


# ParrotSec [proot-distro]
> - arch to blackarch custom build tarball
> - login:`pd sh parrot`
> - uninstall:`pd rm parrot`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && pd sh parrot
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/ParrotSec/parrot.png">
</div>
