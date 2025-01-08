<div align="center">
  
# Termux Proot Distros

</div>

<br>
<br>

<h1 align="center">
  
Download

| [Termux](https://play.google.com/store/apps/details?id=com.termux)
|
| [VNC App](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android)
|
</h1>

<br>
<br>

# General Installer
```
apt update && apt upgrade -y && apt install wget -y && wget https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/install && chmod +x install && bash install
```

------------
# Kali Nethunter Full [proot]
> - Support vnc service
> - login:`kali -r` or `kali`
> - vnc:`(kali vnc) &`
> - uninstall:`cd && rm -rf kali-arm64`

- Install
```
apt update && apt install neofetch axel bsdtar proot wget pulseaudio -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-full | sh && clear && kali
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
sed -i 's/user=kali/user=xiv3r/' /root/.zshrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.zshrc
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Chroot/vnc.jpg">

<br>
<br>
<br>
<br>

-------------
# Kali Nethunter Minimal [proot]
> - pre-build vnc
> - login:`kali` or `kali -r`
> - uninstall:`cd && rm -rf kali-arm64`

- Install
```
apt update && apt install neofetch pulseaudio axel bsdtar proot wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-minimal | sh && clear && kali
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /root/.zshrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.zshrc
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Chroot/kali-chroot.png">


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

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Proot/kali-proot.png">

<br>
<br>
<br>
<br>

----------
# BackBox Linux
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

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BackBox/backbox.png">

<br>
<br>
<br>
<br>

-----------
# BlackArch
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


<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BlackArch/bl4ckarch.png">

<br>
<br>
<br>
<br>

------------
# Debian2Kali
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

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliDeb/debkali.png">

<br>
<br>
<br>
<br>

-----------
# ParrotSec
> - login:`parrot`
> - uninstall:`pd rm parrot`

- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/ParrotSec/install | sh && clear && parrot
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/ParrotSec/Parrot.png">

<br>
<br>
<br>
<br>

-------------
# Alpine
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Alpine/install | sh && alpine
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Alpine/alpine.png">

<br>
<br>
<br>
<br>

-------------
# Archlinux
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Archlinux/install | sh && archlinux
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Archlinux/archlinux.png">

<br>
<br>
<br>
<br>


-------------
# Artix
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Artix/install | sh && artix
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Artix/artix.png">

<br>
<br>
<br>
<br>

-------------
# Centos
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Centos/install | sh && centos
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Centos/centos.png">

<br>
<br>
<br>
<br>


-------------
# Chimera
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Chimera/install | sh && chimera
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Chimera/chimera.png">

<br>
<br>
<br>
<br>


-------------
# Debian 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Debian/install | sh && debian 
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Debian/debian.png">

<br>
<br>
<br>
<br>


-------------
# Deepin 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Deepin/install | sh && deepin
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Deepin/deepin.png">

<br>
<br>
<br>
<br>


-------------
# Fedora 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/Fedora/artix/install | sh && fedora 
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Fedora/fedora.png">

<br>
<br>
<br>
<br>


-------------
# Manjaro 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Manjaro/install | sh && manjaro
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Manjaro/manjaro.png">

<br>
<br>
<br>
<br>

-------------
# Openkylin 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Openkylin/install | sh && openkylin 
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Openkylin/openkylin.png">

<br>
<br>
<br>
<br>

-------------
# Opensuse 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Opensuse/install | sh && opensuse 
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Opensuse/opensuse.png">

<br>
<br>
<br>
<br>

-------------
# Pardus 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Pardus/install | sh && pardus 
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Pardus/pardus.png">

<br>
<br>
<br>
<br>

-------------
# Ubuntu 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Ubuntu/install | sh && ubuntu 
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Ubuntu/ubuntu.png">

<br>
<br>
<br>
<br>


-------------
# Void 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Void/install | sh && void
```

<img width="700" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Void/void.png">

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

<img width="700" height="500" src="https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Termux/Termux.png">

