# Notes for Collaboration with GitHuB
## Branches
    - A branch is a collection of ordered commits
    - Creating a new branch
        - git branch <branch-name>
    - Thinkful Good Practice for working with branches
        - jd--new-feature
    - Switching between branches
        - git checkout <branch-name> Switches to a specified branch
        - git checkout -  Switches to the previous branch
    - Merging Branches
        - git merge <branch-name>
    - Checking changes
        - git log  
    
## Feature Branch Workflow
    Ususal Feature branch Workflow
        1. On the main branch, run git pull so that you have the most up-to-date version.
        2. Create a new feature branch from the main branch.
        3. Create new commits on your new branch.
        4. Push your new branch up to GitHub.
        5. Create a pull request and have it reviewed.
        6. After making any requested changes, merge the pull request, bringing the new commits into the main branch.

## Merge Conflicts
    What is a Merge Conflict?
        A merge conflict occurs when Git attempts to resolve changes to a specific line in a file,but that file has been changed in a different way through another commit. 
        Basically Git does not know which change to keep so the change needs to be handled manually. 

    Solve a local conflict
        Example of a local conflict
            <<<<<<< HEAD
            =======
            Billy the Kid
            Joan of Arc
            Abraham Lincoln
            >>>>>>> main
        
        Conflict occured when merging the feature branch into the main branch. The code was deleted in the feature branch but not changed or added in the main branch

    Avoiding Conflicts
        Communicate often with other developers working on the same codebase. If you are working on the same part of the codebase, consider working together on that feature or fix until it is complete.

        Avoid making commits directly to the main branch or on GitHub. Stick with the feature branch workflow as much as possible.

        Use code formatters like PrettierJS in your code. This will avoid small conflicts, like added line spacing or errant commas.