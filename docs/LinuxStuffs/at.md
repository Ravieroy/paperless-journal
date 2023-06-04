The `at` command is a Linux command-line utility used to schedule a job for later execution. The utility reads commands from standard input and groups them into an at job, which executes only once. The alternative for `at` is a [[crontab]]. However, while `at` jobs execute only once, cron jobs are recurring events.

```bash
Open an `at` prompt to create a new set of scheduled commands, press `Ctrl + D` to save and exit:

      at hh:mm

  Execute the commands and email the result using a local mailing program such as Sendmail:

      at hh:mm -m

  Execute a script at the given time:

      at hh:mm -f path/to/file

  Display a system notification at 11pm on February 18th:

      echo "notify-send 'Wake up!'" | at 11pm Feb 18
```

### Some Examples 

1. Schedules an **`echo`** command invocation five minutes after scheduling the job
```bash
echo "hello" | at now +5 minutes
```

2. schedules an `echo` command invocation at 5PM
```bash
echo "hello" | at 5PM
```

3. View the scheduled job
```bash
atq
```

4. Remove a Scheduled Job
```bash
atrm ID # ID can be known from atq command first column
```

### Useful Links 
1. [How to Use the Linux at Command](https://phoenixnap.com/kb/linux-at-command)

