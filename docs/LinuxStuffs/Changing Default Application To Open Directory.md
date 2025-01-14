???+ note
	How to prevent VS Code from being the default application for opening a directory in Linux


The OS chooses an application when opening a file (directory is a special file type, called inode/directory, in this case) is called "Default applications".

The OS determines the default application by reading the configuration from several files:

- `$HOME/.config/mimeapps.list`
- `/usr/share/applications/mimeinfo.cache`
- `$HOME/.local/share/applications/mimeinfo.cache`

### 1. Check the default application for a specific file type
```bash
xdg-mime query default "inode/directory"
```
This will return the name of the application which is the default application for opening directories. 

For the list of all available options to choose from, use
```bash
gio mime inode/directory
```

OR, 

```bash
cat /usr/share/applications/mimeinfo.cache | grep "inode/directory"
```

The output would be something like, 

```bash
Registered applications:
	kitty-open.desktop
	org.kde.dolphin.desktop
	org.kde.filelight.desktop
	org.kde.gwenview.desktop
	org.kde.kate.desktop
	pcmanfm.desktop
Recommended applications:
	kitty-open.desktop
	org.kde.dolphin.desktop
	org.kde.filelight.desktop
	org.kde.gwenview.desktop
	org.kde.kate.desktop
	pcmanfm.desktop
```

### 2. Change the default application 

Inorder to override the default  edit a local configuration file `~/.config/mimeapps.list`.  Edit or create the above file if it doesn't exist and add the following line in the config file

```text
[Default Applications]
inode/directory=org.gnome.Nautilus.desktop;code.desktop;
```


[Source](https://transang.me/intelij-prevent-open-file-directory-with-vscode/)

DONE!!