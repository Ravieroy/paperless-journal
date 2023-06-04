`ps` command stands for process status and it displays all the current running process in the Linux shell.

### Basic Syntax

```bash
List all running processes:

      ps aux

  List all running processes including the full command string:

      ps auxww

  Search for a process that matches a string:

      ps aux | grep string

  List all processes of the current user in extra full format:

      ps --user $(id -u) -F

  List all processes of the current user as a tree:

      ps --user $(id -u) f

  Get the parent PID of a process:

      ps -o ppid= -p pid

  Sort processes by memory consumption:

      ps --sort size
```

The output of `ps` in [[Terminal]] returns, 

- **PID :** the unique process ID.

- **TTY :** [[Terminal]] type that the user logged-in to.

- **TIME :** The amount of CPU in minutes and seconds that the process has been.

- **CMD :** name of the command.

### Other Examples
1. Show all the running processes
```bash
ps -e
```

2. Show all running processes in BSD format
```bash
ps aux
```

3. Show all running processes in the full-listing format
```bash
ps -ef
```

4. Show all processes by the user
```bash
ps -u userName
```

