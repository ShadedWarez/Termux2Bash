<div align="center">
  
# Termux Penetration Testing Distros
| Kali Linux | BlackArch Linux | BackBox Linux | Parrot Sec Linux | Kali Debian |
</div>

<br>
<br>

<h1 align="center">

| [Termux 0.119.1](https://github.com/xiv3r/Kali-Linux-Termux/releases/download/Apps/Termux_v0.119.1.apk)
|
| [RealVNC App](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android)
|
</h1>

<br>
<br>

------------
# Kali Nethunter Full [chroot]
> - Support vnc service
> - login:`kali -r` or `kali`
> - vnc:`(kali vnc) &`
> - uninstall:`cd && rm -rf kali-arm64`

- Install
```
apt update && apt install axel bsdtar proot wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-full | sh && clear && kali vnc passwd && (kali vnc) & && kali
```

- Start VNC
> `127.0.0.1:5901`
```
kali vnc password
```
```
kali vnc &
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
```

<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Chroot/vnc.jpg">
</div>

<br>
<br>
<br>
<br>

-------------
# Kali Nethunter Minimal [chroot]
> - pre-build vnc
> - login:`kali` or `kali -r`
> - uninstall:`cd && rm -rf kali-arm64`

- Install
```
apt update && apt install axel bsdtar proot wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-minimal | sh && clear && kali
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Chroot/kali-chroot.png">
</div>

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
apt update && apt install git axel bsdtar proot proot-distro wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-full | sh && clear && kali
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
apt update && apt install git axel bsdtar proot proot-distro wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-minimal | sh && clear && kali
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
apt update && apt install axel bsdtar proot proot-distro wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BackBox/install | sh && clear && backbox
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

- Install 
```
apt update && apt install axel bsdtar proot proot-distro wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BlackArch/install | sh && clear && blackarch
```

- Update and Upgrade
```
pacman -Syyu
```
- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc && source /etc/bash.bashrc
```

<details><summary> Blackarch Tools</summary>

- To list all of the available tools, run
```
pacman -Sgg | grep blackarch | cut -d' ' -f2 | sort -u
```

- To install a category of tools, run
```
pacman -S blackarch-<category>
```

- To see the blackarch categories, run
```
pacman -Sg | grep blackarch
````
- To search for a specific package, run
```
pacman -Ss <package_name>
```

</details>

<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BlackArch/bl4ckarch.png">
</div>

<br>
<br>
<br>
<br>

------------
# Kali in Debian [proot-distro]
> - login:`debkali`
> - uninstall:`pd rm debkali`

- Install
```
apt update && apt install axel bsdtar proot proot-distro wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && clear && debkali
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

- Install
```
apt update && apt install git axel bsdtar proot proot-distro wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/ParrotSec/install | sh && clear && parrot
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```
<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/ParrotSec/parrot.png">
</div>

<br>
<br>
<br>
<br>

-------------
# Termux
- Install
```
wget -O $PREFIX/etc/bash.bashrc https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Termux/bash.bashrc && source $PREFIX/etc/bash.bashrc
```

<div align="center">
<img src="https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Termux/termux.png">
</div>
