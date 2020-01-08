# Exercise 01: Git Terminology

## Goal

This is just a document for you to reference for the rest of the exercises. For more information, check the [git documentation](https://git-scm.com/docs).

## Structure of a Git Repository

### Repository

A repository is the container that holds all your code, branches, commits, and history.

### Commit

A commit is a structure that holds all CHANGED data from the last commit.  Think of this as the "delta" of code, that has been recorded.

### Branch

A branch is string of commits, that _branch_ off from another branch.  All repositories start with a "master" branch.  New branches are then usually used to track the progress of a specific bug or feature, without effecting the master branch of code.

## Git Commands & Effects

### init

This command creates a repository in the current directory.  This command must be run befor any others

```bash
git init
```

### config

This command allows you to configure your git repository.  Usually used to assign your username and email.  Your email here should match the email you use on GitHub.  If you use the "--global" flag, that configuration will be automatically assigned to all new repositories you create.

```bash
git config [--global] <variable> <value>
git config --global user.name <your name>
git config --global user.email <your email>
```

### add / rm

These commands add and remove files to be tracked by git.  You might not always want a file to be shared publicly, like a config.json file with your SSH key in it, so you could add all your files, then remove the ones you don't want to be shared.  To add or remove all items in the repository, use the "." token instead of file names.

```bash
git add <filename>
git add . # Adds all files in the current directory
git rm <filename>
git rm .
```

### commit 

This command will commit any _tracked_ changes to the current branch.  It is usually be accompanied by the "-m" tag to add a message.

```bash
git commit -m "Message for this commit"
```

### branch

This commmand creates a new branch to be used and tracked.

```bash
git branch <branch_name>
```

### switch

This command will switch to a different branch.

```bash
git switch <branch_name>
```

### checkout

This command will changes the files on your computer to match the latest commit in a branch.

```bash
git checkout <branch_name>
```

### merge

This command will "replay" commits in a different branch onto the current branch, until the branches are identical.

```bash
git merge <branch_name>
```

### log

This command will display the most recent commits in the current branch.

```bash
git log
```

### fetch

This command downloads branchs from a remote repo (e.g. github).

```bash
git fetch <renote> <branch>
```

### pull

This command is a short cut that runs the "fetch" and then "merge" commands.

```bash
git pull <remote> <branch>
```

### push

This command updates a remote repo (e.g. github) with new commits

```bash
git push <remote> <branch>
```
