[[SSH]] Secure Shell Protocol is a cryptographic protocol for secure data connection and remote command execution. By default, we need to type in our passwords everytime we wamt to login, but it is possible to set up a passwordless login. 

## 1. Check if SSH is running.
We can check if the ssh is already running typing the following command in the [[Terminal]]
```bash
systemctl status ssh
```

In Fedora, we need to use, 

```bash
systemctl status sshd
```

If the service is not running(i.e. active), run the following command to start the ssh service : 
```bash
sudo systemtcl start sshd
```

!!! tip
	Make sure that you are able to login via normal password authentication way.

## 2. Generate private and public keys

In our local machine, a key pair must be created with the command : 
```bash 
ssh-keygen
```

Press _Enter_ three times until the command finishes. A public key file “**_~/.ssh/id_rsa.pub”_** and a private key file “**_~/.ssh/id_rsa”_** will be generated.

## 3. Copy the public key file to the remote machine

Now that we have generated an SSH key pair, in order to be able to login to our machine without a password we need to copy the public key to the server. Use the following command to do that,

```bash
ssh-copy-id remote_username@remote_server_ip_address
```

## 4. Login to your server. 

Once above steps are done, we can login using the command `ssh remote_username@remote_server_ip_address`. Also it is possible to setup [[Custom SSH connections]] to login easily. 

