# 🔀 Pull Requests (PR)

---

## 📌 Overview

A Pull Request (PR) is a way to **propose changes** from one branch to another, typically from a feature branch to the `main` branch.

👉 It is a core part of **team collaboration on GitHub**

---

## 🔧 What is a Pull Request?

A Pull Request allows you to:
- Share your changes
- Request code review
- Discuss improvements
- Merge code safely

---

## 🚀 PR Workflow

```bash
Create Branch → Make Changes → Push → Open PR → Review → Merge
🧪 Step-by-Step Example
1️⃣ Create a new branch
git checkout -b feature/login
2️⃣ Make changes & commit
git add .
git commit -m "feat: add login feature"
3️⃣ Push branch to GitHub
git push -u origin feature/login
4️⃣ Open Pull Request
Go to your GitHub repository
Click "Compare & Pull Request"
Add:
Title
Description
Submit PR
👀 Code Review Process

Reviewers can:

Comment on code
Suggest changes
Approve PR
🔁 Update Pull Request

After changes:

git add .
git commit -m "fix: update login validation"
git push

👉 PR updates automatically

🔀 Merge Pull Request

Once approved:

Click Merge PR
Choose:
Merge commit
Squash merge
Rebase merge
🧹 Delete Branch

After merge:

git branch -d feature/login
git push origin --delete feature/login
🧠 Best Practices
Keep PRs small and focused
Write clear descriptions
Use meaningful titles
Review code carefully
⚠️ Common Mistakes
Large PRs (hard to review)
No description
Not testing before PR
Ignoring review comments
🎯 Summary
PR is used for collaboration
Enables code review and discussion
Essential in team workflows
➡️ Next Step

Continue to:

👉 02-issues.md