### Github Commands - Cheat Sheet
### Miracle Innovation Labs
### Authors: Bhanu Kandregula || Shrikar Schonkar

<br/>


#### 01. Configure your Git user name
> - git config --global user.name

</br>

#### 02. Configure your Git email id
> - git config --global user.email

</br>

#### 03. This is for line endings to save space and extra chars
> - git config --global core.autocrlf true 
> - git config --global core.autocrlf input

</br>

#### 04. This is to set color to default
> git config --global color.ui auto

</br>

#### 05. To display all the branches available
> git branch -a

</br>

#### 06. Log history.
> git log 

</br>

#### 07. Add the specific file to staging area
> git add <filename>

</br>

#### 08. Add all files in current directory to staging area
> git add .

</br>

#### 09 Commit the repo on to github.
##### Note: Commit doesn't work without description.
> git commit -m "nice description here for the repo"

</br>

#### 10. Check out the differences in files before they staged.
> git diff

</br>

#### 11. Check out the differences in files after the files are staged.
> git diff --staged

</br>

#### 12. This will get you the most recent commit in the history
> git diff HEAD

</br>

#### 13. This will get the differences in color. 
> git diff --color-words

</br>

#### 14. East to read report of small changes to long lines.
> git diff --word-diff

</br>

#### 15. This will just give you the file names that are changed.
> git diff --stat

</br>

#### 16. Find out all the commits history with logs.
> git log

</br>

#### 17. Here is the quick summary of commits in single lines.
> git log --oneline

</br>

#### 18. To check what files were involved in each commit
> git log --stat

</br>

#### 19. To check what content actually changed between each commit.
> git log --patch

</br>

#### 20. To get the summary of the commit messages and also the difference output.
> git log --patch --oneline

</br>

#### 21. Get the graph of commits structure.
> git log --graph
> git log --graph --all --decorate --oneline

</br>

#### 22. To delete a single file, also stages the fact that file is deleted. Checkout the status of the repo as well.
> git rm <file-name>
> git status

</br>

#### 23. To list out the deleted files that are in staged now.
> git add -u .

</br>

#### 24. Leave the file in the file system, but don't let git track the file anymore. Keep it igroned.
> git rm --cached <filename>
> git status

</br>

#### 25. Move the files, make sure all files involved should be in the version control - staged.
> git mv source destination
ex: git mv test.txt levelone/test.txt

</br>

#### 26. Check out the deleted and moved files.
> git add -A .
> git log -stat --filename

</br>

#### 27. Get the list of ignored files.
> git ls-files --others --ignored --exclude-standard

</br>

#### 28. Creating a new branch.
> git branch new-branch-name

</br>

#### 29. Change to newly created branch to commit.
> git checkout branch-name

</br>

#### 30. Deleting a branch.
##### Note: We can't delete the branch we are on. You will fall :P
> git branch -D branch-name

</br>

#### 31. List out the available branches.
> git branch

</br>

#### 32. Rewritten the working tree from specific commit - Detatched HEAD state.
> git checkout <commit-id>
> git branch

</br>

#### 33. Come back to current branch from Detatched HEAD. we can't do any commits in HEAD state.
> git checkout new-brach

</br>

#### 34. Create a brnach and checkout to it in a single step.
> git checkout -b new-branch-name

</br>

#### 35. Merge the branches
> git checkout master
> git branch
> git merge <branch-name>
> git log

</br>

#### 36. Clean up your directory from last commit of your current branch.
##### Note: This will cleanup the staging area as well.
> git merge --abort

</br>

#### 37. Get all the commits of a specific branch.
> git merge --squash <target-branch-name>

</br>

#### 38. List out commits that happened.
> git log --online --graph --decorate --all -10

</br>

#### 39. Delete the specific branch.
> git branch -d <branch-name>

</br>

#### 40. Adding a git remote.
> git remote add origin https:####github.com/<user-name>/<repo-name>.git

</br>

#### 41. Edit the assigned remote uri.
> git remote set-url origin https:github.com/<user-name>/<repo-name>.git

</br>

#### 42. Delete the remote.
> git remote rm origin

</br>

#### 43. Get the list of remotes.
> git remote -v

</br>

#### 44. Get the list of branches with their respective remotes.
> git branch -r 

</br>

#### 45. Fetch the remote.
> git fetch remote

</br>

#### 46. Pull the remote.
> git pull origin

</br>

#### 47. Push the local repo to github.
> git push origin

</br>

#### 48. Reflog keeping track of commits that are made and also that are discarded.
> git reflog
> git config gc.reflogexpireunreachable 30

</br>

#### 49. Git Rebase is the ability to take existing commits, and place them on the branch that starts new.
> git checkout new-branch
> git rebase master

</br>

#### 50. Clone specific  branch from git repo.
> git clone -b <branch-name> <master-repo-name>

</br>

#### 51. Push he repo to specific repo
> git push origin <branch-name>

</br>

#### 52. To get the origin URL
> git remote get-url origin








