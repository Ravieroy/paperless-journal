[[Git]] is a is a version control system that lets us manage and keep track of our source code history. It can be used to manage files locally as well. GitHub on the other hand is a cloud-based hosting service that lets us manage Git repositories. It is found in almost all the [[Linux distros]] and can be downloaded from distro repository.

Once we have Git on our system, we need to do a few things to customize our Git environment. We have to do these things only once on any given computer. 

## 1. Setup our Identity

The first thing we should do when we install Git is to set our user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits we start creating:

```bash
git config --global user.name "UserName"
$ git config --global user.email johndoe@example.com
```

## 2. Setup Editor 
Now that our identity is set up, we can configure the default text editor that will be used when Git needs us to type in a message. If not configured, Git uses our system’s default editor.

If we want to use a different text editor, such as Emacs, we can do the following:

```bash
git config --global core.editor vim
```

We can check the changes that has been made by, 
```bash
git config --list
```

Now, we are done. We can start adding and pushing files to GitHub. 

## 3. (Optional) Permanently authenticating with Git repositories

Run the following command to enable [credential caching](https://help.github.com/articles/caching-your-github-password-in-git/#platform-linux)

Globally( for all repositories)
```bash 
git config --global credential.helper credential.helper store
git config --global credential.helper 'cache --timeout 7200'
```

After this, we have to make one git push with password and then for 7200 seconds(2hrs), we do not have to enter password(token) manually.  

!!! tip 
	We should also specify **caching expire**. Requiring to login once a day could be a reasonable idea. 


