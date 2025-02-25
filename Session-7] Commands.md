# Stashing -
- Sometimes you may need to switch branches or pull updates without committing your current work.
- Stashing temporarily saves your changes that you haven’t committed yet. You can then come back to them later after switching to a different task or branch.
- The git stash command temporarily saves your changes and reverts your working directory to the last commit.

#### Syntax -
     git stash  #give any random name to stash
     git stash -m "message"

##### Listing Stashes:
- Use git stash list to view all the stashes you've saved.

          git stash list

##### To apply the most recent stash: 

          git stash apply.

- To apply a specific stash (e.g., stash@{2}): git stash apply stash@{2}.
- Use git stash drop stash@{n} to remove a specific stash
- git stash clear to remove all stashes.
- You can stash only specific files using git stash push <file>, e.g., git stash push file1.txt
- git stash pop — Applies and removes the most recent stash.


# Rebasing -
- Rebasing is a powerful Git command that allows you to integrate changes from one branch into another.
- Switch to target branch and then rebash.
- It helps keep a clean Git history by avoiding unnecessary merge commits.

#### Syntax -
     
      git rebase <branch-name>

# Reverting -
- git revert is a command used to create a new commit that undoes the changes made in a previous commit.
- It can change history, and can be more destructive than reverting.
- It does not delete the original commit. Instead, it creates a new commit that undoes the changes made by the original commit.

#### Syntax -
     git revert <commit-hash>



- git log --oneline: to view the Git commit history in a compact, one-line format.
- you can again revert into reverted commit

        git revert <reverted-hash>
             

# Resetting -
- The git reset is a command used to undo changes in Git.
- It moves your project back to an earlier commit and can affect three areas depending on how you use it:
       - HEAD (the pointer to the current commit)
       - Staging Area (files ready to be committed)
       - Working Directory (your local files).

#### Syntax -
    git reset <commit-hash>

## Types of Git Reset -

#### 1.Soft Reset (git reset --soft):
- Moves the pointer (HEAD) to an earlier commit.
- Keeps your changes staged for commit.
- Use it when you want to change the last commit but keep your work.

#### 2.Mixed Reset (git reset --mixed) (Default):
- Moves the pointer (HEAD) to an earlier commit.
- Removes changes from the staging area but keeps them in your files.
- Use it when you want to unstage changes but not lose your work.


#### 3.Hard Reset (git reset --hard):
- Moves the pointer (HEAD) to an earlier commit.
- Deletes all changes from both the staging area and your files.
- Use it only if you're sure you want to discard all changes.
