An environment variable is a dynamic-named value that cam affect the way running process will behave on a computer. They are a part of the environment in which a process runs. For example, each user in an operating system has its own environment. An admin user has a different environment than other users do.

- To view all environment variables : `printenv` or `env`
- To view ONE environment variable : `echo $envName` for e.g., `echo $SHELL`
- To set the environment variables temporarily : 
	- `export TEST=1`
	- `echo $TEST`
- To set the environment variable permanently 
	- Open the shell config file, for e.g., `.bashrc` in [[Terminal]] or any text editor and place the environment variable there. Then source the config file by `source .bashrc` or restart the shell environment with updated config file by `exec bash`
	- Example : 
		1. `vim .bashrc` then add the following lines.
		2. `TEST=1`
		3. `export $TEST`
- To set the global environment variable permanently make the similar process as above in the file `/etc/profile` or `/etc/bashrc`


