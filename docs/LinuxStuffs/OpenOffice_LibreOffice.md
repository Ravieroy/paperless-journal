## Possible Cause of the Error 
*OpenOffice and LibreOffice have similar dependencies and sometimes they clash with each other, hence both cannot be installed simultaneously. Even after the removal of the LibreOffice, it might be that there is a clash somewhere which can cause the following error.* 

```bash 
The following packages have unmet dependencies:
libreoffice-core : Depends: libreoffice-common (> 1:6.0.3) but it is not going to be installed
libreoffice-java-common : Depends: libreoffice-common (= 1:6.0.3-0ubuntu1) but it is not going to be installed
libreoffice-ogltrans : Depends: libreoffice-common but it is not going to be installed
libreoffice-report-builder : Depends: libreoffice-common (= 1:6.0.3-0ubuntu1) but it is not going to be installed
libreoffice-script-provider-bsh : Depends: libreoffice-common (= 1:6.0.3-0ubuntu1) but it is not going to be installed
libreoffice-script-provider-js : Depends: libreoffice-common (= 1:6.0.3-0ubuntu1) but it is not going to be installed
libreoffice-script-provider-python : Depends: libreoffice-common (= 1:6.0.3-0ubuntu1) but it is not going to be installed
libreoffice-style-galaxy : Depends: libreoffice-common (= 1:6.0.3-0ubuntu1) but it is not going to be installed
libreoffice-style-tango : Depends: libreoffice-common (= 1:6.0.3-0ubuntu1) but it is not going to be installed
E: Unmet dependencies. Try 'apt --fix-broken install' with no packages (or specify a solution).
```


The first thing to try is `sudo apt --fix-broken install` and then `sudo apt purge libreoffice*`

It might or might not work and return the following error 

```bash
Unpacking libreoffice-common (1:6.0.3-0ubuntu1) ...
dpkg: error processing archive /var/cache/apt/archives/libreoffice-common_1%3a6.0.3-0ubuntu1_all.deb (--unpack):
trying to overwrite '/usr/bin/soffice', which is also in package openoffice-debian-menus 4.1.5-9789
rmdir: failed to remove '/var/lib/libreoffice/share/prereg/': No such file or directory
rmdir: failed to remove '/var/lib/libreoffice/share/': No such file or directory
rmdir: failed to remove '/var/lib/libreoffice/program/': No such file or directory
rmdir: failed to remove '/var/lib/libreoffice': No such file or directory
rmdir: failed to remove '/var/lib/libreoffice': No such file or directory
Errors were encountered while processing:
/var/cache/apt/archives/libreoffice-common_1%3a6.0.3-0ubuntu1_all.deb
E: Sub-process /usr/bin/dpkg returned an error code (1)

purge returns:

E: Unable to locate package libreoffice-common_1%3a6.0.3-0ubuntu1_all.deb
E: Couldn't find any package by glob 'libreoffice-common_1%3a6.0.3-0ubuntu1_all.deb'
E: Couldn't find any package by regex 'libreoffice-common_1%3a6.0.3-0ubuntu1_all.deb'
```


This is a kind of catch22 situation here. If you have [[Synaptic]] package manager then you can go there to remove all the instances of OpenOffice. 

## The Fix 
`sudo dpkg -P openoffice-debian-menus`

Then

`sudo apt --fix-broken install`

*This will fix the issue but you won't be able to run OpenOffice. It will show in the searches but won't work. The best way is to now install [[Synaptic]] and remove all the OpenOffice instances and install LibreOffice*

