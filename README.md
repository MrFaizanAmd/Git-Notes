# Git

Git is the free and open source distributed version control system that's responsible for everything GitHub related that happens locally on your computer.

# Git Commands

- Git Cheat Sheet
    
    [git-cheat-sheet-education.pdf](git-cheat-sheet-education.pdf)
    

## Clone from Repository to Local Device

### FIRST SETUP

Configuring user information used across all local repositories.

1. Set User Name :
    
    ```visual-basic
    git config --global user.name “firstname lastname”
    ```
    
2. Set User Email :
    
    ```visual-basic
    git config --global user.email “valid email”
    ```
    
3. Check Configurations :
    
    ```visual-basic
    git config --list
    ```
    
4. Set Color UI : ( Optional )
    
    ```visual-basic
    git config --global color.ui auto
    ```
    

### SETUP & CLONE

Configuring user information, initializing and cloning repositories.

- Clone Repository :
    
    ```visual-basic
    git clone [url]
    ```
    

### STAGE & SNAPSHOT

Working with snapshots and the Git staging area.

1. Check Status :
    - **Git Changed Status :**
        1. **Untracked** : New files that Git doesn’t yet track.
        2. **Modified** : Changed in file.
        3. **Staged** : File ready to be committed.
        4. **Unmodified** : Unchanged in file.
    
    ```visual-basic
    git status
    ```
    
2. Add Files :
    
    ```visual-basic
    git add [filename]
    ```
    
    ```visual-basic
    git add .
    ```
    
3. Reset to Unstaged : ( If you want )
    
    ```visual-basic
    git reset [filename]
    ```
    
    ```visual-basic
    git reset .
    ```
    
4. Check Change not Staged :
    
    ```visual-basic
    git diff
    ```
    
5. Check Staged not Committed :
    
    ```visual-basic
    git diff --staged
    ```
    
6. Git Commit Snapshot :
    
    ```visual-basic
    git commit -m “descriptive message”
    ```
    
7. Show Commits History :
    
    ```visual-basic
    git log
    ```
    
8. Reset to Previous Commit : ( If you want )
    
    ```visual-basic
    git reset HEAD~1
    ```
    
9. Reset to Any Previous Commit : ( If you want )
    
    ```visual-basic
    git reset [commit hash]
    ```
    
10. Hard Reset to Any Previous Commit : ( If you want )
    
    ```visual-basic
    git reset --hard [commit hash]
    ```
    

### SHARE & UPDATE

1. Push to GitHub :
    
    ```visual-basic
    git push -u origin main
    ```
    
    ```visual-basic
    git push [alias] [branch]
    ```
    
    ```visual-basic
    git push
    ```
    
2. Pull from GitHub :
    
    ```visual-basic
    git pull [alias] [branch]
    ```
    

## Connect from Local Device to Repository

### FIRST SETUP

Configuring user information used across all local repositories.

1. Set User Name :
    
    ```visual-basic
    git config --global user.name “firstname lastname”
    ```
    
2. Set User Email :
    
    ```visual-basic
    git config --global user.email “valid email”
    ```
    
3. Check Configurations :
    
    ```visual-basic
    git config --list
    ```
    
4. Set Color UI : ( Optional )
    
    ```visual-basic
    git config --global color.ui auto
    ```
    

### SETUP & INIT

Configuring user information, initializing and cloning repositories.

- Create Repository :
    
    ```visual-basic
    git init
    ```
    

### STAGE & SNAPSHOT

Working with snapshots and the Git staging area.

1. Check Status :
    - **Git Changed Status :**
        1. **Untracked** : New files that Git doesn’t yet track.
        2. **Modified** : Changed in file.
        3. **Staged** : File ready to be committed.
        4. **Unmodified** : Unchanged in file.
    
    ```visual-basic
    git status
    ```
    
2. Add Files :
    
    ```visual-basic
    git add [filename]
    ```
    
    ```visual-basic
    git add .
    ```
    
3. Reset to Unstaged : ( If you want )
    
    ```visual-basic
    git reset [filename]
    ```
    
    ```visual-basic
    git reset .
    ```
    
4. Check Change not Staged :
    
    ```visual-basic
    git diff
    ```
    
5. Check Staged not Committed :
    
    ```visual-basic
    git diff --staged
    ```
    
6. Git Commit Snapshot :
    
    ```visual-basic
    git commit -m “descriptive message”
    ```
    
7. Show Commits History :
    
    ```visual-basic
    git log
    ```
    
8. Reset to Previous Commit : ( If you want )
    
    ```visual-basic
    git reset HEAD~1
    ```
    
9. Reset to Any Previous Commit : ( If you want )
    
    ```visual-basic
    git reset [commit hash]
    ```
    
10. Hard Reset to Any Previous Commit : ( If you want )
    
    ```visual-basic
    git reset --hard [commit hash]
    ```
    

### SHARE & UPDATE

Retrieving updates from another repository and updating local repos.

1. Add a Git URL :
    
    ```visual-basic
    git remote add [alias] [url]
    ```
    
    - **Check Status :**
        1. Verify Remote :
            
            ```visual-basic
            git remote -v
            ```
            
        2. Check Branch :
            
            ```visual-basic
            git branch
            ```
            
2. Remove Remote : ( If you want )
    
    ```visual-basic
    git remote remove [alias]
    ```
    
3. Show Remote :
    
    ```visual-basic
    git remote
    ```
    
4. Show Remote Origin :
    
    ```visual-basic
    git remote -v
    ```
    
5. Change Branch Name :
    
    ```visual-basic
    git branch -m main
    ```
    
    ```visual-basic
    git branch -M main
    ```
    
6. Push to GitHub :
    
    ```visual-basic
    git push -u origin main
    ```
    
    ```visual-basic
    git push [alias] [branch]
    ```
    
    ```visual-basic
    git push
    ```
    
7. Pull from GitHub :
    
    ```visual-basic
    git pull [alias] [branch]
    ```
    

## Branch Commands

1. Check All Branch :
    
    ```visual-basic
    git branch
    ```
    
2. Change Branch Name :
    
    ```visual-basic
    git branch -m main
    ```
    
    ```visual-basic
    git branch -M main
    ```
    
3. Navigate Branch :
    
    ```visual-basic
    git checkout [branch name]
    ```
    
4. Create Branch :
    
    ```visual-basic
    git checkout -b [new branch name]
    ```
    
5. Delete Branch :
    
    ```visual-basic
    git branch -d [branch name]
    ```
    
6. Show Commits History :
    
    ```visual-basic
    git log
    ```
    

### Merge Branches

**WAY 1**

1. Compare Branches :
    
    ```visual-basic
    git diff [branch name]
    ```
    
2. Merge Branches :
    
    ```visual-basic
    git merge [branch name]
    ```
    

**WAY 2**

- Create Pull Request ( PR ) :
    
    Compare and Pull Request ( PR ) by GitHub Options Directly within Repository.
    

## Fork

1. A fork is a new repository that shares code and visibility settings with the original “upstream” repository.
2. Fork is a rough copy.
