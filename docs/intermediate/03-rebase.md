# 🔁 Git Rebase

---

## 📌 Overview

Rebasing is a powerful Git feature used to integrate changes from one branch into another by **rewriting commit history**.

It helps create a **clean, linear project history**.

---

## 🔧 What is Rebase?

Rebase moves or reapplies commits from one branch onto another.

👉 Instead of merging, it **replays commits** on top of the target branch.

---

## 🚀 Basic Rebase Workflow

```bash
# Step 1: Switch to feature branch
git checkout feature-branch

# Step 2: Rebase onto main
git rebase main
🔄 How Rebase Works

Before:

main: A---B---C
             \
feature:      D---E

After rebase:

main: A---B---C
                 \
feature:          D'---E'

👉 Commits are reapplied with new IDs

⚔️ Rebase vs Merge
Merge	Rebase
Creates merge commit	No merge commit
Preserves history	Rewrites history
Safer for teams	Cleaner history
⚠️ Rebase Conflicts

Conflicts can occur during rebase just like merge.

🛠️ Resolve Rebase Conflicts
Fix conflicts in files
Stage changes
git add file-name
Continue rebase
git rebase --continue
❌ Abort Rebase
git rebase --abort

👉 Cancels the rebase process

⏸️ Skip Commit
git rebase --skip

👉 Skips problematic commit

✏️ Interactive Rebase

Used to edit commit history:

git rebase -i HEAD~3

👉 You can:

Reorder commits
Edit messages
Squash commits
🚫 Important Rule

❗ Never rebase shared/public branches (like main)

👉 It rewrites history and can break collaboration

🧠 Best Practices
Use rebase for clean history
Rebase before merging feature branches
Avoid rebasing public branches
⚠️ Common Mistakes
Rebasing main branch
Not resolving conflicts properly
Forgetting to push after rebase
🎯 Summary
Rebase rewrites commit history
Creates clean, linear logs
Requires careful usage
➡️ Next Step

Continue to:

👉 04-stash-reset.md