# Commonly used commands in Git
# git add -
- git add command is used to add changes in your working directory to the staging area in Git.
- When you first add files to an empty repository, they are all untracked. To get Git to track them, you need to stage them, or add them to the staging environment.

#### Syntax for `git add`-
- git add <file_name>         # Add a specific file
- git add .                   # Add all changes in the current directory
- git add <directory_name>/   # Add all files in a specific directory

# git commit -
- The git commit command is used to save changes to the local repository after staging them with git add.
- It’s best practice to include a message with each commit explaining the changes made in a commit. Adding a commit message helps to find a particular change or understanding the changes.
- git commit -m "Your commit message"
- git commit
    - For multi-line message, it will enter you in text editor.

#### Git Commit without Stage :-
- Sometimes, when you make small changes, using the staging environment seems like a waste of time. It is possible to commit changes directly, skipping the staging environment.
- git commit -a -m “<Enter your message here>”

#

