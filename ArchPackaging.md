1. Edit the PKGBUILD, bumping the version number.
1. Create Release in GitHub.
1. Publish Release
```
$ rm -rf plasma-simpleMonitor

$ git clone https://github.com/marco-parillo/plasma-simpleMonitor.git
Cloning into 'plasma-simpleMonitor'...
remote: Enumerating objects: 73, done.
remote: Counting objects: 100% (73/73), done.
remote: Compressing objects: 100% (64/64), done.
remote: Total 627 (delta 34), reused 29 (delta 9), pack-reused 554
Receiving objects: 100% (627/627), 570.63 KiB | 4.36 MiB/s, done.
Resolving deltas: 100% (298/298), done.

$ cd plasma-simpleMonitor

$ updpkgsums
==> Retrieving sources...
  -> Downloading v0.6.3.tar.gz...
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   142  100   142    0     0    609      0 --:--:-- --:--:-- --:--:--   609
100  446k    0  446k    0     0   742k      0 --:--:-- --:--:-- --:--:-- 1659k
==> Generating checksums for source files...

$ git add PKGBUILD

$ git push
Username for 'https://github.com': marco-parillo
Password for 'https://marco-parillo@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 399 bytes | 399.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/marco-parillo/plasma-simpleMonitor.git
   a91087c..816f7a6  master -> master

$ rm -rf plasma-simpleMonitor

$ git clone https://github.com/marco-parillo/plasma-simpleMonitor.git
Cloning into 'plasma-simpleMonitor'...
remote: Enumerating objects: 76, done.
remote: Counting objects: 100% (76/76), done.
remote: Compressing objects: 100% (65/65), done.
remote: Total 630 (delta 36), reused 34 (delta 11), pack-reused 554
Receiving objects: 100% (630/630), 570.96 KiB | 3.14 MiB/s, done.
Resolving deltas: 100% (300/300), done.

$ cd plasma-simpleMonitor

$ makepkg -si
==> Making package: plasma5-applets-simplemonitor-map 0.6.3-1 (Fri 03 Apr 2020 03:56:14 PM EDT)
==> Checking runtime dependencies...
==> Checking buildtime dependencies...
==> Installing missing dependencies...
[sudo] password for mparillo: 
resolving dependencies...
looking for conflicting packages...

Packages (5) cmake-3.17.0-1  jsoncpp-1.9.1-1  libuv-1.35.0-1  rhash-1.3.9-1
             extra-cmake-modules-5.68.0-1

Total Download Size:    9.09 MiB
Total Installed Size:  42.46 MiB

:: Proceed with installation? [Y/n] 
:: Retrieving packages...
 jsoncpp-1.9.1-1-x86_64 1183.4 KiB  4.82 MiB/s 00:00 [###########################] 100%
 libuv-1.35.0-1-x86_64   218.7 KiB  5.93 MiB/s 00:00 [###########################] 100%
 rhash-1.3.9-1-x86_64    151.7 KiB  6.44 MiB/s 00:00 [###########################] 100%
 cmake-3.17.0-1-x86_64     7.3 MiB  6.31 MiB/s 00:01 [###########################] 100%
 extra-cmake-module...   266.6 KiB  7.04 MiB/s 00:00 [###########################] 100%
(5/5) checking keys in keyring                       [###########################] 100%
(5/5) checking package integrity                     [###########################] 100%
(5/5) loading package files                          [###########################] 100%
(5/5) checking for file conflicts                    [###########################] 100%
(5/5) checking available disk space                  [###########################] 100%
:: Processing package changes...
(1/5) installing jsoncpp                             [###########################] 100%
Optional dependencies for jsoncpp
    jsoncpp-doc: documentation
(2/5) installing libuv                               [###########################] 100%
(3/5) installing rhash                               [###########################] 100%
(4/5) installing cmake                               [###########################] 100%
Optional dependencies for cmake
    qt5-base: cmake-gui [installed]
(5/5) installing extra-cmake-modules                 [###########################] 100%
:: Running post-transaction hooks...
(1/4) Arming ConditionNeedsUpdate...
(2/4) Updating icon theme caches...
(3/4) Updating the desktop file MIME type cache...
(4/4) Updating the MIME type database...
==> Retrieving sources...
  -> Downloading v0.6.3.tar.gz...
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   142  100   142    0     0    523      0 --:--:-- --:--:-- --:--:--   523
100  446k    0  446k    0     0   475k      0 --:--:-- --:--:-- --:--:-- 2838k
==> Validating source files with sha512sums...
    v0.6.3.tar.gz ... Passed
==> Extracting sources...
  -> Extracting v0.6.3.tar.gz with bsdtar
==> Starting build()...
-- The C compiler identification is GNU 9.3.0
-- The CXX compiler identification is GNU 9.3.0
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc - works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ - works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Installing in the same prefix as Qt, adopting their path scheme.
-- Configuring done
-- Generating done
-- Build files have been written to: /home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build
make[1]: Entering directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
make[2]: Entering directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
Scanning dependencies of target org.kde.simpleMonitor-plasmoids-metadata-json
make[2]: Leaving directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
make[2]: Entering directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
[100%] Generating org.kde.simpleMonitor-plasmoids-metadata.json
About to parse service type file "/usr/share/kservicetypes5/plasma-applet.desktop"
Found property definition "X-Plasma-API" with type "QString"
Found property definition "X-Plasma-RootPath" with type "QString"
Found property definition "X-Plasma-MainScript" with type "QString"
Found property definition "X-Plasma-ContainmentType" with type "QString"
Found property definition "X-Plasma-DropMimeTypes" with type "QStringList"
Found property definition "X-Plasma-DropUrlPatterns" with type "QStringList"
Found property definition "X-Plasma-NotificationArea" with type "QString"
Found property definition "X-Plasma-NotificationAreaCategory" with type "QString"
Found property definition "X-Plasma-DBusActivationService" with type "QString"
Found property definition "X-KDE-ParentApp" with type "QString"
Found property definition "X-Plasma-Provides" with type "QStringList"
Found property definition "X-Plasma-PreloadWeight" with type "int"
Found property definition "X-Plasma-ConfigPlugins" with type "QStringList"
Found property definition "X-Plasma-StandAloneApp" with type "bool"
Found property definition "X-Plasma-RequiredExtensions" with type "QStringList"
Found property definition "NoDisplay" with type "bool"
Unknown property type for key "X-Plasma-Requires-FileDialog" -> falling back to string
Unknown property type for key "X-Plasma-Requires-LaunchApp" -> falling back to string
Generated  "/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build/org.kde.simpleMonitor-plasmoids-metadata.json"
make[2]: Leaving directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
[100%] Built target org.kde.simpleMonitor-plasmoids-metadata-json
make[1]: Leaving directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
==> Entering fakeroot environment...
==> Starting package()...
make[1]: Entering directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
make[2]: Entering directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
make[2]: Leaving directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
[100%] Built target org.kde.simpleMonitor-plasmoids-metadata-json
make[1]: Leaving directory '/home/mparillo/plasma-simpleMonitor/src/plasma-simpleMonitor-0.6.3/build'
Install the project...
-- Install configuration: "Release"
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/metadata.desktop
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-manjaro-old.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-arch.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/simpleMonitor_icon.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-manjaro.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/simpleMonitor.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/simpleMonitor-skins.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-opensuse.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-fedora.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-ubuntu.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/defaultSkin-preview.png
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-tux.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/resize.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-mint.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/minimalisticSkin-preview.png
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/columnSkin-preview.png
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-slackware.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/images/distro-kubuntu.svg
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Michroma
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Michroma/Michroma.ttf
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Michroma/OFL.txt
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Monda
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Monda/Monda-Bold.ttf
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Monda/Monda-Regular.ttf
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Monda/OFL.txt
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Play
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Play/Play-Regular.ttf
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Play/OFL.txt
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Play/Play-Bold.ttf
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Doppio_One
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Doppio_One/OFL.txt
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/fonts/Doppio_One/DoppioOne-Regular.ttf
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/skins
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/skins/BaseSkin.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/skins/DefaultSkin.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/skins/MinimalisticSkin.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/skins/ColumnSkin.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/components
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/components/LogoImage.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/main.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/CpuWidget.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/DatePicker.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/HighlightCpu.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/AverageCPU.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/UptimePicker.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/OsInfoItem.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/CoreTempList.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/MemArea.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/monitorWidgets/TimePicker.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/config
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/config/ConfigSkins.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/ui/config/ConfigGeneral.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/config
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/config/config.qml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/config/main.xml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/code
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/contents/code/code.js
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/plasma/plasmoids/org.kde.simpleMonitor/metadata.json
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/metainfo/org.kde.simpleMonitor.appdata.xml
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/kservices5/plasma-applet-org.kde.simpleMonitor.desktop
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/locale/pl/LC_MESSAGES/plasma_applet_org.kde.simpleMonitor.mo
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/locale/ru/LC_MESSAGES/plasma_applet_org.kde.simpleMonitor.mo
-- Installing: /home/mparillo/plasma-simpleMonitor/pkg/plasma5-applets-simplemonitor-map/usr/share/locale/zh_CN/LC_MESSAGES/plasma_applet_org.kde.simpleMonitor.mo
==> Tidying install...
  -> Removing libtool files...
  -> Purging unwanted files...
  -> Removing static library files...
  -> Stripping unneeded symbols from binaries and libraries...
  -> Compressing man and info pages...
==> Checking for packaging issues...
==> Creating package "plasma5-applets-simplemonitor-map"...
  -> Generating .PKGINFO file...
  -> Generating .BUILDINFO file...
  -> Generating .MTREE file...
  -> Compressing package...
==> Leaving fakeroot environment.
==> Finished making: plasma5-applets-simplemonitor-map 0.6.3-1 (Fri 03 Apr 2020 03:56:36 PM EDT)
==> Installing package plasma5-applets-simplemonitor-map with pacman -U...
loading packages...
resolving dependencies...
looking for conflicting packages...

Packages (1) plasma5-applets-simplemonitor-map-0.6.3-1

Total Installed Size:  0.93 MiB

:: Proceed with installation? [Y/n] 
(1/1) checking keys in keyring                       [###########################] 100%
(1/1) checking package integrity                     [###########################] 100%
(1/1) loading package files                          [###########################] 100%
(1/1) checking for file conflicts                    [###########################] 100%
(1/1) checking available disk space                  [###########################] 100%
:: Processing package changes...
(1/1) installing plasma5-applets-simplemonitor-map   [###########################] 100%
:: Running post-transaction hooks...
(1/1) Arming ConditionNeedsUpdate...

```
