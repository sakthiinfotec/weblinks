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
```

```sh

# Short Status
git status -s

# Changes in Stagged area
git diff --staged


```
