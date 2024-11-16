
# GSoC and Open Source Guide

This repository contains two key resources to help you get started: a PDF presentation with all the essential information about Google Summer of Code (GSoC), including guidance on applying, selecting projects, and succeeding in the program, and a comprehensive Git guide that covers the setup process, key commands, and GitHub terminology.

# Guide to get started with Git
This guide will help you set up Git for the first time and walk you through the most commonly used Git commands with explanations and examples.


## Step 1: Install Git
1. **Download Git**:  
   - Visit [git-scm.com](https://git-scm.com/) and download Git for your operating system.
2. **Install Git**:  
   - Follow the installation wizard and configure options (use defaults if unsure).

3. **Verify Installation**:  
   ```bash
   git --version
   ```
   - This command displays the installed Git version.



## Step 2: Configure Git
Before using Git, set your username and email address (these are attached to your commits):

1. Set your username:  
   ```bash
   git config --global user.name "Your Name"
   ```
2. Set your email:  
   ```bash
   git config --global user.email "your.email@example.com"
   ```

3. Check your configuration:  
   ```bash
   git config --list
   ```
   - This shows all your Git configuration settings.



## Step 3: Initialize a Repository
1. Navigate to your project folder:  
   ```bash
   cd /path/to/your/project
   ```
2. Initialize Git in the folder:  
   ```bash
   git init
   ```
   - This creates a `.git` directory to track your project's version history.



## Step 4: Important Git Commands

### 1. Add Files to Staging Area
**Why**: Stage changes before committing them.  
```bash
git add <file>       # Stage a specific file
git add .            # Stage all changes in the current directory
```

### 2. Commit Changes
**Why**: Save a snapshot of your staged changes.  
```bash
git commit -m "Your commit message"
```

### 3. Check Repository Status
**Why**: See which files are staged, modified, or untracked.  
```bash
git status
```

### 4. View Commit History
**Why**: See a list of previous commits.  
```bash
git log
```

### 5. Connect to a Remote Repository
**Why**: Link your local repository to a remote one (e.g., on GitHub).  
```bash
git remote add origin <repository-url>
```

### 6. Push Changes to Remote Repository
**Why**: Upload commits to the remote repository.  
```bash
git push origin <branch-name>   # First push
git push                  # Subsequent pushes
```

### 7. Pull Changes from Remote Repository
**Why**: Sync your local repository with the latest changes from the remote.  
```bash
git pull
```

### 8. Create a New Branch
**Why**: Work on features independently without affecting the main branch.  
```bash
git branch <branch-name>      # Create a branch
git checkout <branch-name>    # Switch to the branch
```

### 9. Merge Branches
**Why**: Combine changes from one branch into another.  
```bash
git checkout main
git merge <branch-name>
```

### 10. Undo Changes
**Why**: Revert uncommitted changes.  
```bash
git checkout -- <file>   # Discard changes in a file
git reset HEAD <file>    # Unstage a file
```

### 11. Clone a Repository
**Why**: Create a local copy of a remote repository.
```bash
git clone https://github.com/user/repository.git
```


## Step 4: Important GitHub Terms
### Repository
A repository is a storage space for your project, including all files and version history.

### Commit
A commit is a snapshot of changes made to a repository. Each commit has a unique ID and an associated message.
```bash
git commit -m "Added feature"
```

### Pull Request (PR)
A Pull Request (PR) is a request to merge changes from one branch into another. It allows others to review and discuss the proposed changes before integrating them.

### Fork
A fork is a personal copy of someone else's repository. It allows you to experiment with changes without affecting the original repository.

### Stage (Staging)
Staging means preparing files for a commit. You add files to the staging area using git add.

### Branch
A branch represents an independent line of development. Branches allow you to work on different features or fixes without affecting the main codebase.
```bash
git checkout -b new-feature
```

### Merge
Merging integrates changes from one branch into another. This is commonly done via Pull Requests.

### Checkout
Checkout switches to a different branch or commit.
```bash
git checkout new-feature
```


## Cheat Sheet of Commands

| **Command**          | **Purpose**                                   | **Example**                                      |
|-----------------------|-----------------------------------------------|-------------------------------------------------|
| `git init`           | Initialize a Git repository                   | `git init`                                      |
| `git add .`          | Stage all changes                             | `git add .`                                     |
| `git commit -m ""`   | Save changes with a message                   | `git commit -m "Added new feature"`            |
| `git status`         | Check repo status                             | `git status`                                    |
| `git log`            | View commit history                           | `git log`                                       |
| `git remote add`     | Link to remote repository                     | `git remote add origin <repo-url>`             |
| `git push`           | Upload changes to remote repo                 | `git push -u origin main`                      |
| `git pull`           | Download changes from remote repo             | `git pull`                                      |
| `git branch`         | Create or view branches                       | `git branch <branch-name>`                     |
| `git checkout`       | Switch to a branch                            | `git checkout <branch-name>`                   |
| `git merge`          | Merge another branch into the current branch  | `git merge <branch-name>`                      |

---

## Why Use Git?
- **Track Changes**: See how your code evolves over time.
- **Collaboration**: Work with others without overwriting their changes.
- **Backup**: Keep your code safe on remote repositories like GitHub.
- **Version Control**: Revert to earlier versions when needed.

This setup and command list will help you get started with Git confidently!
