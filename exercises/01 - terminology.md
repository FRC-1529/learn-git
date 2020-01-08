# Exercise 01: Git Terminology

## Structure of a Git Repository

### Repository

A repository is the container that holds all your code, branches, commits, and history.

### Commit

A commit is a structure that holds all CHANGED data from the last commit.  Think of this as the "delta" of code, that has been recorded.

### Branch

A branch is string of commits, that *branch* off from another branch.  All repositories start with a "master" branch.  New branches are then usually used to track the progress of a specific bug or feature, without effecting the master branch of code.

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