# 📘 Introduction to Git

---

## 📌 What is Git?

Git is a **distributed version control system (DVCS)** used to track changes in source code during software development.

It allows multiple developers to work on a project efficiently without overwriting each other's changes.

---

## 🚀 Why Use Git?

- Track changes in code over time
- Collaborate with teams بسهولة
- Maintain version history
- Revert to previous versions if needed
- Work on multiple features using branches

---

## 🧠 What is Version Control?

Version Control is a system that records changes to files over time so you can:
- Recall specific versions later
- Compare changes
- Collaborate safely

---

## 🔄 Types of Version Control Systems

### 1️⃣ Local VCS
- Stores versions locally
- Limited collaboration

### 2️⃣ Centralized VCS (CVCS)
- Single central server
- Example: SVN

### 3️⃣ Distributed VCS (DVCS)
- Every user has a full copy of the repository
- Example: Git

---

## ⚙️ Git Architecture

Git works with three main areas:

### 🗂️ Working Directory
Where your files are currently located and edited.

### 📥 Staging Area (Index)
Where changes are prepared before committing.

### 📦 Repository
Where Git permanently stores your committed changes.

---

## 🔄 Git Workflow

```bash
Working Directory → Staging Area → Repository
🌍 What is GitHub?

GitHub is a cloud-based platform that hosts Git repositories and enables collaboration.

🔑 Key Terms
Repository (Repo) → Project folder tracked by Git
Commit → Snapshot of changes
Branch → Independent line of development
Merge → Combine changes from branches
Clone → Copy a repository
Push → Upload changes to remote
Pull → Fetch and merge changes
🎯 Summary
Git is a powerful version control system
Helps manage code efficiently
Enables collaboration and tracking
Forms the foundation of modern development workflows
➡️ Next Step

Continue to:

👉 02-installation.md


---

# 💻 Git Commands (Add, Commit, Push)

After creating this file, run:

```bash id="cmdgit1"
git add docs/basics/01-introduction.md
git commit -m "docs: add Git introduction module"
git push