- `rsync` is a utility for efficiently transferring and synchronizing files within the same computer or to a remote computer by comparing the modification times and sizes of files. 
- It is lot faster than [[FTP - File Transfer Protocol]] or [[SCP - Secure Copy Protocol]]
- This utility is mostly used to backup the files and directories from one server to another.
- Default `rsync` port = 22 (Same as [[SSH]])

## Some common options used with rsync commands

- **-v** : verbose
- **-r** : copies data recursively (but don’t preserve timestamps and permission while transferring data.
- **-a** : archive mode, which allows copying files recursively and it also preserves symbolic links, file permissions, user & group ownerships, and timestamps.
- **-z** : compress file data.
- **-h** : human-readable, output numbers in a human-readable format.

## Examples and Syntax

1. Transfer a file from local to a remote host
`rsync path/to/local_file remote_host:path/to/remote_directory`

2. Transfer a file from a remote host to local
`rsync remote_host:path/to/remote_file path/to/local_directory`

3. Copy/Sync Files and Directory Locally
`rsync -zvh fileName /path/to/backup_directory`
`rsync -avzh /path/to/local_directory /path/to/backup_directory`

4. Sync Over SSH
`rsync -avzhe ssh root@192.168.0.141:/root/anaconda-ks.cfg /tmp`

5. Use of `–include` and `–exclude` Options
These two options allow us to **include** and **exclude** files by specifying parameters with these option helps us to specify those files or directories which you want to include in your sync and exclude files and folders with you don’t want to be transferred.

Here in this example, the `rsync` command will include those files and directory only which starts with ‘**R**’ and exclude all other files and directory.

`rsync -avze ssh --include 'R*' --exclude '*' root@192.168.0.141:/var/lib/rpm/ /root/rpm`

6. Do a Dry Run with `rsync`
`rsync --dry-run --remove-source-files -zvh backup.tar.gz root@192.168.0.151:/tmp/backups/`
