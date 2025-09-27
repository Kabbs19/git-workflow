# Git Guide

This guide helps with the first steps of creating and initialising git for a new project.

## Create project files on local

1. mkdir [folder-name] /*use within terminal to create a folder*/
2. nano index.html /*creates main html file*/
3. nano README.md /*creates readme file*/
4. nano style.css /*creates stylesheet*/

## Initialise git, create repo and push changes

1. Navigate to new folder with terminal /*cd, ls*/
2. Initialise git and perform initial commit

    '''bash
    git init
    git add . /*or filename*/
    git commit -m "initial commit"
    '''

3. Create new repo on GitHub

   - don't create README file
   - copy remote URL

4. Pase remote URL from GitHub into terminal

    git remote add origin [remote URL]

5. Push code to repo

    git branch -M main /*changes default branch name to main*/
    git push -u origin main /*-u git remembers which branch to push to*/

6. From now on

    git add .
    git commit -m "comment"
    git push

## Useful lines

    git config --global pull.rebase true /*rewrites your local commits on top of the new changes instead of creating a merge commit*/
