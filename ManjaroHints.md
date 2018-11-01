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

 * Wait for Discovered Network Printers

 * EPSON WF-2760 Series

 * IPP Seems Default

 * Searching for Drivers

 * Take the second (non-driverless)

 * Print (Epson Epson)

falkon --disable-gpu

Last release without discover: https://osdn.net/projects/manjaro/storage/kde/18.0-rc1/
