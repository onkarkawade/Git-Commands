
# 🧠 Git Essentials – Cheatsheet & Guide

This guide covers essential Git commands categorized by functionality. It is designed for developers who want a quick reference or to strengthen their understanding of Git workflows.



![git-flow-768x513](https://user-images.githubusercontent.com/14274827/91470661-9d5a8780-e8b2-11ea-9ccb-0d813d2e35d1.png)



# 📋 1. Configuration
### Set global username and email for commits
```
git config --global user.name "YourName"
git config --global user.email "yourname@example.com"
```
# 📁 2. Initialize & Clone Repositories
### Initialize a new Git repository
```
git init
```
### Undo initialization
```
rm -rf .git
```

### Clone a repository (default branch)
```
git clone git@github:user/repo.git  # To clone only skeleton of repo
git lfs clone git@github:user/repo.git # To clone file with all data
```

### Clone a specific branch
```
git clone -b branch_name git@github:user/repo.git
```
# 🌐 3. Remote Repositories

### Push all branches
```
git push --all
```

# 📝 4. Adding & Committing Changes
### Add specific file
```
git add filename.py
```
### Add all files
```
git add .
```
### Commit with message
```
git commit -m "Initial commit"
```
# 🔍 5. Status & Logs
### Show current status of files
```
git status
```
### View commit history
```
git log
```
# 🔀 6. Branching & Switching
### List branches
```
git branch
```
### Create a new branch
```
git branch new_feature
```
### Switch to a branch
```
git checkout dev
```
### Create and switch to new branch
```
git checkout -b new_branch
```
### Delete a branch
```
git branch -d unwanted_branch
```
# 🚀 7. Push & Pull
### Push changes to remote
```
git push origin branch_name
```
### Push a new branch and set upstream
```
git push -u origin new_branch
```
### Pull updates and merge
```
git pull origin branch_name
```
# 📊 8. Comparing Changes
### Compare working directory with index
```
git diff
```
### Compare two branches
```
git diff branch_1 branch_2
```
# ♻️ 9. Revert & Reset
### Revert a specific commit (safe)
```
git revert <commit_hash>
```
### View commit history in short form
```
git log --oneline
```
#### ✅ git revert creates a new commit to undo changes without altering history (preferred for public/shared repos).

# 🔀 10. Merging Changes
### Merge another branch into the current branch
```
git merge branch_to_merge
```

# 💾 11. Stash – Save Temporary Work
### Stash changes (including untracked)
```
git stash -u
```
### Bring back stashed changes
```
git stash pop
```
### 📌 Bonus Tip
To exit a message editor (like after git revert):

Press Shift + Q (for exiting less)

Type :q and press Enter (for exiting vi or vim)

### 📁 Optional: File Structure (for this README repo)
```
git-cheatsheet/
│
├── README.md        ← This file
└── .gitignore       ← Optional: ignore sensitive or auto-generated files
```
