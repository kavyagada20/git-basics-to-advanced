# 📦 Git Stash & Reset

---

## 📌 Overview

Git provides powerful tools to **temporarily save changes** and **undo commits**:

- `git stash` → Save work temporarily
- `git reset` → Undo commits or changes

---

# 📦 Git Stash

---

## 🔧 What is Stash?

Stash temporarily saves your **uncommitted changes** so you can work on something else.

---

## 🚀 Save Changes (Stash)

```bash
git stash

👉 Saves:

Modified files
Staged changes
📝 Stash with Message
git stash push -m "work in progress"
📋 View Stashes
git stash list
🔄 Apply Stash
git stash apply

👉 Keeps stash after applying

📤 Apply & Remove Stash
git stash pop
❌ Drop Stash
git stash drop stash@{0}
🧹 Clear All Stashes
git stash clear
🧠 When to Use Stash
Switching branches quickly
Saving incomplete work
Fixing urgent bugs
🔁 Git Reset
🔧 What is Reset?

Reset is used to undo commits or changes.

⚙️ Types of Reset
1️⃣ Soft Reset
git reset --soft HEAD~1

👉 Removes last commit but keeps changes staged

2️⃣ Mixed Reset (Default)
git reset HEAD~1

👉 Keeps changes but unstaged

3️⃣ Hard Reset ⚠️
git reset --hard HEAD~1

👉 Deletes commit and changes permanently

📍 Reset to Specific Commit
git reset --hard <commit-id>
⚠️ Warning

❗ --hard reset is destructive
👉 Lost changes cannot be recovered easily

🔄 Stash vs Reset
Feature	Stash	Reset
Purpose	Save work	Undo changes
Safe	Yes	Can be dangerous
Use case	Temporary switch	Fix mistakes
🧠 Best Practices
Use stash for temporary work
Use reset carefully
Avoid hard reset on shared branches
⚠️ Common Mistakes
Using --hard without backup
Forgetting stash exists
Resetting wrong commit
🎯 Summary
git stash → Save temporary work
git reset → Undo commits
Both are essential for workflow control
➡️ Next Step

Continue to:

👉 ../advanced/01-cherry-pick.md