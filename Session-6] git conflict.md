# git conflict -
- A conflict in happens when changes made in two different branches are incompatible with each other.
- A conflict arises when two separate branches have made edits to the same line in a file, or when a file has been deleted in one branch but edited in the other.
  - Two people edit the same part of a file in different ways.
  - One person deletes or changes a file that another person has modified.
- Git will often automatically handle merging, but when there are conflicting changes, you'll need to resolve them manually.

## How Git Marks a Conflict:
- When a conflict occurs, Git will mark the conflicting sections in the file using conflict markers.


      <<<<<<< HEAD
      Changes made in the current branch (e.g., main)
      =======
      Changes made in the other branch (e.g., feature-branch)
      >>>>>>> feature-branch
      

- <<<<<<< HEAD: Marks the start of the section with the changes from the current branch (i.e., the branch you are merging into).
- =======: Separates the two conflicting changes.
- >>>>>>> feature-branch: Marks the end of the conflict and indicates the changes from the other branch (i.e., the branch being merged).



## git merge -
- merging the branch with the parent branch once you have finished developing your branch


### Steps -
1. Merge a feature branch into main:

        git checkout main
        git merge feature-branch


2. If there's a conflict, Git will inform you:

      CONFLICT (content): Merge conflict in <filename>


3. Open the conflicted file and manually resolve the conflict:

      <<<<<<< HEAD
      Changes in the main branch
      =======
      Changes in the feature branch
      >>>>>>> feature-branch

Edit the file to resolve the conflict, then remove the conflict markers.

4. Stage the resolved file:

     git add <filename>


5. Commit the merge:

    git commit


6. Push the changes to the remote repository:


    git push origin main

