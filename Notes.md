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
