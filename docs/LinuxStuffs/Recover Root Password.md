!!! warning 
	This is not well written as of now. It is just a set of instruction which might be clear to advanced users only.

Inorder to recover the root password we need to login into system in rescue mode. This is only possible if we have physical access to the device. 

1. Restart the computer in rescue mode
The grub menu appears during the restart, and only for a very short time, and hence we need to be vigilant to get that screen. Once the grub menu appears, press **e** to edit the selection, which is the name of our Linux. 

2. 
	1. edit where `ro` is written to `rw init=/sysroot/bin/sh` and press CTRL-X
	2. `chroot /sysroot`
	3. `passwd root`
	4. Before exiting update selinux information by running the command `touch /.autorelabel`
	5. `exit`
	6. `reboot`

![[edit-mode-1.png]]

Also see [[14-Recover+Root+Password.pdf]]
