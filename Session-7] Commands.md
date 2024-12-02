# Stashing -
- Sometimes you may need to switch branches or pull updates without committing your current work.
- Stashing temporarily saves your changes that you haven’t committed yet. You can then come back to them later after switching to a different task or branch.
- The git stash command temporarily saves your changes and reverts your working directory to the last commit.

#### Syntax -
     git stash


# Rebasing -
- Rebasing is a powerful Git command that allows you to integrate changes from one branch into another.

#### Syntax -
     git rebase <branch-name>

# Reverting -
- Resetting moves your branch pointer to a different commit, discarding (or optionally keeping) the changes you’ve made.
- It can change history, and can be more destructive than reverting.
- It does not delete the original commit. Instead, it creates a new commit that undoes the changes made by the original commit.

#### Syntax -
     git revert <commit-hash>

# Resetting -
- The git reset command is used to undo changes in your working directory or the staging area.

#### Syntax -
    git reset <commit-hash>

