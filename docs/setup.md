# Setup

## Mac OS Setup

### 1. Install XCode Developer Tools

```
xcode-select --install
```

Note: You should not need the full [XCode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12).


### 2. Install Homebrew

[Homebrew](http://brew.sh/) is a package manager for macOS.

Please follow the installation instructions at http://brew.sh/

### 3. Install python, node.js, and npm

To install ``node-version-manager``, please follow:

https://github.com/creationix/nvm#install-script

Python may be required for working with some projects, though macOS has it built in. Installing node.js will provide you with the `node` and `npm` commands.

```
# brew install nvm;  # Note: nvm discourages installation by brew
nvm install 7.4;
nvm alias default 7.4;
```

### 4. Setup git and GitHub

See [Setting up Git][git-setup]
on GitHub's website for instructions to get started with git and GitHub.


## Windows Setup

### 1. Install Visual Studio 2013 or higher

You can download the [community edition for free](http://www.visualstudio.com/products/visual-studio-community-vs).

### 2. Install Python

Python may be required for working with some projects so just [download and run the installer](http://www.python.org/download/releases/2.7/).

### 3. Install node.js

[Download and run the installer][node-download] to get `node` and `npm`.

### 4. Setup git and GitHub

See [Setting up Git][git-setup]
on GitHub's website for instructions to get started with git and GitHub.


## Linux Setup


## Debian / Ubuntu

### 1. Install dependencies

```
sudo apt-get install build-essential clang libdbus-1-dev libgtk2.0-dev \
                       libnotify-dev libgnome-keyring-dev libgconf2-dev \
                       libasound2-dev libcap-dev libcups2-dev libxtst-dev \
                       libxss1 gcc-multilib g++-multilib
```

### 2. Install node.js and npm

Check [this article][install-linux] on how to install
a current version of node.js. (Note: the article is also linked from
[node's wiki page][node-wiki-install].)

### 3. Setup git and GitHub

See [Setting up Git][git-setup]
on GitHub's website for instructions to get started with git and GitHub.


## CentOS / Fedora / Red Hat

### 1. Install VirtualBox Guest Additions

This will get you some useful things like `gcc`, otherwise you may need to install other dependencies:

```
1. Install RHEL 6 minimal installation
2. Do a full `yum update`
3. `yum install kernel-devel gcc make patch`
4. Reboot
5. Mount VirtualBox Tools iso and try to install the Guest additions
```
https://access.redhat.com/discussions/1519903#comment-942153

### 2. Install node v6 LTS

`curl --silent --location https://rpm.nodesource.com/setup_6.x | bash -`

https://nodejs.org/en/download/package-manager/#enterprise-linux-and-fedora

### 3. Install git and GitHub

See [Setting up Git][git-setup]
on GitHub's website for instructions to get started with git and GitHub.

Note: RHEL v6 is so far behind that you may prefer to build your own from the source, which is not hard to do:
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git#Installing-from-Source


[install-linux]: https://nodesource.com/blog/nodejs-v012-iojs-and-the-nodesource-linux-repositories
[node-download]: https://nodejs.org/download/
[node-wiki-install]: https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager
[git-setup]: https://help.github.com/articles/set-up-git/#setting-up-git

