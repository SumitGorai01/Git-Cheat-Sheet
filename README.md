
# Git Command Cheat Sheet

This cheat sheet contains common Git commands to help you manage repositories, track changes, and collaborate effectively. 

## General Commands

- **Show Current Working Directory**
  ```bash
  $ pwd
  ```

- **Show Git Version**
  ```bash
  $ git --version
  ```

- **Clear the Screen**
  ```bash
  $ clear
  ```

## Repository Initialization

- **Initialize a Folder as a Git Repository**
  ```bash
  $ git init
  ```

- **Show the Status of the Repository**
  ```bash
  $ git status
  ```

## Adding Files to Repository

- **Add Specific Files to the Repository**
  ```bash
  $ git add a.txt b.txt
  ```

- **Add All Files to the Repository**
  ```bash
  $ git add .*
  ```

## Configuring Git

- **Set Email (First Time Configuration)**
  ```bash
  $ git config --global user.email "goraisumit01@gmail.com"
  ```

- **Set Username**
  ```bash
  $ git config --global user.name "Sumit"
  ```

## Committing Changes

- **Commit Changes with a Message**
  ```bash
  $ git commit -m "first commit"
  ```

- **Show Commit History**
  ```bash
  $ git log
  ```

- **Commit Modified Files**
  ```bash
  $ git commit -a -m "both files are modified"
  ```

## Viewing Files

- **See All Files in the Working Directory**
  ```bash
  $ git ls
  ```

## Vim Editor Commands

- **Create a File with Vim Editor**
  ```bash
  $ vim index.txt
  ```
  - Press `ctrl+c` to move the cursor to the last line.
  - Type `:wq` and press enter to save and exit.

## Git Diff Command

- **See Differences Between Working Directory and Staging Area**
  ```bash
  $ git diff index.txt
  ```

- **See Differences Between Working Directory and Last Commit**
  ```bash
  $ git diff HEAD index.txt
  ```

- **See Differences Between Staging Area and Last Commit**
  ```bash
  $ git diff --staged HEAD index.txt
  ```

- **See Differences Between Specific Commit and Working Directory**
  ```bash
  $ git diff 1821ad2 index.txt
  ```

- **See Differences Between Specific Commit and Staging Area**
  ```bash
  $ git diff --staged 1821ad2
  ```

- **See Differences Between Two Specific Commits**
  ```bash
  $ git diff 3f5f1a8 286be1f index.txt
  ```

- **See Differences Between Two Branches**
  ```bash
  $ git diff master main
  ```

- **See Differences Between Local and Remote Repositories**
  ```bash
  $ git diff master origin/master
  ```

## Removing Files

- **Remove Files from Staging and Working Directory**
  ```bash
  $ git rm file1.txt
  ```

- **Remove All Files**
  ```bash
  $ git rm -r .
  ```

- **Remove Files Only from Staging Area**
  ```bash
  $ git rm --cached file2.txt
  ```

- **Remove Files Only from Working Directory**
  ```bash
  $ rm file3.txt
  ```

## Resetting Changes

- **Remove Changes from Staging Area**
  ```bash
  $ git reset file.txt
  ```

- **Reset with Mixed Mode**
  ```bash
  $ git reset --mixed 488ceb9
  ```

- **Reset with Soft Mode**
  ```bash
  $ git reset --soft 488ceb9
  ```

- **Reset with Hard Mode**
  ```bash
  $ git reset --hard 488ceb9
  ```

## Branching Commands

- **Create a New File**
  ```bash
  $ touch a.txt
  ```

- **View Available Branches**
  ```bash
  $ git branch
  $ git status
  ```

- **Create a New Branch**
  ```bash
  $ git branch "branch_name"
  ```

- **Switch Between Branches**
  ```bash
  $ git checkout "branch_name"
  ```

- **Create and Switch to a New Branch in a Single Command**
  ```bash
  $ git checkout -b "branch_name"
  ```

- **Merge Two Branches**
  ```bash
  $ git merge "branch_name"
  ```

## Viewing Files in Staging Area

- **See Files in Staging Area**
  ```bash
  $ git ls-files
  ```

## Viewing File Content

- **See Content of a File**
  ```bash
  $ cat file5.txt
  ```

- **Use Checkout Command**
  ```bash
  $ git checkout --file5.txt
  ```

This README serves as a quick reference guide for working with Git. For more detailed information, refer to the official Git documentation.
