# 🔧 Basic Git Commands

---

## 📌 Overview

Git provides a set of commands to track changes, manage versions, and collaborate efficiently.  
This section covers the **most essential Git commands** every developer should know.

---

## 📂 Check Repository Status

```bash
git status

👉 Shows:

Modified files
Staged files
Untracked files
➕ Add Changes to Staging Area
Add a specific file
git add file-name
Add all files
git add .
💾 Commit Changes
git commit -m "your message"

👉 Saves a snapshot of staged changes

✅ Best Practices
Use clear messages
Example:
git commit -m "feat: add login feature"
📜 View Commit History
git log

👉 Shows all commits with:

Commit ID
Author
Date
Message
🔍 View Changes
View unstaged changes
git diff
View staged changes
git diff --staged
🌐 Work with Remote Repository
Add remote
git remote add origin <repo-url>
View remotes
git remote -v
🚀 Push Changes
git push origin main

👉 Uploads local commits to GitHub

📥 Pull Changes
git pull origin main

👉 Fetches and merges latest changes

📡 Fetch Changes
git fetch

👉 Downloads changes without merging

🏷️ Rename Branch
git branch -M main
🧠 Quick Workflow
git add .
git commit -m "message"
git push
⚠️ Common Mistakes
Forgetting git add
Writing poor commit messages
Pushing without pulling latest changes
🎯 Summary
git add → Stage changes
git commit → Save changes
git push → Upload changes
git pull → Sync changes
git status → Check state
➡️ Next Step

Continue to:

👉 ../intermediate/01-branching.md