# 📦 Git Init & Clone

---

## 📌 Overview

To start working with Git, you either:

- Create a new repository → `git init`
- Copy an existing repository → `git clone`

---

## 🆕 Initialize a Repository (`git init`)

### 🔹 What it does
Creates a new Git repository in your project folder.

---

### 🔹 Command

```bash
git init
🔹 Example
mkdir my-project
cd my-project
git init

👉 This creates a hidden .git folder that tracks all changes.

🔹 When to use
Starting a new project
Adding Git to an existing project
📥 Clone a Repository (git clone)
🔹 What it does

Creates a copy of a remote repository on your local machine.

🔹 Command
git clone <repository-url>
🔹 Example
git clone https://github.com/username/repo-name.git
🔹 Clone into a specific folder
git clone https://github.com/username/repo-name.git my-folder
🔹 What gets cloned?
All files
Commit history
Branches
Remote configuration
🔄 Difference: init vs clone
Feature	git init	git clone
Purpose	Create new repo	Copy existing repo
Source	Local folder	Remote repo
History	No history	Full history
⚙️ After Cloning

Move into the project:

cd repo-name
🧠 Best Practices
Use git init for new projects
Use git clone when working on existing projects
Always check repository URL before cloning
🎯 Summary
git init → Start a new repository
git clone → Copy an existing repository
Both are essential starting points in Git
➡️ Next Step

Continue to:

👉 04-basic-commands.md