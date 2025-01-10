<div align="center">
  
  <details><summary>

# Termux Proot-Distro

Proot Distro uses pre-built root filesystems (rootfs) of Linux distributions. These are essentially the core files of a Linux OS.

PRoot is used to "fake" the root environment, allowing you to run the rootfs as if it were a full Linux system.
  </summary>
  
   `Proot Distro is a tool used in environments like Termux (a terminal emulator and Linux environment for Android) to manage and run Linux distributions (distros) in an isolated, containerized environment. It uses PRoot (a user-space implementation of chroot, mount --bind, and binfmt_misc) to run Linux distributions without requiring root access or complex setup.

Key Features of Proot Distro:
No Root Access Required: Proot Distro allows you to run Linux distributions on devices without root access.

Lightweight: It uses minimal resources compared to full virtualization or emulation.

Easy Management: You can install, remove, and manage multiple Linux distributions easily.

Isolation: Each distro runs in its own isolated environment, preventing conflicts with the host system.

Cross-Platform: Works on Android (via Termux) and other platforms where PRoot is supported.

How Proot Distro Works:
Rootfs (Root Filesystem): Proot Distro uses pre-built root filesystems (rootfs) of Linux distributions. These are essentially the core files of a Linux OS.

PRoot: PRoot is used to "fake" the root environment, allowing you to run the rootfs as if it were a full Linux system.

Proot-Distro Scripts: Each distro has a configuration script (e.g., kali.sh, ubuntu.sh) that defines how the rootfs is downloaded, installed, and managed.`

</details>
</div>

<h3 align="center">
  
Download

