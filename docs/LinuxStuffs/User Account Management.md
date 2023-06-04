Important commands 

1. useradd

2. groupadd

3. userdel

4. groupdel

5. usermod 

Important Files
1. /etc/passwd

2. /etc/group

3. /etc/shadow

Examples
```bash
useradd spiderman
```

The above command creates a user spiderman and by default a group called spiderman as well. The newly created user is a part of its own group.  We can create a new group as well in the similar manner, 
```bash 
groupadd avengers
```

Now we can add spiderman to the avengers group as well using the command `usermod`
```bash
usermod -G avengers spiderman
```

!!! tip
	The above command will add the user to avengers group but it will still be part of its own group spiderman. To change that, use `chgrp -R avengers spiderman`


The command `userdel` and `groupdel` is used to delete the group. We can check for the information about the users using the command,
```bash
cat /etc/passwd
```

The complete command to create a user. 
```bash
useradd -g avengers -s /bin/bash -c "avengers character" -m -d /home/spiderman spiderman
```

Finally once the user is created, we need to create a password for the user. We can do that by following command.
```bash
sudo passwd spiderman
```