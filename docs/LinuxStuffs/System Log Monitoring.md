The log files are stored in `/var/log`

1. `/var/log/boot.log` contains all the information while the system boots. It gets rewritten every time system reboots. In Fedora, the boot logs are written in `boot.log-yyyymmdd` format and last few logs are kept in the storage. 
2. `chrony`
3. `cron` or `cron-yyyymmdd` for logs on cron jobs.
4. `maillog` for mail related logs.
5. `secure` contains all login and logout activities.
6. `messages` store all global system activity data, including startup messages.