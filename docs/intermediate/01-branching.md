# 🌿 Git Branching

---

## 📌 Overview

Branching is one of Git’s most powerful features.  
It allows you to create independent lines of development without affecting the main codebase.

---

## 🌳 What is a Branch?

A **branch** is a separate version of your project.

- Default branch → `main`
- Used for developing features, fixing bugs, experimenting safely

---

## 🔧 View Branches

```bash
git branch

👉 Lists all local branches

➕ Create a New Branch
git branch feature-branch
🔄 Switch Branch
git checkout feature-branch
✅ Modern way:
git switch feature-branch
⚡ Create + Switch (Shortcut)
git checkout -b feature-branch
OR
git switch -c feature-branch
📍 Check Current Branch
git branch --show-current
❌ Delete a Branch
git branch -d feature-branch

👉 Use -D to force delete

🔀 Rename a Branch
git branch -m new-branch-name
🌐 Work with Remote Branches
Push branch to remote
git push origin feature-branch
Track remote branch
git push -u origin feature-branch
🔄 Branch Workflow
main → create branch → work → commit → merge → delete branch
🧠 Best Practices
Use meaningful branch names:
feature/login
bugfix/navbar
hotfix/payment
Keep branches small and focused
Delete branches after merging
⚠️ Common Mistakes
Working directly on main
Not pulling latest changes before branching
Keeping unused branches
🎯 Summary
Branches isolate work
Enable parallel development
Improve collaboration
➡️ Next Step

Continue to:

👉 02-merging.md