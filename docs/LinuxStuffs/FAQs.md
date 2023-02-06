
- **What's the easiest way to tell if my Linux system is 32-bit or 64-bit?**

You can simply use the following.
```bash
lscpu | grep -i architecture  
```
If you want a lot of information about your system, then simply do `lscpu`

---

- **What command should you run to see the computer name and Linux version?**

If you want what brand of computer you use along with other information. Remember, you need to have sudo password for this.
```bash
sudo dmidecode | grep -A3 '^System Information'
```

For Linux Version.
```bash
hostnamectl | grep -i "Operating System"
```

OR,
```bash
cat /proc/sys/kernel/hostname
```

---
- **Which keyboard command will delete the text from the cursor to the beginning of the line on Linux?**

***Command Terminal*** :

- Ctrl + u : delete from cursor to the start of the command line

***Some more useful commands*** 

- Ctrl + k : delete from cursor to the end of the command line
- Ctrl + w : delete from cursor to start of word. To delete backwards one word
- Ctrl + y : paste word or text that was cut using one of the deletion shortcuts.

---
