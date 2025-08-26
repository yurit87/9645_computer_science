

1. Create a new subfolder named `9645_<your name>'s_work` inside your fork of the 9645_computer_science directory.

2. Create a new subfolder inside this subfolder and name it `python_scripts`

3. Create a script named `example_best_work.py` that contains some Python code of your choice.

4. Create a script named `example_not_best_work.py` that contains some Python code of your choice.

5. Upload your work folder, the `python_scripts` subfolder, and the `example_best_work.py` file to your GitHub repository (using `stage` / `commit` / `push` as taught  [[git_setup_for_your_course]].

6. Create a new repository on GitHub (e.g., `my_first_repo`), clone the repository to your local system using `git clone`.

7. Create a `README.md` file in the repository. Write a brief introduction about the repository using Markdown (e.g., "This is my first GitHub project").

---

### 3. **Track Changes with Git**

- Edit the `README.md` file (e.g., add another line of text).
- Stage and commit the changes:

   ```bash
    git add README.md
    git commit -m "Updated README with a new line"
    ```
    
- Push the changes to GitHub:
 
    ```bash
    git push
    ```
    

---

### 4. **Create and Switch Branches**

- Create a new branch named `feature_addition`:
    
    bash
    
    Copy
    
    ```bash
    git branch feature_addition
    ```
    
- Switch to the new branch:
    
    bash
    
    Copy
    
    ```bash
    git checkout feature_addition
    ```
    
- Add a new file to this branch (e.g., `new_feature.py`), commit it, and push the branch to GitHub:
    
    bash
    
    Copy
    
    ```bash
    git add new_feature.py
    git commit -m "Added new_feature.py"
    git push -u origin feature_addition
    ```
    

---

### 5. **Pull Requests**

- Open a pull request on GitHub to merge the `feature_addition` branch into the `main` branch.
- Add a meaningful title and description for the pull request.

---

### 6. **Resolve Merge Conflicts**

- Simulate a merge conflict by editing the same line in the `main` branch and the `feature_addition` branch.
- Create a pull request and resolve the conflict manually in GitHub or locally.

---

### 7. **Fork and Clone**

- Fork someone else's public repository.
- Clone the forked repository to your local machine:
    
    bash
    
    Copy
    
    ```bash
    git clone <forked_repo_url>
    ```
    
- Make some changes, commit them, and push them to your forked repository.

---

### 8. **Contribute to Open Source**

- Submit a pull request to the original repository (upstream) from your fork.

---

### 9. **Git Ignore**

- Create a `.gitignore` file in the repository.
- Add rules to ignore files (e.g., `.DS_Store`, `*.log`, or `__pycache__/`).
- Commit the `.gitignore` file.

---

### 10. **Undo Mistakes**

- Practice undoing changes:
    - Reset a staged file:
        
        bash
        
        Copy
        
        ```bash
        git reset <file_name>
        ```
        
    - Undo the last commit:
        
        bash
        
        Copy
        
        ```bash
        git reset --soft HEAD~1
        ```
        
    - Revert a pushed commit:
        
        bash
        
        Copy
        
        ```bash
        git revert <commit_hash>
        ```
        

---

### 11. **Tagging**

- Create a tag for a release:
    
    bash
    
    Copy
    
    ```bash
    git tag -a v1.0 -m "First release"
    ```
    
- Push the tag to GitHub:
    
    bash
    
    Copy
    
    ```bash
    git push origin v1.0
    ```
    

---

### 12. **Collaborate on a Group Project**

- Work with a friend or classmate on the same repository.
- Practice pulling changes from the remote repository:
    
    bash
    
    Copy
    
    ```bash
    git pull
    ```
    
- Discuss and resolve merge conflicts together.

---

### 13. **Git Logs and History**

- View the commit history:
    
    bash
    
    Copy
    
    ```bash
    git log
    ```
    
- Use `git log --oneline` for a simplified view.

---

### 14. **Revert to a Previous Commit**

- Use `git checkout <commit_hash>` to view an old version of your code.
- Reset your branch to an earlier commit:
    
    bash
    
    Copy
    
    ```bash
    git reset --hard <commit_hash>
    ```
    

---

### 15. **Create a Personal Portfolio Repository**

- Create a repository to showcase your projects (e.g., `portfolio`).
- Use GitHub Pages to host a static website:
    - Add HTML/CSS/JS files.
    - Enable GitHub Pages in the repository settings.

These tasks cover a wide range of beginner-friendly Git/GitHub skills and are perfect for developing confidence in version control systems.



