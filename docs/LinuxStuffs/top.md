- `top` command is used to show the Linux process and it provides a real-time view of the running system
- This command shows the summary of information of the system and list of processes or threads which are currently managed by the Linux Kernel.
- When the `top` command is executed then it goes into interactive mode and we can exit by pressing **q**

### Basic Syntax

```bash
Start top:

      top

  Do not show any idle or zombie processes:

      top -i

  Show only processes owned by given user:

      top -u username

  Sort processes by a field:

      top -o field_name

  Show the individual threads of a given process:

      top -Hp process_id

  Show only the processes with the given PID(s), passed as a comma-separated list. (Normally you would not know PIDs off hand. This example picks the PIDs from the process name):

      top -p $(pgrep -d ',' process_name)

  Get help about interactive commands:

      ?
```

The output of `ps` in [[Terminal]] returns, 

- **PID :** shows task's unique process ID

- **USER :** username of the owner of the task

- **PR :** shows the scheduling priority of the process from the perspective of kernel

- **NI :** represents the *Nice Value* of the task. A negative value implies higher priority.

- **VIRT :** total virtual memory used by the task.

- **RES :** memory consumed by the process in RAM

- **SHR :** represents the amount of shared memory used by the task.

- **S :** this field shows the process state in the single-letter form

- **%CPU :** CPU usage 

- **%MEM :** memory usage of the task

- **TIME+ :** CPU time

### Other Examples 

1. Shows tasks by username 
```bash
top -u userName
```

2. Show commands absolute path : `top` then press **c**
3. Kill a process by PID within the session : `top` then pres **K**
4. Sort all Linux running commands by memory usage : `top` then M and P