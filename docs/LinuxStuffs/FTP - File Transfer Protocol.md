- Check for `ftp` using the command `rpm -qa | grep ftp`
- Install `vsftpd` using the command `dnf install vsftpd` in Fedora/RHEL based distros
- Edit the `vsftpd.conf` file using `vim /etc/vsftpd/vsftpd.conf`
- Find the following lines and make the changes as shown below,
	1. **Disable anonymous login** 
		1. `anonymous_enable=NO`
	2. Uncomment
		1. `ascii_upload_enable=YES`
		2. `ascii_download_enable=YES`
	3. Uncomment -Enter your welcome message(Optional)
		1. `ftpd_banner=Welcome to UNIXMEN FTP services`
	4. Add at the end of this file
		1. `use_localtime=YES`
- `systemctl start vsftpd`
- `systemctl enable vsftpd`
- `systemctl stop firewalld`
	- TIP : Instead of stopping the `firewalld`, we can allow for the default port 21 in the `firewalld` 
- `systemctl disable firewalld`
- Install FTP client on the client server using `dnf install ftp`

## Commands to transfer files
1. `ftp ip_addr`
2. Enter username and password
3. `bin`
4. `hash`
5. `put fileName`
6. `bye`

