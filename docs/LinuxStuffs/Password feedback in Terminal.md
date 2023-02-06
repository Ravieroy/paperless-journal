## Enable Password Feedback in Terminal
!!! Warning

***In order to enable the well known asterisk behavior while typing the password in [[Terminal]], sudoers file needs to be edited, so be very careful while following the steps. 
Make sure the sudo version is 1.8.31 or above.***

**Step 1 : Check sudo version**
Older sudo versions have been known to have [exploit](https://www.sudo.ws/security/advisories/pwfeedback/) which can be used to grant sudo privileges to any normal user. This has been fixed in version 1.8.31 and hence it is to be made sure that before proceeding ahead, sudo is the right version. 
```bash 
sudo --version
```

**Step 2 : Only use [[visudo]] command to edit the sudoers file**

Type the following in [[Terminal]] which will open up the typical sudoer file in `vi` editor which is similar to [[Vim]]. 
```bash
sudo visudo
```

**Step 3 : Add the necessary line**
```text
Defaults        pwfeedback
```
The file would look similar to this, 
![[visudo.png]]

**Step 4: Save, exit and restart the [[Terminal]] session**
After the above line is added,simply save and exit using `:wq` command and restart the terminal session(i.e., close this terminal and start again). DONE
