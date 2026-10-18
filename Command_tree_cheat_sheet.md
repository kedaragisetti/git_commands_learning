# 🌳 Git Command Tree & Cheat Sheet

## 1. Setup & Basics
- `git --version`  
  → Check installed Git version.
- `git init`  
  → Initialize a new repository in the current folder.
- `git clone <url>`  
  → Copy a remote repository to your local machine.

---

## 2. File Operations
- `git status`  
  → Show current changes, staged files, and branch info.
- `git add file.txt`  
  → Stage a file for commit.  
- `git add .`  
  → Stage all files in the folder.
- `git commit -m "Message"`  
  → Save staged changes with a message.
- `git rm file.txt`  
  → Remove a file from repo and stage deletion.

---

## 3. Branching
- `git branch`  
  → List all branches.
- `git branch new-feature`  
  → Create a new branch.
- `git checkout new-feature`  
  → Switch to another branch.  
- `git switch new-feature`  
  → Alternative to checkout for switching.
- `git branch -d branchname`  
  → Delete a branch locally (safe).  
- `git branch -D branchname`  
  → Force delete branch locally.  
- `git push origin --delete branchname`  
  → Delete branch from remote (GitHub).

---

## 4. Remote Operations
- `git remote add origin <url>`  
  → Link local repo to a remote (GitHub).
- `git push origin main`  
  → Upload commits to remote branch.
- `git fetch`  
  → Download changes from remote without merging.
- `git pull origin main`  
  → Fetch + merge changes from remote branch.

---

## 5. Viewing History
- `git log`  
  → Show commit history.
- `git log --oneline`  
  → Compact commit history.
- `git diff`  
  → Show differences between working files and last commit.
- `git diff file.txt`  
  → Show differences for a specific file.

---

## 6. Undo & Reset
- `git restore --staged file.txt`  
  → Unstage a file (remove from staging area).
- `git restore file.txt`  
  → Discard changes in working file.
- `git reset --hard <commit_id>`  
  → Reset repo to a specific commit (dangerous, discards changes).

---

## 7. Advanced
- `git revert <commit_id>`  
  → Create a new commit that undoes a previous commit.
- `git rebase main`  
  → Reapply commits from current branch on top of `main`.
- `git merge feature`  
  → Merge another branch into current branch.

---

## 8. Collaboration
- **Pull Request (PR)**  
  → Not a Git command, done via GitHub/GitLab UI.  
  Steps:  
  1. Push your branch: `git push origin feature`  
  2. Go to GitHub → “Compare & pull request”  
  3. Submit PR for review.

---

## 🌟 Quick Workflow Example
```bash
git init
git add .
git commit -m "Initial commit"
git branch feature
git checkout feature
git push origin feature
