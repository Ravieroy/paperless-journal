Git is widely used modern version control system originally developed in 2005 by Linus Torvalds. 

## 1. Install Git on Linux 

### Debian / Ubuntu (apt)

Type the following in the [[Terminal]]
```bash 
sudo apt update 
sudo apt install git
```

### Fedora(dnf)
```bash 
sudo dnf update 
sudo dnf install git
```

## 2. Configure Git username and email

Next we create our Git username and email which will be associated with any commits that we create later.

```bash 
git config --global user.name "Ravi Roy"
git config --global user.email "ravieroy123@gmail.com"
```

## 3. Important Git commands
### Basics
- `git init <directory>` : Create empty Git repo in specified directory. Run with no  
arguments to initialize the current directory as a git repository
- `git clone <repo>` : Clone repo located at `<repo>` onto local machine. Original repo can be located on the local filesystem or on a remote machine via HTTP or SSH. 
- `git add <directory>` : Stage all changes in `<directory>` for the next commit.  
Replace `<directory>` with a `<file>` to change a specific file.
- `git commit -m "<message>"` : Commit the staged snapshot, but instead of launching  
a text editor, use `<message>` as the commit message.
- `git status` : List which files are staged, unstaged, and untracked.
- `git log` : Display the entire commit history using the default format. 
- `git diff` : Show unstaged changes between your index and working directory.
- `git pull <remote>` : Fetch the specified remote’s copy of current branch and  
immediately merge it into the local copy.

### Undoing changes 
- `git revert <commit>` : Create new commit that undoes all of the changes made in  
`<commit>`, then apply it to the current branch.
- `git reset <file>` : Remove `<file>` from the staging area, but leave the working directory  
unchanged. This unstages a file without overwriting any changes.

### Branches 
- `git branch` : List all of the branches in your repo. Add a `branch` argument to  
create a new branch with the name `branch`
- `git checkout -b branch` : Create and check out a new branch named `branch`.  
Drop the -b flag to checkout an existing branch
- `git merge <branch>` : Merge `<branch>` into the current branch.

### Typical Workflow while working with remote repository
**Step 1** : Check status of what files are modified and added or deleted using `git status`

**Step 2 :** Add the files using `git add fileName` or the present working directory `git add .`

**Step 3** : Commit the files using `git commit -m "commit message"`

**Step 4** : Push the changes to GitHub repository by `git push`

For more detail, please refer to the [cheatsheet by Atlassian](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet), or read the PDF [here](./assets/SWTM-2088_Atlassian-Git-Cheatsheet.pdf). 

