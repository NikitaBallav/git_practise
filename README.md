
---

```markdown
# git_practise

## ✅ Case 1: From GitHub Repo to Local Machine

### Step 1: Clone the Repository  
Cloned this Git repo into my local machine using the command in the terminal of VS Code:

```bash
git clone "https://github.com/NikitaBallav/git_practise.git"
```

---

### Step 2: Navigate into the Repository Folder  
Used the below command to get into the repository folder:

```bash
cd git_practise
```

This step is crucial to understand:  
The local folder does not have Git by default. Inside the local folder, we have cloned the repository, which is already a folder having `git init`. Hence, Git commands will work inside the repo folder.

---

### Step 3: Check for Changes  
To check if any changes are made inside the repo folder, use the command below. It will display the output of any changes made that are not staged for commit:

```bash
git status
```

---

### Step 4: Stage the Changes  
To add the changes made, use one of the following commands. This will stage the changes, ready for commitment:

```bash
git add <file name>     # To stage changes for a specific file
```
or
```bash
git add .               # To stage all changes in the repo folder
```

---

### Step 5: Commit the Changes  
Use the following command to commit the staged changes. This updates the history of Git with the latest changes:

```bash
git commit -m "Update message"
```

---

### Step 6: Push Changes to GitHub  
To reflect the changes in the GitHub repository, i.e., to push the changes from local to remote workspace, use:

```bash
git push origin main
```

---

## ✅ Case 2: From Local Project to Remote GitHub Repo  
If you already have a local project folder and want to upload it to GitHub, follow these steps:

---

### Step 1: Initialize Git in Your Local Folder  
Open terminal and run:

```bash
git init
```

This will turn your folder into a Git repository.

---

### Step 2: Add Files to Git  
Stage all files you want to include:

```bash
git add .
```

---

### Step 3: Commit Your Work  
Create your first commit:

```bash
git commit -m "Initial commit"
```

---

### Step 4: Create a Repository on GitHub  
1. Go to [GitHub.com](https://github.com)  
2. Click on **New Repository**  
3. Give it a name (e.g., `my-project`)  
4. **DO NOT** initialize with README, license, etc. (to avoid conflicts)  
5. Click **Create Repository**

---

### Step 5: Link Your Local Repo to the GitHub Repo  
Copy the remote URL from GitHub and run:

```bash
git remote add origin "https://github.com/NikitaBallav/git_practise.git"
```

---

### Step 6: Push Your Code to GitHub  
Send your local code to the remote repository:

```bash
git push -u origin main
```

