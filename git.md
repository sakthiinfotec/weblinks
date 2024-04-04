#### Git Concepts
 - Working Directory
 - Staging Area
 - Local Repository
 - Remote Repository

#### Git Init & Config
```sh
git init

# Config scopes
# -------------
# Sytem - All users
# Global - User level but for all the repositories
# Local - Only to a particular repository

git config --global user.name "Sakthi"
git config --global user.name sakthi@gmail.com

# Set Visual code as default editor
git config --global core.editor "code --wait"

# To edit config via editor
git config --global -e

git config --global core.autocrlf input # or true (for Windows)

git config --help
git config -h
```

#### Git Clone
```sh
git clone https://github.com/sakthiinfotec/marsrover.git
git remote -v

# To show current branch
git branch

# To list all the available branches
git branch -a

# Create and checkout a branch - develop
git branch develop
git checkout develop

# Create and checkout a branch - develop in single step
git checkout -b develop

git pull -r
```

#### Git Status
```sh
# Short Status
git status -s

# List files in staging area
git ls-files

git rm index.html

# To unstage - index.html file
git rm --cached index.html

# To remove already stagged file or folder
git rm --cached bin/
git rm --cached -r bin/ # recursive

# Add files or folder in .gigignore to ignore from Git to track 
code .gitignore

# Rename file name using git command
git mv severe.js server.js
```

#### Git Diff
- To view difference between 2 commits. By default it will show a difference between current working directory and HEAD commit.

```sh
# Changes between Working Dir vs Stagged
git diff

# Changes between Stagged vs Committed
git diff --staged

# Configure difftool settings
git config --global diff.tool "vscode"
git config --global difftool.vscode.cmd "code --wait --diff $LOCAL $REMOTE"

git difftool
git difftool --staged
```

#### Git Commit
```sh
# Add file to the staging area
git add index.html
git add bin/*.sh app/*.js

git commit -am "User sign in validation added"

git merge <source-branch> <target-branch>

# Change to target branch
git checkout qa
git merge develop qa

# Delete unwanted branch
git branch -a
git branch -d qa

```

#### Git branch
```sh
# Rename a branch
git branch -m old-name new-name

```

#### Git Push/Pull to or from Remote Repository
```sh
git push origin master

# Pul from remote repository(-r)
git pull -r

# Set/Change remote URL (for both Push and Pull)
git remove set-url origin https://github.com/sakthiinfotec/monitorr.git

# Update Push only 
git remove set-url --push origin https://github.com/sakthiinfotec/marsrover.git

# Update Pull/Fetch alone
git remove set-url --fetch origin https://github.com/sakthiinfotec/marsrover.git

# Push an existing repository
git push -u origin master
```

#### Git log
```sh
# View git logs
git log
git log --oneline

git log --since='Jul 28 2023' --author="developer@company.com" --pretty=format:"%h %ad %s"  --date=short

git show <commig id / HEAD pointer>
git show HEAD
git show HEAD~1 # One step back to HEAD commit

# To see commit details of any particular file
git show HEAD~1:bin/start.sh

git ls-tree HEAD~2 # To see all the files and directories in the commit
```

#### Git reset
To point the HEAD to a particular commit position
- Sort (`--soft # This is default and recommended`)
- Hard (`--hard # not recommended as it will also remove data in the working directory`)

```sh
git reset HEAD~2 # or explicit with --soft like below
git reset --soft HEAD~2

git reset --hard HEAD~1
```

#### Git revert
Revert or Delete change/commit

```sh
git revert <commit id>

# Suppose commit id 003e45ab is last 2nd, last and last 3rd changes will be there but last 2nd alone will be reverted/deleted
# It will reverte the changes and automatically add a commit
git revert 003e45ab

# This will not add another commit automatically but need to commit revert changes
git revert 003e45ab --no-commit
```


#### Git Restore
```sh
git restore --staged server.js # Reset staged file with last commited content

# To reset changes in local working directory
git restore .

# To restore lwd including newly added/untracked files (-f Force; -d Directory)
git clean -fd

# Restore from last commit
git restore --source=HEAD~2 bin/start.sh
```


#### Git Rebase/Cherry Pick
- Rebase: Merging sequence of commits to a specified target branch
- Cherry pick: picking a particular commit alone
```sh
git rebase feature develop

# Go to target branch first and then cherry pick
git checkout develop

git cherry-pick <commit id>
git cherry-pick 02ae45d
```

#### Git Stash and Patch
- Stash: Reverts the changes made
```sh
git stash
git stash list

# Stash and push the changes with comment
git stash push -m "Search term filter in search bar"

# Apply a particular stashed changes to the current branch
git stash apply |  git stash apply stash@{0}
git stash apply stash@{0}

# Pop and apply the last pushed changes
git stash pop 
git stash pop 0 # Pop out a specific stash and returns a stash commit hash
git stash apply [stash_commit_hash]

# Apply stashed changes to a new branch
git branch [branch_name] [stash_commit_hash]
git branch ps-2321 a93aef24a93aef24a93aef24a93aef24a93aef24
git checkout ps-2321

# Apply latest stash
git stash apply stash@{0}

# Drop a stashed changes
git stash drop stash@{0}

# Drop all the stashes
git stash clear

# Move stashed changes to a new branch
git stash branch push-notification stash@{0}
git checkout -b new-feature stash@{0}

# To stash the output into a patch file
git stash show -p stash@{<number>} > <name>.patch
git stash show -p stash@{0} > fcm-changes.patch
git stash show -p --color=never > my-patch-name.patch 

# Info about both saving the patch and applying binary data
git stash show stash@{0} -p --binary

# Get Patch info
git apply --stat my-patch-name.patch   # Verify if patch looks good
git apply --check my-patch-name.patch  # Valide if patch does not have any errors

# Generate patch from diff
git diff > some-changes.patch
git diff --staged path/to/file # Diff between a file in current working directory and the one in staged area

# Apply a patch to the current branch
git apply my-patch-name.patch
curl https://example.com/file-0.0.1.diff | git apply 

# Apply a patch of the reverse diff
git diff commit2 commit1 > some-changes.patch
git apply -R some-changes.patch
```

#### Git Merge and Resolve Conflicts
- Merge and resolve conflicts

Step 1: From local project, bring in the changes
```sh
git fetch origin
git checkout -b filter-fixes origin/filter-fixes
git merge develop
```

```sh
# OR follow other way, because merge conflicts when mergin to develop branch
git pull origin develop
git status # To list modified & conflict files

# Merge the conflich manually, commit and push to remote
vi app/server.js
git add .
git push origin develop
```

Step 2: Merge the changes and update on the remote repository
```sh
git checkout develop
git merge --no-ff filter-fixes
git push origin develop
```


##### Guides
[Git and GitHub - The Complete Guides - Chapter 1: Git Started](https://dev.to/ifierygod/git-and-github-the-complete-guides-chapter-1-23cp)  
