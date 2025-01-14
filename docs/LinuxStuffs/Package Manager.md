A package manager is a tool that allows users to install, remove, upgrade, configure and manage software packages on an operating system. The package manager can be a graphical application like a software center or a command line tool like [apt](https://ubuntu.com/server/docs/package-management) or [pacman](https://wiki.archlinux.org/title/pacman) and [dnf](https://docs.fedoraproject.org/en-US/quick-docs/dnf/).

## Quick Overview

### Fedora 

To search the repositories for a package type:
```bash
dnf search packagename
```

To check if the package exists:
```bash
rpm -qa | grep packagename
```

To install the package:
```bash
sudo dnf install packagename
```

To remove a package:
```bash
#using dnf
sudo dnf remove packagename

# using rpm
rpm -e packagename
```

To install from a `.rpm` file:
```bash
#using rpm
rpm -hiv packagename.rpm

#using dnf
sudo dnf install packagename.rpm
```

To verify package details and information:
```bash
rpm -qi packagename

#search for exact name if required using rpm -qa | grep packagename
```

To see the location of configuration files:
```bash
rpm -qc packagename
```

To check the package any particular command belongs to:
```bash
rpm -qf /path/to/command

#example
rpm -qf /usr/bin/pwd
```

Other common `dnf` commands 
-   `autoremove` - removes packages installed as dependencies that are no longer required by currently installed programs.
    
-   `check-update` - checks for updates, but does not download or install the packages.
    
-   `downgrade` - reverts to the previous version of a package.
    
-   `info` - provides basic information about the package including name, version, release, and description.
    
-   `reinstall` - reinstalls the currently installed package.
    
-   `upgrade` - checks the repositories for newer packages and updates them.
    
-   `exclude` - exclude a package from the transaction.

### Ubuntu 
To search the repositories for a package type:
```bash
apt search packagename
```

To install the package:
```bash
sudo apt install packagename
```

To remove a package:
```bash
sudo apt remove packagename
sudo apt purge packagename
```

Other common APT commands 
-   `autoremove` - removes packages installed as dependencies that are no longer required by currently installed programs.

-   `downgrade` - reverts to the previous version of a package.
    
-   `upgrade` - checks the repositories for newer packages and updates them.

-   `show` - Show information about the given package(s) including its dependencies, installation and download size, sources the package is available from, the description of the packages content and much more.

-   `update` - used to download package information from all configured sources.

-   `full-upgrade` - full-upgrade performs the function of upgrade but will remove   currently installed packages if this is needed to upgrade the system as a whole.

For more visit [Using apt Commands | itsfoss](https://itsfoss.com/apt-command-guide/). Also read [Difference Between apt and apt-get | itsfoss](https://itsfoss.com/apt-vs-apt-get-difference/)

### Arch
To search the repositories for a package type:
```bash
pacman -Ss packagename
```

To install the package:
```bash
sudo pacman -S packagename
```

To remove a package:
```bash
sudo pacman -R packagename #removes single package leaving dependencies
sudo pacman -Rs packagename # removes packages and its dependencies
```

Removes orphan packages 
```bash
pacman -Qdtq | pacman -Rs -
```

Upgrading packages 
```bash
pacman -Syu
```

Other common pacman commands
To search for already installed packages:
```bash 
pacman -Qs string1
```

To view the dependency tree of a package:
```bash
pactree packagename
```
For more about `pactree`, visit [pacman | geekdiary](https://www.thegeekdiary.com/pactree-command-examples-in-linux/). For getting started with pacman visit [itsfoss | pacman](https://itsfoss.com/pacman-command/).

