## Quick setup
For any [[Linux distros]] the quick setup steps can be found [here](https://flatpak.org/setup/). Following steps are for Debian/Ubuntu based distros. 

### Step 1: Install Flatpak
```ad-note
For Ver. 18.10 and higher. For older versions Official Flatpak PPA can be installed.
```
```bash
sudo apt install flatpak
```

### Step 2: Install the Software Flatpak plugin
The Flatpak plugin for the Software app makes it possible to install apps without needing the command line. To install, run:
```bash
sudo apt install gnome-software-plugin-flatpak
```

### Step 3: Add the Flathub repository
Flathub is the best place to get Flatpak apps. To enable it, run:
```bash
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Finally restart the system. 