# 🍒 Git Cherry-Pick

---

## 📌 Overview

`git cherry-pick` is used to **apply a specific commit from one branch to another**.

Instead of merging entire branches, you can pick only the commits you need.

---

## 🔧 What is Cherry-Pick?

Cherry-pick copies a commit from one branch and applies it to your current branch.

👉 Useful when you need **specific changes without merging everything**

---

## 🚀 Basic Syntax

```bash
git cherry-pick <commit-id>
📍 Example Workflow
Step 1: View commits
git log --oneline
Step 2: Copy commit ID

Example:

a1b2c3d Fix login bug
Step 3: Switch branch
git checkout main
Step 4: Apply commit
git cherry-pick a1b2c3d
🔄 Cherry-Pick Multiple Commits
git cherry-pick commit1 commit2
📦 Cherry-Pick Range
git cherry-pick A..B

👉 Applies commits between A and B

⚔️ Cherry-Pick Conflicts

Conflicts may occur if changes overlap.

🛠️ Resolve Conflicts
Fix conflicts manually
Stage changes
git add file-name
Continue cherry-pick
git cherry-pick --continue
❌ Abort Cherry-Pick
git cherry-pick --abort
⏭️ Skip Commit
git cherry-pick --skip
🧠 When to Use Cherry-Pick
Apply a bug fix to another branch
Move specific commits between branches
Avoid full merges
⚠️ Important Notes
Creates a new commit (different ID)
Can duplicate commits if used incorrectly
🧠 Best Practices
Use for small, specific changes
Avoid overusing (can clutter history)
Prefer merge/rebase for large changes
⚠️ Common Mistakes
Cherry-picking wrong commit
Creating duplicate history
Ignoring conflicts
🎯 Summary
Cherry-pick applies specific commits
Useful for selective changes
Requires careful handling
➡️ Next Step

Continue to:

👉 02-reflog.md