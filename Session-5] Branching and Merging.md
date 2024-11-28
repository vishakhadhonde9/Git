# Branching -
-  Branching is a way for developers to create separate workspaces for their code without modifying the main version.
-  Branch is a new/separate version of the main repository.
-  Branches are pointers to a snapshot of the code, and developers can use them to add features or fix bugs.

# Types of Branches -
- The main idea behind the Git flow branching strategy is to isolate your work into different types of branches.
- There are five different branch types in total:
  - Main
  - Develop
  - Feature
  - Release
  - Hotfix
## 1] Main Branch (Master)-
- This is the default branch in Git.
- It represents the stable version of the project and is typically where the production-ready code resides.
## 2] Feature Branch -
- Feature branches are created to develop new features or implement enhancements.
- These branches allow developers to work on isolated changes without disturbing the stability of the main branch.

## 3] Bugfix Branch -
- These branches are used specifically to fix bugs or address issues.
- Just like feature branches, they are created off of the main branch or the most relevant branch.

## 4] Release Branch -
- A release branch is created to prepare for a new version or release of the software.
- It allows for final testing, minor bug fixes, and preparation of release notes.



## Create a branch: Use the git branch command to create a new branch.
     git branch <branch-name>

# Switch to a branch:  
- Use the git checkout command to switch to an existing branch.
- **Git checkout -**
- We can create and switch to a new branch or an existing branch using the Git checkout command.
- To accomplish this, you must have access to the branch you wish to switch to on your local system, and you must commit or stash any modifications to your current branch before switchin

#### Syntax - 
       git checkout <branch-name>
       
       If you want to create and switch to a new branch, use the command:
       git checkout -b <new-branch-name>

## Benefits of branching in Git:
- Avoids impacting the live version: Developers can make copies of files without affecting the live version. 
- Collaborates with other developers: Branches allow for easier collaboration among developers who have access to the repository. 
- Saves disk space: Branches don't waste disk space like a simple file system copy would.

# Merging in git-
#### Git merge-
- The very last step is merging the branch with the parent branch once you have finished developing your branch and everything is working as it should.
- The Git merge command is used to achieve this.
- To combine various branches into one, the Git merge command is used.

#### Syntax-
     git merge <branch-name>


