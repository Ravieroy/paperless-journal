## Dolphin installation and theming in GNOME
^^***Installing dolphin is easy but since it is QT based app and GNOME uses mostly GTK, hence the theme do not exactly correlate. Hence, a few extra steps is required.***^^

**Step 1 : Install dolphin**
```bash
sudo apt install dolphin
```

Now it can be run simply by searching for `dolphin`, although the theme would be light. So if light theme is desired then the work is done here. Follow below to activate dark theme.

**Step 2: Install qt5ct**
```bash 
sudo apt install qt5ct
```

This app manages the theming for qt-based app. It can be run graphically just by searching `qt5ct` but it will complain about environment issues which we will resolve now. Follow this [answer](https://unix.stackexchange.com/questions/502722/dolphin-background-and-font-color-are-both-white/660222#660222) for more details

**Step 3 : Set environment**

Using desired text editor such as [[Vim]] open the environment file in /etc directory using [[Terminal]]. `sudo` privilege is required to edit the file. 

```bash 
sudo vim /etc/environment
```

Add the following line in the file 

```text
QT_QPA_PLATFORMTHEME='qt5ct'
```

**Restart the system for the changes to take effect and then open the `qt5ct` and make the changes according to choice.**

***Choose kvantum-dark with any icon theme, like pop or Infinity-dark-icons***
