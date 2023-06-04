- `kill` command is used to terminate a process manually. It sends a signal which ultimately terminates or kills a particular process or group of processes. 

### Usage
Syntax

```bash
kill [OPTION] [PID]
```

```bash
Terminate a program using the default SIGTERM (terminate) signal:

      kill process_id

  List available signal names (to be used without the `SIG` prefix):

      kill -l

  Terminate a background job:

      kill %job_id

  Terminate a program using the SIGHUP (hang up) signal. Many daemons will reload instead of terminating:

      kill -1|HUP process_id

  Terminate a program using the SIGINT (interrupt) signal. This is typically initiated by the user pressing `Ctrl + C`:

      kill -2|INT process_id

  Signal the operating system to immediately terminate a program (which gets no chance to capture the signal):

      kill -9|KILL process_id

  Signal the operating system to pause a program until a SIGCONT ("continue") signal is received:

      kill -17|STOP process_id

  Send a `SIGUSR1` signal to all processes with the given GID (group id):

      kill -SIGUSR1 -group_id
```

### Most used signals 

To get list of all signal names or signal number, use the command `kill -l`. 

- `kill PID` : Kill a process with  a default signal 

- `kill -1` : Restart 

- `kill -2` : Interrupt from keyboard (like Ctrl C)

- `kill -9` : Forcefully kill the process

- `kill -15` : Kill a process gracefully.

### Other similar kill commands 

- `killall` :  kills the processes and its child processes as well.

- `pkill`
