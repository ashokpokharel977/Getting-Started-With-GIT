# Getting-Started-With-GIT
This is a written tutorial on how to get started with Git- version controlling system without being overwhelmed. 

# Getting Satarted with git -some version controlling

## Insatlling the git software in local machine

[DownloadLink](https://git-scm.com/downloads)

## Setting up Global Variables

### Username & Email configuration

**Don't Copy $ symbol it only inditcated the command should be run inside termilal.**
```sh
$ git config --global user.name = "John"
$ git config --global user.name = "example@gmail.com"
```
### creating github account
[Github](https://github.com/)

## Creating new Repository
    create directory && open terminal
```sh
    $ git init
```
This will initialize the git reopsitory

![Image of workflow](http://rogerdudler.github.io/git-guide/img/trees.png)Format: ![Alt Text](url)

### Adding the file & commiting
```sh
    $ git add <filename>
```
#### Adding all files
```sh
    git add *
```
#### Committing
```sh
    $ git commit -m "Commit Message"
```
**This will only add to your local workspace**
### Now pushing the code
**It pushes the code to remote repository**

```sh
    $ git push origin master
```
**Origin is your file Origin i.e your local storage**
### Adding the remote path

```sh
    $ git remote add origin <server>
```
## Branching

### Create new branch and move to it

```sh
    $ git checkout -b <Branchname>
```
#### Switching back to master 

```sh
    $ git checkout master
```
#### Want to delete the branch

```sh
    $ git branch -d <BranchName>
```
### Pushing to Branch

```sh
    $ git push origin <branchname>
```
## Update & Merge
**Pulling the latest changes from remote repository**

```sh
    $ git pull
```
### Want to merge branch master

```sh
    $ git merge <branchname>
```

## Finding the difference between 

```sh
    $ git diff <source_branch> <target_branch></target_branch>
```
## Log
### Used to study repository history

```sh
    $ git log
```
#### Want to see the commits by Hancy

```sh
    $ git log --author=Hancy
```
**For decorated output use**
```sh
    $ git log --graph --online --decorate --all
```

## Replace Local Changes
**What if I made a mistake ?**

```sh
    $ git checkout <filename>
```
**What if You Screwed all files and want to start from latest satble changes**

```sh
    $ git fetch origin
    $ git reset --hard origin/master
```
