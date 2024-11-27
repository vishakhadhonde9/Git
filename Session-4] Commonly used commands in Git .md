# Commonly used commands in Git -

# git config -
- Git needs to be configured before you can use it.
- The Git config command is used enter the login and email addresses you want to be associated with your commits.
#### sets up Git with your name-
        git config --global user.name "<Your-Full-Name>“

#### sets up Git with your email-
        git config --global user.email "<your-email-address>"


# git add -
- git add command is used to add changes in your working directory to the staging area in Git.
- When you first add files to an empty repository, they are all untracked. To get Git to track them, you need to stage them, or add them to the staging environment.

#### Syntax for `git add`-
       git add <file_name>         # Add a specific file
       git add .                   # Add all changes in the current directory
       git add <directory_name>/   # Add all files in a specific directory

# git commit -
- The git commit command is used to save changes to the local repository after staging them with git add.
- It’s best practice to include a message with each commit explaining the changes made in a commit. Adding a commit message helps to find a particular change or understanding the changes.

#### Syntax -
       git commit -m "Your commit message"
       git commit
           - For multi-line message, it will enter you in text editor.

#### Git Commit without Stage :-
- Sometimes, when you make small changes, using the staging environment seems like a waste of time. It is possible to commit changes directly, skipping the staging environment.
- git commit -a -m “<Enter your message here>”

# git clone -
- git clone is used to download current source code from a remote repository (like GitHub, for example).
- It essentially creates an exact copy of the most recent version of a project in a repository and stores it on your computer.

#### Syntax -
      git clone {repository-url}

# git status -
- Git status command is the key to understanding Git. It will let us know what Git is processing and how Git perceives the condition of our repository.
- It shows the current state of the working directory and the staging area.

#### Syntax -
        git status

# git push -
- After committing your changes, git push send them to the remote server. Your commits are updated to the remote repository by Git push.

#### Syntax -
      git push {remote} {branch}

# git pull -
- git pull command is used to fetch and download content from a remote repository and immediately update the local repository to match that content.

#### Syntax -
     git pull <remote> <branch>
