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

#### Git Status
```sh
# Short Status
git status -s

# Changes in Stagged area
git diff --staged

# List files in staging area
git ls-files

git rm index.html

git mv severe.js server.js
```

#### Git Commit
```sh
# Add file to staging area
git add index.html
git add bin/*.sh app/*.js

git commit -am "User signin validation added"
```

