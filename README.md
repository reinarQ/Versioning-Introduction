# Git and GitHub
## INTRODUCTION
### Git?
Git is software for tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing source code during software development. 
Its goals include speed, data integrity, and support for distributed, non-linear workflows.
### GitHub?
GitHub is a web-based hosting service for software development projects that use the Git revision control system.

## SETUP
### Installing Git
1. Browse to the official Git website: https://git-scm.com/downloads
2. Click the download link for Windows and allow the download to complete.
3. Run the installation Wizard
4. Launch Git Bash after completing the installation process
### Creating GitHub account
1. Go to https://github.com/join.
2. Fill out the form.
3. Click Create account.
4. Verify your email address & logging in
### Creating new repositry in GitHub
1. Log-in to your GitHub account 
2. Click on the plus symbol in the upper right
![new repository] (repository.png)
3. Select 'new repository'
4. Fill in the form and create new repository
### Cloning repository
Open Git and type following command:
git clone followed by the url of the repository

## Git CHEATSHEET

### 1. Configuring user information used across all local repositories

##### *git config --global user.name “[firstname lastname]”* :
set a name that is identifiable for credit when review version history
##### *git config --global user.email “[valid-email]”* :
set an email address that will be associated with each history marker
##### *git config --global color.ui auto* :
set automatic command line coloring for Git for easy reviewing

### 2. Configuring user information, initializing and cloning repositories

#### *git init* :
initialize an existing directory as a Git repository
#### *git clone* [url] :
retrieve an entire repository from a hosted location via URL

### 3. Working with snapshots and the Git staging area

#### *git status* : 
show modified files in working directory, staged for your next commit
#### *git add [file]* : 
add a file as it looks now to your next commit (stage)
#### *git reset [file]* : 
unstage a file while retaining the changes in working directory
#### *git diff* :
diff of what is changed but not staged
#### *git diff --staged* :
diff of what is staged but not yet committed
#### *git commit -m “[descriptive message]”* :
commit your staged content as a new commit snapshot

### 4. Isolating work in branches, changing context, and integrating changes

#### *git branch* :
list your branches. a * will appear next to the currently active branch
#### *git branch [branch-name]* :
create a new branch at the current commit
#### *git checkout* :
switch to another branch and check it out into your working directory
#### *git merge [branch]* :
merge the specified branch’s history into the current one

### 5. Examining logs, diffs and object information

#### *git log* :
show the commit history for the currently active branch
#### *git log branchB..branchA* :
show the commits on branchA that are not on branchB
#### *git log --follow [file]* :
show the commits that changed file, even across renames
#### *git diff branchB...branchA* :
show the diff of what is in branchA that is not in branchB
#### *git show [SHA]* :
show any object in Git in human-readable format

### 6. Versioning file removes and path changes

#### *git rm [file]* :
delete the file from project and stage the removal for commit
#### *git mv [existing-path] [new-path]* :
change an existing file path and stage the move
#### *git log --stat -M* :
show all commit logs with indication of any paths that moved

### 7. Retrieving updates from another repository and updating local repos

#### *git remote add [alias] [url]* :
add a git URL as an alias
#### *git fetch [alias]* :
fetch down all the branches from that Git remote
#### *git merge [alias]/[branch]* :
merge a remote branch into your current branch to bring it up to date
#### *git push [alias] [branch]* :
Transmit local branch commits to the remote repository branch
#### *git pull* :
fetch and merge any commits from the tracking remote branch



