## Git Terminologies
### Repository
A Git repository (or repo for short) contains all of the project files and the entire revision history. You’ll take an ordinary folder of files (such as a website’s root folder), and tell Git to make it a repository. This creates a .git subfolder, which contains all of the Git metadata for tracking changes. On Unix-based operating systems such as macOS, files and folders that start with a period (.) are hidden, so you will not see the .git folder in the macOS Finder unless you show hidden files, but it’s there! You might be able to see it in some code editors.

[Here is a detailed **Step by Step Procedure** to create a repository.](https://www.geeksforgeeks.org/creating-repository-in-github/)

A working tree in a Git Repository is the collection of files which are originated form a certain version of the repository.
There are a few stages of a file in the working tree of a repository:
* **Untracked :** In this stage, the Git repository is unable to track the file, which means that the file is never staged nor it is committed.
* **Tracked:** When the Git repository tracks a file, which means the file is committed but is not staged in the working directory.
* **Staged:** In this stage, the file is ready to be committed and is placed in the staging area waiting for the next commit.
* **Modified/Dirty:** When the changes are made to the file i.e. the file is modified but the change is not yet staged.

GIT needs to follow two more steps to save these changes in the local repository.
These steps are:

i) **Adding the changes to the Index(Staging Area)**

        Syntax:
        $ git add File-name
        Different ways to use add command: 
        To add a specific list of files to staging area.
        $ git add
        To add all files of current directory to staging area.
        $ git add --all
        To add all text files of the current directory to staging area.
        $ git add *.txt
        
        
ii) **Committing the indexed changes into the repository**

Committing process are done in the staging area on the files which are added to the Index after git add command is executed. This committing process is done by the use of git commit command. This command commits the staged changes to the local repository.
        
        Syntax:
        $ git commit -m "Add existing file"


![Git Repo Image](images/Picture4.png)