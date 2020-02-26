What that means is that your installed packages are at the same version as in the mirror you sync with. However, a newbie might think that means that your installation is identical to a freshly-installed ISO, when it is not.

For example, if you read all the release announcements you might learn that:

* A package was removed because it becomes problematic. For example: Plymouth was removed from new ISOs, and you had to manually [remove it](https://wiki.manjaro.org/index.php?title=Plymouth#Removal) for your installation to boot the same way as an installation from a newer ISO.

* A package was could be replaced with a different one performing much the same function. So, for example, on the Manjaro KDE edition, newer ISOs replaced Octopi with pamac. Unless you manually removed Octopi and installed pamac, you would be using a different front-end to your package manager.

* A package was added, for example 
`ms-office-online`
You would never get it unless you manually added it.

* Themes might be upgraded, for example from breath to breath2, but [you will need to manually download the packages and change the themes yourself](https://forum.manjaro.org/t/manjaro-19-0-released/126148/2?u=mparillo).

* A package could be 'demoted' to the AUR. For example, `openssl-1.0` was used with steam. but dropped from the Manjaro repos. You can list your AUR packages with:
`$ pacman -Qm`
And remove the ones you do not want. But if you do not, you will have AUR packages that would not be on a freshly-installed Manjaro.

* Packages can become orphans. You can remove them with
`$ sudo pacman -Rsn $(pacman -Qqdt)`

* Configuration files may change. Most changes are harmless to most users, but users should know [how to manage pacnew and pacsave files](https://wiki.manjaro.org/index.php?title=Pacnew_and_Pacsave_Files).

* Default permissions can change over time. [For example](https://forum.manjaro.org/t/stable-update-2018-07-06-kernels-firefox-virtualbox-python-haskell/51574/2):
`Directory permissions differ on /var/lib/samba/private/`
`filesystem: 755 package: 700`
So, you are advised to change them with:
`$ sudo chmod 700 /var/lib/samba/private/`

* The default kernel can get upgraded. In my case, I have been happily running 4.19 for years, but to match a freshly-installed Manjaro running 5.x, I would need to use [Manjaro Settings Manager](https://wiki.manjaro.org/index.php/Manjaro_Kernels#GUI_Tool) or the terminal equivalents.

Now, with manual effort, none of these are impossible, but it is important to be clear to newbies that, wth a rolling release, if you set it and forget it, your packages get upgraded, but your system will *not* match a fresh installation.
