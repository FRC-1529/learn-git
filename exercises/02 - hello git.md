# Exercise 01: Hello Git

> Our first real forrary into using git.

## Goal

The goal of this exercise is to familiarise you with creating repos, commiting changes, and interacting with github.

## Step-by-step guide

1. On your computer, create a directory (folder) to hold all your programming projects. (e.g. /Documents/Projects or /Documents/CyberCards)
2. On GitHub, fork the "learn-git" repo from https://github.com/FRC-1529/learn-git, by using the "fork" button on the top right. (Help: [How-to Guide](https://help.github.com/en/github/getting-started-with-github/fork-a-repo))
3. On the commandline, in the projects director, clone this repository.
```bash
git clone https://github.com/<your_github_username>/learn-git # git clone https://github.com/CalobHumble/learn-git
```
4. Configure your git to your name and email
```bash
git config --global user.name "your_name" # git config --global user.name "Calob Humble"
git config --global user.email "your_email" # git config --global user.email "cshumble@protonmail.com"
```
5. Then, create a new branch on that repo called "yourname-02" (e.g. calob-02).

```bash
git branch <yourname>-02 #git branch calob-02
git checkout <yourname>-02 #git checkout calob-02
```
6. Create a folder called "yourname", then in that folder another called "exercise-02".  So the current directory should be "learn-git/<yourname>/exercise-02"
7. In that folder, create a simple "about-me.txt" file that states your name, and give a few sentances about what you want to learn with the CyberCards.
8. Add that file to be tracked
```bash
git add <file_name> # OR git add .
```
9. Commit that file, with any message
```bash
git commit -m "a short message"
```
10. Push your commit to github
```bash
git push -u origin <branch_name> # git push -u origin calob-02
```
11.  Create a new pull request to merge your custom branch to the master repo at at FRC-1529 (Help: [How-to Guide](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request))
