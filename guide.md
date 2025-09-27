# Git Guide

This guide helps with the first steps of creating and initialising git for a new project.

## Create project files on local

1. Create folder

```bash
    nano mkidr folder-name
```

1. nano index.html /*creates main html file*/

```bash
    nano README.d
    nano style.css
```

## Initialise git, create repo and push changes

1. Navigate to new folder with terminal /*cd, ls*/
1. Initialise git and perform initial commit

```bash
    git init
    git add . /* or filename */
    git commit -m "initial commit"
```

1. Create new repo on GitHub

   - don't create README file
   - copy remote URL

1. Pase remote URL from GitHub into terminal

    git remote add origin [remote URL]

1. Push code to repo

```bash
    git branch -M main /*changes default branch name to main*/
    git push -u origin main /*-u git remembers which branch to push to*/
```

1. From now on

```bash
    git add .
    git commit -m "comment"
    git push
```

## Useful lines

```bash
    git config --global pull.rebase true # rewrites your local commits on top of the new changes instead of creating a merge commit
```
