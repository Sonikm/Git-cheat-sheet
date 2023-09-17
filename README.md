
# Git and GitHub command cheat sheet  
 <img src="https://raw.githubusercontent.com/arslanbilal/git-cheat-sheet/master/Img/git-logo.png" alt="git-logo" width="600" >

## What is Git?
A distributed version control system is a system that helps you keep track of changes you've made to files in your project, and it is exist locally on your system.

- Track the history of files
- Tracking code changes
- Tracking who made changes
- Coding collaboration

## What is GitHub?
Git is not the same as GitHub, GitHub is a company that let's you host your file using git.


## Setup

Configure your user name

```
 $ git config --global user.name "[your_name]"
```
Configure the user email address

```
 $ git config --global user.email "[your_email_Id]"
```

## Git configuration and files

Check list of information about your git configuration

```
 $ git config -l
```
Show list of files

```
 $ git ls
```
## initialize

Creating a local repository

```
 $ git init
```
## diff, status

Display the differences of changed files

```
$ git diff
```

Show modified files in working directory

```
$ git status
```

## add

Add a file to the staging area in Git

```
$ git add [filename]
```

Add all files in the staging area

```
$ git add .
```
This command opens a prompt and asks if you want to stage changes or not

```
$ git add -p
```

## commit

Commit files that have been added to the index

```
$ git commit
```

Commit a file with the commit message

```
$ git commit -m "[comment]"
```

## log and show

See the commit history 

```
$ git log
```

Display the latest commit content

```
$ git show
```
## reset and remove

Unstage a file 

```
$ git reset [file_name]
```

Remove tracked files from the current working tree

```
$ git rm filename
```

## branch

Create branches

```
$ git branch [branch_name]
```

Display a list of branch

```
$ git branch
```

Display all branches

```
$ git branch -a
```

Display the remote branch

```
$ git branch -r
```

Delete the branch

```
$ git branch -d [branch_name]
```

## Branch and merge

Switch the branch

```
$ git checkout [branch_name]
```

Switching to create a branch

```
$ git checkout -b [branch_name]
```

Check all chenges in branches

```
$ git log --all
```

Merge the branch

```
$ git merge [branch_name]
```

## remote and push

Check remote name

```
$ git remote
```
Adds a remote repository to your local repository

```
$ git remote add origin https://repo_here
```

Submit to commit the local repository to the remote repository

```
$ git push [remote_name] [branch_name]
```

Submit to commit the master of the local repository to the master of the remote repository

```
$ git push origin master
```

See all remote repository for your local repository
```
$ git repository -v
```

Get more info about a remote repository 
```
$ git remote show origin
```

Push all save changes to the remote repository
```
$ git push
```

Remove remote origin from a git repository
```
$ git remote remove origin
```
## clone

Copy the project from the remote repository

```
$ git clone [repository_path]
```

Copy the project by specifying the name of the directory you want to create

```
$ git clone [repository_path] [new repository_path]
```

Change the current working directory
```
$ cd [new repository_path]
```

Save all changes to the remote repository
```
$ git push
```

## fetch and merge

Fetch down all the branches from that Git remote
```
$ git fetch origin
```

Merge a remote branch into your current branch to bring it up to date
```
$ git merge origin/master
```

Push all the changes on remote repository
```
$ git push origin master
```

## pull

Fetch and merge any commits from the tracking remote branch
```
$ git pull origin BRANCH_NAME
```

## Checking out pull requests locally

Fetch the reference to the pull request based on its ID number
```
$ git fetch origin pull/ID/head:BRANCH_NAME
```

Switch to the new branch that's based on this pull request:
```
$ git checkout BRANCH_NAME
```
## cherry-pick

Copy the commit of another branch to the current branch

```
$ git cherry-pick [commit id]
```

## Checking out pull requests locally

Fetch the reference to the pull request based on its ID number

```
$ git fetch origin pull/ID/head:BRANCH_NAME
```

Switch to the new branch that's based on this pull request:

```
$ git checkout BRANCH_NAME
```

## browse, open

Open a page of the project of GitHub

```
$ git browse
```

```
$ open https://github.com/USER_NAME/REPOSITORY_NAME
```

Open a page of the issues of the project of GitHub

```
$ git browse -- issues
```

```
$ open https://github.com/USER_NAME/REPOSITORY_NAME/issues
```

Opening the wiki pages of the project of GitHub

```
$ git browse -- wiki
```

```
$ open https://github.com/USER_NAME/REPOSITORY_NAME/wiki
```







