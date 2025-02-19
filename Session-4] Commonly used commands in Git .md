# Commonly used commands in Git -

## Create a Repository-
### git init- 
- git init is used to initialize a new Git repository in a project directory.
- When you run git init, the following happens:
   - Creates a .git folder: Git creates a hidden folder called .git inside your project directory. This folder contains all the metadata and configuration files that Git uses to track your project’s history.
   - Makes the folder a Git repository: After running git init, the folder is now considered a Git repository.

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
- Clone means to create a copy of a repository, typically from a remote server (like GitHub, GitLab, or Bitbucket), onto your local machine.
- When you clone a repository, you get the entire project, including all its files, commit history, branches, and configurations, so that you can work on it locally.

![image](https://github.com/user-attachments/assets/3bc4a7ba-ad3a-4695-aae2-e1aaf8d60f2c)


### Syntax -
    git clone [repository URL] folder_path
       folder path where you have to download 

### Clone branch -
    git clone --branch branch-name URL
                  OR
    
    git clone -b branch-name URL


# git status -
- Git status command is the key to understanding Git. It will let us know what Git is processing and how Git perceives the condition of our repository.
- It shows the current state of the working directory and the staging area.

#### Syntax -
        git status

# git push -
- After committing your changes, git push send them to the remote server. Your commits are updated to the remote repository by Git push.

#### Syntax -
      git push {remote} {branch}

## Generate an SSH key:
       ssh-keygen -t rsa -b 4096 -C "youremail@example.com"

## Add your SSH key to the SSH agent:
      eval "$(ssh-agent -s)"
      ssh-add ~/.ssh/id_rsa
- The SSH agent will store this key and allow it to be used when you connect to remote servers like GitHub, without needing you to re-enter the password or passphrase each time.
- ssh-add is a command used to add SSH private keys to the SSH agent.
 
## Copy your SSH public key to GitHub:
      cat /home/ec2-user/.ssh/id_rsa.pub
   
## Git Push -
      git remote add origin git@github.com:username/repository.git
      git push -u origin main

# git pull -
- git pull command is used to fetch and download content from a remote repository and immediately update the local repository to match that content.

#### Syntax -
     git pull <remote> <branch>

     git pull origin <branch-name>





     
