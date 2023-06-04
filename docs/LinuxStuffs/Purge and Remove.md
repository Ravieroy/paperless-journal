## Difference between purge and remove
**remove** - remove is identical to install except that packages are removed instead of installed. Note that removing a package leaves its configuration files on the system. If a plus sign is appended to the package name (with no intervening space), the identified package will be installed instead of removed.

**purge** - purge is identical to remove except that packages are removed and purged (any *configuration files are deleted too*).

==This does not apply to packages that hold configuration files inside the user's home folder (e.g. /home/UserName), these files will not be touched.==
