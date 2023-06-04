## Special permissions with *setuid*, *setgid* and *sticky bit*
- There are 3 additional permissions in Linux 
	- *setuid :* bit tells Linux to run a program with the effective user id of the owner instead of the executor. (e.g. `passwd` command). We can check by running the command `ls -l /usr/bin/passwd` which will give the output similar to `.rwsr-xr-x. root root 32 KB Fri Jul 22 08:22:29 2022  /usr/bin/passwd`
	- *setgid : bit tells Linux to run a program with the effective group id of the owner instead of the executor. (e.g. `locate` or `wall` command)
	- *sticky bit :*  A bit set on files/directories that allows only the owner or root to delete those files.
- To assign special permissions at the user level
	- `chmod u+x fileName.sh`
- To assign special permissions at the group level
	- `chmod g+x fileName.sh`
- To remove special permissions at the user or group level
	- `chmod u-x fileName.sh`
	-  `chmod g-x fileName.sh`
- To find all executables in Linux with *setuid* and *setgid*
	- `find / -perm /6000 -type f`

!!! Note 
	These bits work on c programming executables, not on bash shell scripts.

- *sticky bit :* It is assigned to the last bit of permissions (e.g. `/tmp` directory)
	- `-rwx rwx rwt`
