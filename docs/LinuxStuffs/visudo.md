## Linux visudo command
Read more at [Computer Hope](https://www.computerhope.com/unix/visudo.htm)
On Unix-like operating systems, the visudo command edits the sudoers file, which is used by the sudo command. To change what users and groups are allowed to run sudo, run visudo.

*One  should not edit sudoers directly*, by opening it in a text editor. Instead, *edit it with visudo*, which will *verify its validity before saving the changes to disk*.

```bash 
sudo visudo
```

- Visudo edits the sudoers file in a safe fashion, similar to the way that [[vipw]] safely edits the passwd file. 
- Visudo locks the sudoers file against multiple simultaneous edits, provides basic sanity checks, and checks for parse errors. 
- If the sudoers file is currently being edited by someone else, or by you in another session, you will receive a message to try again later.
- Visudo parses the sudoers file after the edit, and will not save the changes if there is a syntax error
- Upon finding an error, visudo prints a message stating the line number(s) where the error occurred and the *user will receive the "What now?*"
- At the prompt, *type e to re-edit the sudoers file*, *x to exit without saving the changes*, or *Q***(**NOT RECOMMENDED AT ALL**) to quit and save changes.

