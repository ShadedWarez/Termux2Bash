# Termux-Pentesting-Distro
Kali Linux | BlackArch Linux | BackBox Linux | Parrot Sec Linux | Kali Debian | for Termux Proot-Distro

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
