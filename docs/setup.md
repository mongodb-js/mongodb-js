# Setup

## OSX Setup

### 1. Install XCode

You can easily [install XCode from the App Store](https://itunes.apple.com/us/app/xcode/id497799835?mt=12).

### 2. Install Homebrew

[Homebrew](http://brew.sh/) is a package manager for OSX.  You can install it simply by pasting the below into your terminal:

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### 3. Install python, node.js, and npm

Python may be required for working with some projects.  Installing node.js will provide you with the `node` and `npm` commands.

```
brew install python nodejs;
sudo easy_install pip;
pip install pyobjc;
npm install -g node-gyp;
```

## 4. Setup git and GitHub

See [Setting up Git][git-setup]
on GitHub's website for instructions to get started with git and GitHub.

## 5. Join gitter channel

We're hanging out on [gitter.im][gitter-mongodb-js], join the channel to stay
up to date or ask questions.

## Windows Setup

## 1. Install Visual Studio 2013 or higher

You can download the [community edition for free](http://www.visualstudio.com/products/visual-studio-community-vs).

## 2. Install Python

Python may be required for working with some projects so just [download and run the installer](http://www.python.org/download/releases/2.7/).

## 3. Install node.js

[Download and run the installer][node-download] to get `node` and `npm`.

## 4. Setup git and GitHub

See [Setting up Git][git-setup]
on GitHub's website for instructions to get started with git and GitHub.

## 5. Join gitter channel

We're hanging out on [gitter.im][gitter-monogodb-js], join the channel to stay
up to date or ask questions.

## Linux Setup

## 1. Install dependencies

```
sudo apt-get install build-essential clang libdbus-1-dev libgtk2.0-dev \
                       libnotify-dev libgnome-keyring-dev libgconf2-dev \
                       libasound2-dev libcap-dev libcups2-dev libxtst-dev \
                       libxss1 gcc-multilib g++-multilib
```

## 2. Install node.js and npm

Check [this article][install-linux] on how to install
a current version of node.js. (Note: the article is also linked from
[node's wiki page][node-wiki-install].)

## 3. Setup git and GitHub

See [Setting up Git][git-setup]
on GitHub's website for instructions to get started with git and GitHub.

## 4. Join gitter channel

We're hanging out on [gitter.im][gitter-mongodb-js], join the channel to stay
up to date or ask questions.

[install-linux]: https://nodesource.com/blog/nodejs-v012-iojs-and-the-nodesource-linux-repositories
[node-download]: https://nodejs.org/download/
[node-wiki-install]: https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager
[git-setup]: https://help.github.com/articles/set-up-git/#setting-up-git
[gitter-mongodb-js]: https://gitter.im/mongodb-js/mongodb-js
