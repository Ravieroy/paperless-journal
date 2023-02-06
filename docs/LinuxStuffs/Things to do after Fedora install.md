# Things to do after Fedora install
---

## DNF Configuration 
Open the config file for dnf using your desired editor using `sudo` privileges. Here I will be using [[Vim]] editor. You can use [[nano]] or most preferably [[gedit]] which is a GUI based text editor. 

```bash 
sudo vim /etc/dnf/dnf.conf
```

Then add the follow lines in the config file:

```text
# Added for speed
fastestmirror=True
max_parallel_downloads=10
defaultyes=True
keepcache=True
```
To know about above options, read the official documentation [here](https://dnf.readthedocs.io/en/latest/conf_ref.html)

Then *save and exit*. After this, you should see faster updates. 

**If you want to clean the cache, just do**

```bash
sudo dnf clean all
```

## System Update

It is nice to update your dnf config you just edited in the last step. 
```bash
sudo dnf update
```

## RPM Fusion 
It provides software programs that Fedora doesn't provide by default. Read more about this [here](https://rpmfusion.org/RPM%20Fusion). In the [link,](https://rpmfusion.org/Configuration) you can read how to do this by GUI as well. For command line you can type

```bash
sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
```

In order to install these non-free packages from graphical [[Package manager]] do the following. 
```bash
sudo dnf groupupdate core
```

## Adding Flathub

Fedora ships with [[flatpak]] by default, but this is a stripped down version of it. We need to enable flathub. 

```bash
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Now you can see in your GUI the option to install the [[flatpak]] packages. 

## Change hostname
When you open the terminal, you would see something in this format `username@hostname`. We can change the hostname of the new installation.

```bash
sudo hostnamectl set-hostname new-name
```
Now you can reboot to see the changes take effect. 

## Add media codecs 
RPM Fusion repositories also provide a lot of complement packages which is neccessary. 
```bash
sudo dnf groupupdate multimedia --setop="install_weak_deps=False" --exclude=PackageKit-gstreamer-plugin
```
and,

```bash
sudo dnf groupupdate sound-and-video
```
## Few more apps
A few more apps can be installed from graphical [[Package manager]] for customizability.
- Gnome Tweaks 
- Extensionssudo dnf groupupdate sound-and-videosudo dnf groupupdate sound-and-videosudo dnf groupupdate sound-and-video

---
