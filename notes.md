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

