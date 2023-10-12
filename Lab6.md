# Lecture Note on Git - It is essential to use a version control system for software development!
## Changes vs Snapshots
### **Changes**
  Storing data as changes to the base version
  ![IMG_7B9D93E1A305-1](https://github.com/H0JunP/reppopotamus/assets/134226638/97d5486c-dc3c-4210-babb-e0bca99f6039)

### **Snapshots**
  Storing data as snapshots  
  ![IMG_F088C1EE5022-1](https://github.com/H0JunP/reppopotamus/assets/134226638/1bd04c53-a5b2-49a3-8d55-b1d0aa154dda)
---
## Local, Centralized, and Distributed Version Control
![IMG_79A4733A8E1A-1](https://github.com/H0JunP/reppopotamus/assets/134226638/e4081a1a-4afe-4250-9fa2-bcb59f31ff7d)
---
## 3 States in Git - Modified, Staged, Commited
![IMG_61664031DCF1-1](https://github.com/H0JunP/reppopotamus/assets/134226638/9cefbf43-f547-4559-93ab-02186282b063)
---
## **Checking/Installing Git**
### Checking already installed git
  Command is all same on Windows/Linux/MacOS
  ```sh
  $ git --version
  git version [your installed version]
  ```
### Installing Git
  #### Linux (Debian Distro)
  ```sh
  # sudo apt install git-all
  ```
  #### MacOS
  [Visit git-scm](https://git-scm.com/download/mac)
  #### Windows (Run "Git Bash")
  [Visit git-scm](https://git-scm.com/download/win)
---
## Git config: First-time Setup
  **Git configurations are stored in three levels**
  1. System Level: --system option. Affects all uses and repositories on the system (administrative)
  2. Global (User) Level: --gloval option. Affects all repositories of a current user
  3. Local Level: --local option. Specific to the current repository

  ***Each level overrides values in the previous level: system > global > local***
---
## Initializing a repository in an existing directory
  ```sh
  $ git init
  ```
---
## Checking repository status
  ```sh
  $ git status
  ```
---
## Adding a new file to be staged (tracked)
  ```sh
  $ git add [file name]
  ```
---
## Unstaging a file
  ```sh
  $ git rm -cached [file name]
  ```
---
## Commit
  ```sh
  $ git commit -m "commit message"
  ```
---
