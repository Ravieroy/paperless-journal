`crontab` command is used to schedule tasks. Crontab stands for Cron Table. This is a Linux system file that creates a table-like structure where fields are separated by white space. Users can populate the table by assigning values to each field (asterisk).

![[crontab-syntax.png]]


!!! tip
	Use absolute path for the script when making the crontab entry. 


### Usage
```bash
Edit the crontab file for the current user:

      crontab -e

  Edit the crontab file for a specific user:

      sudo crontab -e -u user

  Replace the current crontab with the contents of the given file:

      crontab path/to/file

  View a list of existing cron jobs for current user:

      crontab -l

  Remove all cron jobs for the current user:

      crontab -r

  Sample job which runs at 10:00 every day (* means any value):

      0 10 * * * command_to_execute

  Sample crontab entry, which runs a command every 10 minutes:

      */10 * * * * command_to_execute

  Sample crontab entry, which runs a certain script at 02:30 every Friday:

      30 2 * * Fri /absolute/path/to/script.sh

```

### Additional Cron Jobs

- by default there are 4 different types of cronjobs
	- Hourly
	- Daily
	- Weekly
	- Monthly

- All the above crons are setup in, `/etc/cron.<directory>`

- The timing for each are set in, `/etc/anacrontab` except hourly. 

- For Hourly, `/etc/cron.d/0hourly`

We can put our script in their respective directories and let cron handle them on timely basis. 
