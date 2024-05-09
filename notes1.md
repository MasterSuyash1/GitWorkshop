What is Git?
------------

Git is a distributed version control system that allows multiple developers to collaborate on a project. It tracks changes to files, allows users to create branches for development, and provides tools for merging changes from different branches.

Git vs GitHub
-------------

Git is a version control system that tracks changes to files and directories, while GitHub is a web-based platform that hosts Git repositories and provides collaboration tools for developers.

Check Git Version
-----------------

```bash
git --version
```
This command displays the current version of Git installed on your system.


Configure User Details
-----------------------

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"

git config --global --list
```
The `git config` command is used to configure the user details. The `--global` option is used to set the configuration globally for the user. The `--list` option is used to display the current configuration.

Initialize a Git Repository
---------------------------

```bash
git init
``` 
Creates a new Git repository in the current directory, setting up the necessary files and folders to start version controlling your project.



Check Repository Status
-----------------------

```bash
git status
```
This command displays the current status of the repository. It shows which files are staged, unstaged, and untracked.

Stage Changes
-------------

```bash
git add <file>
git add .
```
The `git add` command is used to stage changes. The `git add <file>` command stages a specific file, while `git add .` stages all changes in the current directory.

Commit Changes
--------------
```bash
git commit -m "Commit message"
```
The `git commit` command is used to commit staged changes to the repository. The `-m` option is used to specify a commit message.

View Commit History
-------------------

```bash
git log
```
The `git log` command is used to view the commit history of the repository. It displays a list of commits, including the commit hash, author, date, and commit message.


Add and Commit Changes Together
-------------------------------

```bash
git commit -am "Commit message"
```
The `-a` option is used to automatically stage all changes before committing. This allows you to add and commit changes in a single command.
Stages and commits all modified files in one step. Use this for convenience when you don't need to separately stage files.


Create .gitignore File
----------------------

```bash
touch .gitignore
```
The `touch` command is used to create a new file. The `.gitignore` file is used to specify files and directories that should be ignored by Git.

List files or patterns in .gitignore to specify which files Git should ignore (e.g., temporary files, build outputs, or sensitive data).


View Git Configuration
----------------------

```bash
git config --list
cat .gitconfig

```
The `git config` command is used to view or set configuration options. The `--list` option is used to display all configuration settings.


Create a New Branch
-------------------

```bash
git branch <branchname>
```
The `git branch` command is used to create a new branch in the repository. Replace `<branchname>` with the desired branch name.

Switch to Another Branch
------------------------


```bash
git checkout <branchname>
```

The `git checkout` command is used to switch to another branch in the repository. Replace `<branchname>` with the desired branch name.

Create and Switch to a New Branch
---------------------------------

```bash
git checkout -b <branchname>
```
The `-b` option is used to create a new branch and switch to it in a single command. Replace `<branchname>` with the desired branch name.


Merge Branches
-------------

first checkout to the branch you want to merge into 
```bash
git checkout <branchname>
```
then merge the branch you want to merge into the current branch

```bash
git merge <branchname>
```
The `git merge` command is used to merge changes from one branch into another. Replace `<branchname>` with the branch you want to merge into the current branch.

## Types of merges:

- Fast-forward merge: When the branch being merged has a linear history and can be merged without creating a new commit.
- Recursive merge: When the branch being merged has diverged and requires a new commit to reconcile the changes.


Git add remote
--------------

```bash
git remote add origin <remote-url>
```
The `git remote add` command is used to add a remote repository to the local repository. Replace `<remote-url>` with the URL of the remote repository.

Push Changes to Remote Repository
---------------------------------

```bash
git push -u origin <branchname>
```
The `git push` command is used to push changes from the local repository to the remote repository. The `-u` option is used to set the upstream branch for the current branch. Replace `<branchname>` with the branch you want to push.

Pull Changes from Remote Repository
------------------------------------

```bash
git pull origin <branchname>
```

The `git pull` command is used to fetch and merge changes from the remote repository to the local repository. Replace `<branchname>` with the branch you want to pull.

View Remote Repositories
------------------------

```bash
git remote -v
```
The `git remote` command is used to view the remote repositories associated with the local repository. The `-v` option is used to display the URLs of the remote repositories.

Clone a Remote Repository
-------------------------

```bash
git clone <remote-url>
```
The `git clone` command is used to clone a remote repository to the local machine. Replace `<remote-url>` with the URL of the remote repository.

Git remove origin
-----------------

```bash
git remote remove origin
```
The `git remote remove` command is used to remove a remote repository from the local repository. Replace `origin` with the name of the remote repository.

Git diff
--------

```bash
git diff
```
The `git diff` command is used to view the changes between the working directory and the staging area. It shows the differences in the content of files that are staged or unstaged.

