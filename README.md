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

- Autologin
```
echo "kali -r && vnc start" >>$PREFIX/etc/bash.bashrc
```

- Install
```
apt update && apt install axel proot wget -y && wget https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-full && chmod +x kali-full && ./kali-full
```

- Configure profile
```
apt update && apt install wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/rcfiles/install.sh | sh
```

- VNC
```
vnc start
```

- Update and Upgrade
```
apt update && apt full-upgrade -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" -y
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
```

<div align="center">
<img src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Chroot/kali-vnc.png">
</div>

<br>
<br>
<br>
<br>

-------------
# Kali Nethunter Minimal [chroot]
> - login:`nethunter` or `nethunter -r` `kali` or `kali -r`
> - uninstall:`cd && rm -rf chroot`

- Autologin
```
echo "kali -r" >>$PREFIX/etc/bash.bashrc
```

- Install
```
apt update && apt install bsdtar proot wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-minimal | sh && kali -r
```

- Configure profile
```
apt update && apt install wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/rcfiles/install.sh | sh
```

- Update and Upgrade
```
apt update && apt full-upgrade -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" -y
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
```
<br>
<br>
<br>
<br>

---------------
# Kali Nethunter Full [proot-distro]
> - login:`kali`
> - uninstall:`pd rm kali-full`

- Autologin
```
echo "kali" >>$PREFIX/etc/bash.bashrc
```

- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-full | sh && kali
```

- Setup .zshrc profile
```
apt update && apt install wget -y && wget -O /root/.zshrc https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/.zshrc
```

- Update and Upgrade
```
apt update && apt full-upgrade -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" -y
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

- Autologin
```
echo "kali" >>$PREFIX/etc/bash.bashrc
```

- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-minimal | sh && kali
```

- Setup .zshrc profile
```
apt update && apt install wget -y && wget -O /root/.zshrc https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/.zshrc && source .zshrc
```

- Update and Upgrade
```
apt update && apt full-upgrade -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" -y
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

- Autologin
```
echo "backbox" >>$PREFIX/etc/bash.bashrc
```

- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BackBox/install | sh && backbox
```

- Update and Upgrade
```
apt update && apt full-upgrade -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" -y
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

- Autologin
```
echo "blackarch" >>$PREFIX/etc/bash.bashrc
```

- Install 
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BlackArch/install | sh && blackarch
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

- Autologin
```
echo "debkali" >>$PREFIX/etc/bash.bashrc
```

- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | sh && debkali
```

- Update and Upgrade
```
apt update && apt full-upgrade -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" -y
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

- Autologin
```
echo "parrot" >>$PREFIX/etc/bash.bashrc
```

- Install
```
apt update && apt install bsdtar proot-distro wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/ParrotSec/install | sh && parrot
```

- Update and Upgrade
```
apt update && apt full-upgrade -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" -y
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
