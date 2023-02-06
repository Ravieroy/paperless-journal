==Brightnessctl only works as root==

Check to make sure you have [the right udev rules installed](https://github.com/Hummer12007/brightnessctl/blob/master/90-brightnessctl.rules). The udev rules are found at `/usr/lib/udev/rules.d/90-brightnessctl.rules`. If it is fine, try adding yourself to the video group. I think this is necessary for light as well. REBOOT is neccesary. 

```bash
sudo gpasswd -a <user_name> video
```
