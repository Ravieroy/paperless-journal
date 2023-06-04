Few(among many) commands to monitor users are, 

1. `who`
	1. tells us the name of the users who are currently logged in the system. 

2. `last`
	1. gives us a list of all the users who have previously(or currently) logged in the system. 
	2. useful for sysadmins who need to track user activity on a server.
	3. `last | awk '{print $1}' | sort | uniq` will give all the usernames who have logged in previously. 

3. `w`
	1. It is same as who but with more information like load usage, running session etc.

4. `finger` or `pinky`
	1. doesn't come preinstalled. 
	2. gives details of all the users logged in.
	3. provides details like login name, user name, idle time, login time, and in some cases their email address

5. `id`
	1. used to confirm the identity of a specified Linux user.
	2. to find user and group names, along with the UID and GID of any user in Linux


