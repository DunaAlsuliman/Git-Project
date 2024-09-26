# Git project command for each part

**1. Set Up the Repository:**  

     git init task-manager
     cd task-manager

**2. Add Initial Tasks:**  

    # tasks.txt file created with contents, then stage & commit  
    - git add .
    - git commit -m "Initial commit"

**3. Create Branches and Work on Features:**  

    - git checkout -b feature/add-tasks
    - echo "- Practice Git branching" >> tasks.txt
    - git add .
    - git commit -m "add tasks"
    # back to main branch to create remove branch 
    - git checkout main 
    - git checkout -b feature/remove-tasks
    # stage & commit changes
    - git add . 
    - git commit -m "remove tasks"

**4. Merge Branches and Handle Conflicts:**  

    - git checkout main 
    - git merge feature/add-tasks
    - git merge feature/remove-tasks
    # resolve conflicts then commit the merge
    - git add .
    - git commit 

**5. Use Git Rebase:**  

    # create new branch 
    - git checkout -b feature/update-tasks
    # stage and commit changes 
    - git add . 
    - git commit -m "update tasks"
    # rebase changes to main branch 
    - git checkout main  
    - git rebase feature/update-tasks

**6. Reverting to Previous Commits:**  

    # in main branch revert the last incorrect commit
    - git revert HEAD

**7. Working with Remote Repository:**  

    - git remote add origin https://github.com/DunaAlsuliman/Git-Project.git
    - git push -u origin main
    - git push -u origin feature/update-tasks
    - git push -u origin feature/remove-tasks
    - git push -u origin feature/add-tasks