| [Termux](https://play.google.com/store/apps/details?id=com.termux)
|
| [VNC App](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android)
|
</h3>

<br>
<br>

# General Installer
> Only `Arm64/Aarch64` is supported
```
apt update && apt upgrade -y && apt install wget -y && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Install/install | bash && PROOT-DISTRO
```
# Install Distro
> Install a specific distro
```sh
PROOT-DISTRO
```
### Login
> Example: `kali`
```
kali
```
### Logout
> Back to Termux
```
exit
```
### Uninstall
> Example: `uninstall-kali`
```
uninstall-kali
```

# Proot Options
## List of the available proot-distro commands:

- `pd help`         - Show this help information.
- `pd backup`       - Backup a specified distribution.
- `pd list`         - List supported distributions and their installation status.
- `pd login`        - Start login shell for the specified distribution.
- `pd remove`       - Delete a specified distribution.
- `pd rename`       - Rename installed distribution.
- `pd reset`        - Reinstall from scratch a specified distribution.
- `restore`         - Restore a specified distribution
- `clear-cache`     - Clear cache of downloaded files.

Example: `pd install ubuntu`

  
------------

# Kali Nethunter Full [proot]
> - Support vnc service
> - login:`kali`
> - vnc:`(kali vnc) &`
> - uninstall:`cd && rm -rf kali-arm64`

- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-full | bash && clear && kali
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

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Chroot/vnc.jpg">

<br>
<br>
<br>
<br>

-------------
# Kali Nethunter Minimal [proot]
> - login:`kali`
> - uninstall:`cd && rm -rf kali-arm64`

- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Chroot/kali-minimal | bash && clear && kali
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /root/.bashrc
sed -i 's/user=kali/user=xiv3r/' /root/.zshrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.bashrc
sed -i 's/user=kali/user=xiv3r/' /home/kali/.zshrc
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Chroot/kali-linux.png">

<br>
<br>
<br>
<br>

-------------
# Alma
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Alma/install | bash && alma
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Alma/alma.png">

<br>
<br>
<br>
<br>

-------------
# Alpine
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Alpine/install | bash && alpine
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Alpine/alpine.png">

<br>
<br>
<br>
<br>

-------------
# Amazon
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Amazon/install | bash && amazon
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Amazon/amazon.png">

<br>
<br>
<br>
<br>

-------------
# Archlinux
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Archlinux/install | bash && archlinux
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Archlinux/archlinux.png">

<br>
<br>
<br>
<br>


-------------
# Artix
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Artix/install | bash && artix
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Artix/artix.png">

<br>
<br>
<br>
<br>


----------
# BackBox
> - login:`backbox`
> - uninstall:`pd rm backbox`

- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BackBox/install | bash && clear && backbox
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc && source /etc/bash.bashrc
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BackBox/backbox.png">

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
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/BlackArch/install | bash && clear && blackarch
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


<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/BlackArch/Blackarch.png">

<br>
<br>
<br>
<br>

-------------
# Centos
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Centos/install | bash && centos
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Centos/centos.png">

<br>
<br>
<br>
<br>

-------------
# Chimera
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Chimera/install | bash && chimera
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Chimera/chimera.png">

<br>
<br>
<br>
<br>


-------------
# Debian 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Debian/install | bash && debian 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Debian/debian.png">

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
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliDeb/install | bash && clear && debkali
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' /etc/bash.bashrc && source /etc/bash.bashrc
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliDeb/NH.png">

<br>
<br>
<br>
<br>

-------------
# Deepin 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Deepin/install | bash && deepin
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Deepin/deepin.png">

<br>
<br>
<br>
<br>

-------------
# Fedora 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/Fedora/artix/install | bash && fedora 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Fedora/fedora.png">

<br>
<br>
<br>
<br>


---------------
# Kali Nethunter Full
> - login:`kali-full`
> - uninstall:`pd rm kali-full`

- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-full | bash && clear && kali-full
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```
<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Proot/NH.png">

<br>
<br>
<br>
<br>

----------------
# Kali Nethunter Minimal
> - login:`kali`
> - uninstall:`pd rm kali-minimal`

- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/KaliLinux/Proot/kali-minimal | bash && clear && kali
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/KaliLinux/Proot/NH.png">

<br>
<br>
<br>
<br>


-------------
# Manjaro 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Manjaro/install | bash && manjaro
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Manjaro/manjaro.png">

<br>
<br>
<br>
<br>

-------------
# Openkylin 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Openkylin/install | bash && openkylin 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/OpenKylin/openkylin.png">

<br>
<br>
<br>
<br>

-------------
# Opensuse 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Opensuse/install | bash && opensuse 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Opensuse/opensuse.png">

<br>
<br>
<br>
<br>

-------------
# Oracle 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Oracle/install | bash && oracle 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Oracle/oracle.png">

<br>
<br>
<br>
<br>


-------------
# Pardus 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Pardus/install | bash && pardus 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Pardus/pardus.png">

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
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/ParrotSec/install | bash && clear && parrot
```

- Add custom terminal name
> replace `xiv3r` to your name
```
sed -i 's/user=kali/user=xiv3r/' .zshrc && source .zshrc
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/ParrotSec/Parrot.png">

<br>
<br>
<br>
<br>

-------------
# Photon 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Photon/install | bash && photon 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Photon/photon.png">

<br>
<br>
<br>
<br>


-------------
# Rocky 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Rocky/install | bash && rocky 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Rocky/rocky.png">

<br>
<br>
<br>
<br>

-------------
# Termux
- Install
```
apt update && apt install wget neofetch -y && wget -O $PREFIX/etc/bash.bashrc https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Termux/bash.bashrc && source $PREFIX/etc/bash.bashrc
```

<img width="800" height="500" src="https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Termux/term.png">

-------------
# Ubuntu 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Ubuntu/install | bash && ubuntu 
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Ubuntu/ubuntu.png">

<br>
<br>
<br>
<br>

-------------
# Void 
- Install
```
apt update && apt install wget -y && clear && wget -qO- https://raw.githubusercontent.com/xiv3r/Termux-Pentesting-Distro/refs/heads/main/Void/install | bash && void
```

<img width="800" height="500" src="https://github.com/xiv3r/Termux-Pentesting-Distro/blob/main/Void/void.png">

<br>

