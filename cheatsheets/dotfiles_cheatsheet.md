# Dotfiles Cheatsheet

## Table of contents
* [Setup Repo](#setup-repo)
* [Setup a new machine](#setup-a-new-machine)
* 🚨 NEVER CHECKIN SENSITIVE DATA 🚨

## Setup Repo
In order to be able to checkin the dotfiles, a Git repo needs to exist.
Preferably, we put the repo in the home directory, also beaing a dotfile with the path `~/.dotfiles` but it can be anywhere.

Then, if starting from scratch, we need to add the dotfiles to the repo by simply copying them into the repo directory.

### Create a README file and store a shell script with symlink commands

To make it easier to setup the dotfiles on a new machine, we create a README file and store a shell script with symlink commands.

## Setup a new machine
The process to setup a new machine with the exisiting dotfiles is then to simply copy the dotfiles from the repo to the home directory and run the shell script.

## 🚨 NEVER CHECKIN SENSITIVE DATA 🚨