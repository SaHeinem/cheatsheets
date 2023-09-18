# Git Cheatsheet
this document is intended as reference for some git commands. The author does not claim completeness

## Table of contents
* [Setup](#setup)
* [Start, clone, stage and snapshot](#start-clone-stage-and-snapshot)
* [Branch and merge](#branch-and-merge1)
* [Changes](#changes)
* [Ignoring patterns](#ignoring-patterns)
* [Update and push](#update-and-push)
* [Temporary](#temporary)

## Setup
.gitconfig file stores all global configs

More commands are:
````sh
git config --global user.name “[firstname lastname]”
git config --global user.email “[valid-email]”
git config --global color.ui auto
````

## Start, clone, stage and snapshot
````sh
ginit init
git clone
git status
git add [file / .]
git reset [file / --hard]
git diff [--staged]
git commit -m "[message]"
git commit -am "[message]"
````

## Branch and merge
````sh
git branch //list branches
git branch [branch name]
git checkout
git merge [branch]
git log
````

## Changes
````sh
git rm [file]
git mv [current path] [new path]
````

## Ignoring patterns
````sh
logs/
*.notes
pattern*/
````

## Update and push
````sh
git remote add [alias] [url]
git fetch [alias]
git merge [alias]/[branch]
git push [alias] [branch]
git pull
````

## Temporary
````sh
git stash
git stash push -m "[message]"
git stash list
git stash pop
git stash apply stash^{/[message]}
git stash drop
````
