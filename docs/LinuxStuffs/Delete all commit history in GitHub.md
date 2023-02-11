# Delete all commit history in GitHub 
Source : [StackOverflow](https://stackoverflow.com/questions/13716658/how-to-delete-all-commit-history-in-github)
!!! warning 
	Deleting the `.git` folder and initializing a new repository may cause problems in the git repository. 

To deleete all the commit history but keep the code in current state, follow the steps below. 

1. Checkout 
``git checkout --orphan latest_branch``
2. Add all files 
`git add -A`
3. Commit the changes
`git commit -am "commit message"`
4. Delete the branch 
`git branch -D main`
5. Rename the current branch to main
`git branch -m main`
6. Force update the repository
`git push -f origin main`
7. Housekeeping 
`git gc --aggressive --prune=all`

