# Project 0 - Git Guide

## Command line git
- status - lists the number of local commits not synced with GitHub, and the local files not being tracked or that are being tracked and have changes that need to be committed. `git status`
- clone - clones repository and creates connection to GitHub. `git clone git@github.com:WSU-kduncan/ceg3120-EvanSwepston.git`
- rm - remove. `rm example.txt`
- commit - lists changes made. `git commit -a -m "message"`
- push - pushes changes to GitHub. `git push`
- fetch - downloads all new files from GitHub to show you what's different, but does not change anything until `git pull` is used. `git fetch --all`
- merge - merges branch with main. `git merge branchName`
- pull - pulls changes from GitHub. `git pull`
- branch - creates a copy to change files separately from main. `git branch branchName`
- checkout - moves to branch (or back to main). `git checkout branchName`

## git files and folders
- .git folder - contains commit history `git add` and `git remove` can be used to control what files are tracked or untracked
- .gitignore file - contains files that are completely ignored by git, which must be edited directly to start ignoring certain files `*.log` in the file would cause git to ignore any file that ends in `.log`

## GitHub
- Pull requests - a way to allow other people working on a project to review a commit and merge it into the main branch. On GitHub, you must navigate to a branch, then click the `pull request` button
- SSH authentication to repositories - allows you to more securely access your repository. `ssh-keygen -t ed25519 -C "your_email@example.com"` then copy the contents of the file that ends in `.pub`. On GitHub, go to settings then add a new SSH key, pasting the contents of `.pub` into the box
