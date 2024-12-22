# Git Repositories -
- A Git repository (or repo for short) contains all of the project files and the entire revision history.
- A Git repository is a virtual storage of your project. It allows you to save versions of your code, which you can access when needed.
- It is like a folder that not only holds your files but also tracks their evolution over time.

# Types of Git Repositories -
- There are two types of Git repositories:
- **Local repository:**
          This is the copy of the repository stored on your own computer. Every time you create a Git project on your machine, it’s a local repository.
- **Remote repository:**
         This is the version of the repository stored online, on a server or platform like GitHub, GitLab, or Bitbucket. It allows you to share your project and collaborate with others.

# Create a Repository-
### git init- 
- git init is used to initialize a new Git repository in a project directory.
- When you run git init, the following happens:
   - Creates a .git folder: Git creates a hidden folder called .git inside your project directory. This folder contains all the metadata and configuration files that Git uses to track your project’s history.
   - Makes the folder a Git repository: After running git init, the folder is now considered a Git repository.

# Clone Repository-
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


   


    
