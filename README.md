<div align="center">
  
# Termux Penetration Testing Distros
| Kali Linux | BlackArch Linux | BackBox Linux | Parrot Sec Linux | Kali Debian |
</div>

<br>
<br>
<br>
<br>

------------
# Kali Nethunter Full [chroot]
> - support vnc service
> - login:`nethunter` or `nethunter -r` `kali` or `kali -r`
> - login w/ vnc:`nethunter kex &` or `nethunter -r kex &` or `kali kex &` `kali -r kex &`
> - uninstall:`cd && rm -rf chroot`
- Install
```
apt update && apt install bsdtar proot wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-full | sh && kali -r
```
- Configure profile
```
wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/rcfiles/install.sh | sh
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc
```
<br>
<br>
<br>
<br>

-------------
# Kali Nethunter Minimal [chroot]
> - login:`nethunter` or `nethunter -r` `kali` or `kali -r`
> - uninstall:`cd && rm -rf chroot`
- Install
```
apt update && apt install bsdtar proot wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-minimal | sh && kali -r
```
- Configure profile
```
wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/rcfiles/install.sh | sh
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc
```
<br>
<br>
<br>
<br>

---------------
# Kali Nethunter Full [proot-distro]
> - login:`kali`
> - uninstall:`pd rm kali-full`
- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-full | sh && kali
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
<br>
<br>
<br>
<br>

----------------
# Kali Nethunter Minimal [proot-distro]
> - login:`kali`
> - uninstall:`pd rm kali-minimal`
- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-minimal | sh && kali
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

<br>
<br>
<br>
<br>

----------
# BackBox Linux [proot-distro]
> - login:`backbox`
> - uninstall:`pd rm backbox`
- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BackBox/install | sh && backbox
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc && source /etc/bash.bashrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BackBox/backbox.png">
</div>

<br>
<br>
<br>
<br>

-----------
# BlackArch Linux [proot-distro]
> - Custom build rootfs tarball
> - login:`blackarch`
> - uninstall:`pd rm blackarch`
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BlackArch/install | sh && blackarch
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BlackArch/blackarch.png">
</div>

<br>
<br>
<br>
<br>

------------
# Kali in Debian [proot-distro]
> - login:`debkali`
> - uninstall:`pd rm debkali`
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && debkali
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc && source /etc/bash.bashrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliDeb/debkali.png">
</div>

<br>
<br>
<br>
<br>

-----------
# ParrotSec [proot-distro]
> - login:`parrot`
> - uninstall:`pd rm parrot`
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && parrot
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc && source /etc/bash.bashrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/ParrotSec/parrot.png">
</div>
