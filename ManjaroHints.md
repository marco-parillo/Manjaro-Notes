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

falkon --disable-gpu

Last release without discover: https://osdn.net/projects/manjaro/storage/kde/18.0-rc1/

Date of installation
```
$ stat / | grep Birth
```

If ordering a new laptop:
 * No Secureboot
 * No Fast Boot
 * EFI only
 * No CSM
 * No Legacy BIOS/MBR boot.
 * No RAID; Disks on AHCI

VPN
VPN Page: https://remote.vpn.comcast.net/
The first time click on the Web Network Access Link, and download the file 
Save the .deb Firefox plugin
Convert to Arch Package
Install debtap: https://aur.archlinux.org/packages/debtap/
$ sudo debtap -u
$ debtap linux_f5vpn.x86_64.deb
Install the generated package (in my case)
$ sudo pacman -U f5vpn-7170.2018.0626.1-1-x86_64.pkg.tar.xz




. Then you can reload the page, login, and it sends an MFA request
