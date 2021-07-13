# ANDigital Mac Setup

A script to set up a macOS laptop for development.

It can be run multiple times on the same machine safely. It installs, upgrades, or skips packages based on what is already installed on the machine.

Forked from [here](https://github.com/codeclan/laptop)

## Requirements

We support:

- macOS Big Sur (11)
- macOS Catalina (10.15)

Older versions may work but aren't tested.

## Install

(These commands should be run in **Terminal**)

To open Terminal:

1. Press Command+Space and search for Terminal.
2. Hit enter

Copy the below code command into Terminal and hit enter:

```sh
curl --remote-name https://raw.githubusercontent.com/codeclan/laptop/master/mac
```

Then run it and start the installation:

```sh
sh mac 2>&1 | tee ~/laptop.log
```

**You will need to enter your computer password a few times throughout the script to allow installations**

At the end of the installation script, another script will run to attempt to check if any applications failed to install. (occasionally may claim some application are missing that aren't)

You can repeat this by running the following lines in terminal:

```sh
curl --remote-name https://raw.githubusercontent.com/codeclan/laptop/master/laptop_install_test
sh laptop_install_test
```

---

## What it sets up

### macOS tools:

- [Apple's Command Line Developer Tools](https://developer.apple.com/) to enable developer functionality on our macOS system.

### Command line tools:

- [Homebrew](http://brew.sh/) for managing operating system libraries.
- [Git](https://git-scm.com/) for version control
- [Zsh](http://www.zsh.org/) as your command line shell
- [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh) to add nice features to zsh - autocompletions, shortcuts etc.
- [tree](https://linux.die.net/man/1/tree) for visualising directory structure from the Terminal

### Programming languages and configuration:

- [Ruby](https://www.ruby-lang.org/en/)
- [Rbenv](https://github.com/sstephenson/rbenv) for managing versions of Ruby
- [Bundler](http://bundler.io/) for managing Ruby libraries
- [Ruby Build](https://github.com/sstephenson/rbenv) for installing Rubies
- [Java](https://java.com/en/)
- [Node.js](http://nodejs.org/) for JavaScript back-end development, and
- [NPM](https://www.npmjs.org/) for installing JavaScript packages

### Databases:

- [PostgreSQL](http://www.postgresql.org/) for storing relational data
- [MongoDB](https://www.mongodb.com/) for storing non-relational data

### GUI Apps:

- [Google Chrome](https://www.google.com/chrome/) for web browsing and development
- [VSCode](https://code.visualstudio.com/) IDE
- [Slack](https://slack.com) for team chat
- [IntelliJ IDEA CE](https://www.jetbrains.com/idea/) for Java development
- [MongoDB Compass](https://www.mongodb.com/products/compass) for accessing MongoDB databases from a GUI
- [Docker](https://www.docker.com/)

### Fonts:

- Open Dyslexic for accessibility

It should take less than 15 minutes to install (though this depends on your machine).
