# Git/GitHub

[Source Playlist](https://youtube.com/playlist?list=PLRAV69dS1uWT4v4iK1h6qejyhGObFH9_o&si=5rRAn7y3GDL1QLDq)

## Goal of this Series  
1. Learn Git(Theory+Practical).
2. Associated Services like GitHub, BitBucket, GitLab etc.

## Git 
- Git is a **distributed version control system(DVCS)** that tracks files and folders for changes.
- Git and GitHub are totally different.
- Git is a software, whereas, GitHub is a service.

## Repository  
- Repository or repo simply means a folder which is being tracked by version control system like Git.  

![reference](/assets/repo.png)

## Initializing an Empty Git Repository  
```bash
git init
```
- This command is used to initialize an empty git repository.
- This command is ran only one time per project.
- This command creates a **.git** folder, which is a hidden folder that keeps history of all files and folders.

## Cheking Git Version  
```bash
git --version
git -v
```
- This two commands are used to check the git version.

## Checking Git Status  
```bash
git status
```
- This command is used to check the git status of a repository.

## Commits  
- Commit is like a checkpoint in a game.
- Write -> Add -> Commit.  

![reference](/assets/working.png)

## Adding Files and Folders to Staging Area  
- Staging area is the area where files and folders are being tracked by a version control system like Git.
- Following command can be ran to add files and folders to staging area :  
```bash
# Add file1 and file2 to staging area 
git add file1.md file2.txt
# Add folder to staging area 
git add folder/
# Add all files and folders to staging area 
git add .
```

## Making a Commit  
- Following command can be ran to make a commit after adding the respective file or folder to staging area.
```bash
git commit -m "commit message"
```

## Rules for Making a Commit [Atomic Commits] 
- Keep commits centric to one feature, one component or one bug fix.  
- Present or Past commit message.  
- For present tense, it should be an imperative sentence. 

## Behind the Scenes of Commits  
![reference](/assets/commitsbts.png)  

## Log 
- Used to print the log of commits in different ways.  
```bash
# Prints complete log of commits with commit hash, message, name of author and other details
git log
# Prints log of commits with commit hash and message in single line
git log --oneline
# Prints log of commits from a particular author
git log --author "Author Name"
```

## Setting Username, Email and Default Editor for Git (Globally)  
```bash
git config --global user.name "Your Name"
git config --global user.email "Your Email"
git config --global core.editor "code --wait"
```
- Above commands can be used to set the username, email and default editor for git globally.

## Checking Username, Email and Default Editor for Git (Globally)  
```bash
git config --global user.name
git config --global user.email
git config --global core.editor
```
- Above commands can be used to check the username, email and default editor for git globally.

## Setting Username, Email and Default Editor for Git (Locally)  
```bash
git config user.name "Your Name"
git config user.email "Your Email"
git config core.editor "code --wait"
```
- Above commands can be used to set the username, email and default editor for git locally.

## Checking Username, Email and Default Editor for Git (Locally)  
```bash
git config user.name
git config user.email
git config core.editor
```
- Above commands can be used to check the username, email and default editor for git locally.

## .gitignore File  
- **.gitignore** file is used to keep some important files free from being tracked by Git such as .env, modules, secrets etc.
- We can just search .gitignore file generator in google, and copy-paste the result in our respective file.
- Alternative, we can specify files and folders in **.gitignore** file as given below :  
```bash
.env
secrets/
modules/
```

## .gitconfig File  
- **.gitconfig** file contains all the personal git data such as username, email-id, sign-in keys, default editor details etc.
- To view the contents of .gitconfig file, we must be in the home directory.
```bash
cd ~
cat .gitconfig
```

## Branch  
- A branch is like an alternate timeline or a parallel universe where we can work on new ideas without affecting the main ones.
- To check current branch, run the following command :  
```bash
git branch
```
- Here * denotes the current branch.

## Creating a New Branch  
- Run the following command to create a new branch :  
```bash
git branch branchName
```

## Switching to another Branch  
- Run the following command to switch to another branch :  
```bash
git switch branchName
```

## Creating a New Branch and Switch to that Branch  
- Run the following commands to create a new branch and switch to that branch :  
```bash
git switch -c branchName
git checkout -b branchName
```  

## Deleting a Branch  
- Run the following command to delete a branch :  
```bash
git branch -d branchName
```

## Renaming a Branch   
- Run the following command to rename a branch :  
```bash
git branch -m newName
git branch -m oldName newName
```

## Merging a Branch  
- To merge a branch, we must be in the branch where we want the desired branch to merge at :  
```bash
git merge branchName -m "merge message"
```

## Merge Conflicts  
- Arises during merging when changes are made to the same code in different branches.
- In case of merge conflicts, remove the markers, keep whatever you want, and then save the file.  