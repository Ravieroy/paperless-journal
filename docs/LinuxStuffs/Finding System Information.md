1. To see the release version of the operating system `cat /etc/os-release`
	1. Fedora : `cat /etc/fedora-release`
	2. Redhat : `cat /etc/red-release`

2. Uname prints information about the machine and operating system it is run on.

```bash
Print all information:

      uname --all

  Print the current kernel name:

      uname --kernel-name

  Print the current network node host name:

      uname --nodename

  Print the current kernel release:

      uname --kernel-release

  Print the current kernel version:

      uname --kernel-version

  Print the current machine hardware name:

      uname --machine

  Print the current processor type:

      uname --processor

  Print the current operating system name:

      uname --operating-system
```

3. `dmidecode` : Display the DMI (alternatively known as SMBIOS) table contents in a human-readable format.  Requires root privileges.

```bash
Show all DMI table contents:

      sudo dmidecode

  Show the BIOS version:

      sudo dmidecode -s bios-version

  Show the system serial number:

      sudo dmidecode -s system-serial-number

  Show BIOS information:

      sudo dmidecode -t bios

  Show CPU information:

      sudo dmidecode -t processor

  Show memory information:

      sudo dmidecode -t memory
```