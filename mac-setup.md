#### Install Homebrew

```sh
# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

#### Install Node.js via NVM

```sh
# Use Homebrew to install NVM
brew install nvm

# Add nvm to your shell profile: source $(brew --prefix nvm)/nvm.sh
(echo; echo 'source $(brew --prefix nvm)/nvm.sh') >> /Users/sakthi/.zshrc

# Install Node.js
nvm install node

# List available Node.js versions
nvm ls-remote

# Instal desired Node.js version
nvm install 18

# Use the desired version from installed list
nvm use 18

nvm alias default 16

````
