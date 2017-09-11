# macOS Sierra v. 10.12 Setup

[See Blog post here.](http://johnawotwi.me/setupmacos/)

This is a simple list of instructions to make setting up your Apple computer as fast and efficient as possible for front end web development and anything else.

First install MacOS's missing installer ->
## Homebrew

```shell
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### Mac App Store

```shell
brew install mas
```

#### Sign in

```shell
mas signin email@email.com
```

### Brewfile

```shell
touch Brewfile
```

```shell
cask 'atom'
cask 'firefox'
cask 'gimp'
cask 'google-chrome'
cask 'opera'
cask 'spectacle'
cask 'sequel-pro'
cask 'vlc'
cask 'virtualbox'
cask 'libreoffice'
cask 'imageoptim'
cask 'appcleaner'
cask 'the-unarchiver'
cask 'teamviewer'
cask 'cyberduck'
cask 'transmission'
cask 'Virtualbox'
cask 'Libreoffice'
cask 'imageoptim'
cask 'dash'
cask 'android-file-transfer'
cask 'adapter'
cask 'mamp'




mas 'Slack', id: 803453959

```
Run ```brew bundle install``` in the same directory you have the ==brewfile== in


### Generate SSH key

```shell
ssh-keygen -t rsa -b 4096 -C "email@email.com"
```

## SSH

### Config - `~./ssh/config`

```shell
Host *
    AddKeysToAgent yes
    UseKeychain yes
    IdentityFile ~/.ssh/XX_XXX
```

## Bash

### Config - `~/.bash_profile`

Found this alias to be beautiful.Thanks to **Tania Rascia**

```shell
alias brewup='brew update; brew upgrade; brew prune; brew cleanup; brew doctor;'
```

```shell
source ~/.bash_profile
```


## Node.js

### Download Node

```shell
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash
```

```shell
nvm install node
```

```shell
nvm use node
```

## Node Package Manager



## Ruby Version Manager

### Download rvm

```shell
\curl -sSL https://get.rvm.io | bash -s stable
```

### Install Ruby version

```shell
rvm install ruby-head
```
==or==

```shell
rvm --default use 2.4.0
```

```shell
gem install bundler
```
