It is commonly used to integrate feature branches into the main branch.

---

## 🔧 What is Merge?

A **merge** takes the changes from one branch and applies them to another.

Example:
- Merge `feature-branch` into `main`

---

## 🚀 Basic Merge Workflow

```bash
# Step 1: Switch to main branch
git checkout main

# Step 2: Merge feature branch
git merge feature-branch
🔄 Types of Merge
1️⃣ Fast-Forward Merge
Happens when there are no new commits in the target branch
Git simply moves the pointer forward
git merge feature-branch

👉 No merge commit created

2️⃣ Three-Way Merge
Happens when both branches have changes
Git creates a new merge commit

👉 Preserves history of both branches

⚔️ Merge Conflicts

A merge conflict occurs when:

Same file is changed in both branches
Git cannot decide which change to keep
🛠️ Example Conflict
<<<<<<< HEAD
Your code
=======
Incoming code
>>>>>>> feature-branch
✅ How to Resolve Conflicts
Open the conflicted file
Edit and fix the conflict manually
Remove conflict markers
Add the resolved file
git add file-name
Commit the merge
git commit -m "resolve merge conflict"
❌ Abort Merge
git merge --abort

👉 Cancels the merge process

🔍 Check Merge Status
git status
🧠 Best Practices
Always pull latest changes before merging
Keep branches updated
Resolve conflicts carefully
Test code after merge
⚠️ Common Mistakes
Ignoring conflicts
Merging without checking branch
Not testing after merge
🎯 Summary
Merge combines branches
Can be fast-forward or three-way
Conflicts must be resolved manually
➡️ Next Step

Continue to:

👉 03-rebase.md