# Manage user profiles
There are two major ways you can do this: Graphical User Interface and Command [[Terminal]].

## Using CLI
### Creating a user

**Step 1:** Open your command Terminal using either from Applications menu or using shortcuts (Ctrl+Alt+T or Win+T). The syntax to add a user on Linux is: 
`sudo useradd -m \<name of the user\>` So say you have to add Ravi as a user, 
```bash
sudo useradd -m ravi
```

**Step 2 :** Set a password for the user
The syntax to set a password for the user is: `sudo passwd \<username\>`
```bash
sudo passwd ravi
```

**Step 3 (optional) :** Provide sudo privilege (*to be done if you want the user to have sudo privileges. This will work in Debian-based distros. You should look up if you have a different distro.*)
```bash
sudo usermod -a -G sudo ravi
```

### Delete a user
The syntax to delete a user is `sudo userdel <username>`
```bash
sudo userdel -r ravi
```
---

## Using GUI
Head over to *settings > users*. Most probably the settings would be locked by default. Click on unlock and enter your password.

![[manage_user_1.png]]

Once you have done that, you should see this.

![[manage_user_2.png]]

Just click on Add user. Here you can now add your username and password. You can select if the user is a standard or administrator. You can set the password now or in the next login. Once you do that, you can easily log out and log in as a newly created user.

![[manage_user_3.png]]

!!! tip

You can go into the same settings > users section and see the remove user icon at the bottom. Just use that to delete the user.

---
