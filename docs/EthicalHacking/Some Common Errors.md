### 1. Unable to enumerate USB device under virtualbox.

1. [Download the extension pack](https://download.virtualbox.org/virtualbox/7.0.2/Oracle_VM_VirtualBox_Extension_Pack-7.0.2.vbox-extpack)
	1. Open your file manager and double-click on the file that should be named something like Oracle_VM_VirtualBox_Extension_Pack-7.0.0.vbox-extpack. When you double-click that file, VirtualBox 7.0 will automatically open and install the extension pack for you.
2. Add user to vboxusers group
	1. For your user to do a number of things with VirtualBox, it must be a member of the vboxusers group.
	2. Open a [[Terminal]] window and issue the command:`sudo usermod -aG vboxusers $USER`
	3. Log out of the desktop and log back in.
3. Add specific USB device
	1. Open settings from the virtual box main screen. 
	2. Settings > USB
	3. Select USB 3.0 from the menu.
	4. Add your device from the USB device filters

Useful Links : 
1. [How to Add a USB Device to VirtualBox on Windows](https://www.makeuseof.com/windows-virtualbox-add-usb/)
2. [How to fix the VirtualBox USB enumeration error and extension pack installation | TechRepublic](https://www.techrepublic.com/article/fix-virtualbox-usb-error/)
### 2. SIOCSIFFLAGS: Operation not permitted and SIOCSIFHWADDR: Operation not permitted

This error happens when we want to disable a device like `wlan0` (changing the MAC address). Simply use the `sudo` command to do that and it will work.
```bash
sudo ifconfig eth0 up/down
sudo ifconfig wlan0 up/down
```

