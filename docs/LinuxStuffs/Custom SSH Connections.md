[[SSH]] (SSH client) is a program for remotely accessing a machine, and can be easily installed from repositories. By default, users are authenticated in ssh using passwords, however, we can setup [[SSH Passwordless Login]] for easy access.

## SSH config  files
There is a default system-wide configuration file. It contains settings that apply to all users of ssh client machine. Here we will the user-specific/custom configuration file. located at `~/.ssh/config` or `$HOME/.ssh/config`. It has configurations that apply to a specific user. It therefore overrides default settings in the system-wide config file. This is the file we will create and use.

Usually `~/.ssh` directory already exists, but In case it does not exist on your desktop system, create it with the following permissions. 
```bash
mkdir -p ~/.ssh
chmod 0700 ~/.ssh
```

Now, we Create user specific SSH configuration file which is not created by defaut. We can use following command to create this file with proper permissions. 
```bash 
touch ~/.ssh/config
chmod 0700 ~/.ssh/config
```

The conventional format of `~/.ssh/config` is as follows, 
```bash
Host    host1
	ssh_option1=value1
	ssh_option2=value1 value2
	ssh_option3=value1 

Host    host2
	ssh_option1=value1
	ssh_option2=value1 value2

Host  *
	ssh_option1=value1
	ssh_option2=value1 value2
```

and, the syntax to login is then, 

```bash 
ssh host1
```

???+ note
	For more detailed and explanation visit [here](https://www.tecmint.com/configure-custom-ssh-connection-in-linux/)

## Working Example

Open the config file using any editor of choice. Here we are using [[Vim]] to do that. 
```bash 
vim ~/.ssh/config
```

and define the necessary sections as shown below in the config file. 

```bash
Host myfedora37
        HostName 192.168.56.15
        Port 22
        ForwardX11 no

Host myraspi
        HostName 192.168.56.10
        Port 22
        ForwardX11 no

Host myubuntu22
        HostName 192.168.56.5
        Port 2222
        ForwardX11 yes

Host *
        User raviroy
        IdentityFile ~/.ssh/id_rsa
        Protocol 2
        Compression yes
        ServerAliveInterval 60
        ServerAliveCountMax 20
        LogLevel INFO
```

- **HostName** – defines the real host name to log into, alternatively, you can use a numeric IP addresses, it is also permitted (both on the command line and in **HostName** specifications). 
	
- **User** – specifies the user to log in as.

The above values and the `Host host1` should be changed accordingly. We can add as many hosts as we want. 

Once that is done, we can login simply by typing in [[Terminal]]
```bash
ssh myfedora37 # to login into myfedora37
```

```bash
ssh myraspi # to login into myraspi
```

----
Source : [Configure Custom SSH Connections to Simplify Remote Access Tecmint](https://www.tecmint.com/configure-custom-ssh-connection-in-linux/)


