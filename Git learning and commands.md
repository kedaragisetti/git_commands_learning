<h2>Getting started with GIT</h2>

- To get git version ```--git version```

1. Working Directory : The folder where you're working on your project 
2. Stage : My changes are ready they can move to the next step 
1. Local Repository : Temporary area where files sit between working directory and repository save.

> Git means we save our files locally


> Git hub is used when we want to share it with others or being backup online or to access it from another computer

- Git the local repository to the pulling to the Git hub means remote repository other words pulling it to the online cloud.

## Commands ---
**git clone** - To clone the local files to the online repository

**git status** - Check the changes made on the files.

**git add --all or -A** : to stage the every changes made to the files.

**git reset** : Resets all the changes made and reset to the old version or files.

**git add .** : Stage the changes within the current directory you're in.

**`git add *`** : It stages all the visible changes except for deleted files

- **git config --global user.email "Your email address"**

- **git config --global user.name "Your Name here"** 
- This will set both your name and email address globally

- **git commit -m "I have made some changes to files"**

**git rest HEAD~**  : It will reset all the committed or staged files back to the normal it was and again we can get back them by using **git add .**

**git reset**: Removes files from the staging area, returning them to the working directory without deleting the changes.

**git reset --hard**: Discards all uncommitted changes and reverts the repository to the state of the last commit.

### Branching and Merging

- git branch: Lists all local branches in the repository.
- git branch [name]: Creates a new branch with the specified name.
- git checkout [name]: Switches the current working directory to  the specified branch.
- git merge [branch]: Integrates changes from the specified branch into the current branch.

### **Viewing History and Comparing**
* **git log**: Shows the full commit history.
* **git log --oneline**: Displays a compact, single-line summary of commit history.
* **git diff [commit1] [commit2]**: Compares changes between two specific commits.

### **Remote Synchronization**
* **git clone [url]**: Creates a local copy of a remote repository.
* **git push**: Uploads local commits to a remote repository.
* **git fetch**: Downloads remote data without merging.
* **git pull**: Fetches and merges remote changes into the local branch.

### **File Management**
* **git rm [file]**: Deletes a file from both Git and the local filesystem.
* **git rm --cached [file]**: Removes a file from tracking but keeps it in your local folder.
* **git rm -r [folder]**: Recursively removes a folder and its contents.
* **git restore [file]**: Discards local changes to a file.

### **Advanced Utilities**
* **git stash**: Temporarily saves uncommitted work.
* **git stash list**: Shows the list of saved stashes.
* **git stash apply**: Restores stashed work without removing it from the stash list.
* **git stash pop**: Restores stashed work and removes it from the stash list.
* **git stash drop**: Manually removes a specific stash entry.
* **git revert [commit_id]**: Creates a new commit to undo the changes of a specific previous commit.
* **git rebase [branch]**: Reapplies commits on top of another branch for a linear history


Revert and rebase needs to be practiced again