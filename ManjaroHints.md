# Printing

CUPS needs sys
```
$ sudo gpasswd -a mparillo sys
[sudo] password for mparillo: 
Adding user mparillo to group sys
```
May also need
```
sudo pacman -Si gtk3-print-backends
```
To Print:

 * Printers > Add Printers
 * Wait for Discovered Network Printers (need to be on the same wireless network)
 * EPSON WF-2760 Series
 * IPP Seems Default
 * Searching for Drivers
 * Take the second (non-driverless)
 * Print (Epson Epson)

# New Manjaro Themes
The theme package does not automatically come with the update. If you want it, install the following packages:

 * breath2-icon-themes
 * breath2-wallpaper
 * plasma5-themes-breath2
 * sddm-breath2-theme

# Falkon rendering

falkon --disable-gpu

# Date of installation
```
$ stat / | grep Birth
```

# If ordering a new laptop:
 * No Secureboot
 * No Fast Boot
 * EFI only
 * No CSM
 * No Legacy BIOS/MBR boot.
 * No RAID; Disks on AHCI

# REISUB
```
$ su -
Password: 
[marco-T61 ~]# echo "kernel.sysrq=1" > /etc/sysctl.d/99-sysctl.conf
[marco-T61 ~]# exit
logout
[mparillo@marco-T61 ~]$ cat /etc/sysctl.d/99-sysctl.conf
kernel.sysrq=1
[mparillo@marco-T61 ~]$ 
```


# VPN
 * VPN Page: https://remote.vpn.comcast.net/
 * The first time click on the Web Network Access Link, and download the file 
 * Save the .deb Firefox plugin
 * Convert to Arch Package
 * Install debtap: https://aur.archlinux.org/packages/debtap/
```
$ sudo debtap -u
$ debtap linux_f5vpn.x86_64.deb
$ sudo pacman -U f5vpn-7170.2018.0626.1-1-x86_64.pkg.tar.xz
```
Then you can reload the page, login, and it sends an MFA request

# Only unique commands in Bash History.

Edit ~/.bash_profile
```
export HISTCONTROL=ignoreboth:erasedups
```

# VMWare

Edit /etc/mkinitcpio.conf and comment out the old MODULES, replacing it:
```
# MODULES=""
MODULES=(vsock vmw_vsock_vmci_transport vmw_balloon vmw_vmci vmwgfx)
```
Regenerate the initramfs simply by doing an upgrade (if possible), or rebuild initramfs and grub config:
```
sudo mkinitcpio -P
sudo grub-mkconfig -o /boot/grub/grub.cfg
```
And reboot.

Or maybe llvmpipe

```
Operating System: Manjaro Linux
KDE Plasma Version: 5.20.80
KDE Frameworks Version: 5.76.0
Qt Version: 5.15.1
Kernel Version: 5.8.16-2-MANJARO
OS Type: 64-bit
Processor: 1 × Intel® Core™ i7-6600U CPU @ 2.60GHz
Memory: 1.9 GiB of RAM
Graphics Processor: llvmpipe
```
