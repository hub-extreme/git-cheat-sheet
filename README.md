## Overview
This cheat sheet provides essential Git commands for managing your code base. Use these commands to commit changes, manage branches, and synchronize with remote repositories.

## Key Concepts
- **Commit**: A snapshot of your code base.
- **Branch**: A separate line of development.
- **Tag**: A marker for specific commits.
- **HEAD**: The current state of your working directory.

## 1. Git Configuration
Set up your identity:
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global color.ui auto
```

## 2. Starting a Project
Initialize or clone a repository:
```bash
git init [project_name]     # Initialize a new repo
git clone <project_url>     # Clone a remote repo
```

## 3. Day-to-Day Work
Check status and manage files:
```bash
git status                   # Show current status
git add [file]               # Stage changes
git commit -m "message"      # Commit changes
git diff [file]              # Show changes in working dir
```

## 4. Branching
Manage branches for parallel development:
```bash
git branch                   # List branches
git branch [branch_name]     # Create a new branch
git checkout [branch_name]   # Switch to a branch
git merge [branch_name]      # Merge a branch into the current one
```

## 5. Synchronizing Repositories
Fetch and push changes:
```bash
git fetch [remote]           # Fetch changes from remote
git pull [remote]            # Fetch and merge changes
git push [remote] [branch]   # Push changes to remote
```

## 6. Tagging Commits
Create and manage tags:
```bash
git tag                      # List tags
git tag [name]               # Create a tag
git tag -a [name]            # Create an annotated tag
```

## 7. Undoing Changes
Revert or reset changes:
```bash
git reset [file]             # Unstage a file
git revert [commit_sha]      # Create a new commit that undoes changes
```

## 8. Ignoring Files
Use `.gitignore` to exclude files:
```plaintext
# Create .gitignore
logs/
*.tmp
!.gitkeep
```

## Practice Commands
### Create a Repository
```bash
git init my_project
cd my_project
```

### Make Changes
```bash
touch file1.txt
echo "Hello World" > file1.txt
git add file1.txt
git commit -m "Initial commit"
```

### Create and Switch Branches
```bash
git branch feature-x
git checkout feature-x
```

### Merge Changes
```bash
git checkout main
git merge feature-x
```

### Tag a Release
```bash
git tag -a v1.0 -m "Release version 1.0"
```

## Resources
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)