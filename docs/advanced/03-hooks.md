# 🪝 Git Hooks

---

## 📌 Overview

Git Hooks are **scripts that run automatically** when certain Git events occur.

They help automate tasks like:
- Code validation
- Testing
- Formatting
- Deployment

---

## 🔧 What are Git Hooks?

Git hooks are custom scripts stored inside:

```bash
.git/hooks/

👉 They trigger on events like:

Commit
Push
Merge
📂 Types of Hooks
🔹 Client-Side Hooks

Run on your local machine

pre-commit
commit-msg
post-commit
pre-push
🔹 Server-Side Hooks

Run on the server (GitHub, Git server)

pre-receive
update
post-receive
🚀 Common Hooks
1️⃣ Pre-Commit Hook

Runs before a commit is created

👉 Use cases:

Lint code
Run tests
Check formatting
2️⃣ Commit-Message Hook

Validates commit messages

👉 Example:

Enforce format: feat: add login feature
3️⃣ Pre-Push Hook

Runs before pushing code

👉 Use cases:

Run test suite
Prevent broken code
🛠️ Create a Hook
Step 1: Navigate to hooks folder
cd .git/hooks
Step 2: Create a hook file

Example: pre-commit

touch pre-commit
Step 3: Add script
#!/bin/sh
echo "Running pre-commit checks..."
Step 4: Make it executable
chmod +x pre-commit
⚙️ Example: Prevent Empty Commits
#!/bin/sh
if [ -z "$(git diff --cached)" ]; then
  echo "No changes staged!"
  exit 1
fi
🧠 Best Practices
Keep hooks simple and fast
Use hooks for validation, not heavy tasks
Share hooks using tools (like Husky)
⚠️ Limitations
Hooks are not shared by default
Each developer must set them up locally
🧠 Common Use Cases
Enforcing coding standards
Running tests before commit
Blocking bad commits
Automating workflows
⚠️ Common Mistakes
Forgetting to make hooks executable
Writing slow scripts
Not testing hooks
🎯 Summary
Git hooks automate workflows
Triggered by Git events
Useful for quality control
➡️ Next Step

Continue to:

👉 04-submodules.md