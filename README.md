<div align="center">
  
# Termux Penetration Testing Distros
| Kali Linux | BlackArch Linux | BackBox Linux | Parrot Sec Linux | Kali Debian |
</div>

# Kali Nethunter Full [chroot]
> - official tarball
> - support vnc service
> - login:`nethunter` or `nethunter -r` `nh` or `nh -r`
> - login w/ vnc:`nethunter kex &` or `nethunter -r kex &` or `nh kex &` `nh -r kex &`
> - uninstall:`cd && rm -rf chroot`
```
apt update && apt install proot wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-full | sh && nh -r
```
- Configure profile
```
wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/rcfiles/install.sh | sh
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .bashrc
sed -i 's/user=kali/user=xiv3r/' /home/.bashrc
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc
```


# Kali Nethunter Minimal [chroot]
> - official tarball
> - login:`nethunter` or `nethunter -r` `nh` or `nh -r`
> - uninstall:`cd && rm -rf chroot`
```
apt update && apt install proot wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-minimal | sh && nh -r
```
- Configure profile
```
wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/rcfiles/install.sh | sh
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .bashrc
sed -i 's/user=kali/user=xiv3r/' /home/.bashrc
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc
```

# Kali Nethunter Full [proot-distro]
> - Official tarball
> - login:`kali`
> - uninstall:`pd rm kali-full`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-full | sh && kali
```
- Setup .zshrc profile
```
wget -O /root/.zshrc https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/.zshrc
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```
# Kali Nethunter Minimal [proot-distro]
> - Official tarball
> - login:`kalimin`
> - uninstall:`pd rm kali-minimal`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-minimal | sh && kalimin
```
- Setup .zshrc profile
```
wget -O /root/.zshrc https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/.zshrc && source .zshrc
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Proot/kali-proot.png">
</div>

# BackBox Linux [proot-distro]
> - Custom build tarball
> - login:`backbox`
> - uninstall:`pd rm backbox`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BackBox/install | sh && backbox
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BackBox/backbox.png">
</div>

# BlackArch Linux [proot-distro]
> - Arch to Balackarch
> - Custom build tarball
> - login:`blackarch`
> - uninstall:`pd rm blackarch`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BlackArch/install | sh && blackarch
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BlackArch/blackarch.png">
</div>


# Kali in Debian [proot-distro]
> - debian convert to kali custom build tarball
> - login:`debkali`
> - uninstall:`pd rm debkali`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && debkali
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliDeb/debkali.png">
</div>


# ParrotSec [proot-distro]
> - custom build tarball
> - login:`parrot`
> - uninstall:`pd rm parrot`
```
apt update && apt install proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && parrot
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/ParrotSec/parrot.png">
</div>
