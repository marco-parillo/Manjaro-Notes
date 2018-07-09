What that means is that your installed packages are at the same version as in the mirror you sync with. However, a newbie might think that means that your installation is identical to a freshly-installed ISO.

For example, if you read all the release announcements you might learn that:

* A package was removed because it becomes problematic. For example: Plymouth was removed from new ISOs, and you could manually remove it. https://wiki.manjaro.org/index.php?title=Plymouth#Removal

* A package could be 'demoted' to the AUR. You can list your AUR packages with:
$ pacman -Qm
And remove the ones you do not want.

* Packages can become orphans. You can remove them with
$ sudo pacman -Rsn $(pacman -Qqdt)

* Configuration files may change. Most changes are harmless to most users, but users should know that there are ways of understanding how they change https://wiki.manjaro.org/index.php?title=Pacnew_and_Pacsave_Files

* Permissions can differ.
