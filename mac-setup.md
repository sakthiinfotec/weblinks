#### Install Homebrew

```sh
# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

#### [Install Node.js via NVM](https://collabnix.com/how-to-install-and-configure-nvm-on-mac-os/)

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

nvm alias default 18

````

#### [Install MongoDB 6.0 Community Edition](https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/)

```sh
# Install Xcode Command-Line Tools
xcode-select --install

brew tap mongodb/brew

brew update

brew install mongodb-community@6.0
```

The installation includes the following binaries:

- The `mongod` server

- The `mongos` sharded cluster query router

- The MongoDB Shell, `mongosh`

To run MongoDB (i.e. the mongod process) as a macOS service, run:

`brew services start mongodb-community@6.0`

To stop a mongod running as a macOS service, use the following command as needed:

`brew services stop mongodb-community@6.0`

