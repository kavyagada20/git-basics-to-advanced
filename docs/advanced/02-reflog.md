`git reflog` is a powerful command used to **track all changes to your repository references (HEAD)**.

👉 It helps you **recover lost commits**, even after reset or rebase.

---

## 🔧 What is Reflog?

Reflog records every movement of:
- `HEAD`
- Branch pointers

👉 Think of it as a **history of your Git actions**

---

## 🚀 Basic Command

```bash
git reflog
📍 Example Output
a1b2c3d HEAD@{0}: commit: added login feature
d4e5f6g HEAD@{1}: reset: moving to HEAD~1
h7i8j9k HEAD@{2}: commit: initial commit
🔍 Understanding Output
HEAD@{0} → current state
HEAD@{1} → previous state
Each entry shows an action
🛠️ Recover Lost Commits
Step 1: Find commit in reflog
git reflog
Step 2: Reset to commit
git reset --hard <commit-id>
🔄 Recover Deleted Branch
git checkout -b recovered-branch <commit-id>
⏪ Undo Hard Reset
git reset --hard HEAD@{1}
⏱️ Reflog Time Reference
git reset --hard HEAD@{2}

👉 Moves back to earlier state

⚠️ Important Notes
Reflog is local only (not shared)
Entries expire over time (default ~90 days)
🧠 Best Use Cases
Recover deleted commits
Undo mistakes
Restore previous state
Debug Git history
⚠️ Common Mistakes
Not using reflog after losing commits
Confusing reflog with git log
Forgetting commit IDs
🎯 Summary
git reflog tracks all HEAD changes
Helps recover lost work
Essential for debugging and recovery
➡️ Next Step

Continue to:

👉 03-hooks.md