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

git pull -r
```

#### Git Status
```sh
# Short Status
git status -s

# List files in staging area
git ls-files

git rm index.html

# To remove already stagged file or folder
git rm --cached bin/
git rm --cached -r bin/ # recursive

# Add files or folder in .gigignore to ignore from Git to track 

git mv severe.js server.js
```

#### Git Diff

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
# Add file to staging area
git add index.html
git add bin/*.sh app/*.js

git commit -am "User signin validation added"
```

#### Git log
```sh
# View git logs
git log
git log --oneline

git show <commig id / HEAD pointer>
git show HEAD
git show HEAD~1 # One step back to HEAD commit

# To see commit details of any particular file
git show HEAD~1:bin/start.sh

git ls-tree HEAD~2 # To see all the files and directories in the commit
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
