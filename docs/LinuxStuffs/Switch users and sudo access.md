- **Commands** 
	- `su` - username 
	- `sudo` command 
	- `visudo` (used to edit the sudoers file safely)
- **File** : /etc/sudoers 

```bash
## Allows people in group wheel to run all commands
wheel  ALL=(ALL)       ALL
```

If we want a user to be able to execute sudo command, we can add them in the `wheel` group using `usermod` command (see [[User Account Management]])
```bash
usermod -aG wheel userName
```

