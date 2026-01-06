# practicegithub 

Git
Git is a version control system used to manage and track changes in source code. It works on your local machine and stores code in a local repository. It helps maintain commit history and allows reverting changes.

GitHub
GitHub is a remote repository hosting service that stores Git repositories on the cloud. It is used for backup, collaboration, and code sharing with teams using features like pull, push, and merge.

Git manages code locally, while GitHub hosts Git repositories remotely for collaboration.
=================================================

git init
git init is a command used to initialize a new Git repository in your project folder. It works on your local machine and creates a .git folder to start tracking changes. It allows you to maintain commit history and manage versions of your code locally.

git clone
git clone is a command used to copy an existing Git repository from a remote source like GitHub to your local machine. It downloads the entire project along with its commit history, allowing you to work on the code locally and later push changes back to the remote repository.
===========================================
git status

Untracked
A file is untracked when it exists in your working directory but Git is not tracking it yet. These are usually new files you created but haven’t added with git add. (New file created still not Recoganized)

Modified
A file is modified when it has been changed in the working directory but the changes have not yet been staged. Git knows the file changed, but it’s not ready to be committed.

Staged
A file is staged when changes have been added to the staging area using git add. Staged files are ready to be committed to the local repository.

Unmodified
A file is unmodified when it has no changes since the last commit. Git considers it up-to-date.

Quick visual flow: Untracked → Modified → Staged → Committed → Unmodified
==========================================

git add
git add is a Git command used to move changes from the working directory to the staging area. It tells Git which files should be included in the next commit. You can add individual files or all changes at once.

Example: 
git add file.txt → Adds a single file to the staging area

git add . → Adds all modified and untracked files in the folder

Purpose:
Using git add helps Git track changes selectively and prepares them to be committed to the local repository.


Quick summary table (all options)
Command	What it does	Notes
git add <file>	:Add a specific file	:Selective commit
git add .	:Add all new & modified files in current directory	:Simple “all in folder”
git add -A / --all	:Add all changes including deletions :Full repository commit
git add -u	:Add modified & deleted files, ignores new files	:Update only existing files
git add -v	:Verbose mode, shows what’s being staged	:Useful to confirm staged files
git add -p	:Add changes hunk by hunk	:Stage partial changes in a file
git add -i	:Interactive mode	:Menu-based staging
git add -f / --force	:Force add ignored files	:Override .gitignore temporarily
===============================================

git commit

git commit is a Git command used to save staged changes to the local repository. It records a snapshot of your project at a specific point in time. Every commit has a commit message that describes the changes made.

Example:

git commit -m "Added login feature" → Commits staged changes with a message

git commit → Opens an editor to write a commit message
-m : message
Purpose:
Using git commit allows Git to maintain a history of changes, making it possible to revert, review, or track your project over time.
====================================================