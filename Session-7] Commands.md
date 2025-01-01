# Stashing -
- Sometimes you may need to switch branches or pull updates without committing your current work.
- Stashing temporarily saves your changes that you haven’t committed yet. You can then come back to them later after switching to a different task or branch.
- The git stash command temporarily saves your changes and reverts your working directory to the last commit.

#### Syntax -
     git stash  #give any random name to stash
     git stash -m "message"

- Listing Stashes:
      - Use git stash list to view all the stashes you've saved.

- To apply the most recent stash: git stash apply.
- To apply a specific stash (e.g., stash@{2}): git stash apply stash@{2}.
- Use git stash drop stash@{n} to remove a specific stash
- git stash clear to remove all stashes.
- You can stash only specific files using git stash push <file>, e.g., git stash push file1.txt
- git stash pop — Applies and removes the most recent stash.


# Rebasing -
- Rebasing is a powerful Git command that allows you to integrate changes from one branch into another.
- Switch to target branch and then rebash.

#### Syntax -
     git rebase <branch-name>

# Reverting -
- git revert is a command used to create a new commit that undoes the changes made in a previous commit.
- It can change history, and can be more destructive than reverting.
- It does not delete the original commit. Instead, it creates a new commit that undoes the changes made by the original commit.

#### Syntax -
     git revert <commit-hash>

# Resetting -
- The git reset command is used to undo changes in your working directory or the staging area.

#### Syntax -
    git reset <commit-hash>

