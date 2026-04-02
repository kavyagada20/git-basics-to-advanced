# 📦 Git Submodules

---

## 📌 Overview

Git Submodules allow you to **include one Git repository inside another** as a subdirectory.

👉 Useful for managing external dependencies or shared libraries.

---

## 🔧 What is a Submodule?

A submodule is a **separate Git repository** linked inside your main project.

- Keeps independent version history  
- Tracks a specific commit of the sub-repo  

---

## 🚀 Add a Submodule

```bash
git submodule add <repository-url> path/to/submodule
🔹 Example
git submodule add https://github.com/username/library.git libs/library
📥 Clone Repository with Submodules
git clone --recurse-submodules <repo-url>
🔄 Initialize Submodules (if not cloned with recurse)
git submodule init
git submodule update
🔁 Update Submodules
git submodule update --remote
📍 Check Submodule Status
git submodule status
❌ Remove Submodule
git submodule deinit -f path/to/submodule
rm -rf .git/modules/path/to/submodule
git rm -f path/to/submodule
🧠 How Submodules Work
Main repo stores a reference to a specific commit of submodule
Submodule has its own .git directory
Changes must be committed separately
⚠️ Important Notes
Submodules are not automatically updated
Requires manual update
Can be complex for beginners
🧠 Best Practices
Use submodules for stable dependencies
Always commit submodule changes
Keep submodules updated
⚠️ Common Mistakes
Forgetting to initialize submodules
Not committing submodule updates
Confusion between main repo and submodule
🎯 Summary
Submodules embed repositories inside repositories
Useful for managing external code
Requires careful handling
➡️ Next Step

Continue to:

👉 ../github/01-pull-requests.md