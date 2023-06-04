- Background : Ctrl + z, `jobs` and `bg`
- Foreground : `fg`
- Run process even after exit : `nohup process &` or `nohup process > /dev/null 2>&1 &`
- Kill a process by name = `pkill`
- Process priority : `nice`
	- The niceness scale goes from -20 to 19. The lower the number, more priority the that task gets. 
- Process monitoring : [[top]]
- List process :  [[ps]]

1. `jobs`
```bash
View jobs spawned by the current shell:

      jobs

  List jobs and their process IDs:

      jobs -l

  Display information about jobs with changed status:

      jobs -n

  Display process ID of process group leader:

      jobs -p

  Display running processes:

      jobs -r

  Display stopped processes:

      jobs -s
```

2. `bg`
```bash
Resume the most recently suspended job and run it in the background:

      bg

  Resume a specific job (use `jobs -l` to get its ID) and run it in the background:

      bg %job_id
```

3. `nohup`
```bash
Run a process that can live beyond the terminal:

      nohup command argument1 argument2 ...

  Launch `nohup` in background mode:

      nohup command argument1 argument2 ... &

  Run a shell script that can live beyond the terminal:

      nohup path/to/script.sh &

  Run a process and write the output to a specific file:

      nohup command argument1 argument2 ... > path/to/output_file &
```

4. `pkill`
```bash
Kill all processes which match:

      pkill "process_name"

  Kill all processes which match their full command instead of just the process name:

      pkill -f "command_name"

  Force kill matching processes (can not be blocked):

      pkill -9 "process_name"

  Send SIGUSR1 signal to processes which match:

      pkill -USR1 "process_name"

  Kill the main `firefox` process to close the browser:

      pkill --oldest "firefox"
```

5. `nice`
```bash
Launch a program with altered priority:

      nice -n niceness_value command
```

---

### Useful Links 
1. [[Process Commands]]



