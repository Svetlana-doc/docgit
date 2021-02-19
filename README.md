# Working with Git in the terminal
Git — is a tool that allows you to control a project in separate versions.
With its help, the documentation is stored in a structured form and allows you to view a detailed history: when, who at what time made changes. You can view these changes, accept or reject them, return to the previous state.
To get started with Git, create a new document, or edit the current one, you need to run some commands.

## Basic Git Commands

### Installing and configuring Git
To get started with Git, you need to check whether it is installed on your computer. To do this, enter the terminal:

`git --version`  — checking the Git installation.

When you press *Enter*, the installed version of Git should be displayed, if not, then you need to install it. Read more [here](https://git-scm.com/book/ru/v2/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-Git). 

After successfully installing Git, you need to configure the user information so that when working with the project, you can see who made certain changes:

`git config --global <user.name>` — set a name that will be visible when viewing the version history.

`git config --global <user.email>` — set the email address to which notifications about changes will be sent.

### Getting started
Initializing and cloning repositories.

`git clone  <url_repository>` — clone the repository.

### Making changes

Getting updates from another repository and updating local repositories.

`git checkout master` — switch to the master.

`git pull` — download changes from a remote repository.

`git checkout -b <branch_name>` — switch and create a new branch.

`git add .` — add files to commit (the dot means that all modified files will be added to the commit).

`git commit -m <message>` — commit to the local repository with the message.

`git commit --amend` — commit changes to the previous commit.

`git push` — upload changes to a remote repository.

### Merging branches
In order to inject a branch into the master, you need to run the following commands.

`git checkout master` — switch to the master.

`git merge <feature_branch>` — pour the branch into the master.
