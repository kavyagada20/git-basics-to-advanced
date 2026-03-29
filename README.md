# Git Basics to Advanced 🚀

## 🧠 Core Concepts

### 🔹 Version Control System (VCS)
A system that tracks changes in code over time.

### 🔹 Distributed Version Control System (DVCS)
Git allows every developer to have a full copy of the repository.

### 🔹 Git Architecture
- Working Directory
- Staging Area (Index)
- Local Repository
- Remote Repository

---

## 🔧 Git Workflow

```bash
Working Directory → Staging Area → Repository → Remote
🔧 Git Commands
📍 Basic Commands
git init
git clone <repo-url>
git add .
git commit -m "message"
git status
git log
📍 Remote Commands
git remote add origin <url>
git push origin main
git pull origin main
git fetch
📍 Branching
git branch
git checkout -b feature-branch
git switch branch-name
📍 Merging
git merge branch-name
📍 Rebasing
git rebase branch-name
📍 Undo & Recovery
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit-id>
📍 Stashing
git stash
git stash pop
📍 Advanced
git cherry-pick <commit-id>
git reflog
git tag
git bisect
🌳 Branching Strategies
Git Flow
Feature Branch Workflow
Trunk-Based Development
⚔️ Merge vs Rebase
Merge	Rebase
Keeps history	Linear history
Safe	Cleaner
Creates merge commit	No merge commit
🧪 Real-World Scenarios
Fixing merge conflicts
Recovering deleted commits
Working with teams
Managing production branches
📂 Repository Structure
git-basics-to-advanced/
│
├── docs/
├── examples/
├── scripts/
├── cheatsheets/
├── interview-prep/
├── assets/
├── .github/
├── README.md
├── .gitignore
└── LICENSE
📘 Learning Modules
📗 Basics
Git installation
Git init & clone
Add, commit, push
📙 Intermediate
Branching
Merging
Stashing
📕 Advanced
Rebase
Cherry-pick
Hooks
Submodules
📘 GitHub
Pull Requests
Issues
CI/CD (GitHub Actions)
💻 Getting Started
git clone https://github.com/kavyagada20/git-basics-to-advanced.git
cd git-basics-to-advanced
⚡ Features
Beginner → Advanced roadmap
Hands-on examples
Real-world workflows
Interview preparation
Clean documentation
🤝 Contributing
Fork the repo
Create a branch
Commit changes
Push and create PR
📜 License

MIT License

⭐ Support

If this helped you, give it a ⭐ and share!
